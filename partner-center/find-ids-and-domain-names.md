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
# <a name="locate-important-ids-for-a-user"></a>为用户找到重要 Id

**相应的角色**：全局管理员

本文介绍如何使用 [Azure 门户](https://portal.azure.com/) 查找用户的以下信息：

- Microsoft Azure Active Directory (Azure AD 用户的组织或公司的) 租户 ID

- 与 Azure AD 租户相关联的组织或公司的主域名

- 用户对象 ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>查找 Microsoft Azure AD 租户 ID 和主域名

按照以下步骤在 Azure 门户中查找 Azure AD 租户 ID 或主域名。  (如果要以编程方式查找租户 ID，请参阅 [使用 PowerShell 或 CLI 查找租户 id](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)。 ) 

> [!NOTE]
> 租户 ID 在不同的应用程序或资源中可以被称为不同的名称。 例如，租户 ID 可能称为目录 ID，Azure Active Directory (Azure AD) 租户、Microsoft ID 或某些报表，甚至是 *tenantguid*。

1. 登录到 [Azure 门户](https://portal.azure.com/)。

2. 从菜单中选择“Azure Active Directory”。

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="显示 Azure 门户从菜单中选择 &quot;Azure Active Directory&quot; 选项。":::

3. 此时将显示 Azure Active Directory **概述** "页。 若要查找 Azure AD 租户 ID 或主域名，请查找 " **租户 id** " 字段和 " **主域** " 字段。 这些字段显示在 "租户信息" 部分中。

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="显示具有两个突出显示的字段、租户 ID 和主域名的 &quot;概述&quot; 页。":::

4. 您可以通过其他一些方式在 Azure 门户中找到租户 ID。 从菜单中选择“Azure Active Directory”。 然后，找到菜单上的 " **管理** " 部分，然后选择 " **属性**"。

   "属性"页还显示用户的关联租户 ID。

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="显示&quot;属性&quot;页，突出显示了&quot;租户 ID&quot;字段。":::

## <a name="find-the-user-object-id"></a>查找用户对象 ID

仅查找域名和租户 ID 可能并不总是足够。 可能还需要查找分配给用户的特定对象 ID。 按照以下步骤查找用户的对象 ID，具体Azure 门户：

1. 登录到 [Azure 门户](https://portal.azure.com/)。

2. 从菜单中选择“Azure Active Directory”。

3. 找到菜单 **上的"** 管理"部分，然后选择"用户 **"。**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="显示Azure Active Directory菜单，并突出显示&quot;用户&quot;选项。":::

4. 在"用户"页的搜索框中键入用户名。

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="显示包含搜索框的&quot;用户&quot;页，用于搜索特定用户。":::

5. 选择在列表中显示用户的名称。  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="显示显示已搜索用户的行的用户页。":::

6. 在用户的"个人资料"页上找到"标识"部分。 此处将显示"对象 ID"字段，以及用户的唯一对象 ID。

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="显示&quot;用户配置文件&quot;页，其中&quot;标识&quot;部分和一个突出显示的对象 ID 字段。":::

## <a name="next-steps"></a>后续步骤

- [使用 PowerShell 或 CLI 以编程方式查找租户 ID](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [在中详细了解用户配置文件Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [了解合作伙伴如何查看或导出客户详细信息合作伙伴中心](see-your-customer-list.md)

