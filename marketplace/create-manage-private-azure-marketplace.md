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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="a3f4c-104">在专用 Azure 市场创建和管理Azure 门户</span><span class="sxs-lookup"><span data-stu-id="a3f4c-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="a3f4c-105">专用 Azure 市场管理员可以控制其用户可以使用的第三方解决方案。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="a3f4c-106">它通过允许用户仅部署管理员批准且符合企业策略的优惠来实现此目标。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="a3f4c-107">使用专用 Azure 市场，用户可以在在线商店中搜索要购买和部署的合规产品/服务。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="a3f4c-108">作为市场管理员 (分配的角色) ，你将从已禁用且空的专用存储开始，可以在其中添加已批准的产品/服务与计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="a3f4c-109">本文介绍如何分配所需角色、创建专用存储、管理项、批准用户请求，以及专用 Azure 市场用户。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="a3f4c-110">专用 Azure 市场处于租户级别，因此租户下的所有用户都将看到相同的策展列表。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="a3f4c-111">所有 Microsoft 解决方案 (包括认可的 [Linux](/azure/virtual-machines/linux/endorsed-distros) 分发版) 自动添加到 专用 Azure 市场。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="a3f4c-112">分配市场管理员角色</span><span class="sxs-lookup"><span data-stu-id="a3f4c-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="a3f4c-113">租户全局管理员管理员必须将市场 **管理员** 角色分配给专用 Azure 市场管理专用存储的管理员。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="a3f4c-114">只有专用 AZURE 市场市场管理员角色的 IT 管理员才能访问管理权限。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="a3f4c-115">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3f4c-115">Prerequisites</span></span>

<span data-ttu-id="a3f4c-116">在将"市场管理员"角色分配给租户范围的用户之前，需要满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="a3f4c-117">你 **有权访问全局管理员用户** 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="a3f4c-118">租户至少有一个订阅 (可以是任何类型) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="a3f4c-119">为全局管理员订阅分配参与者角色或更高级的用户。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="a3f4c-120">为市场管理员角色分配访问控制 (IAM) </span><span class="sxs-lookup"><span data-stu-id="a3f4c-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="a3f4c-121">登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="a3f4c-122">选择 **"所有服务"，** 然后选择"**市场"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="a3f4c-123">从 **专用市场** 菜单中选择"设置"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="在市场左侧显示专用市场菜单选项。":::

1. <span data-ttu-id="a3f4c-125">选择 **"访问控制 (IAM)** 以分配市场管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="显示&quot;I A M 访问控制&quot;屏幕。":::

1. <span data-ttu-id="a3f4c-127">选择“+ 添加”   >   “添加角色分配”。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="a3f4c-128">在"**角色"** 下，选择 **"市场管理员"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="显示&quot;角色分配&quot;菜单。":::

1. <span data-ttu-id="a3f4c-130">从下拉列表中选择所需的用户，然后选择"完成 **"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="a3f4c-131">使用 PowerShell 分配市场管理员角色</span><span class="sxs-lookup"><span data-stu-id="a3f4c-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="a3f4c-132">使用以下 PowerShell 脚本分配"市场管理员"角色;它需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="a3f4c-133">**TenantId：** "市场管理员"角色 (租户的 ID 可分配给租户) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="a3f4c-134">**SubscriptionId：** 为其分配了全局管理员"参与者 **"** 角色或更高角色的订阅。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="a3f4c-135">**GlobalAdminUsername：** 全局管理员的用户名。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="a3f4c-136">**UsernameToAssignRoleFor：** 将为其分配市场管理员角色的用户名。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="a3f4c-137">对于受邀加入租户的来宾用户，可能需要最多 48 小时，直到其帐户可用于分配"市场管理员"角色。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="a3f4c-138">有关详细信息，请参阅[B2B 协作Azure Active Directory的属性](/azure/active-directory/b2b/user-properties)。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="a3f4c-139">有关 Az.Portal PowerShell 模块中包含的 cmdlet 详细信息，请参阅[Microsoft Azure PowerShell：门户仪表板 cmdlet。](/powershell/module/az.portal/)</span><span class="sxs-lookup"><span data-stu-id="a3f4c-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="a3f4c-140">创建专用 Azure 市场</span><span class="sxs-lookup"><span data-stu-id="a3f4c-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="a3f4c-141">登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="a3f4c-142">选择 **"所有服务"，** 然后选择"**市场"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="显示Azure 门户窗口。":::

