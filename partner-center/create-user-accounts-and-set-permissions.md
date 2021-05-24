---
title: 创建用户帐户并分配角色
description: 必须先为每个员工分配一个角色，然后他们才能访问合作伙伴中心。 了解如何创建用户帐户、分配角色和设置权限。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148136"
---
# <a name="create-user-accounts"></a><span data-ttu-id="a17bd-104">创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="a17bd-104">Create user accounts</span></span>  

<span data-ttu-id="a17bd-105">**相应的角色**：帐户管理员 | 全局管理员 |“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="a17bd-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="a17bd-106">为需要访问合作伙伴中心的员工创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a17bd-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="a17bd-107">这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。</span><span class="sxs-lookup"><span data-stu-id="a17bd-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="a17bd-108">有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="a17bd-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="a17bd-109">添加新用户</span><span class="sxs-lookup"><span data-stu-id="a17bd-109">Add a new user</span></span>

1. <span data-ttu-id="a17bd-110">在合作伙伴中心右上角的“设置”图标中，选择“帐户设置”，再选择“用户管理”  。</span><span class="sxs-lookup"><span data-stu-id="a17bd-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="a17bd-111">选择“添加用户”。</span><span class="sxs-lookup"><span data-stu-id="a17bd-111">Select **Add user**.</span></span>

3. <span data-ttu-id="a17bd-112">输入用户全名和唯一的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a17bd-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="a17bd-113">选择要分配给用户的代理类型和/或管理员类型。</span><span class="sxs-lookup"><span data-stu-id="a17bd-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="a17bd-114">合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。</span><span class="sxs-lookup"><span data-stu-id="a17bd-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="a17bd-115">如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="a17bd-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="a17bd-116">选择“添加”以创建用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a17bd-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="a17bd-117">在下一页上确认用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a17bd-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="a17bd-118">记下此页面上显示的新用户的登录信息。</span><span class="sxs-lookup"><span data-stu-id="a17bd-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="a17bd-119">确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。</span><span class="sxs-lookup"><span data-stu-id="a17bd-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="a17bd-120">用户将需要使用其用户名和临时密码来登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="a17bd-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="a17bd-121">当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。</span><span class="sxs-lookup"><span data-stu-id="a17bd-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="a17bd-122">分配用户角色</span><span class="sxs-lookup"><span data-stu-id="a17bd-122">Assign user roles</span></span>

<span data-ttu-id="a17bd-123">若要在合作伙伴中心操作，必须分配有一个角色。</span><span class="sxs-lookup"><span data-stu-id="a17bd-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="a17bd-124">目前，角色包括 Azure Active Directory 租户角色、云解决方案提供商 (CSP) 角色和非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="a17bd-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="a17bd-125">单个公司可以需要所有这些角色。</span><span class="sxs-lookup"><span data-stu-id="a17bd-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="a17bd-126">用户必须在租户中列出才能访问合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="a17bd-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="a17bd-127">角色分配提供额外的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a17bd-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a17bd-128">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a17bd-128">Next steps</span></span>

- [<span data-ttu-id="a17bd-129">为需要在合作伙伴中心工作的员工分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="a17bd-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
