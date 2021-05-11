---
title: 查找租户 ID、域名、用户对象 ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在租户 ID、Azure 门户或特定用户对象 ID Azure AD中查找 ID。 某些任务需要此信息。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740278"
---
# <a name="locate-important-ids-for-a-user"></a>查找用户的重要 ID

**相应的角色**

- 全局管理员

本文介绍如何使用 Azure 门户查找用户的[](https://portal.azure.com/)以下信息：

- Microsoft Azure Active Directory (Azure AD) 组织或公司的租户 ID

- 与租户关联的组织或公司的主Azure AD域名

- 用户对象 ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>查找Microsoft Azure AD ID 和主域名

按照以下步骤在Azure AD中查找租户 ID 或Azure 门户。  (若要以编程方式查找租户 ID，请参阅使用 [PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)或 CLI .) 

> [!NOTE]
> 租户 ID 可能在不同的应用程序或资源中称为不同的名称。 例如，租户 ID 可能称为目录 ID、Azure Active Directory (Azure AD) 租户、Microsoft ID 或某些报表，甚至是 *租户的*。

1. 登录 [Azure 门户](https://portal.azure.com/)。

2. 从菜单中选择“Azure Active Directory”。

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="显示Azure 门户菜单中Azure Active Directory选项的选项。":::

3. 将显示Azure Active Directory **概述** "页。 若要查找Azure AD ID 或主域名，请查找"租户 **ID"** 字段和" **主域"** 字段。 这些字段显示在"租户信息"部分中。

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="显示&quot;概述&quot;页，其中突出显示了两个字段：租户 ID 和主域名。":::

4. 可以通过其他几种方法Azure 门户租户 ID。 从菜单中选择“Azure Active Directory”。 然后，找到 **菜单上的"** 管理"部分，然后选择"属性 **"。**

   "属性" 页还显示用户的关联租户 ID。

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="显示 &quot;属性&quot; 页，其中包含突出显示的租户 ID 字段。":::

## <a name="find-the-user-object-id"></a>查找用户对象 ID

仅查找域名和租户 ID 可能并不总是足够的。 你可能还需要查找分配给用户的特定对象 ID。 按照以下步骤在 Azure 门户中查找用户的对象 ID：

1. 登录 [Azure 门户](https://portal.azure.com/)。

2. 从菜单中选择“Azure Active Directory”。

3. 找到菜单上的 " **管理** " 部分，然后选择 " **用户**"。

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="显示 Azure Active Directory 菜单，其中突出显示了 &quot;用户&quot; 选项。":::

4. 在 "用户" 页上，在 "搜索" 框中键入用户的名称。

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="显示 &quot;用户&quot; 页，其中包含用于搜索特定用户的搜索框。":::

5. 选择用户在列表中显示的名称。  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="显示用户页，其中显示搜索用户的行。":::

6. 在用户的配置文件页上找到标识部分。 "对象 ID" 字段显示在此处，其中包含用户的唯一对象 ID。

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="显示 &quot;用户配置文件&quot; 页，其中包含标识部分和一个突出显示的对象 ID 字段。":::

## <a name="next-steps"></a>后续步骤

- [通过 PowerShell 或 CLI 以编程方式查找租户 ID](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [详细了解 Azure Active Directory 中的用户配置文件](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [了解合作伙伴可以如何查看或导出合作伙伴中心的客户详细信息](see-your-customer-list.md)

