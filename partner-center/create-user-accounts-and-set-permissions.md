---
title: 创建用户帐户和设置权限 | 合作伙伴中心
ms.topic: article
ms.date: 02/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心创建用户帐户，以及如何为每个需要访问权限的员工分配角色。 具有不同管理员权限的用户可以执行此操作。
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: LauraBrenner
ms.author: labrenne
Keywords: 角色, 权限, 添加用户, 分配角色, 管理员, 代理
ms.localizationpriority: high
ms.openlocfilehash: f163e37f537f537b6eae086e355c87d892d1a745
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798485"
---
# <a name="create-user-accounts-and-assign-permissions"></a>创建用户帐户并分配权限

**相应的角色**

- 帐户管理员
- 全局管理员
- “用户管理”管理员

为需要访问合作伙伴中心的员工创建用户帐户。 这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。 有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。


## <a name="add-a-new-user"></a>添加新用户

1. 在合作伙伴中心右上角的“设置”图标中，选择“用户管理”。  

2. 选择“添加用户”。 

3. 输入用户全名和唯一的电子邮件地址。

4. 选择要分配给用户的代理类型和/或管理员类型。 合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。  如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。 

5. 选择“添加”  以创建用户帐户。 在下一页上确认用户的详细信息。

> [!IMPORTANT]  
> 记下此页面上显示的新用户的登录信息。 确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。 


用户将需要使用其用户名和临时密码来登录合作伙伴中心。 当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。 


### <a name="find-your-global-admin"></a>查找全局管理员

有时，用户可能需要更改其角色，或者新用户可能需要特定的角色分配。  
若要查找可以进行角色更改或将角色分配给新用户的全局管理员，请在合作伙伴中心右上角的“设置”图标中，选择“用户管理”并筛选全局管理员。   


### <a name="new-global-admin"></a>新的全局管理员

如果全局管理员离开组织，而其他人需要接替此角色，那么你可以向 Azure 或 Office 365 团队提交票证。 有关如何执行此操作的信息，请选择以下选项之一。

[Azure 的新全局管理员](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Office 365 的新全局管理员](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>分配用户角色

若要在合作伙伴中心操作，必须分配有一个角色。  目前，角色包括 Azure Active Directory 租户角色、云解决方案提供商 (CSP) 角色和非 AAD 公司角色。 单个公司可以需要所有这些角色。

>[!Important]
>用户必须在租户中列出才能访问合作伙伴中心。 角色分配提供额外的访问权限。


**AAD 租户角色包括**：
- 全局管理员
- 用户管理员

**云解决方案提供商角色包括**：
- 管理员代理
- 计费管理员
- 销售代理
- 支持人员代理

**可管理 MPN 会员和公司的角色（非 AAD）**
- MPN 合作伙伴管理员
- 帐户管理员
- 引荐管理员
- 企业档案管理员
- 奖励管理员和用户

**控制面板供应商是云解决方案提供商，而非 AAD 角色**。
- 全局管理员

**来宾用户**必须是 AAD 租户的一部分，可以充当任何非 AAD 角色。

有关角色以及每个角色可以执行哪些操作的特定信息，请参阅[分配用户权限](permissions-overview.md)。

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>在合作伙伴中心关联用户的 Microsoft Learn 帐户

用户需要将其 MCP ID 关联到其合作伙伴中心帐户，才能查看在取得资质的过程中可以参考的培训内容和学习路径。 全局管理员在添加新用户时，请务必提醒用户将其 MCP ID 关联到其帐户。 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>如何将 MCP ID 关联到合作伙伴中心帐户

1. 在合作伙伴中心面板中，选择面板右上角的“我的帐户”图标，然后选择“我的个人资料”   。

2. 在“我的 Learning”下方，可以关联你的 Microsoft Learning 帐户，还可以将你的 Microsoft 帐户连接到 Partner University  。







