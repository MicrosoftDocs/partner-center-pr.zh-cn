---
title: 在 Azure 门户中创建和管理专用 Azure Marketplace
description: 了解如何创建和管理专用 Azure Marketplace (预览) 在 Azure 门户中。 专用 Azure Marketplace (预览版) 使管理员可以控制其用户可以使用的第三方解决方案。
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 2459e7841c2c33227ad38f9d6fa1fc139fc0326e
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439258"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>在 Azure 门户中创建和管理私有 Azure Marketplace (预览) 

专用 Azure Marketplace (预览版) 使管理员可以控制其用户可以使用的第三方解决方案。 它通过允许你仅部署你批准并符合企业策略的产品/服务来实现此功能。 通过专用 Azure Marketplace，你的用户可以在在线商店中搜索适用于购买和部署的符合性产品/服务。 

作为 Marketplace 管理员 (分配的角色) ，你将从一个禁用且空的私有存储开始，你可以在其中添加已批准的产品/服务和计划。 本文介绍如何为用户创建、管理和启用专用 Azure Marketplace。

注意：

- Azure Marketplace 专用于租户级别，因此租户下的所有用户都将看到相同的特选列表。
- 所有 Microsoft 解决方案都将自动添加到专用 Azure Marketplace。

## <a name="assign-the-marketplace-admin-role"></a>分配 Marketplace 管理员角色

租户全局管理员必须将 **Marketplace 管理员** 角色分配给将管理专用存储的专用 Azure Marketplace 管理员。

>[!IMPORTANT]
> 只有分配有 Marketplace 管理员角色的 IT 管理员才能访问专用 Azure Marketplace 管理。

### <a name="prerequisites"></a>先决条件

必须满足这些先决条件，然后才能将 Marketplace 管理员角色分配给租户范围内的用户：

- 你有权访问 **全局管理员** 用户。
- 租户至少有一个订阅 (可以是任何类型) 。
- 为全局管理员用户分配所选订阅的 " **参与者** " 角色或更高级别。
- 全局管理员用户已将访问权限设置为 **"是"** (参阅 " [提升访问权限以管理所有 Azure 订阅和管理组](/azure/role-based-access-control/elevate-access-global-admin) ") 。

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

有关 Az PowerShell 模块中包含的 cmdlet 的详细信息，请参阅 [Microsoft Azure PowerShell：门户面板 cmdlet](/powershell/module/az.portal/)。

## <a name="create-private-azure-marketplace"></a>创建专用 Azure Marketplace

1. 登录 [Azure 门户](https://portal.azure.com/)。
2. 选择 " **所有服务** "，然后选择 " **Marketplace**"。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure 门户主窗口。":::

3. 从左侧的选项中选择 " **专用 Marketplace** "。

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="在 Azure 门户主窗口上选择 &quot;专用 Marketplace&quot;。":::

4. 选择 " **开始** 使用" 创建专用 Azure Marketplace (你只需) 完成此操作。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="选择 Azure 门户主窗口上的 &quot;开始&quot;。":::

    如果此租户已存在专用 Azure Marketplace，则默认情况下将选择 " **管理 marketplace** "。

5. 完成后，你将拥有一个空且已禁用的专用 Azure Marketplace。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空的专用 Azure Marketplace 屏幕。":::

## <a name="add-items-from-gallery"></a>从库中添加项

项是产品/服务和计划的组合。 你可以在 "管理应用商店" 页中搜索和添加项。

1. 选择 " **添加项**"。

2. 浏览 **库** ，或使用搜索字段查找所需的项。

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="浏览库或使用搜索字段。":::

3. 默认情况下，在添加新产品/服务时，所有当前计划将添加到 "允许列表"。 若要在添加选定项之前修改计划选择，请在产品的磁贴中选择下拉菜单，并更新所需的计划。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="更新所需的计划。":::

4. 做出选择后，请选择左下角的 " **完成** "。

>[!Note]
> 将 **项目添加** 到 Marketplace 仅适用于非 Microsoft 产品/服务。 默认情况下允许 Microsoft 产品/服务。

## <a name="edit-item-plans"></a>编辑项计划

你可以在 "管理应用商店" 页中编辑项的计划。

1. 在 " **计划** " 列中，查看该项的下拉菜单中的可用计划。
2. 选中或清除相应的复选框，以选择要对用户提供哪些计划。

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="选中或清除所需项的复选框。":::

> [!NOTE]
> 每个服务都需要至少选择一个计划才能进行更新。 若要删除与产品/服务相关的所有计划，请删除整个提议 (参阅下一部分) 。

## <a name="delete-offers"></a>删除产品/服务

在 "管理应用商店" 页上，选中 "产品/服务名称" 旁边的复选框 (参阅上方的屏幕) 并选择 " **删除项目**"。

## <a name="enabledisable-private-azure-marketplace"></a>启用/禁用专用 Azure Marketplace

在 "管理应用商店" 页上，你将看到其中一个横幅，其中显示了专用 Azure Marketplace 的当前状态：

:::image type="content" source="media/private-azure/state-disable.png" alt-text="禁用状态横幅":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="启用状态横幅":::

你可以根据需要启用或禁用专用 Azure Marketplace。

1. 如果已禁用，请选择 " **启用专用 Marketplace** " 启用。
2. 如果已启用，请选择 **禁用专用 Marketplace** 禁用。

## <a name="browsing-private-azure-marketplace"></a>浏览私有 Azure Marketplace

启用专用 Azure Marketplace 后，用户将看到 Marketplace 管理员允许哪些计划。

- 绿色 **允许** 通知表示允许 (非 Microsoft) 提议的合作伙伴。
- 蓝色 **允许** 通知表示允许的 Microsoft 产品。

用户可以筛选不允许使用的产品/服务：

:::image type="content" source="media/private-azure/filter-option.png" alt-text="筛选选项。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>在专用 Azure Marketplace 中购买或部署

虽然 "产品详细信息" 页面体验类似于公共 Azure Marketplace，但有三个专用的 Azure Marketplace 特定方案。

- 当用户选择允许的计划时，将启用 " **创建** " 按钮：

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="提供横幅说明可以创建一个计划。":::

- 如果用户选择了不允许的计划，则会出现一个横幅，指出不允许该计划，并且禁用了 " **创建** " 按钮。

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="提供横幅指出，无法创建计划。":::

- 如果产品计划选择未出现在 "产品详细信息" 页中，但管理员批准了一个或多个计划，则标题会说明允许哪些计划，并启用了 " **创建** " 按钮：

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="提供横幅指出，可以创建计划并显示可用计划。":::

## <a name="contact-support"></a>联系支持

有关 Azure Marketplace 支持，请访问 [Microsoft 问答&](/answers/products/)。 
