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
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="e82e8-104">在 Azure 门户中创建和管理私有 Azure Marketplace (预览) </span><span class="sxs-lookup"><span data-stu-id="e82e8-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="e82e8-105">专用 Azure Marketplace (预览版) 使管理员可以控制其用户可以使用的第三方解决方案。</span><span class="sxs-lookup"><span data-stu-id="e82e8-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="e82e8-106">它通过允许你仅部署你批准并符合企业策略的产品/服务来实现此功能。</span><span class="sxs-lookup"><span data-stu-id="e82e8-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="e82e8-107">通过专用 Azure Marketplace，你的用户可以在在线商店中搜索适用于购买和部署的符合性产品/服务。</span><span class="sxs-lookup"><span data-stu-id="e82e8-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="e82e8-108">作为 Marketplace 管理员 (分配的角色) ，你将从一个禁用且空的私有存储开始，你可以在其中添加已批准的产品/服务和计划。</span><span class="sxs-lookup"><span data-stu-id="e82e8-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="e82e8-109">本文介绍如何为用户创建、管理和启用专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="e82e8-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="e82e8-110">注意：</span><span class="sxs-lookup"><span data-stu-id="e82e8-110">Notes:</span></span>

- <span data-ttu-id="e82e8-111">Azure Marketplace 专用于租户级别，因此租户下的所有用户都将看到相同的特选列表。</span><span class="sxs-lookup"><span data-stu-id="e82e8-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="e82e8-112">所有 Microsoft 解决方案都将自动添加到专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="e82e8-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="e82e8-113">分配 Marketplace 管理员角色</span><span class="sxs-lookup"><span data-stu-id="e82e8-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="e82e8-114">租户全局管理员必须将 **Marketplace 管理员** 角色分配给将管理专用存储的专用 Azure Marketplace 管理员。</span><span class="sxs-lookup"><span data-stu-id="e82e8-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="e82e8-115">只有分配有 Marketplace 管理员角色的 IT 管理员才能访问专用 Azure Marketplace 管理。</span><span class="sxs-lookup"><span data-stu-id="e82e8-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="e82e8-116">先决条件</span><span class="sxs-lookup"><span data-stu-id="e82e8-116">Prerequisites</span></span>

<span data-ttu-id="e82e8-117">必须满足这些先决条件，然后才能将 Marketplace 管理员角色分配给租户范围内的用户：</span><span class="sxs-lookup"><span data-stu-id="e82e8-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="e82e8-118">你有权访问 **全局管理员** 用户。</span><span class="sxs-lookup"><span data-stu-id="e82e8-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="e82e8-119">租户至少有一个订阅 (可以是任何类型) 。</span><span class="sxs-lookup"><span data-stu-id="e82e8-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="e82e8-120">为全局管理员用户分配所选订阅的 " **参与者** " 角色或更高级别。</span><span class="sxs-lookup"><span data-stu-id="e82e8-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="e82e8-121">全局管理员用户已将访问权限设置为 **"是"** (参阅 " [提升访问权限以管理所有 Azure 订阅和管理组](/azure/role-based-access-control/elevate-access-global-admin) ") 。</span><span class="sxs-lookup"><span data-stu-id="e82e8-121">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="e82e8-122">向 PowerShell 分配 Marketplace 管理员角色</span><span class="sxs-lookup"><span data-stu-id="e82e8-122">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="e82e8-123">使用以下 PowerShell 脚本分配 Marketplace 管理员角色;它需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="e82e8-123">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="e82e8-124">**TenantId：** 范围 (Marketplace 管理员角色的租户的 ID 可在租户范围) 上分配。</span><span class="sxs-lookup"><span data-stu-id="e82e8-124">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="e82e8-125">**SubscriptionId：** 全局管理员具有 **参与者** 角色或分配更高的订阅。</span><span class="sxs-lookup"><span data-stu-id="e82e8-125">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="e82e8-126">**GlobalAdminUsername：** 全局管理员的用户名。</span><span class="sxs-lookup"><span data-stu-id="e82e8-126">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="e82e8-127">**UsernameToAssignRoleFor：** 将向其分配 Marketplace 管理员角色的用户名。</span><span class="sxs-lookup"><span data-stu-id="e82e8-127">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="e82e8-128">对于受邀加入租户的来宾用户，最多可能需要48小时才能分配给 Marketplace 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e82e8-128">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="e82e8-129">有关详细信息，请参阅 [AZURE ACTIVE DIRECTORY B2B 协作用户的属性](/azure/active-directory/b2b/user-properties)。</span><span class="sxs-lookup"><span data-stu-id="e82e8-129">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="e82e8-130">有关 Az PowerShell 模块中包含的 cmdlet 的详细信息，请参阅 [Microsoft Azure PowerShell：门户面板 cmdlet](/powershell/module/az.portal/)。</span><span class="sxs-lookup"><span data-stu-id="e82e8-130">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="e82e8-131">创建专用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="e82e8-131">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="e82e8-132">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="e82e8-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="e82e8-133">选择 " **所有服务** "，然后选择 " **Marketplace**"。</span><span class="sxs-lookup"><span data-stu-id="e82e8-133">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure 门户主窗口。":::

