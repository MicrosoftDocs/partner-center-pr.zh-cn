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
ms.openlocfilehash: f71df7df213b2c6410fab37ce323825511a18b6d
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846927"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="69abb-104">创建用户帐户并分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="69abb-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="69abb-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="69abb-105">**Appropriate roles**</span></span>

- <span data-ttu-id="69abb-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-106">Account admin</span></span>
- <span data-ttu-id="69abb-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-107">Global admin</span></span>
- <span data-ttu-id="69abb-108">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-108">User management admin</span></span>

<span data-ttu-id="69abb-109">为需要访问合作伙伴中心的员工创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="69abb-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="69abb-110">这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。</span><span class="sxs-lookup"><span data-stu-id="69abb-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="69abb-111">有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="69abb-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="69abb-112">添加新用户</span><span class="sxs-lookup"><span data-stu-id="69abb-112">Add a new user</span></span>

1. <span data-ttu-id="69abb-113">在合作伙伴中心右上角的“设置”图标中，选择“用户管理”。</span><span class="sxs-lookup"><span data-stu-id="69abb-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="69abb-114">选择“添加用户”。</span><span class="sxs-lookup"><span data-stu-id="69abb-114">Select **Add user**.</span></span>

3. <span data-ttu-id="69abb-115">输入用户全名和唯一的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="69abb-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="69abb-116">选择要分配给用户的代理类型和/或管理员类型。</span><span class="sxs-lookup"><span data-stu-id="69abb-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="69abb-117">合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。</span><span class="sxs-lookup"><span data-stu-id="69abb-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="69abb-118">如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="69abb-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="69abb-119">选择“添加”以创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="69abb-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="69abb-120">在下一页上确认用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="69abb-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="69abb-121">记下此页面上显示的新用户的登录信息。</span><span class="sxs-lookup"><span data-stu-id="69abb-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="69abb-122">确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。</span><span class="sxs-lookup"><span data-stu-id="69abb-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="69abb-123">用户将需要使用其用户名和临时密码来登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="69abb-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="69abb-124">当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。</span><span class="sxs-lookup"><span data-stu-id="69abb-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="69abb-125">查找已分配的角色</span><span class="sxs-lookup"><span data-stu-id="69abb-125">Find the role you've been assigned</span></span>

<span data-ttu-id="69abb-126">如果全局管理员没有告诉你，你可以通过执行以下操作来了解你在合作伙伴中心具有哪些角色：</span><span class="sxs-lookup"><span data-stu-id="69abb-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="69abb-127">登录到合作伙伴中心 [面板]https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="69abb-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="69abb-128">选择“帐户设置”图标，然后选择“我的配置文件” 。</span><span class="sxs-lookup"><span data-stu-id="69abb-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="69abb-129">选择“角色和权限”选项卡。你将看到你的角色和权限。</span><span class="sxs-lookup"><span data-stu-id="69abb-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="69abb-130">如果在登录时看不到程序，则通常意味着你无权使用该程序。</span><span class="sxs-lookup"><span data-stu-id="69abb-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="69abb-131">例如，如果在登录时看不到“奖励”页，则你没有奖励权限。</span><span class="sxs-lookup"><span data-stu-id="69abb-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="69abb-132">全局管理员可以向你授予所需的权限。</span><span class="sxs-lookup"><span data-stu-id="69abb-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="69abb-133">查找全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-133">Find your global admin</span></span>

<span data-ttu-id="69abb-134">有时，用户可能需要更改其角色，或者新用户可能需要特定的角色分配。</span><span class="sxs-lookup"><span data-stu-id="69abb-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="69abb-135">若要查找可以进行角色更改或将角色分配给新用户的全局管理员，请从合作伙伴中心右上角的“帐户设置”图标，选择“用户管理”并筛选全局管理员，或者可以转到“我的配置文件”，选择“角色和权限”并查看可帮助你提升权限的不同管理员的列表   。</span><span class="sxs-lookup"><span data-stu-id="69abb-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="69abb-136">新的全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-136">New global admin</span></span>

<span data-ttu-id="69abb-137">如果全局管理员离开组织，而其他人需要接替此角色，那么你可以向 Azure 或 Office 365 团队提交票证。</span><span class="sxs-lookup"><span data-stu-id="69abb-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="69abb-138">有关如何执行此操作的信息，请选择以下选项之一。</span><span class="sxs-lookup"><span data-stu-id="69abb-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="69abb-139">Azure 的新全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="69abb-140">Office 365 的新全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="69abb-141">分配用户角色</span><span class="sxs-lookup"><span data-stu-id="69abb-141">Assign user roles</span></span>

