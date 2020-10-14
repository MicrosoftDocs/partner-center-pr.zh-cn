---
title: 创建用户帐户并分配角色
description: 必须先为每个员工分配一个角色，然后他们才能访问合作伙伴中心。 了解如何创建用户帐户、分配角色和设置权限。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006765"
---
# <a name="create-user-accounts"></a>创建用户帐户  

**相应的角色**

- 帐户管理员
- 全局管理员
- “用户管理”管理员

为需要访问合作伙伴中心的员工创建用户帐户。 这些任务必须由用户管理员、帐户管理员或全局管理员来完成。执行这些任务的用户还必须分配有 Azure Active Directory (AAD) 角色“用户管理员”或“全局管理员”。 有关 AAD 角色的详细信息，请参阅 [Azure Active Directory 中的管理员角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。

## <a name="add-a-new-user"></a>添加新用户

1. 在合作伙伴中心右上角的“设置”图标中，选择“帐户设置”，再选择“用户管理”  。

2. 选择“添加用户”。

3. 输入用户全名和唯一的电子邮件地址。

4. 选择要分配给用户的代理类型和/或管理员类型。 合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，仅显示用户完成特定任务所需的功能。  如果用户需要角色分配，他们可以转到“用户管理”并筛选帐户管理员，来查找可联系的全局管理员。

5. 选择“添加”以创建用户帐户。 在下一页上确认用户的详细信息。

> [!IMPORTANT]  
> 记下此页面上显示的新用户的登录信息。 确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。 

用户将需要使用其用户名和临时密码来登录合作伙伴中心。 当用户首次登录到合作伙伴中心时，系统会提示他们更改密码。

## <a name="assign-user-roles"></a>分配用户角色

若要在合作伙伴中心操作，必须分配有一个角色。  目前，角色包括 Azure Active Directory 租户角色、云解决方案提供商 (CSP) 角色和非 AAD 公司角色。 单个公司可以需要所有这些角色。

>[!Important]
>用户必须在租户中列出才能访问合作伙伴中心。 角色分配提供额外的访问权限。

## <a name="next-steps"></a>后续步骤

- [为需要在合作伙伴中心工作的员工分配用户角色和权限](permissions-overview.md)
