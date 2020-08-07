---
title: 创建用户帐户并分配角色
description: 必须先为每个员工分配一个角色，然后他们才能访问合作伙伴中心。 了解如何创建用户帐户、分配角色和设置权限。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: cfd681a56bfaebcc1fd6c77de3e5a0c6deb4a46f
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527733"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="4db83-104">创建用户帐户并分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="4db83-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="4db83-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="4db83-105">**Appropriate roles**</span></span>

- <span data-ttu-id="4db83-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-106">Account admin</span></span>
- <span data-ttu-id="4db83-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-107">Global admin</span></span>
- <span data-ttu-id="4db83-108">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-108">User management admin</span></span>

<span data-ttu-id="4db83-109">为需要访问合作伙伴中心的员工创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="4db83-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="4db83-110">这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。</span><span class="sxs-lookup"><span data-stu-id="4db83-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="4db83-111">有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="4db83-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="4db83-112">添加新用户</span><span class="sxs-lookup"><span data-stu-id="4db83-112">Add a new user</span></span>

1. <span data-ttu-id="4db83-113">在合作伙伴中心右上角的“设置”图标中，选择“用户管理”。</span><span class="sxs-lookup"><span data-stu-id="4db83-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="4db83-114">选择“添加用户”。</span><span class="sxs-lookup"><span data-stu-id="4db83-114">Select **Add user**.</span></span>

3. <span data-ttu-id="4db83-115">输入用户全名和唯一的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4db83-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="4db83-116">选择要分配给用户的代理类型和/或管理员类型。</span><span class="sxs-lookup"><span data-stu-id="4db83-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="4db83-117">合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。</span><span class="sxs-lookup"><span data-stu-id="4db83-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="4db83-118">如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="4db83-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="4db83-119">选择“添加”以创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="4db83-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="4db83-120">在下一页上确认用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4db83-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="4db83-121">记下此页面上显示的新用户的登录信息。</span><span class="sxs-lookup"><span data-stu-id="4db83-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="4db83-122">确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。</span><span class="sxs-lookup"><span data-stu-id="4db83-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="4db83-123">用户将需要使用其用户名和临时密码来登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="4db83-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="4db83-124">当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。</span><span class="sxs-lookup"><span data-stu-id="4db83-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="4db83-125">查找全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-125">Find your global admin</span></span>

<span data-ttu-id="4db83-126">有时，用户可能需要更改其角色，或者新用户可能需要特定的角色分配。</span><span class="sxs-lookup"><span data-stu-id="4db83-126">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="4db83-127">若要查找可以进行角色更改或将角色分配给新用户的全局管理员，请在合作伙伴中心右上角的“设置”图标中，选择“用户管理”并筛选全局管理员。</span><span class="sxs-lookup"><span data-stu-id="4db83-127">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="4db83-128">新的全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-128">New global admin</span></span>

<span data-ttu-id="4db83-129">如果全局管理员离开组织，而其他人需要接替此角色，那么你可以向 Azure 或 Office 365 团队提交票证。</span><span class="sxs-lookup"><span data-stu-id="4db83-129">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="4db83-130">有关如何执行此操作的信息，请选择以下选项之一。</span><span class="sxs-lookup"><span data-stu-id="4db83-130">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="4db83-131">Azure 的新全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-131">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="4db83-132">Office 365 的新全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-132">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="4db83-133">分配用户角色</span><span class="sxs-lookup"><span data-stu-id="4db83-133">Assign user roles</span></span>

<span data-ttu-id="4db83-134">若要在合作伙伴中心操作，必须分配有一个角色。</span><span class="sxs-lookup"><span data-stu-id="4db83-134">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="4db83-135">目前，角色包括 Azure Active Directory 租户角色、云解决方案提供商 (CSP) 角色和非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="4db83-135">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="4db83-136">单个公司可以需要所有这些角色。</span><span class="sxs-lookup"><span data-stu-id="4db83-136">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="4db83-137">用户必须在租户中列出才能访问合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="4db83-137">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="4db83-138">角色分配提供额外的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4db83-138">Role assignments provide additional access.</span></span>


<span data-ttu-id="4db83-139">**AAD 租户角色包括**：</span><span class="sxs-lookup"><span data-stu-id="4db83-139">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="4db83-140">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-140">Global admin</span></span>
- <span data-ttu-id="4db83-141">用户管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-141">User admin</span></span>

<span data-ttu-id="4db83-142">**云解决方案提供商角色包括**：</span><span class="sxs-lookup"><span data-stu-id="4db83-142">**CSP roles include**:</span></span>
- <span data-ttu-id="4db83-143">管理员代理</span><span class="sxs-lookup"><span data-stu-id="4db83-143">Admin agent</span></span>
- <span data-ttu-id="4db83-144">计费管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-144">Billing admin</span></span>
- <span data-ttu-id="4db83-145">销售代理</span><span class="sxs-lookup"><span data-stu-id="4db83-145">Sales agent</span></span>
- <span data-ttu-id="4db83-146">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="4db83-146">Helpdesk agent</span></span>

<span data-ttu-id="4db83-147">**可管理 MPN 会员和公司的角色（非 AAD）**</span><span class="sxs-lookup"><span data-stu-id="4db83-147">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="4db83-148">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-148">MPN partner admin</span></span>
- <span data-ttu-id="4db83-149">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-149">Account admin</span></span>
- <span data-ttu-id="4db83-150">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-150">Referral admin</span></span>
- <span data-ttu-id="4db83-151">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-151">Business profile admin</span></span>
- <span data-ttu-id="4db83-152">奖励管理员和用户</span><span class="sxs-lookup"><span data-stu-id="4db83-152">Incentives admin and user</span></span>

<span data-ttu-id="4db83-153">**控制面板供应商是云解决方案提供商，而非 AAD 角色**。</span><span class="sxs-lookup"><span data-stu-id="4db83-153">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="4db83-154">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4db83-154">Global admin</span></span>

<span data-ttu-id="4db83-155">**来宾用户**必须是 AAD 租户的一部分，可以充当任何非 AAD 角色。</span><span class="sxs-lookup"><span data-stu-id="4db83-155">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="4db83-156">有关角色以及每个角色可以执行哪些操作的特定信息，请参阅[分配用户权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="4db83-156">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="4db83-157">在合作伙伴中心关联用户的 Microsoft Learn 帐户</span><span class="sxs-lookup"><span data-stu-id="4db83-157">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="4db83-158">用户需要将其 MCP ID 关联到其合作伙伴中心帐户，才能查看在取得资质的过程中可以参考的培训内容和学习路径。</span><span class="sxs-lookup"><span data-stu-id="4db83-158">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="4db83-159">全局管理员在添加新用户时，请务必提醒用户将其 MCP ID 关联到其帐户。</span><span class="sxs-lookup"><span data-stu-id="4db83-159">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="4db83-160">如何将 MCP ID 关联到合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="4db83-160">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="4db83-161">在合作伙伴中心面板中，选择面板右上角的“我的帐户”图标，然后选择“我的个人资料” 。</span><span class="sxs-lookup"><span data-stu-id="4db83-161">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="4db83-162">在“我的 Learning”下方，可以关联你的 Microsoft Learning 帐户，还可以将你的 Microsoft 帐户连接到 Partner University。</span><span class="sxs-lookup"><span data-stu-id="4db83-162">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4db83-163">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4db83-163">Next steps</span></span>

- [<span data-ttu-id="4db83-164">为需要在合作伙伴中心工作的公司用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="4db83-164">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)