3. <span data-ttu-id="a3f4c-144">从 **专用市场** 菜单中选择"设置"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="a3f4c-145">选择 **入门"专用 Azure 市场 (** 创建一次，只需执行一次) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="演示如何选择&quot;入门&quot;主Azure 门户&quot;。":::

    <span data-ttu-id="a3f4c-147">如果专用 Azure 市场租户已存在，则 **默认情况下** 将选择"管理市场"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="a3f4c-148">完成后，将拥有一个空且已禁用专用 Azure 市场。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="显示空的专用 Azure 市场屏幕。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="a3f4c-150">从库中添加项</span><span class="sxs-lookup"><span data-stu-id="a3f4c-150">Add items from gallery</span></span>

<span data-ttu-id="a3f4c-151">项是套餐和计划的组合。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="a3f4c-152">可以在"管理市场"页上搜索和添加项。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="a3f4c-153">选择"**添加项"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-153">Select **Add items**.</span></span>

2. <span data-ttu-id="a3f4c-154">浏览 **库或使用** 搜索字段查找想要的项目。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="演示如何浏览库或使用搜索字段。":::

3. <span data-ttu-id="a3f4c-156">默认情况下，添加新产品/服务时，所有当前计划都将添加到已批准列表中。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="a3f4c-157">若要在添加所选项之前修改计划选择，请选择产品/服务磁贴中的下拉菜单并更新所需的计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="演示如何更新所需的计划。":::

4. <span data-ttu-id="a3f4c-159">选择 **选择** 后，选择左下角的"完成"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="a3f4c-160">**将项** 添加到市场仅适用于非 Microsoft 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="a3f4c-161">包括 ([Linux](/azure/virtual-machines/linux/endorsed-distros) 分发版) 的 Microsoft 解决方案将被标记为"默认批准"，并且无法在 专用市场。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="a3f4c-162">编辑项的计划</span><span class="sxs-lookup"><span data-stu-id="a3f4c-162">Edit item's plans</span></span>

<span data-ttu-id="a3f4c-163">可以在"管理市场"页上编辑项的计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="a3f4c-164">在" **计划** "列中，从该项的下拉菜单中查看可用计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="a3f4c-165">选中或清除复选框，以选择要为用户提供的计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="演示如何选择或清除所需项的复选框。":::

   > [!NOTE]
   > <span data-ttu-id="a3f4c-167">每个产品/服务至少需要选择一个计划，进行更新。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="a3f4c-168">若要删除与套餐相关的所有计划，请删除整个套餐 (请参阅下一部分) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="a3f4c-169">删除产品/服务</span><span class="sxs-lookup"><span data-stu-id="a3f4c-169">Delete offers</span></span>

<span data-ttu-id="a3f4c-170">在"管理市场"页中，选中产品/服务名称旁边的复选框 (上方的屏幕) 选择"删除 **项"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="a3f4c-171">启用/禁用专用 Azure 市场</span><span class="sxs-lookup"><span data-stu-id="a3f4c-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="a3f4c-172">在"管理市场"页中，你将看到以下横幅之一，其中显示了当前专用 Azure 市场：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="显示&quot;禁用状态&quot;横幅。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="显示&quot;启用状态&quot;横幅。":::

<span data-ttu-id="a3f4c-175">可根据需要启用专用 Azure 市场禁用。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="a3f4c-176">如果已禁用，请选择 **"启用专用市场** 启用" 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="a3f4c-177">如果已启用，请选择 **"禁用专用市场** 禁用" 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="a3f4c-178">专用 Azure 市场通知中心</span><span class="sxs-lookup"><span data-stu-id="a3f4c-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="a3f4c-179">通知中心包含三种类型的通知，并允许市场管理员根据通知采取措施：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="a3f4c-180">对于未在批准列表中的项目，用户 (请求添加以下产品/服务或) 。 [](#request-to-add-offers-or-plans)</span><span class="sxs-lookup"><span data-stu-id="a3f4c-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="a3f4c-181">已批准列表中已有一个或多个计划的套餐的新计划通知。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="a3f4c-182">删除了已批准列表中但已从全局列表中删除的项的计划Azure 市场。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="a3f4c-183">访问通知中心：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-183">To access the notification center:</span></span>

1. <span data-ttu-id="a3f4c-184">从 **左侧** 菜单中选择"通知"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="显示&quot;通知&quot;菜单。":::

1. <span data-ttu-id="a3f4c-186">选择省略号菜单以执行更多操作。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="显示&quot;更多选项&quot;菜单结果。":::

1. <span data-ttu-id="a3f4c-188">对于计划请求，" **显示** 请求"将打开审批请求表单，可在其中查看特定产品/服务的所有用户请求。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="a3f4c-189">选择 **"批准** 或拒绝 **"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="显示批准和拒绝选项。":::

