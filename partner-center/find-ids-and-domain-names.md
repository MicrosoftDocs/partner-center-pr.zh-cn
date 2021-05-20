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
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150856"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="be0fe-104">为用户找到重要 Id</span><span class="sxs-lookup"><span data-stu-id="be0fe-104">Locate important IDs for a user</span></span>

<span data-ttu-id="be0fe-105">**相应的角色**：全局管理员</span><span class="sxs-lookup"><span data-stu-id="be0fe-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="be0fe-106">本文介绍如何使用 [Azure 门户](https://portal.azure.com/) 查找用户的以下信息：</span><span class="sxs-lookup"><span data-stu-id="be0fe-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="be0fe-107">Microsoft Azure Active Directory (Azure AD 用户的组织或公司的) 租户 ID</span><span class="sxs-lookup"><span data-stu-id="be0fe-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="be0fe-108">与 Azure AD 租户相关联的组织或公司的主域名</span><span class="sxs-lookup"><span data-stu-id="be0fe-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="be0fe-109">用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="be0fe-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="be0fe-110">查找 Microsoft Azure AD 租户 ID 和主域名</span><span class="sxs-lookup"><span data-stu-id="be0fe-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="be0fe-111">按照以下步骤在 Azure 门户中查找 Azure AD 租户 ID 或主域名。</span><span class="sxs-lookup"><span data-stu-id="be0fe-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="be0fe-112"> (如果要以编程方式查找租户 ID，请参阅 [使用 PowerShell 或 CLI 查找租户 id](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)。 ) </span><span class="sxs-lookup"><span data-stu-id="be0fe-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="be0fe-113">租户 ID 在不同的应用程序或资源中可以被称为不同的名称。</span><span class="sxs-lookup"><span data-stu-id="be0fe-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="be0fe-114">例如，租户 ID 可能称为目录 ID，Azure Active Directory (Azure AD) 租户、Microsoft ID 或某些报表，甚至是 *tenantguid*。</span><span class="sxs-lookup"><span data-stu-id="be0fe-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="be0fe-115">登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="be0fe-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="be0fe-116">从菜单中选择“Azure Active Directory”。</span><span class="sxs-lookup"><span data-stu-id="be0fe-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="显示 Azure 门户从菜单中选择 &quot;Azure Active Directory&quot; 选项。":::

3. <span data-ttu-id="be0fe-118">此时将显示 Azure Active Directory **概述** "页。</span><span class="sxs-lookup"><span data-stu-id="be0fe-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="be0fe-119">若要查找 Azure AD 租户 ID 或主域名，请查找 " **租户 id** " 字段和 " **主域** " 字段。</span><span class="sxs-lookup"><span data-stu-id="be0fe-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="be0fe-120">这些字段显示在 "租户信息" 部分中。</span><span class="sxs-lookup"><span data-stu-id="be0fe-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="显示具有两个突出显示的字段、租户 ID 和主域名的 &quot;概述&quot; 页。":::

4. <span data-ttu-id="be0fe-122">您可以通过其他一些方式在 Azure 门户中找到租户 ID。</span><span class="sxs-lookup"><span data-stu-id="be0fe-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="be0fe-123">从菜单中选择“Azure Active Directory”。</span><span class="sxs-lookup"><span data-stu-id="be0fe-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="be0fe-124">然后，找到菜单上的 " **管理** " 部分，然后选择 " **属性**"。</span><span class="sxs-lookup"><span data-stu-id="be0fe-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="be0fe-125">"属性"页还显示用户的关联租户 ID。</span><span class="sxs-lookup"><span data-stu-id="be0fe-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="显示&quot;属性&quot;页，突出显示了&quot;租户 ID&quot;字段。":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="be0fe-127">查找用户对象 ID</span><span class="sxs-lookup"><span data-stu-id="be0fe-127">Find the user object ID</span></span>

<span data-ttu-id="be0fe-128">仅查找域名和租户 ID 可能并不总是足够。</span><span class="sxs-lookup"><span data-stu-id="be0fe-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="be0fe-129">可能还需要查找分配给用户的特定对象 ID。</span><span class="sxs-lookup"><span data-stu-id="be0fe-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="be0fe-130">按照以下步骤查找用户的对象 ID，具体Azure 门户：</span><span class="sxs-lookup"><span data-stu-id="be0fe-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="be0fe-131">登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="be0fe-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="be0fe-132">从菜单中选择“Azure Active Directory”。</span><span class="sxs-lookup"><span data-stu-id="be0fe-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="be0fe-133">找到菜单 **上的"** 管理"部分，然后选择"用户 **"。**</span><span class="sxs-lookup"><span data-stu-id="be0fe-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="显示Azure Active Directory菜单，并突出显示&quot;用户&quot;选项。":::

4. <span data-ttu-id="be0fe-135">在"用户"页的搜索框中键入用户名。</span><span class="sxs-lookup"><span data-stu-id="be0fe-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="显示包含搜索框的&quot;用户&quot;页，用于搜索特定用户。":::

5. <span data-ttu-id="be0fe-137">选择在列表中显示用户的名称。</span><span class="sxs-lookup"><span data-stu-id="be0fe-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="显示显示已搜索用户的行的用户页。":::

6. <span data-ttu-id="be0fe-139">在用户的"个人资料"页上找到"标识"部分。</span><span class="sxs-lookup"><span data-stu-id="be0fe-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="be0fe-140">此处将显示"对象 ID"字段，以及用户的唯一对象 ID。</span><span class="sxs-lookup"><span data-stu-id="be0fe-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="显示&quot;用户配置文件&quot;页，其中&quot;标识&quot;部分和一个突出显示的对象 ID 字段。":::

## <a name="next-steps"></a><span data-ttu-id="be0fe-142">后续步骤</span><span class="sxs-lookup"><span data-stu-id="be0fe-142">Next steps</span></span>

- [<span data-ttu-id="be0fe-143">使用 PowerShell 或 CLI 以编程方式查找租户 ID</span><span class="sxs-lookup"><span data-stu-id="be0fe-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="be0fe-144">在中详细了解用户配置文件Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="be0fe-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="be0fe-145">了解合作伙伴如何查看或导出客户详细信息合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="be0fe-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

