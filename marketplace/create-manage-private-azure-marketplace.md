---
title: 在 Azure 门户中创建和管理专用 Azure Marketplace
description: 了解如何创建和管理专用 Azure Marketplace (预览) 在 Azure 门户中。 专用 Azure Marketplace (预览版) 使管理员可以控制其用户可以使用的第三方解决方案。
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712760"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>在 Azure 门户中创建和管理专用 Azure Marketplace

私有 Azure Marketplace 使管理员可以控制其用户可以使用的第三方解决方案。 它通过允许用户仅部署管理员批准并符合企业策略的产品/服务来实现此功能。 通过专用 Azure Marketplace，用户可以在在线商店中搜索符合要求的产品/服务以购买和部署。

作为 Marketplace 管理员 (分配的角色) ，你将从一个禁用且空的私有存储开始，你可以在其中添加已批准的产品/服务和计划。 本文介绍如何分配所需的角色、创建专用存储、管理项目、批准用户请求，并为用户启用私有 Azure Marketplace。

> [!NOTE]
> - Azure Marketplace 专用于租户级别，因此租户下的所有用户都将看到相同的特选列表。
> - 所有 Microsoft 解决方案 (包括 [认可的 Linux 分发](/azure/virtual-machines/linux/endorsed-distros)) 自动添加到专用 Azure Marketplace。

## <a name="assign-the-marketplace-admin-role"></a>分配 Marketplace 管理员角色

租户全局管理员必须将 **Marketplace 管理员** 角色分配给将管理专用存储的专用 Azure Marketplace 管理员。

>[!IMPORTANT]
> 只有分配有 Marketplace 管理员角色的 IT 管理员才能访问专用 Azure Marketplace 管理。

### <a name="prerequisites"></a>必备条件

在将 Marketplace 管理员角色分配给租户范围内的用户之前，需要满足以下先决条件：

- 你有权访问 **全局管理员** 用户。
- 租户至少有一个订阅 (可以是任何类型) 。
- 为全局管理员用户分配所选订阅的 " **参与者** " 角色或更高级别。

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>使用访问控制 (IAM 分配 Marketplace 管理员角色) 

