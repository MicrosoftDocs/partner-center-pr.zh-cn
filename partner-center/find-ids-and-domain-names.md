---
title: 查找租户 ID、域名、用户对象 ID
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何查找 Azure 门户中的 Id-组织的 Azure AD 租户 ID、域名或特定用户对象 ID。 某些任务需要此信息。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/17/2020
ms.locfileid: "90740379"
---
# <a name="locate-important-ids-for-a-user"></a>为用户找到重要 Id

本文介绍如何使用 [Azure 门户](https://portal.azure.com/) 查找用户的以下信息：

- Microsoft Azure Active Directory (Azure AD 用户的组织或公司的) 租户 ID

- 与 Azure AD 租户相关联的组织或公司的主域名

- 用户对象 ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>查找 Microsoft Azure AD 租户 ID 和主域名

按照以下步骤在 Azure 门户中查找 Azure AD 租户 ID 或主域名。

> [!NOTE]
> 租户 ID 在不同的应用程序或资源中可以被称为不同的名称。 例如，租户 ID 可能称为目录 ID，Azure Active Directory (Azure AD) 租户、Microsoft ID 或某些报表，甚至是 *tenantguid*。

1. 登录 [Azure 门户](https://portal.azure.com/)。

2. 从菜单中选择“Azure Active Directory”。

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="显示 Azure 门户从菜单中选择 "Azure Active Directory" 选项。":::

3. 此时将显示 Azure Active Directory **概述** "页。 若要查找 Azure AD 租户 ID 或主域名，请查找 " **租户 id** " 字段和 " **主域** " 字段。 这些字段显示在 "租户信息" 部分中。

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="显示具有两个突出显示的字段、租户 ID 和主域名的 "概述" 页。":::

4. 您可以通过其他一些方式在 Azure 门户中找到租户 ID。 从菜单中选择“Azure Active Directory”。 然后，找到菜单上的 " **管理** " 部分，然后选择 " **属性**"。

   "属性" 页还显示用户的关联租户 ID。

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="显示 "属性" 页，其中包含突出显示的租户 ID 字段。":::

## <a name="find-the-user-object-id"></a>查找用户对象 ID

仅查找域名和租户 ID 可能并不总是足够的。 你可能还需要查找分配给用户的特定对象 ID。 按照以下步骤在 Azure 门户中查找用户的对象 ID：

1. 登录 [Azure 门户](https://portal.azure.com/)。

2. 从菜单中选择“Azure Active Directory”。

3. 找到菜单上的 " **管理** " 部分，然后选择 " **用户**"。

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="显示 Azure Active Directory 菜单，其中突出显示了 "用户" 选项。":::

4. 在 "用户" 页上，在 "搜索" 框中键入用户的名称。

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="显示 "用户" 页，其中包含用于搜索特定用户的搜索框。":::

5. 选择用户在列表中显示的名称。  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="显示用户页，其中显示搜索用户的行。":::

6. 在用户的配置文件页上找到标识部分。 "对象 ID" 字段显示在此处，其中包含用户的唯一对象 ID。

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="显示 "用户配置文件" 页，其中包含标识部分和一个突出显示的对象 ID 字段。":::

## <a name="next-steps"></a>后续步骤

- [详细了解 Azure Active Directory 中的用户配置文件](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [了解合作伙伴可以如何查看或导出合作伙伴中心的客户详细信息](see-your-customer-list.md)