<span data-ttu-id="69abb-142">若要在合作伙伴中心操作，必须分配有一个角色。</span><span class="sxs-lookup"><span data-stu-id="69abb-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="69abb-143">目前，角色包括 Azure Active Directory 租户角色、云解决方案提供商 (CSP) 角色和非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="69abb-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="69abb-144">单个公司可以需要所有这些角色。</span><span class="sxs-lookup"><span data-stu-id="69abb-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="69abb-145">用户必须在租户中列出才能访问合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="69abb-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="69abb-146">角色分配提供额外的访问权限。</span><span class="sxs-lookup"><span data-stu-id="69abb-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="69abb-147">**AAD 租户角色包括**：</span><span class="sxs-lookup"><span data-stu-id="69abb-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="69abb-148">全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-148">Global admin</span></span>
- <span data-ttu-id="69abb-149">用户管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-149">User admin</span></span>

<span data-ttu-id="69abb-150">**云解决方案提供商角色包括**：</span><span class="sxs-lookup"><span data-stu-id="69abb-150">**CSP roles include**:</span></span>
- <span data-ttu-id="69abb-151">管理员代理</span><span class="sxs-lookup"><span data-stu-id="69abb-151">Admin agent</span></span>
- <span data-ttu-id="69abb-152">计费管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-152">Billing admin</span></span>
- <span data-ttu-id="69abb-153">销售代理</span><span class="sxs-lookup"><span data-stu-id="69abb-153">Sales agent</span></span>
- <span data-ttu-id="69abb-154">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="69abb-154">Helpdesk agent</span></span>

<span data-ttu-id="69abb-155">**可管理 MPN 会员和公司的角色（非 AAD）**</span><span class="sxs-lookup"><span data-stu-id="69abb-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="69abb-156">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-156">MPN partner admin</span></span>
- <span data-ttu-id="69abb-157">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-157">Account admin</span></span>
- <span data-ttu-id="69abb-158">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-158">Referral admin</span></span>
- <span data-ttu-id="69abb-159">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-159">Business profile admin</span></span>
- <span data-ttu-id="69abb-160">奖励管理员和用户</span><span class="sxs-lookup"><span data-stu-id="69abb-160">Incentives admin and user</span></span>

<span data-ttu-id="69abb-161">**控制面板供应商是云解决方案提供商，而非 AAD 角色**。</span><span class="sxs-lookup"><span data-stu-id="69abb-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="69abb-162">全局管理员</span><span class="sxs-lookup"><span data-stu-id="69abb-162">Global admin</span></span>

<span data-ttu-id="69abb-163">**来宾用户**必须是 AAD 租户的一部分，可以充当任何非 AAD 角色。</span><span class="sxs-lookup"><span data-stu-id="69abb-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="69abb-164">有关角色以及每个角色可以执行哪些操作的特定信息，请参阅[分配用户权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="69abb-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="69abb-165">在合作伙伴中心关联用户的 Microsoft Learn 帐户</span><span class="sxs-lookup"><span data-stu-id="69abb-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="69abb-166">用户需要将其 MCP ID 关联到其合作伙伴中心帐户，才能查看在取得资质的过程中可以参考的培训内容和学习路径。</span><span class="sxs-lookup"><span data-stu-id="69abb-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="69abb-167">全局管理员在添加新用户时，请务必提醒用户将其 MCP ID 关联到其帐户。</span><span class="sxs-lookup"><span data-stu-id="69abb-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="69abb-168">如何将 MCP ID 关联到合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="69abb-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="69abb-169">在合作伙伴中心面板中，选择面板右上角的“我的帐户”图标，然后选择“我的个人资料” 。</span><span class="sxs-lookup"><span data-stu-id="69abb-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="69abb-170">在“我的 Learning”下方，可以关联你的 Microsoft Learning 帐户，还可以将你的 Microsoft 帐户连接到 Partner University。</span><span class="sxs-lookup"><span data-stu-id="69abb-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="69abb-171">后续步骤</span><span class="sxs-lookup"><span data-stu-id="69abb-171">Next steps</span></span>

- [<span data-ttu-id="69abb-172">为需要在合作伙伴中心工作的公司用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="69abb-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)