1. 登录 [Azure 门户](https://portal.azure.com/)。
1. 选择 " **所有服务** "，然后选择 " **Marketplace**"。
1. 从左侧菜单中选择 " **专用 Marketplace** "。

    [![在 Marketplace 的左侧显示 "专用市场" 菜单选项。](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. 选择 **(IAM) 的 "访问控制** " 以分配 Marketplace 管理员角色。

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="显示 I A M 访问控制屏幕。":::

1. 选择“+ 添加”   >   “添加角色分配”。
1. 在 " **角色**" 下，选择 " **Marketplace 管理**"。

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="显示 &quot;角色分配&quot; 菜单。":::

1. 从下拉列表中选择所需的用户，然后选择 " **完成**"。

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>向 PowerShell 分配 Marketplace 管理员角色

使用以下 PowerShell 脚本分配 Marketplace 管理员角色;它需要以下参数：

- **TenantId：** 范围 (Marketplace 管理员角色的租户的 ID 可在租户范围) 上分配。
- **SubscriptionId：** 全局管理员具有 **参与者** 角色或分配更高的订阅。
- **GlobalAdminUsername：** 全局管理员的用户名。
- **UsernameToAssignRoleFor：** 将向其分配 Marketplace 管理员角色的用户名。

> [!NOTE]
> 对于受邀加入租户的来宾用户，最多可能需要48小时才能分配给 Marketplace 管理员角色。 有关详细信息，请参阅 [AZURE ACTIVE DIRECTORY B2B 协作用户的属性](/azure/active-directory/b2b/user-properties)。

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

有关 Az PowerShell 模块中包含的 cmdlet 的详细信息，请参阅 [Microsoft Azure PowerShell：门户面板 cmdlet](/powershell/module/az.portal/)。

## <a name="create-private-azure-marketplace"></a>创建专用 Azure Marketplace

1. 登录 [Azure 门户](https://portal.azure.com/)。
2. 选择 " **所有服务** "，然后选择 " **Marketplace**"。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="显示 Azure 门户主窗口。":::

3. 从左侧菜单中选择 " **专用 Marketplace** "。

4. 选择 " **开始** 使用" 创建专用 Azure Marketplace (你只需) 完成此操作。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="说明如何选择 &quot;Azure 门户&quot; 主窗口中的 &quot;入门&quot;。":::

    如果此租户已存在专用 Azure Marketplace，则默认情况下将选择 " **管理 marketplace** "。

5. 完成后，你将拥有一个空且已禁用的专用 Azure Marketplace。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="显示空的专用 Azure Marketplace 屏幕。":::

## <a name="add-items-from-gallery"></a>从库中添加项

项是产品/服务和计划的组合。 你可以在 "管理应用商店" 页上搜索和添加项。

1. 选择 " **添加项**"。

2. 浏览 **库** ，或使用搜索字段查找所需的项。

    [![演示如何浏览库或使用搜索字段。](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. 默认情况下，在添加新产品/服务时，所有当前计划将添加到 "已批准" 列表中。 若要在添加选定项之前修改计划选择，请在产品的磁贴中选择下拉菜单，并更新所需的计划。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="说明如何更新所需的计划。":::

4. 做出选择后，请选择左下角的 " **完成** "。

>[!Note]
> 将 **项目添加** 到 Marketplace 仅适用于非 Microsoft 产品/服务。 包括 [认可的 Linux 分发](/azure/virtual-machines/linux/endorsed-distros) (的 Microsoft 解决方案) 将被标记为 "默认情况下获得批准"，并且不能在私有 Marketplace 中进行管理。

## <a name="edit-items-plans"></a>编辑项的计划

你可以在 "管理应用商店" 页上编辑项的计划。

1. 在 " **计划** " 列中，查看该项的下拉菜单中的可用计划。
2. 选中或清除相应的复选框，以选择要对用户提供哪些计划。

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="演示如何选中或清除所需项的复选框。":::

> [!NOTE]
> 每个产品/服务至少需要选择一个计划才能进行更新。 若要删除与产品/服务相关的所有计划，请删除整个提议 (参阅下一部分) 。

## <a name="delete-offers"></a>删除产品/服务

在 "管理应用商店" 页上，选中 "产品/服务名称" 旁边的复选框 (参阅上方的屏幕) 并选择 " **删除项目**"。

## <a name="enabledisable-private-azure-marketplace"></a>启用/禁用专用 Azure Marketplace

在 "管理应用商店" 页上，你将看到其中一个横幅，其中显示了专用 Azure Marketplace 的当前状态：

:::image type="content" source="media/private-azure/state-disable.png" alt-text="显示 &quot;禁用状态&quot; 横幅。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="显示 &quot;启用状态&quot; 横幅。":::

你可以根据需要启用或禁用专用 Azure Marketplace。

- 如果已禁用，请选择 " **启用专用 Marketplace** " 启用。
- 如果已启用，请选择 **禁用专用 Marketplace** 禁用。

## <a name="private-azure-marketplace-notification-center"></a>私有 Azure Marketplace 通知中心

通知中心包含三种类型的通知，并允许 Marketplace 管理员根据通知执行操作：

- 来自用户的针对不在已批准列表中的项目的审批请求 (参阅下面) 中 [添加产品/服务的请求](#request-to-add-offers-or-plans) 。
- 已在批准列表中有一个或多个计划的产品/服务的新计划通知。
- 已删除批准列表中的项目的计划通知，但已将其从全局 Azure Marketplace 中删除。

访问通知中心：

1. 从左侧菜单中选择 " **通知** "。

    [![显示 "通知" 菜单。](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. 选择省略号菜单以获取更多操作。

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="显示 &quot;更多选项&quot; 菜单结果。":::

1. 对于计划请求，" **显示请求** " 将打开 "批准请求" 表单，你可以在其中查看针对特定产品/服务的所有用户请求。
1. 选择 " **批准** " 或 " **拒绝**"。

    [![显示 "批准" 和 "拒绝" 选项。](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. 从下拉菜单中选择要批准的计划。
1. 添加注释，然后选择 " **提交**"。

## <a name="browsing-private-azure-marketplace"></a>浏览私有 Azure Marketplace

启用专用 Azure Marketplace 后，用户将看到 Marketplace 管理员批准了哪些计划。

- 绿色 **批准** 通知表示已批准的合作伙伴 (非 Microsoft) 提议。
- 已 **批准** 的蓝色通知表示 Microsoft 产品/服务 (包括已批准的 [认可的 Linux 分发](/azure/virtual-machines/linux/endorsed-distros)) 。

用户可以筛选不是批准的产品/服务：

[![显示筛选选项。](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>在专用 Azure Marketplace 中购买或部署

虽然 "产品详细信息" 页面体验与全球 Azure Marketplace 类似，但有三个专用 Azure Marketplace 特定方案。

- 当用户选择已批准的计划时，将启用 " **创建** " 按钮：

    [![显示 "产品/服务" 标题，说明可以创建一个计划。](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- 如果产品计划选择未出现在 "产品详细信息" 页中，但管理员批准了一个或多个计划，则标题会说明批准了哪些计划并启用了 " **创建** " 按钮：

    [![显示 "产品/服务" 标题，指出可以创建计划并显示可用计划。](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- 当用户选择非批准的计划时，标题将说明 "未批准" 和 " **创建** " 按钮已禁用。 用户仍可以请求将计划添加到已批准列表中 (参阅下一部分) 。

## <a name="request-to-add-offers-or-plans"></a>添加产品/服务或计划的请求

可以请求添加 Azure 私有 Azure Marketplace 中当前未批准的公开提议或计划。

1. 选择要添加到横幅中的 **请求** 以打开 **访问请求窗体**。

    [![显示带有 "请求添加" 链接的横幅。](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![显示产品/服务或计划的访问请求窗体。](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. 选择要将哪些计划添加到请求 (**任何计划** 告诉 Marketplace 管理员你没有在产品/服务) 的计划。

1. 添加 " **理由** " 并选择 " **请求** " 以提交请求。
  
    [![显示具有示例条目的产品/服务或计划的访问请求窗体。](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. 针对挂起的请求的指示将显示在访问请求窗体中，其中包含用于 **撤消请求** 的选项。

    [![使用 "撤消请求" 链接显示批准或挂起的计划的列表。](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> 提交后，将向市场管理员发送批准请求窗体 [，以查看](#private-azure-marketplace-notification-center) 请求并采取措施。

## <a name="frequently-asked-questions-faqs"></a>常见问题解答 (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>我已通过 Azure 策略阻止 Marketplace 第三方应用程序。 这有何不同？

目前有两种方法可限制 Marketplace 中的第三方服务：

1. 通过 EA 门户或 Azure 门户禁用第三方服务，或将其限制为 "仅限免费或 BYOL Sku"。

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="演示如何限制 Azure 门户中的服务。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="演示如何限制 E A 门户中的服务。":::

2. 创建 Azure 策略以仅允许特定 Vm。 有关如何对 Windows Vm 强制执行策略的详细信息，请参阅 [使用 Azure 资源管理器将策略应用于 Windows vm](/azure/virtual-machines/windows/policy)。

私有 Azure Marketplace 可以更灵活地限制和允许特定的产品/服务和计划。 即使在尝试部署第三方服务之前，它也会通知最终用户在 marketplace 库中的部署是否可用。 若要允许部署第三方服务，请在 EA 门户和 Azure 门户中将 "Azure Marketplace" 设置为 "开/启用"。

- 私有 Azure Marketplace 可以组织不受限于虚拟机的合作伙伴解决方案。
- 私有 Azure Marketplace 可以组织计划级别，还可以设置 "当前和未来的计划"。
- 私有 Azure Marketplace 可以提前通知最终用户可以部署哪些内容。

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>专用产品/服务和专用 Azure Marketplace 之间的区别是什么？

通过 **专用产品/服务** ，发布者可以创建仅对目标客户可见的计划。 这样，他们就可以将自定义解决方案与协商定价、私有条款和条件以及专用配置私下共享。 有关详细信息，请参阅 [商业应用商店中的专用产品/服务](/azure/marketplace/private-offers)。

Azure 门户中的 **私有 Azure Marketplace** 使管理员能够预先批准其用户可以部署的第三方解决方案。 通过专用的 Azure Marketplace，用户可以通过查找、购买和部署符合要求的产品/服务来享受 Azure Marketplace 的权益。 若要在私有 Marketplace 中管理基于订阅的专用产品/服务，Marketplace 管理员在特定订阅上必须至少具有 "读取" 角色。

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>我将专用产品/服务添加到专用 Azure Marketplace，原因是它不会显示在 "管理 Marketplace" 选项卡中？

基于订阅的专用产品/服务仅对 "专用产品/服务" 设置中列出的订阅可见。 若要查看专用产品/服务，请确保全局订阅筛选器显示所有订阅。

[![显示 "专用 marketplace" 筛选器。](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>能否在专用 Azure Marketplace 中包含自定义映像？

不是。 通过专用 Azure Marketplace，任何 IT 管理员都可从全球 Azure Marketplace 管理和组织第三方解决方案。 由于自定义映像不在全球 Azure Marketplace 上，因此 IT 管理员无法选择自定义映像。 如果要共享自定义映像，请使用 [共享映像库](/azure/virtual-machines/shared-image-galleries)。

1.  ([CLI](/azure/virtual-machines/shared-images-cli)、 [POWERSHELL](/azure/virtual-machines/shared-images-powershell))  (SIG) 创建共享图像库的分步指南。
2. 在 SIG 中创建映像定义。 客户应为 "OS-状态" 字段选择 " **通用化** "。  ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)、 [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)) 。
3.  ([CLI](/azure/virtual-machines/image-version-managed-image-cli)、 [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)) 将托管映像引入共享映像库。
4. SIG VM 映像将驻留在一个订阅中。 若要使其可用于其他订阅，请使用 ([CLI](/azure/virtual-machines/linux/share-images-across-tenants)、 [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) 的应用注册。

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>为什么尽管发布商不是 Microsoft，也会看到一些 **默认情况下已批准** 的产品？

Microsoft 支持 Azure 中的 Linux 和开源技术。 Azure 支持[认可的 Linux 分发](/azure/virtual-machines/linux/endorsed-distros)版，并在虚拟机中集成了价格。 由于 Azure Linux 代理已预安装在 Azure Marketplace 上，因此将其视为 Microsoft 产品/服务。 由于 Microsoft 产品/服务默认已获批准，因此无法在专用 Azure Marketplace 中管理认可的 Linux 分发版，默认情况下已获得批准。

## <a name="contact-support"></a>联系支持人员

- 有关 Azure Marketplace 支持，请访问 [Microsoft 问答&](/answers/products/)。