1. <span data-ttu-id="a3f4c-191">从下拉菜单中选择要批准的计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="a3f4c-192">添加注释，然后选择"提交 **"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="a3f4c-193">浏览专用 Azure 市场</span><span class="sxs-lookup"><span data-stu-id="a3f4c-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="a3f4c-194">启用专用 Azure 市场后，用户将看到市场管理员已批准的计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="a3f4c-195">绿色" **已批准** "通知指示合作伙伴 (批准的非 Microsoft) 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="a3f4c-196">蓝色" **已批准** "通知表示 Microsoft (产品/服务，包括) 认可的 [Linux](/azure/virtual-machines/linux/endorsed-distros) 分发版。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="a3f4c-197">用户可以在已批准和未批准的产品/服务之间进行筛选：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="显示筛选选项。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="a3f4c-199">购买或部署专用 Azure 市场</span><span class="sxs-lookup"><span data-stu-id="a3f4c-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="a3f4c-200">虽然产品详细信息页面体验类似于全局Azure 市场，但有三专用 Azure 市场特定方案。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="a3f4c-201">当用户选择已批准的计划时，将启用 **"创建** "按钮：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="显示产品/服务横幅，表明可以创建计划。":::

- <span data-ttu-id="a3f4c-203">如果产品计划选择未显示在产品详细信息页中，但管理员已批准了一个或多个计划，则横幅会记录哪些计划获得批准并启用" **创建"按钮** ：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="显示产品/服务横幅，指出可以创建计划，并显示可用计划。":::

- <span data-ttu-id="a3f4c-205">当用户选择未批准的计划时，横幅将计划注释为"未批准"，并禁用"创建"按钮。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="a3f4c-206">用户仍可以请求将计划添加到已批准列表 (请参阅下一部分) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="a3f4c-207">请求添加套餐或计划</span><span class="sxs-lookup"><span data-stu-id="a3f4c-207">Request to add offers or plans</span></span>

<span data-ttu-id="a3f4c-208">可以请求添加当前未在计划中添加专用 Azure 市场。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="a3f4c-209">选择 **"请求"以** 在横幅中添加 ，打开" **访问请求"窗体**。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="显示包含&quot;请求添加&quot;链接的横幅。":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="显示套餐或计划的访问请求窗体。":::

1. <span data-ttu-id="a3f4c-212">选择要添加到请求的计划 ("任何计划"都告知市场管理员，你对于套餐中的计划没有) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="a3f4c-213">添加理由 **并选择** " **请求** "以提交请求。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="显示包含示例条目的套餐或计划的访问请求表单。":::

1. <span data-ttu-id="a3f4c-215">"访问请求"窗体中将显示挂起请求的指示，其选项为 **"撤消请求"。**</span><span class="sxs-lookup"><span data-stu-id="a3f4c-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="显示包含&quot;撤消请求&quot;链接的已批准或挂起计划的列表。":::

