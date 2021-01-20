---
title: 使用多重身份验证来设置用户
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何为员工设置 MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182369"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>使用多重身份验证来设置用户

**相应的角色**

- 全局管理员

增强隐私保护和安全性是我们优先关注的事项。 我们知道，最好的防御措施是防患于未然，链条的强度取决于其最弱的一环。 因此，我们需要生态系统中的所有人都行动起来，确保将安全保护措施实施到位。 强烈建议所有合作伙伴为其合作伙伴租户中的用户启用多重身份验证 (MFA)。 

## <a name="add-multi-factor-authentication-for-your-users"></a>为用户添加多重身份验证

必须具有公司的全局管理员身份才能完成此任务。

为用户启用 MFA 的最简单方法是将用户添加到 Azure AD 租户。

1. 登录 [Azure 门户](https://portal.azure.com)，然后转到“用户管理”。
1. 选择“多重身份验证”。
1. 选择要启用的用户，然后选择“启用”。

这可为此用户启用 MFA。 “已启用”表示用户首次登录时，系统会要求其设置自己的 MFA 验证。 此后，这些用户在登录时需要提供通过电子邮件或短信（取决于其具体设置）收到的代码。  

:::image type="content" source="images/MFA/securityverification.png" alt-text="指定如何验证":::

>[!NOTE]
>可以强制用户使用 MFA，方法是使用与上面相同的步骤，并选择“强制执行” 。 若要了解详细信息，请参阅[启用每用户 Azure 多重身份验证来保护登录事件](/azure/active-directory/authentication/howto-mfa-userstates)。 

所有用户的初始状态都为“已禁用” **** 。 将用户注册到每用户 Azure 多重身份验证中后，用户状态更改为“已启用” **** 。 当已启用的用户登录并完成注册过程后，其状态更改为“已强制执行” **** 。 

## <a name="next-steps"></a>后续步骤

- [向用户分配角色和权限](permissions-overview.md)