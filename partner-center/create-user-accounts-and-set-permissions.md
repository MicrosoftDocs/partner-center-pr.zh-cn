---
title: 创建用户帐户和设置权限 | 合作伙伴中心
ms.topic: article
ms.date: 02/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心创建用户帐户，以及如何为每个需要访问权限的员工分配角色。 具有不同管理员权限的用户可以执行此操作。
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.author: evansma
Keywords: 角色, 权限, 添加用户, 分配角色, 管理员, 代理
ms.localizationpriority: high
ms.openlocfilehash: 6bbae5b8bcd2882c7ba32a8b660fc256dec4e49a
ms.sourcegitcommit: 717ef04f5c0040611af3ba9e5a324ab67e99ba14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "78240204"
---
# <a name="create-user-accounts-and-assign-permissions"></a><span data-ttu-id="bd2e8-105">创建用户帐户并分配权限</span><span class="sxs-lookup"><span data-stu-id="bd2e8-105">Create user accounts and assign permissions</span></span>

<span data-ttu-id="bd2e8-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="bd2e8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="bd2e8-107">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-107">Account admin</span></span>
- <span data-ttu-id="bd2e8-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-108">Global admin</span></span>
- <span data-ttu-id="bd2e8-109">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-109">User management admin</span></span>

<span data-ttu-id="bd2e8-110">为需要访问合作伙伴中心的员工创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-110">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="bd2e8-111">这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-111">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="bd2e8-112">有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-112">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="bd2e8-113">添加新用户</span><span class="sxs-lookup"><span data-stu-id="bd2e8-113">Add a new user</span></span>

1. <span data-ttu-id="bd2e8-114">在合作伙伴中心右上角的“设置”图标中，选择“用户管理”。  </span><span class="sxs-lookup"><span data-stu-id="bd2e8-114">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="bd2e8-115">选择“添加用户”。 </span><span class="sxs-lookup"><span data-stu-id="bd2e8-115">Select **Add user**.</span></span>

