---
title: 在专用 Azure 市场创建和管理Azure 门户
description: 了解如何在门户专用 Azure 市场 () 管理Azure 门户。 专用 Azure 市场 (预览版) 管理员可以控制其用户可以使用的第三方解决方案。
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173701"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>在专用 Azure 市场创建和管理Azure 门户

专用 Azure 市场管理员可以控制其用户可以使用的第三方解决方案。 它通过允许用户仅部署管理员批准且符合企业策略的优惠来实现此目标。 使用专用 Azure 市场，用户可以在在线商店中搜索要购买和部署的合规产品/服务。

作为市场管理员 (分配的角色) ，你将从已禁用且空的专用存储开始，可以在其中添加已批准的产品/服务与计划。 本文介绍如何分配所需角色、创建专用存储、管理项、批准用户请求，以及专用 Azure 市场用户。

> [!NOTE]
> - 专用 Azure 市场处于租户级别，因此租户下的所有用户都将看到相同的策展列表。
> - 所有 Microsoft 解决方案 (包括认可的 [Linux](/azure/virtual-machines/linux/endorsed-distros) 分发版) 自动添加到 专用 Azure 市场。

## <a name="assign-the-marketplace-admin-role"></a>分配市场管理员角色

租户全局管理员管理员必须将市场 **管理员** 角色分配给专用 Azure 市场管理专用存储的管理员。

>[!IMPORTANT]
> 只有专用 AZURE 市场市场管理员角色的 IT 管理员才能访问管理权限。

### <a name="prerequisites"></a>先决条件

在将"市场管理员"角色分配给租户范围的用户之前，需要满足以下先决条件：

- 你 **有权访问全局管理员用户** 。
- 租户至少有一个订阅 (可以是任何类型) 。
- 为全局管理员订阅分配参与者角色或更高级的用户。

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>为市场管理员角色分配访问控制 (IAM) 