> [!NOTE]
> <span data-ttu-id="a3f4c-217">提交后，审批请求表单将发送到通知中心，供市场[](#private-azure-marketplace-notification-center)管理员查看请求并采取措施。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="a3f4c-218">批准专用市场并不表示已采购解决方案。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="a3f4c-219">常见问题解答 (FAQ)</span><span class="sxs-lookup"><span data-stu-id="a3f4c-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="a3f4c-220">我已阻止市场第三方应用程序通过 Azure Policy。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="a3f4c-221">这有多不同？</span><span class="sxs-lookup"><span data-stu-id="a3f4c-221">How is this different?</span></span>

<span data-ttu-id="a3f4c-222">目前，有两种方法可以限制市场中的第三方服务：</span><span class="sxs-lookup"><span data-stu-id="a3f4c-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="a3f4c-223">通过 EA 门户或Azure 门户，禁用第三方服务或限制为"免费或 BYOL SKUS"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="演示如何限制服务中的Azure 门户。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="演示如何在 E A 门户中限制服务。":::

2. <span data-ttu-id="a3f4c-226">创建仅允许特定 VM 的 Azure 策略。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="a3f4c-227">若要详细了解如何强制实施策略来Windows VM，请参阅将策略Windows [VM Azure 资源管理器。](/azure/virtual-machines/windows/policy)</span><span class="sxs-lookup"><span data-stu-id="a3f4c-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="a3f4c-228">专用 Azure 市场可以更灵活地限制和允许特定的套餐和计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="a3f4c-229">它通知最终用户在尝试部署第三方服务之前，在市场库中部署的可用性。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="a3f4c-230">若要允许部署第三方服务，请Azure 市场中将"EA 门户"设置为"Azure 门户"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="a3f4c-231">专用 Azure 市场可以组织合作伙伴解决方案，而不限于虚拟机。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="a3f4c-232">专用 Azure 市场可在计划级别进行组织，还可以设置"当前和未来计划"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="a3f4c-233">专用 Azure 市场可以提前通知最终用户可以部署和不能部署哪些内容。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="a3f4c-234">专用产品/服务与专用服务之间有什么专用 Azure 市场？</span><span class="sxs-lookup"><span data-stu-id="a3f4c-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="a3f4c-235">专用 **套餐** 允许发布者创建仅对目标客户可见的计划。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="a3f4c-236">这样，他们可私密共享自定义解决方案，并采用协商定价、专用条款和条件以及专用配置。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="a3f4c-237">有关详细信息，请参阅 [商业市场中的专用产品/服务](/azure/marketplace/private-offers)。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="a3f4c-238">**专用 Azure 市场** 中Azure 门户管理员可以预先批准其用户可以部署的第三方解决方案。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="a3f4c-239">借助专用 Azure 市场，用户可以通过查找、Azure 市场和部署合规产品/服务来享受产品/服务的好处。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="a3f4c-240">若要在 专用市场 中管理基于订阅的专用产品/服务，市场管理员必须对特定订阅至少具有"读取"角色。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="a3f4c-241">我向市场添加了专用专用 Azure 市场，为什么它未显示在"管理市场"选项卡中？</span><span class="sxs-lookup"><span data-stu-id="a3f4c-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="a3f4c-242">基于订阅的专用套餐仅对"专用套餐"设置中所列的订阅可见。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="a3f4c-243">若要查看专用套餐，请确保全局订阅筛选器显示所有订阅。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="显示专用市场筛选器。":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="a3f4c-245">我们能否在映像中包括自定义专用 Azure 市场？</span><span class="sxs-lookup"><span data-stu-id="a3f4c-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="a3f4c-246">否。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-246">No.</span></span> <span data-ttu-id="a3f4c-247">专用 Azure 市场允许任何 IT 管理员管理和策展来自全球客户的第三方Azure 市场。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="a3f4c-248">由于自定义映像不在全局Azure 市场，因此 IT 管理员无法选取和选择自定义映像。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="a3f4c-249">若要共享自定义映像，请使用 [共享映像库](/azure/virtual-machines/shared-image-galleries)。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="a3f4c-250">分步指南使用 SIG ([CLI、PowerShell](/azure/virtual-machines/shared-images-powershell))  (创建共享映像) 。 [](/azure/virtual-machines/shared-images-cli)</span><span class="sxs-lookup"><span data-stu-id="a3f4c-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="a3f4c-251">在 SIG 内创建映像定义。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="a3f4c-252">客户应为"OS **状态"** 字段选择"通用化"。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="a3f4c-253"> ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [、PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="a3f4c-254">使用[CLI、PowerShell](/azure/virtual-machines/image-version-managed-image-powershell) (将托管映像引入[](/azure/virtual-machines/image-version-managed-image-cli)共享) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="a3f4c-255">SIG VM 映像将驻留在一个订阅中。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="a3f4c-256">若要使其可供其他订阅使用，请通过 [CLI](/azure/virtual-machines/linux/share-images-across-tenants) ([PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) 。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="a3f4c-257">为什么即使发布者不是 Microsoft，也看到默认批准的某些产品/服务？ </span><span class="sxs-lookup"><span data-stu-id="a3f4c-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="a3f4c-258">Microsoft 支持 Azure 中的 Linux 和开源技术。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="a3f4c-259">[Azure 支持](/azure/virtual-machines/linux/endorsed-distros) 认可的 Linux 分发版，价格已集成到虚拟机中。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="a3f4c-260">由于 Azure Linux 代理已预安装在 Azure 市场，因此它被视为 Microsoft 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="a3f4c-261">由于 Microsoft 产品/服务是默认批准的，因此无法在 专用 Azure 市场中管理认可的 Linux 分发版，并且默认情况下会获得批准。</span><span class="sxs-lookup"><span data-stu-id="a3f4c-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="a3f4c-262">联系支持人员</span><span class="sxs-lookup"><span data-stu-id="a3f4c-262">Contact support</span></span>

- <span data-ttu-id="a3f4c-263">有关Azure 市场，请访问[Microsoft Q&A。](/answers/products/)</span><span class="sxs-lookup"><span data-stu-id="a3f4c-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>