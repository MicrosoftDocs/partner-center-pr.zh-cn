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
ms.openlocfilehash: 637e88205d9944f7220e227b5101220d94ed42db
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000431"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a>创建用户帐户并分配角色和权限

**相应的角色**

- 帐户管理员
- 全局管理员
- “用户管理”管理员

为需要访问合作伙伴中心的员工创建用户帐户。 这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。 有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。


## <a name="add-a-new-user"></a>添加新用户

1. 在合作伙伴中心右上角的“设置”图标中，选择“用户管理”。

2. 选择“添加用户”。

3. 输入用户全名和唯一的电子邮件地址。

4. 选择要分配给用户的代理类型和/或管理员类型。 合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。  如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。

5. 选择“添加”以创建用户帐户。 在下一页上确认用户的详细信息。

> [!IMPORTANT]  
> 记下此页面上显示的新用户的登录信息。 确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。 


用户将需要使用其用户名和临时密码来登录合作伙伴中心。 当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。 

## <a name="find-the-role-youve-been-assigned"></a>查找已分配的角色

如果全局管理员没有告诉你，你可以通过执行以下操作来了解你在合作伙伴中心具有哪些角色：

1. 登录到合作伙伴中心 [面板]https://partner.microsoft.com/dashboard/home).

1. 选择“帐户设置”图标，然后选择“我的配置文件” 。
 
1. 选择“角色和权限”选项卡。你将看到你的角色和权限。
 

>[!Note]
>如果在登录时看不到程序，则通常意味着你无权使用该程序。 例如，如果在登录时看不到“奖励”页，则你没有奖励权限。 全局管理员可以向你授予所需的权限。


## <a name="find-your-global-admin"></a>查找全局管理员

有时，用户可能需要更改其角色，或者新用户可能需要特定的角色分配。  
若要查找可以进行角色更改或将角色分配给新用户的全局管理员，请从合作伙伴中心右上角的“帐户设置”图标，选择“用户管理”并筛选全局管理员，或者可以转到“我的配置文件”，选择“角色和权限”并查看可帮助你提升权限的不同管理员的列表   。 


## <a name="new-global-admin"></a>新的全局管理员

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

1. 在合作伙伴中心面板中，选择面板右上角的“我的帐户”图标，然后选择“我的个人资料” 。

2. 在“我的 Learning”下方，可以关联你的 Microsoft Learning 帐户，还可以将你的 Microsoft 帐户连接到 Partner University。

## <a name="next-steps"></a>后续步骤

- [为需要在合作伙伴中心工作的公司用户分配用户角色和权限](permissions-overview.md)