3. <span data-ttu-id="bd2e8-116">输入用户全名和唯一的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-116">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="bd2e8-117">选择要分配给用户的代理类型和/或管理员类型。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-117">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="bd2e8-118">合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-118">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="bd2e8-119">如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。 </span><span class="sxs-lookup"><span data-stu-id="bd2e8-119">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="bd2e8-120">选择“添加”  以创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-120">Select **Add** to create the user account.</span></span> <span data-ttu-id="bd2e8-121">在下一页上确认用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-121">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="bd2e8-122">记下此页面上显示的新用户的登录信息。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-122">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="bd2e8-123">确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-123">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="bd2e8-124">用户将需要使用其用户名和临时密码来登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-124">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="bd2e8-125">当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-125">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="bd2e8-126">如果全局管理员已离职或充当了其他角色，而你需要添加新的全局管理员，则必须在 [MPN 门户](https://partner.microsoft.com/support)上登记服务请求。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-126">If your global admin has left your organization or moved onto another role and you need to add a new global admin, you have to log a service request on the [MPN portal](https://partner.microsoft.com/support).</span></span> <span data-ttu-id="bd2e8-127">如果支持代理能够提供必要的个人身份信息以及关于组织的其他信息，则该代理可以请求将某个用户提升为全局管理员。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-127">The support agent can request elevation of a user to global admin if your requestor is able to provide the requisite Personal identity information and provide additional information about your organization.</span></span>

### <a name="find-your-global-admin"></a><span data-ttu-id="bd2e8-128">查找全局管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-128">Find your global admin</span></span>

<span data-ttu-id="bd2e8-129">有时，用户可能需要更改其角色，或者新用户可能需要特定的角色分配。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-129">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="bd2e8-130">若要查找可以进行角色更改或将角色分配给新用户的全局管理员，请在合作伙伴中心右上角的“设置”图标中，选择“用户管理”并筛选全局管理员。  </span><span class="sxs-lookup"><span data-stu-id="bd2e8-130">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 

## <a name="assign-user-roles"></a><span data-ttu-id="bd2e8-131">分配用户角色</span><span class="sxs-lookup"><span data-stu-id="bd2e8-131">Assign user roles</span></span>

<span data-ttu-id="bd2e8-132">若要在合作伙伴中心操作，必须分配有一个角色。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-132">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="bd2e8-133">目前，角色包括 Azure Active Directory 租户角色、云解决方案提供商 (CSP) 角色和非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-133">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="bd2e8-134">单个公司可以需要所有这些角色。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-134">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="bd2e8-135">用户必须在租户中列出才能访问合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-135">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="bd2e8-136">角色分配提供额外的访问权限。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-136">Role assignments provide additional access.</span></span>


<span data-ttu-id="bd2e8-137">**AAD 租户角色包括**：</span><span class="sxs-lookup"><span data-stu-id="bd2e8-137">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="bd2e8-138">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-138">Global admin</span></span>
- <span data-ttu-id="bd2e8-139">用户管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-139">User admin</span></span>

<span data-ttu-id="bd2e8-140">**云解决方案提供商角色包括**：</span><span class="sxs-lookup"><span data-stu-id="bd2e8-140">**CSP roles include**:</span></span>
- <span data-ttu-id="bd2e8-141">管理员代理</span><span class="sxs-lookup"><span data-stu-id="bd2e8-141">Admin agent</span></span>
- <span data-ttu-id="bd2e8-142">计费管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-142">Billing admin</span></span>
- <span data-ttu-id="bd2e8-143">销售代理</span><span class="sxs-lookup"><span data-stu-id="bd2e8-143">Sales agent</span></span>
- <span data-ttu-id="bd2e8-144">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="bd2e8-144">Helpdesk agent</span></span>

<span data-ttu-id="bd2e8-145">**可管理 MPN 会员和公司的角色（非 AAD）**</span><span class="sxs-lookup"><span data-stu-id="bd2e8-145">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="bd2e8-146">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-146">MPN partner admin</span></span>
- <span data-ttu-id="bd2e8-147">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-147">Account admin</span></span>
- <span data-ttu-id="bd2e8-148">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-148">Referral admin</span></span>
- <span data-ttu-id="bd2e8-149">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-149">Business profile admin</span></span>
- <span data-ttu-id="bd2e8-150">奖励管理员和用户</span><span class="sxs-lookup"><span data-stu-id="bd2e8-150">Incentives admin and user</span></span>

<span data-ttu-id="bd2e8-151">**控制面板供应商是云解决方案提供商，而非 AAD 角色**。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-151">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="bd2e8-152">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bd2e8-152">Global admin</span></span>

<span data-ttu-id="bd2e8-153">**来宾用户**必须是 AAD 租户的一部分，可以充当任何非 AAD 角色。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-153">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="bd2e8-154">有关角色以及每个角色可以执行哪些操作的特定信息，请参阅[分配用户权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-154">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="bd2e8-155">在合作伙伴中心关联用户的 Microsoft Learn 帐户</span><span class="sxs-lookup"><span data-stu-id="bd2e8-155">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="bd2e8-156">用户需要将其 MCP ID 关联到其合作伙伴中心帐户，才能查看在取得资质的过程中可以参考的培训内容和学习路径。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-156">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="bd2e8-157">全局管理员在添加新用户时，请务必提醒用户将其 MCP ID 关联到其帐户。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-157">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="bd2e8-158">如何将 MCP ID 关联到合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="bd2e8-158">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="bd2e8-159">在合作伙伴中心面板中，选择面板右上角的“我的帐户”图标，然后选择“我的个人资料”   。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-159">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="bd2e8-160">在“我的 Learning”下方，可以关联你的 Microsoft Learning 帐户，还可以将你的 Microsoft 帐户连接到 Partner University  。</span><span class="sxs-lookup"><span data-stu-id="bd2e8-160">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>