1. 登录到 [Azure 门户](https://portal.azure.com/)。

1. 选择 **"所有服务"，** 然后选择"**市场"。**

1. 从 **专用市场** 菜单中选择"设置"。

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="在市场左侧显示专用市场菜单选项。":::

1. 选择 **"访问控制 (IAM)** 以分配市场管理员角色。

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="显示&quot;I A M 访问控制&quot;屏幕。":::

1. 选择“+ 添加”   >   “添加角色分配”。

1. 在"**角色"** 下，选择 **"市场管理员"。**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="显示&quot;角色分配&quot;菜单。":::

1. 从下拉列表中选择所需的用户，然后选择"完成 **"。**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>使用 PowerShell 分配市场管理员角色

使用以下 PowerShell 脚本分配"市场管理员"角色;它需要以下参数：

- **TenantId：** "市场管理员"角色 (租户的 ID 可分配给租户) 。
- **SubscriptionId：** 为其分配了全局管理员"参与者 **"** 角色或更高角色的订阅。
- **GlobalAdminUsername：** 全局管理员的用户名。
- **UsernameToAssignRoleFor：** 将为其分配市场管理员角色的用户名。

> [!NOTE]
> 对于受邀加入租户的来宾用户，可能需要最多 48 小时，直到其帐户可用于分配"市场管理员"角色。 有关详细信息，请参阅[B2B 协作Azure Active Directory的属性](/azure/active-directory/b2b/user-properties)。

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

有关 Az.Portal PowerShell 模块中包含的 cmdlet 详细信息，请参阅[Microsoft Azure PowerShell：门户仪表板 cmdlet。](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>创建专用 Azure 市场

1. 登录到 [Azure 门户](https://portal.azure.com/)。
2. 选择 **"所有服务"，** 然后选择"**市场"。**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="显示Azure 门户窗口。":::

3. 从 **专用市场** 菜单中选择"设置"。

4. 选择 **入门"专用 Azure 市场 (** 创建一次，只需执行一次) 。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="演示如何选择&quot;入门&quot;主Azure 门户&quot;。":::

    如果专用 Azure 市场租户已存在，则 **默认情况下** 将选择"管理市场"。

5. 完成后，将拥有一个空且已禁用专用 Azure 市场。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="显示空的专用 Azure 市场屏幕。":::

## <a name="add-items-from-gallery"></a>从库中添加项

项是套餐和计划的组合。 可以在"管理市场"页上搜索和添加项。

1. 选择"**添加项"。**

2. 浏览 **库或使用** 搜索字段查找想要的项目。

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="演示如何浏览库或使用搜索字段。":::

3. 默认情况下，添加新产品/服务时，所有当前计划都将添加到已批准列表中。 若要在添加所选项之前修改计划选择，请选择产品/服务磁贴中的下拉菜单并更新所需的计划。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="演示如何更新所需的计划。":::

4. 选择 **选择** 后，选择左下角的"完成"。

>[!Note]
> **将项** 添加到市场仅适用于非 Microsoft 产品/服务。 包括 ([Linux](/azure/virtual-machines/linux/endorsed-distros) 分发版) 的 Microsoft 解决方案将被标记为"默认批准"，并且无法在 专用市场。

## <a name="edit-items-plans"></a>编辑项的计划

可以在"管理市场"页上编辑项的计划。

1. 在" **计划** "列中，从该项的下拉菜单中查看可用计划。

2. 选中或清除复选框，以选择要为用户提供的计划。

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="演示如何选择或清除所需项的复选框。":::

   > [!NOTE]
   > 每个产品/服务至少需要选择一个计划，进行更新。 若要删除与套餐相关的所有计划，请删除整个套餐 (请参阅下一部分) 。

## <a name="delete-offers"></a>删除产品/服务

在"管理市场"页中，选中产品/服务名称旁边的复选框 (上方的屏幕) 选择"删除 **项"。**

## <a name="enabledisable-private-azure-marketplace"></a>启用/禁用专用 Azure 市场

在"管理市场"页中，你将看到以下横幅之一，其中显示了当前专用 Azure 市场：

:::image type="content" source="media/private-azure/state-disable.png" alt-text="显示&quot;禁用状态&quot;横幅。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="显示&quot;启用状态&quot;横幅。":::

可根据需要启用专用 Azure 市场禁用。

- 如果已禁用，请选择 **"启用专用市场** 启用" 。
- 如果已启用，请选择 **"禁用专用市场** 禁用" 。

## <a name="private-azure-marketplace-notification-center"></a>专用 Azure 市场通知中心

通知中心包含三种类型的通知，并允许市场管理员根据通知采取措施：

- 对于未在批准列表中的项目，用户 (请求添加以下产品/服务或) 。 [](#request-to-add-offers-or-plans)
- 已批准列表中已有一个或多个计划的套餐的新计划通知。
- 删除了已批准列表中但已从全局列表中删除的项的计划Azure 市场。

访问通知中心：

1. 从 **左侧** 菜单中选择"通知"。

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="显示&quot;通知&quot;菜单。":::

1. 选择省略号菜单以执行更多操作。

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="显示&quot;更多选项&quot;菜单结果。":::

1. 对于计划请求，" **显示** 请求"将打开审批请求表单，可在其中查看特定产品/服务的所有用户请求。
1. 选择 **"批准** 或拒绝 **"。**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="显示批准和拒绝选项。":::

1. 从下拉菜单中选择要批准的计划。
1. 添加注释，然后选择"提交 **"。**

## <a name="browsing-private-azure-marketplace"></a>浏览专用 Azure 市场

启用专用 Azure 市场后，用户将看到市场管理员已批准的计划。

- 绿色" **已批准** "通知指示合作伙伴 (批准的非 Microsoft) 产品/服务。
- 蓝色" **已批准** "通知表示 Microsoft (产品/服务，包括) 认可的 [Linux](/azure/virtual-machines/linux/endorsed-distros) 分发版。

用户可以在已批准和未批准的产品/服务之间进行筛选：

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="显示筛选选项。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>购买或部署专用 Azure 市场

虽然产品详细信息页面体验类似于全局Azure 市场，但有三专用 Azure 市场特定方案。

- 当用户选择已批准的计划时，将启用 **"创建** "按钮：

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="显示产品/服务横幅，表明可以创建计划。":::

- 如果产品计划选择未显示在产品详细信息页中，但管理员已批准了一个或多个计划，则横幅会记录哪些计划获得批准并启用" **创建"按钮** ：

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="显示产品/服务横幅，指出可以创建计划，并显示可用计划。":::

- 当用户选择未批准的计划时，横幅将计划注释为"未批准"，并禁用"创建"按钮。 用户仍可以请求将计划添加到已批准列表 (请参阅下一部分) 。

## <a name="request-to-add-offers-or-plans"></a>请求添加套餐或计划

可以请求添加当前未在计划中添加专用 Azure 市场。

1. 选择 **"请求"以** 在横幅中添加 ，打开" **访问请求"窗体**。

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="显示包含&quot;请求添加&quot;链接的横幅。":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="显示套餐或计划的访问请求窗体。":::

1. 选择要添加到请求的计划 ("任何计划"都告知市场管理员，你对于套餐中的计划没有) 。

1. 添加理由 **并选择** " **请求** "以提交请求。

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="显示包含示例条目的套餐或计划的访问请求表单。":::

1. "访问请求"窗体中将显示挂起请求的指示，其选项为 **"撤消请求"。**

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="显示包含&quot;撤消请求&quot;链接的已批准或挂起计划的列表。":::

> [!NOTE]
> 提交后，审批请求表单将发送到通知中心，供市场[](#private-azure-marketplace-notification-center)管理员查看请求并采取措施。

> [!CAUTION]
> 批准专用市场并不表示已采购解决方案。

## <a name="frequently-asked-questions-faqs"></a>常见问题解答 (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>我已阻止市场第三方应用程序通过 Azure Policy。 这有多不同？

目前，有两种方法可以限制市场中的第三方服务：

1. 通过 EA 门户或Azure 门户，禁用第三方服务或限制为"免费或 BYOL SKUS"。

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="演示如何限制服务中的Azure 门户。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="演示如何在 E A 门户中限制服务。":::

2. 创建仅允许特定 VM 的 Azure 策略。 若要详细了解如何强制实施策略来Windows VM，请参阅将策略Windows [VM Azure 资源管理器。](/azure/virtual-machines/windows/policy)

专用 Azure 市场可以更灵活地限制和允许特定的套餐和计划。 它通知最终用户在尝试部署第三方服务之前，在市场库中部署的可用性。 若要允许部署第三方服务，请Azure 市场中将"EA 门户"设置为"Azure 门户"。

- 专用 Azure 市场可以组织合作伙伴解决方案，而不限于虚拟机。
- 专用 Azure 市场可在计划级别进行组织，还可以设置"当前和未来计划"。
- 专用 Azure 市场可以提前通知最终用户可以部署和不能部署哪些内容。

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>专用产品/服务与专用服务之间有什么专用 Azure 市场？

专用 **套餐** 允许发布者创建仅对目标客户可见的计划。 这样，他们可私密共享自定义解决方案，并采用协商定价、专用条款和条件以及专用配置。 有关详细信息，请参阅 [商业市场中的专用产品/服务](/azure/marketplace/private-offers)。

**专用 Azure 市场** 中Azure 门户管理员可以预先批准其用户可以部署的第三方解决方案。 借助专用 Azure 市场，用户可以通过查找、Azure 市场和部署合规产品/服务来享受产品/服务的好处。 若要在 专用市场 中管理基于订阅的专用产品/服务，市场管理员必须对特定订阅至少具有"读取"角色。

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>我向市场添加了专用专用 Azure 市场，为什么它未显示在"管理市场"选项卡中？

基于订阅的专用套餐仅对"专用套餐"设置中所列的订阅可见。 若要查看专用套餐，请确保全局订阅筛选器显示所有订阅。

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="显示专用市场筛选器。":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>我们能否在映像中包括自定义专用 Azure 市场？

否。 专用 Azure 市场允许任何 IT 管理员管理和策展来自全球客户的第三方Azure 市场。 由于自定义映像不在全局Azure 市场，因此 IT 管理员无法选取和选择自定义映像。 若要共享自定义映像，请使用 [共享映像库](/azure/virtual-machines/shared-image-galleries)。

1. 分步指南使用 SIG ([CLI、PowerShell](/azure/virtual-machines/shared-images-powershell))  (创建共享映像) 。 [](/azure/virtual-machines/shared-images-cli)
2. 在 SIG 内创建映像定义。 客户应为"OS **状态"** 字段选择"通用化"。  ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [、PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)) 。
3. 使用[CLI、PowerShell](/azure/virtual-machines/image-version-managed-image-powershell) (将托管映像引入[](/azure/virtual-machines/image-version-managed-image-cli)共享) 。
4. SIG VM 映像将驻留在一个订阅中。 若要使其可供其他订阅使用，请通过 [CLI](/azure/virtual-machines/linux/share-images-across-tenants) ([PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) 。

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>为什么即使发布者不是 Microsoft，也看到默认批准的某些产品/服务？ 

Microsoft 支持 Azure 中的 Linux 和开源技术。 [Azure 支持](/azure/virtual-machines/linux/endorsed-distros) 认可的 Linux 分发版，价格已集成到虚拟机中。 由于 Azure Linux 代理已预安装在 Azure 市场，因此它被视为 Microsoft 产品/服务。 由于 Microsoft 产品/服务是默认批准的，因此无法在 专用 Azure 市场中管理认可的 Linux 分发版，并且默认情况下会获得批准。

## <a name="contact-support"></a>联系支持人员

- 有关Azure 市场，请访问[Microsoft Q&A。](/answers/products/)