3. <span data-ttu-id="e82e8-135">从左侧的选项中选择 " **专用 Marketplace** "。</span><span class="sxs-lookup"><span data-stu-id="e82e8-135">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="在 Azure 门户主窗口上选择 &quot;专用 Marketplace&quot;。":::

4. <span data-ttu-id="e82e8-137">选择 " **开始** 使用" 创建专用 Azure Marketplace (你只需) 完成此操作。</span><span class="sxs-lookup"><span data-stu-id="e82e8-137">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="选择 Azure 门户主窗口上的 &quot;开始&quot;。":::

    <span data-ttu-id="e82e8-139">如果此租户已存在专用 Azure Marketplace，则默认情况下将选择 " **管理 marketplace** "。</span><span class="sxs-lookup"><span data-stu-id="e82e8-139">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="e82e8-140">完成后，你将拥有一个空且已禁用的专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="e82e8-140">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空的专用 Azure Marketplace 屏幕。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="e82e8-142">从库中添加项</span><span class="sxs-lookup"><span data-stu-id="e82e8-142">Add items from gallery</span></span>

<span data-ttu-id="e82e8-143">项是产品/服务和计划的组合。</span><span class="sxs-lookup"><span data-stu-id="e82e8-143">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="e82e8-144">你可以在 "管理应用商店" 页中搜索和添加项。</span><span class="sxs-lookup"><span data-stu-id="e82e8-144">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="e82e8-145">选择 " **添加项**"。</span><span class="sxs-lookup"><span data-stu-id="e82e8-145">Select **Add items**.</span></span>

2. <span data-ttu-id="e82e8-146">浏览 **库** ，或使用搜索字段查找所需的项。</span><span class="sxs-lookup"><span data-stu-id="e82e8-146">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="浏览库或使用搜索字段。":::

3. <span data-ttu-id="e82e8-148">默认情况下，在添加新产品/服务时，所有当前计划将添加到 "允许列表"。</span><span class="sxs-lookup"><span data-stu-id="e82e8-148">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="e82e8-149">若要在添加选定项之前修改计划选择，请在产品的磁贴中选择下拉菜单，并更新所需的计划。</span><span class="sxs-lookup"><span data-stu-id="e82e8-149">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="更新所需的计划。":::

4. <span data-ttu-id="e82e8-151">做出选择后，请选择左下角的 " **完成** "。</span><span class="sxs-lookup"><span data-stu-id="e82e8-151">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="e82e8-152">将 **项目添加** 到 Marketplace 仅适用于非 Microsoft 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="e82e8-152">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="e82e8-153">默认情况下允许 Microsoft 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="e82e8-153">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="e82e8-154">编辑项计划</span><span class="sxs-lookup"><span data-stu-id="e82e8-154">Edit item plans</span></span>

<span data-ttu-id="e82e8-155">你可以在 "管理应用商店" 页中编辑项的计划。</span><span class="sxs-lookup"><span data-stu-id="e82e8-155">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="e82e8-156">在 " **计划** " 列中，查看该项的下拉菜单中的可用计划。</span><span class="sxs-lookup"><span data-stu-id="e82e8-156">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="e82e8-157">选中或清除相应的复选框，以选择要对用户提供哪些计划。</span><span class="sxs-lookup"><span data-stu-id="e82e8-157">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="选中或清除所需项的复选框。":::

