---
title: 如果你的 MPN 计划的唯一管理员离开了公司怎么办？
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何查找新的 MPN 管理员，或从公司的全局管理员那里获取帮助。同时，了解如何添加新的合作伙伴中心全局管理员。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3702ebd5a9421036a053a9a142a2f40d3e488137
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441993"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>如果你的 MPN 计划的唯一管理员离开了公司怎么办？

**相应的角色**

- MPN 合作伙伴管理员
- 帐户管理员
- 全局管理员

下面的文章将指导你完成 MPN 管理员离开公司时要执行的操作的三个典型方案。

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>方案1： MPN 合作伙伴管理员/帐户管理员已离开公司，但帐户中仍有全局管理员

在这种情况下，可以为公司中的其他人分配 MPN 合作伙伴管理员角色。要为其分配特定 MPN 合作伙伴管理员/帐户管理员角色的角色：

1. 使用工作帐户登录到合作伙伴中心帐户 (例如 tom@contoso.com) 。
1. 从 "全局管理员" 的 " **用户管理** " 页筛选器，查看你的公司的全局管理员是谁。 
1. 联系其中一个全局管理员，并请求他们为你分配所需的 MPN 特定角色。 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>方案2： MPN 合作伙伴管理员/帐户管理员已离开公司，帐户中没有全局管理员 

如果你进入 " **用户管理** " 页并筛选全局管理员，但你发现公司中没有可帮助你获取 MPN 特定角色的全局管理员，请执行以下步骤：

1. 请参阅 [portal.azure.com](https://ms.portal.azure.com/)，使用工作帐户登录 (例如 tom@contoso.com) 。 
1. 在左侧菜单导航栏中选择 " **帮助 + 支持** " 选项。
1. 在下一页上，在下拉菜单中选择 " **新建支持请求** 和 **技术问题** 类型"，插入任何其他详细信息，然后单击 " **下一步：解决方案"。**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="在 Azure 门户中找到管理员":::

4. 查看下一页中的推荐解决方案之后，选择 " **下一步：详细信息** " 并完成必需的字段。
1. 查看并创建支持请求。


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>方案3： MPN 合作伙伴管理员/帐户管理员/全局管理员离开了公司，但没有其他用户可以访问公司的 Azure AD。 这是完全的访问权限丢失。

按照 [管理员接管](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) 步骤将非托管目录作为 Azure Active Directory 管理员接管。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>不确定公司是否已有工作帐户？

如果你不确定你的公司是否具有工作帐户，请按照以下步骤进行检查。

1. 登录到 [Azure 管理门户](https://ms.portal.azure.com)。
2. 从左侧菜单中选择 " **Azure Active Directory** "，然后选择 " **域名**"。
如果你已有工作帐户，门户将列出你的域名。

>[!Note]
>如果你有 Microsoft Azure 或 Office 365 的活动订阅，你已经有了一个工作帐户，并且登录凭据应与用于访问这些服务的凭据相同。