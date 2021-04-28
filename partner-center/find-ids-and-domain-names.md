---
title: 查找租户 ID、域名、用户对象 ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何查找 Azure 门户中的 Id-组织的 Azure AD 租户 ID、域名或特定用户对象 ID。 某些任务需要此信息。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172245"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="0b4e7-104">为用户找到重要 Id</span><span class="sxs-lookup"><span data-stu-id="0b4e7-104">Locate important IDs for a user</span></span>

<span data-ttu-id="0b4e7-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="0b4e7-105">**Appropriate roles**</span></span>

- <span data-ttu-id="0b4e7-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0b4e7-106">Global admin</span></span>

<span data-ttu-id="0b4e7-107">本文介绍如何使用 [Azure 门户](https://portal.azure.com/) 查找用户的以下信息：</span><span class="sxs-lookup"><span data-stu-id="0b4e7-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="0b4e7-108">Microsoft Azure Active Directory (Azure AD 用户的组织或公司的) 租户 ID</span><span class="sxs-lookup"><span data-stu-id="0b4e7-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="0b4e7-109">与 Azure AD 租户相关联的组织或公司的主域名</span><span class="sxs-lookup"><span data-stu-id="0b4e7-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="0b4e7-110">用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="0b4e7-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="0b4e7-111">查找 Microsoft Azure AD 租户 ID 和主域名</span><span class="sxs-lookup"><span data-stu-id="0b4e7-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="0b4e7-112">按照以下步骤在 Azure 门户中查找 Azure AD 租户 ID 或主域名。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="0b4e7-113"> (如果要以编程方式查找租户 ID，请参阅 [使用 PowerShell 或 CLI 查找租户 id](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)。 ) </span><span class="sxs-lookup"><span data-stu-id="0b4e7-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="0b4e7-114">租户 ID 在不同的应用程序或资源中可以被称为不同的名称。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="0b4e7-115">例如，租户 ID 可能称为目录 ID，Azure Active Directory (Azure AD) 租户、Microsoft ID 或某些报表，甚至是 *tenantguid*。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="0b4e7-116">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="0b4e7-117">从菜单中选择“Azure Active Directory”。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="显示 Azure 门户从菜单中选择 &quot;Azure Active Directory&quot; 选项。":::

3. <span data-ttu-id="0b4e7-119">此时将显示 Azure Active Directory **概述** "页。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="0b4e7-120">若要查找 Azure AD 租户 ID 或主域名，请查找 " **租户 id** " 字段和 " **主域** " 字段。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="0b4e7-121">这些字段显示在 "租户信息" 部分中。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="显示具有两个突出显示的字段、租户 ID 和主域名的 &quot;概述&quot; 页。":::

4. <span data-ttu-id="0b4e7-123">您可以通过其他一些方式在 Azure 门户中找到租户 ID。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="0b4e7-124">从菜单中选择“Azure Active Directory”。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="0b4e7-125">然后，找到菜单上的 " **管理** " 部分，然后选择 " **属性**"。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="0b4e7-126">"属性" 页还显示用户的关联租户 ID。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="显示 &quot;属性&quot; 页，其中包含突出显示的租户 ID 字段。":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="0b4e7-128">查找用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="0b4e7-128">Find the user object ID</span></span>

<span data-ttu-id="0b4e7-129">仅查找域名和租户 ID 可能并不总是足够的。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="0b4e7-130">你可能还需要查找分配给用户的特定对象 ID。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="0b4e7-131">按照以下步骤在 Azure 门户中查找用户的对象 ID：</span><span class="sxs-lookup"><span data-stu-id="0b4e7-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="0b4e7-132">登录 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="0b4e7-133">从菜单中选择“Azure Active Directory”。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="0b4e7-134">找到菜单上的 " **管理** " 部分，然后选择 " **用户**"。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="显示 Azure Active Directory 菜单，其中突出显示了 &quot;用户&quot; 选项。":::

4. <span data-ttu-id="0b4e7-136">在 "用户" 页上，在 "搜索" 框中键入用户的名称。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="显示 &quot;用户&quot; 页，其中包含用于搜索特定用户的搜索框。":::

5. <span data-ttu-id="0b4e7-138">选择用户在列表中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="显示用户页，其中显示搜索用户的行。":::

6. <span data-ttu-id="0b4e7-140">在用户的配置文件页上找到标识部分。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="0b4e7-141">"对象 ID" 字段显示在此处，其中包含用户的唯一对象 ID。</span><span class="sxs-lookup"><span data-stu-id="0b4e7-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="显示 &quot;用户配置文件&quot; 页，其中包含标识部分和一个突出显示的对象 ID 字段。":::

## <a name="next-steps"></a><span data-ttu-id="0b4e7-143">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0b4e7-143">Next steps</span></span>

- [<span data-ttu-id="0b4e7-144">通过 PowerShell 或 CLI 以编程方式查找租户 ID</span><span class="sxs-lookup"><span data-stu-id="0b4e7-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="0b4e7-145">详细了解 Azure Active Directory 中的用户配置文件</span><span class="sxs-lookup"><span data-stu-id="0b4e7-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="0b4e7-146">了解合作伙伴可以如何查看或导出合作伙伴中心的客户详细信息</span><span class="sxs-lookup"><span data-stu-id="0b4e7-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