> [!NOTE]
> <span data-ttu-id="e82e8-159">每个服务都需要至少选择一个计划才能进行更新。</span><span class="sxs-lookup"><span data-stu-id="e82e8-159">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="e82e8-160">若要删除与产品/服务相关的所有计划，请删除整个提议 (参阅下一部分) 。</span><span class="sxs-lookup"><span data-stu-id="e82e8-160">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="e82e8-161">删除产品/服务</span><span class="sxs-lookup"><span data-stu-id="e82e8-161">Delete offers</span></span>

<span data-ttu-id="e82e8-162">在 "管理应用商店" 页上，选中 "产品/服务名称" 旁边的复选框 (参阅上方的屏幕) 并选择 " **删除项目**"。</span><span class="sxs-lookup"><span data-stu-id="e82e8-162">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="e82e8-163">启用/禁用专用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="e82e8-163">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="e82e8-164">在 "管理应用商店" 页上，你将看到其中一个横幅，其中显示了专用 Azure Marketplace 的当前状态：</span><span class="sxs-lookup"><span data-stu-id="e82e8-164">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="禁用状态横幅":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="启用状态横幅":::

<span data-ttu-id="e82e8-167">你可以根据需要启用或禁用专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="e82e8-167">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="e82e8-168">如果已禁用，请选择 " **启用专用 Marketplace** " 启用。</span><span class="sxs-lookup"><span data-stu-id="e82e8-168">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="e82e8-169">如果已启用，请选择 **禁用专用 Marketplace** 禁用。</span><span class="sxs-lookup"><span data-stu-id="e82e8-169">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="e82e8-170">浏览私有 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="e82e8-170">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="e82e8-171">启用专用 Azure Marketplace 后，用户将看到 Marketplace 管理员允许哪些计划。</span><span class="sxs-lookup"><span data-stu-id="e82e8-171">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="e82e8-172">绿色 **允许** 通知表示允许 (非 Microsoft) 提议的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="e82e8-172">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="e82e8-173">蓝色 **允许** 通知表示允许的 Microsoft 产品。</span><span class="sxs-lookup"><span data-stu-id="e82e8-173">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="e82e8-174">用户可以筛选不允许使用的产品/服务：</span><span class="sxs-lookup"><span data-stu-id="e82e8-174">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="筛选选项。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="e82e8-176">在专用 Azure Marketplace 中购买或部署</span><span class="sxs-lookup"><span data-stu-id="e82e8-176">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="e82e8-177">虽然 "产品详细信息" 页面体验类似于公共 Azure Marketplace，但有三个专用的 Azure Marketplace 特定方案。</span><span class="sxs-lookup"><span data-stu-id="e82e8-177">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="e82e8-178">当用户选择允许的计划时，将启用 " **创建** " 按钮：</span><span class="sxs-lookup"><span data-stu-id="e82e8-178">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="提供横幅说明可以创建一个计划。":::

- <span data-ttu-id="e82e8-180">如果用户选择了不允许的计划，则会出现一个横幅，指出不允许该计划，并且禁用了 " **创建** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="e82e8-180">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="提供横幅指出，无法创建计划。":::

- <span data-ttu-id="e82e8-182">如果产品计划选择未出现在 "产品详细信息" 页中，但管理员批准了一个或多个计划，则标题会说明允许哪些计划，并启用了 " **创建** " 按钮：</span><span class="sxs-lookup"><span data-stu-id="e82e8-182">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="提供横幅指出，可以创建计划并显示可用计划。":::

## <a name="contact-support"></a><span data-ttu-id="e82e8-184">联系支持</span><span class="sxs-lookup"><span data-stu-id="e82e8-184">Contact support</span></span>

<span data-ttu-id="e82e8-185">有关 Azure Marketplace 支持，请访问 [Microsoft 问答&](/answers/products/)。</span><span class="sxs-lookup"><span data-stu-id="e82e8-185">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
