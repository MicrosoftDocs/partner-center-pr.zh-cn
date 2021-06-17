---
title: 如果 MPN 计划的唯一管理员已离开公司，该怎么办？
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何查找新的 MPN 管理员或从公司的全局管理员获取帮助。此外，了解如何向全局管理员合作伙伴中心帐户。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277668"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>如果 MPN 计划的唯一管理员已离开公司，该怎么办？

**适当角色**：MPN 合作伙伴管理员|帐户管理员|全局管理员

以下文章将指导你完成三个典型方案，说明 MPN 管理员离开公司后该怎么办。

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>方案 1：MPN 合作伙伴管理员/帐户管理员已离开公司，但帐户中仍有全局管理员

在这种情况下，公司中的其他人可以分配 MPN 合作伙伴管理员角色。若要分配特定 MPN 合作伙伴管理员/帐户管理员角色的角色，

1. 使用工作合作伙伴中心登录你的 (帐户，例如 tom@contoso.com) 。
1. 从 **"全局管理员** "上的"用户管理"页筛选器中，查看公司的全局管理员是谁。 
1. 联系其中一个全局管理员，要求他们分配所需的 MPN 特定角色。 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>方案 2：MPN 合作伙伴管理员/帐户管理员已离开公司，并且帐户中没有全局管理员 

如果转到"用户管理"页并筛选"全局管理员"，但发现公司中没有任何全局管理员可以帮助你获得 MPN 特定的角色，请执行以下步骤：

1. 转到 [portal.azure.com，](https://ms.portal.azure.com/)使用工作帐户登录 (例如 tom@contoso.com ，) 。 
1. 选择左侧 **菜单导航栏中** 的"帮助 + 支持"选项。
1. 下一页上，在下拉菜单 **中选择**"支持请求和技术问题类型"，插入任何其他详细信息，然后单击"下一步 **： 解决方案"。**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="在&quot;管理员&quot;Azure 门户。":::

4. 查看下一页中建议的解决方案后，选择"下一步 **： 详细信息"并** 填写必要的字段。
1. 查看并创建支持请求。


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>方案 3：MPN 合作伙伴管理员/帐户管理员/全局管理员已离开公司，并且没有其他用户可以访问公司的Azure AD。 这是完全失去访问权限。

按照 [管理员接管](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) 步骤以管理员角色接管非Azure Active Directory目录。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>不确定公司是否已有工作帐户？

如果你不确定你的公司是否具有工作帐户，请按照以下步骤进行检查。

1. 登录到 Azure [管理门户](https://ms.portal.azure.com)。
2. 从 **Azure Active Directory** 选择"名称"，然后选择"**域名"。**
如果你已有工作帐户，门户将列出你的域名。

>[!Note]
>如果具有对 Microsoft Azure Office 365 的活动订阅，则已有一个工作帐户，并且登录凭据应与用于访问这些服务的凭据相同。