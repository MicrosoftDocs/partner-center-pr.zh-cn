---
title: 在 Azure 门户中创建和管理专用 Azure Marketplace
description: 了解如何创建和管理专用 Azure Marketplace (预览) 在 Azure 门户中。 专用 Azure Marketplace (预览版) 使管理员可以控制其用户可以使用的第三方解决方案。
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "101757073"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="44a40-104">在 Azure 门户中创建和管理专用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="44a40-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="44a40-105">私有 Azure Marketplace 使管理员可以控制其用户可以使用的第三方解决方案。</span><span class="sxs-lookup"><span data-stu-id="44a40-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="44a40-106">它通过允许用户仅部署管理员批准并符合企业策略的产品/服务来实现此功能。</span><span class="sxs-lookup"><span data-stu-id="44a40-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="44a40-107">通过专用 Azure Marketplace，用户可以在在线商店中搜索符合要求的产品/服务以购买和部署。</span><span class="sxs-lookup"><span data-stu-id="44a40-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="44a40-108">作为 Marketplace 管理员 (分配的角色) ，你将从一个禁用且空的私有存储开始，你可以在其中添加已批准的产品/服务和计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="44a40-109">本文介绍如何分配所需的角色、创建专用存储、管理项目、批准用户请求，并为用户启用私有 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="44a40-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="44a40-110">Azure Marketplace 专用于租户级别，因此租户下的所有用户都将看到相同的特选列表。</span><span class="sxs-lookup"><span data-stu-id="44a40-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="44a40-111">所有 Microsoft 解决方案 (包括 [认可的 Linux 分发](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) 自动添加到专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="44a40-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="44a40-112">分配 Marketplace 管理员角色</span><span class="sxs-lookup"><span data-stu-id="44a40-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="44a40-113">租户全局管理员必须将 **Marketplace 管理员** 角色分配给将管理专用存储的专用 Azure Marketplace 管理员。</span><span class="sxs-lookup"><span data-stu-id="44a40-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="44a40-114">只有分配有 Marketplace 管理员角色的 IT 管理员才能访问专用 Azure Marketplace 管理。</span><span class="sxs-lookup"><span data-stu-id="44a40-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="44a40-115">先决条件</span><span class="sxs-lookup"><span data-stu-id="44a40-115">Prerequisites</span></span>

<span data-ttu-id="44a40-116">在将 Marketplace 管理员角色分配给租户范围内的用户之前，需要满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="44a40-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="44a40-117">你有权访问 **全局管理员** 用户。</span><span class="sxs-lookup"><span data-stu-id="44a40-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="44a40-118">租户至少有一个订阅 (可以是任何类型) 。</span><span class="sxs-lookup"><span data-stu-id="44a40-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="44a40-119">为全局管理员用户分配所选订阅的 " **参与者** " 角色或更高级别。</span><span class="sxs-lookup"><span data-stu-id="44a40-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="44a40-120">使用访问控制 (IAM 分配 Marketplace 管理员角色) </span><span class="sxs-lookup"><span data-stu-id="44a40-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="44a40-121">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="44a40-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="44a40-122">选择 " **所有服务** "，然后选择 " **Marketplace**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="44a40-123">从左侧菜单中选择 " **专用 Marketplace** "。</span><span class="sxs-lookup"><span data-stu-id="44a40-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="44a40-124">[![在 Marketplace 的左侧显示 "专用市场" 菜单选项。](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="44a40-125">选择 **(IAM) 的 "访问控制** " 以分配 Marketplace 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="44a40-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="显示 I A M 访问控制屏幕。":::

1. <span data-ttu-id="44a40-127">选择“+ 添加”   >   “添加角色分配”。</span><span class="sxs-lookup"><span data-stu-id="44a40-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="44a40-128">在 " **角色**" 下，选择 " **Marketplace 管理**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="显示 &quot;角色分配&quot; 菜单。":::

1. <span data-ttu-id="44a40-130">从下拉列表中选择所需的用户，然后选择 " **完成**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="44a40-131">向 PowerShell 分配 Marketplace 管理员角色</span><span class="sxs-lookup"><span data-stu-id="44a40-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="44a40-132">使用以下 PowerShell 脚本分配 Marketplace 管理员角色;它需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="44a40-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="44a40-133">**TenantId：** 范围 (Marketplace 管理员角色的租户的 ID 可在租户范围) 上分配。</span><span class="sxs-lookup"><span data-stu-id="44a40-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="44a40-134">**SubscriptionId：** 全局管理员具有 **参与者** 角色或分配更高的订阅。</span><span class="sxs-lookup"><span data-stu-id="44a40-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="44a40-135">**GlobalAdminUsername：** 全局管理员的用户名。</span><span class="sxs-lookup"><span data-stu-id="44a40-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="44a40-136">**UsernameToAssignRoleFor：** 将向其分配 Marketplace 管理员角色的用户名。</span><span class="sxs-lookup"><span data-stu-id="44a40-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="44a40-137">对于受邀加入租户的来宾用户，最多可能需要48小时才能分配给 Marketplace 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="44a40-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="44a40-138">有关详细信息，请参阅 [AZURE ACTIVE DIRECTORY B2B 协作用户的属性](/azure/active-directory/b2b/user-properties)。</span><span class="sxs-lookup"><span data-stu-id="44a40-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="44a40-139">有关 Az PowerShell 模块中包含的 cmdlet 的详细信息，请参阅 [Microsoft Azure PowerShell：门户面板 cmdlet](/powershell/module/az.portal/)。</span><span class="sxs-lookup"><span data-stu-id="44a40-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="44a40-140">创建专用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="44a40-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="44a40-141">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="44a40-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="44a40-142">选择 " **所有服务** "，然后选择 " **Marketplace**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="显示 Azure 门户主窗口。":::

3. <span data-ttu-id="44a40-144">从左侧菜单中选择 " **专用 Marketplace** "。</span><span class="sxs-lookup"><span data-stu-id="44a40-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="44a40-145">选择 " **开始** 使用" 创建专用 Azure Marketplace (你只需) 完成此操作。</span><span class="sxs-lookup"><span data-stu-id="44a40-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="说明如何选择 &quot;Azure 门户&quot; 主窗口中的 &quot;入门&quot;。":::

    <span data-ttu-id="44a40-147">如果此租户已存在专用 Azure Marketplace，则默认情况下将选择 " **管理 marketplace** "。</span><span class="sxs-lookup"><span data-stu-id="44a40-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="44a40-148">完成后，你将拥有一个空且已禁用的专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="44a40-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="显示空的专用 Azure Marketplace 屏幕。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="44a40-150">从库中添加项</span><span class="sxs-lookup"><span data-stu-id="44a40-150">Add items from gallery</span></span>

<span data-ttu-id="44a40-151">项是产品/服务和计划的组合。</span><span class="sxs-lookup"><span data-stu-id="44a40-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="44a40-152">你可以在 "管理应用商店" 页上搜索和添加项。</span><span class="sxs-lookup"><span data-stu-id="44a40-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="44a40-153">选择 " **添加项**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-153">Select **Add items**.</span></span>

2. <span data-ttu-id="44a40-154">浏览 **库** ，或使用搜索字段查找所需的项。</span><span class="sxs-lookup"><span data-stu-id="44a40-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="44a40-155">[![演示如何浏览库或使用搜索字段。](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="44a40-156">默认情况下，在添加新产品/服务时，所有当前计划将添加到 "已批准" 列表中。</span><span class="sxs-lookup"><span data-stu-id="44a40-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="44a40-157">若要在添加选定项之前修改计划选择，请在产品的磁贴中选择下拉菜单，并更新所需的计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="说明如何更新所需的计划。":::

4. <span data-ttu-id="44a40-159">做出选择后，请选择左下角的 " **完成** "。</span><span class="sxs-lookup"><span data-stu-id="44a40-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="44a40-160">将 **项目添加** 到 Marketplace 仅适用于非 Microsoft 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="44a40-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="44a40-161">包括 [认可的 Linux 分发](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) (的 Microsoft 解决方案) 将被标记为 "默认情况下获得批准"，并且不能在私有 Marketplace 中进行管理。</span><span class="sxs-lookup"><span data-stu-id="44a40-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="44a40-162">编辑项的计划</span><span class="sxs-lookup"><span data-stu-id="44a40-162">Edit item's plans</span></span>

<span data-ttu-id="44a40-163">你可以在 "管理应用商店" 页上编辑项的计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="44a40-164">在 " **计划** " 列中，查看该项的下拉菜单中的可用计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="44a40-165">选中或清除相应的复选框，以选择要对用户提供哪些计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="演示如何选中或清除所需项的复选框。":::

> [!NOTE]
> <span data-ttu-id="44a40-167">每个产品/服务至少需要选择一个计划才能进行更新。</span><span class="sxs-lookup"><span data-stu-id="44a40-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="44a40-168">若要删除与产品/服务相关的所有计划，请删除整个提议 (参阅下一部分) 。</span><span class="sxs-lookup"><span data-stu-id="44a40-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="44a40-169">删除产品/服务</span><span class="sxs-lookup"><span data-stu-id="44a40-169">Delete offers</span></span>

<span data-ttu-id="44a40-170">在 "管理应用商店" 页上，选中 "产品/服务名称" 旁边的复选框 (参阅上方的屏幕) 并选择 " **删除项目**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="44a40-171">启用/禁用专用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="44a40-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="44a40-172">在 "管理应用商店" 页上，你将看到其中一个横幅，其中显示了专用 Azure Marketplace 的当前状态：</span><span class="sxs-lookup"><span data-stu-id="44a40-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="显示 &quot;禁用状态&quot; 横幅。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="显示 &quot;启用状态&quot; 横幅。":::

<span data-ttu-id="44a40-175">你可以根据需要启用或禁用专用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="44a40-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="44a40-176">如果已禁用，请选择 " **启用专用 Marketplace** " 启用。</span><span class="sxs-lookup"><span data-stu-id="44a40-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="44a40-177">如果已启用，请选择 **禁用专用 Marketplace** 禁用。</span><span class="sxs-lookup"><span data-stu-id="44a40-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="44a40-178">私有 Azure Marketplace 通知中心</span><span class="sxs-lookup"><span data-stu-id="44a40-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="44a40-179">通知中心包含三种类型的通知，并允许 Marketplace 管理员根据通知执行操作：</span><span class="sxs-lookup"><span data-stu-id="44a40-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="44a40-180">来自用户的针对不在已批准列表中的项目的审批请求 (参阅下面) 中 [添加产品/服务的请求](#request-to-add-offers-or-plans) 。</span><span class="sxs-lookup"><span data-stu-id="44a40-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="44a40-181">已在批准列表中有一个或多个计划的产品/服务的新计划通知。</span><span class="sxs-lookup"><span data-stu-id="44a40-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="44a40-182">已删除批准列表中的项目的计划通知，但已将其从全局 Azure Marketplace 中删除。</span><span class="sxs-lookup"><span data-stu-id="44a40-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="44a40-183">访问通知中心：</span><span class="sxs-lookup"><span data-stu-id="44a40-183">To access the notification center:</span></span>

1. <span data-ttu-id="44a40-184">从左侧菜单中选择 " **通知** "。</span><span class="sxs-lookup"><span data-stu-id="44a40-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="44a40-185">[![显示 "通知" 菜单。](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="44a40-186">选择省略号菜单以获取更多操作。</span><span class="sxs-lookup"><span data-stu-id="44a40-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="显示 &quot;更多选项&quot; 菜单结果。":::

1. <span data-ttu-id="44a40-188">对于计划请求，" **显示请求** " 将打开 "批准请求" 表单，你可以在其中查看针对特定产品/服务的所有用户请求。</span><span class="sxs-lookup"><span data-stu-id="44a40-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="44a40-189">选择 " **批准** " 或 " **拒绝**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="44a40-190">[![显示 "批准" 和 "拒绝" 选项。](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="44a40-191">从下拉菜单中选择要批准的计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="44a40-192">添加注释，然后选择 " **提交**"。</span><span class="sxs-lookup"><span data-stu-id="44a40-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="44a40-193">浏览私有 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="44a40-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="44a40-194">启用专用 Azure Marketplace 后，用户将看到 Marketplace 管理员批准了哪些计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="44a40-195">绿色 **批准** 通知表示已批准的合作伙伴 (非 Microsoft) 提议。</span><span class="sxs-lookup"><span data-stu-id="44a40-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="44a40-196">已 **批准** 的蓝色通知表示 Microsoft 产品/服务 (包括已批准的 [认可的 Linux 分发](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) 。</span><span class="sxs-lookup"><span data-stu-id="44a40-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="44a40-197">用户可以筛选不是批准的产品/服务：</span><span class="sxs-lookup"><span data-stu-id="44a40-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="44a40-198">[![显示筛选选项。](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="44a40-199">在专用 Azure Marketplace 中购买或部署</span><span class="sxs-lookup"><span data-stu-id="44a40-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="44a40-200">虽然 "产品详细信息" 页面体验与全球 Azure Marketplace 类似，但有三个专用 Azure Marketplace 特定方案。</span><span class="sxs-lookup"><span data-stu-id="44a40-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="44a40-201">当用户选择已批准的计划时，将启用 " **创建** " 按钮：</span><span class="sxs-lookup"><span data-stu-id="44a40-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="44a40-202">[![显示 "产品/服务" 标题，说明可以创建一个计划。](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="44a40-203">如果产品计划选择未出现在 "产品详细信息" 页中，但管理员批准了一个或多个计划，则标题会说明批准了哪些计划并启用了 " **创建** " 按钮：</span><span class="sxs-lookup"><span data-stu-id="44a40-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="44a40-204">[![显示 "产品/服务" 标题，指出可以创建计划并显示可用计划。](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="44a40-205">当用户选择非批准的计划时，标题将说明 "未批准" 和 " **创建** " 按钮已禁用。</span><span class="sxs-lookup"><span data-stu-id="44a40-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="44a40-206">用户仍可以请求将计划添加到已批准列表中 (参阅下一部分) 。</span><span class="sxs-lookup"><span data-stu-id="44a40-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="44a40-207">添加产品/服务或计划的请求</span><span class="sxs-lookup"><span data-stu-id="44a40-207">Request to add offers or plans</span></span>

<span data-ttu-id="44a40-208">可以请求添加 Azure 私有 Azure Marketplace 中当前未批准的公开提议或计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="44a40-209">选择要添加到横幅中的 **请求** 以打开 **访问请求窗体**。</span><span class="sxs-lookup"><span data-stu-id="44a40-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="44a40-210">[![显示带有 "请求添加" 链接的横幅。](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="44a40-211">[![显示产品/服务或计划的访问请求窗体。](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="44a40-212">选择要将哪些计划添加到请求 (**任何计划** 告诉 Marketplace 管理员你没有在产品/服务) 的计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="44a40-213">添加 " **理由** " 并选择 " **请求** " 以提交请求。</span><span class="sxs-lookup"><span data-stu-id="44a40-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="44a40-214">[![显示具有示例条目的产品/服务或计划的访问请求窗体。](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="44a40-215">针对挂起的请求的指示将显示在访问请求窗体中，其中包含用于 **撤消请求** 的选项。</span><span class="sxs-lookup"><span data-stu-id="44a40-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="44a40-216">[![使用 "撤消请求" 链接显示批准或挂起的计划的列表。](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="44a40-217">提交后，将向市场管理员发送批准请求窗体 [，以查看](#private-azure-marketplace-notification-center) 请求并采取措施。</span><span class="sxs-lookup"><span data-stu-id="44a40-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="44a40-218">常见问题解答 (FAQ)</span><span class="sxs-lookup"><span data-stu-id="44a40-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="44a40-219">我已通过 Azure 策略阻止 Marketplace 第三方应用程序。</span><span class="sxs-lookup"><span data-stu-id="44a40-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="44a40-220">这有何不同？</span><span class="sxs-lookup"><span data-stu-id="44a40-220">How is this different?</span></span>

<span data-ttu-id="44a40-221">目前有两种方法可限制 Marketplace 中的第三方服务：</span><span class="sxs-lookup"><span data-stu-id="44a40-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="44a40-222">通过 EA 门户或 Azure 门户禁用第三方服务，或将其限制为 "仅限免费或 BYOL Sku"。</span><span class="sxs-lookup"><span data-stu-id="44a40-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="演示如何限制 Azure 门户中的服务。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="演示如何限制 E A 门户中的服务。":::

2. <span data-ttu-id="44a40-225">创建 Azure 策略以仅允许特定 Vm。</span><span class="sxs-lookup"><span data-stu-id="44a40-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="44a40-226">有关如何对 Windows Vm 强制执行策略的详细信息，请参阅 [使用 Azure 资源管理器将策略应用于 Windows vm](https://docs.microsoft.com/azure/virtual-machines/windows/policy)。</span><span class="sxs-lookup"><span data-stu-id="44a40-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="44a40-227">私有 Azure Marketplace 可以更灵活地限制和允许特定的产品/服务和计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="44a40-228">即使在尝试部署第三方服务之前，它也会通知最终用户在 marketplace 库中的部署是否可用。</span><span class="sxs-lookup"><span data-stu-id="44a40-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="44a40-229">若要允许部署第三方服务，请在 EA 门户和 Azure 门户中将 "Azure Marketplace" 设置为 "开/启用"。</span><span class="sxs-lookup"><span data-stu-id="44a40-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="44a40-230">私有 Azure Marketplace 可以组织不受限于虚拟机的合作伙伴解决方案。</span><span class="sxs-lookup"><span data-stu-id="44a40-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="44a40-231">私有 Azure Marketplace 可以组织计划级别，还可以设置 "当前和未来的计划"。</span><span class="sxs-lookup"><span data-stu-id="44a40-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="44a40-232">私有 Azure Marketplace 可以提前通知最终用户可以部署哪些内容。</span><span class="sxs-lookup"><span data-stu-id="44a40-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="44a40-233">专用产品/服务和专用 Azure Marketplace 之间的区别是什么？</span><span class="sxs-lookup"><span data-stu-id="44a40-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="44a40-234">通过 **专用产品/服务** ，发布者可以创建仅对目标客户可见的计划。</span><span class="sxs-lookup"><span data-stu-id="44a40-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="44a40-235">这样，他们就可以将自定义解决方案与协商定价、私有条款和条件以及专用配置私下共享。</span><span class="sxs-lookup"><span data-stu-id="44a40-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="44a40-236">有关详细信息，请参阅 [商业应用商店中的专用产品/服务](https://docs.microsoft.com/azure/marketplace/private-offers)。</span><span class="sxs-lookup"><span data-stu-id="44a40-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="44a40-237">Azure 门户中的 **私有 Azure Marketplace** 使管理员能够预先批准其用户可以部署的第三方解决方案。</span><span class="sxs-lookup"><span data-stu-id="44a40-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="44a40-238">通过专用的 Azure Marketplace，用户可以通过查找、购买和部署符合要求的产品/服务来享受 Azure Marketplace 的权益。</span><span class="sxs-lookup"><span data-stu-id="44a40-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="44a40-239">若要在私有 Marketplace 中管理基于订阅的专用产品/服务，Marketplace 管理员在特定订阅上必须至少具有 "读取" 角色。</span><span class="sxs-lookup"><span data-stu-id="44a40-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="44a40-240">我将专用产品/服务添加到专用 Azure Marketplace，原因是它不会显示在 "管理 Marketplace" 选项卡中？</span><span class="sxs-lookup"><span data-stu-id="44a40-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="44a40-241">基于订阅的专用产品/服务仅对 "专用产品/服务" 设置中列出的订阅可见。</span><span class="sxs-lookup"><span data-stu-id="44a40-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="44a40-242">若要查看专用产品/服务，请确保全局订阅筛选器显示所有订阅。</span><span class="sxs-lookup"><span data-stu-id="44a40-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="44a40-243">[![显示 "专用 marketplace" 筛选器。](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="44a40-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="44a40-244">能否在专用 Azure Marketplace 中包含自定义映像？</span><span class="sxs-lookup"><span data-stu-id="44a40-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="44a40-245">否。</span><span class="sxs-lookup"><span data-stu-id="44a40-245">No.</span></span> <span data-ttu-id="44a40-246">通过专用 Azure Marketplace，任何 IT 管理员都可从全球 Azure Marketplace 管理和组织第三方解决方案。</span><span class="sxs-lookup"><span data-stu-id="44a40-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="44a40-247">由于自定义映像不在全球 Azure Marketplace 上，因此 IT 管理员无法选择自定义映像。</span><span class="sxs-lookup"><span data-stu-id="44a40-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="44a40-248">如果要共享自定义映像，请使用 [共享映像库](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries)。</span><span class="sxs-lookup"><span data-stu-id="44a40-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="44a40-249"> ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli)、 [POWERSHELL](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell))  (SIG) 创建共享图像库的分步指南。</span><span class="sxs-lookup"><span data-stu-id="44a40-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="44a40-250">在 SIG 中创建映像定义。</span><span class="sxs-lookup"><span data-stu-id="44a40-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="44a40-251">客户应为 "OS-状态" 字段选择 " **通用化** "。</span><span class="sxs-lookup"><span data-stu-id="44a40-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="44a40-252"> ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)) 。</span><span class="sxs-lookup"><span data-stu-id="44a40-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="44a40-253"> ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)) 将托管映像引入共享映像库。</span><span class="sxs-lookup"><span data-stu-id="44a40-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="44a40-254">SIG VM 映像将驻留在一个订阅中。</span><span class="sxs-lookup"><span data-stu-id="44a40-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="44a40-255">若要使其可用于其他订阅，请使用 ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)) 的应用注册。</span><span class="sxs-lookup"><span data-stu-id="44a40-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="44a40-256">为什么尽管发布商不是 Microsoft，也会看到一些 **默认情况下已批准** 的产品？</span><span class="sxs-lookup"><span data-stu-id="44a40-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="44a40-257">Microsoft 支持 Azure 中的 Linux 和开源技术。</span><span class="sxs-lookup"><span data-stu-id="44a40-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="44a40-258">Azure 支持[认可的 Linux 分发](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)版，并在虚拟机中集成了价格。</span><span class="sxs-lookup"><span data-stu-id="44a40-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="44a40-259">由于 Azure Linux 代理已预安装在 Azure Marketplace 上，因此将其视为 Microsoft 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="44a40-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="44a40-260">由于 Microsoft 产品/服务默认已获批准，因此无法在专用 Azure Marketplace 中管理认可的 Linux 分发版，默认情况下已获得批准。</span><span class="sxs-lookup"><span data-stu-id="44a40-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="44a40-261">联系支持人员</span><span class="sxs-lookup"><span data-stu-id="44a40-261">Contact support</span></span>

- <span data-ttu-id="44a40-262">有关 Azure Marketplace 支持，请访问 [Microsoft 问答&](/answers/products/)。</span><span class="sxs-lookup"><span data-stu-id="44a40-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
