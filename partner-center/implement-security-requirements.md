---
title: 实现合作伙伴安全要求
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何为用户实现必要的安全要求
author: LauraBrenner
ms.author: labrenne
keywords: 安全性
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133260"
---
# <a name="implement-the-partner-security-requirements"></a>实现合作伙伴安全要求

**相应的角色**

- 全局管理员

客户和合作伙伴的安全和隐私是 Microsoft 首要关注的重点。 我们不断看到有越来越多更为复杂的安全攻击在发生，这些安全攻击主要与身份遭到泄露相关。 若要通过整体防御策略来阻止安全攻击，预防性的控制至关重要，因此我们将开始实施一系列强制性安全要求，以便对合作伙伴及其客户进行保护。

本教程将介绍合作伙伴安全要求的详细信息，并介绍如何满足这些要求以及对合作伙伴目录中的用户所产生的影响。

所有参与云解决方案提供商计划的合作伙伴、控制面板供应商和顾问合作伙伴都需要对他们合作伙伴租户中的每位用户强制实施多重身份验证 (MFA)。 这一实施可以通过启用两种 [Azure Active Directory 基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)来完成。 基线策略是一组预定义的策略，用于帮助组织防范许多常见攻击。 这些常见攻击可能包括密码喷射、重播和钓鱼。 基线策略在所有版本的 Azure Active Directory 中提供。 Microsoft 会将这些基线保护策略提供给所有人，因为基于身份的攻击在过去几年呈上升趋势。

以下过程描述了如何启用两个必需的基线策略：

- **对管理员要求 MFA** 启用“对管理员要求 MFA”策略后，担任管理员角色的用户需要使用 Authenticator 应用来注册 MFA。 完成 MFA 注册以后，管理员在每次登录时都需要执行 MFA。

- **最终用户保护** “最终用户保护”是一种基于风险的 MFA 基线策略，用于保护目录中的所有用户。 启用此策略以后，所有用户就必须使用 Authenticator 应用注册 MFA。 用户可以忽略 MFA 注册提示 14 天，此期限过后系统会阻止用户登录，直至用户注册 MFA 为止。 注册 MFA 以后，系统仅在检测到风险登录尝试时提示用户进行 MFA。 系统会阻止被盗用的用户帐户，直至用户重置密码并消除风险事件为止。

启用这些策略后，每位用户都能够使用 Azure MFA，无需额外成本。 如果你使用的是第三方解决方案，则需要在每位用户访问 Microsoft 商业云服务时对他们强制实施 MFA。

>[!NOTE]
>由于将对合作伙伴目录中的每位用户强制实施 MFA，因此利用用户凭据的所有自动化或集成都将受到影响。 若要消除这种影响，你需要修改将自动化或集成连接到 Microsoft 商业云服务的方式。 如果所连接的服务支持基于令牌的身份验证，我们建议你实现[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)。

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>步骤一：阻止任何现有的旧版身份验证协议

启用“对管理员和最终用户保护要求 MFA”前，请确保用户未使用旧版身份验证协议。 请参阅[如何：使用条件访问阻止向 Azure AD 进行旧身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use)一文以了解详细信息。

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>步骤二：启用“对管理员要求 MFA”基线策略

“对管理员要求 MFA”基线策略要求对以下目录角色实施 MFA，这些角色被认为是具有最高特权的 Azure AD 角色：

- 全局管理员
- SharePoint 管理员
- Exchange 管理员
- 条件访问管理员
- 安全管理员
- 支持管理员/密码管理员
- 帐务管理员
- 用户管理员

启用“对管理员要求 MFA”策略以后，以上九种管理员角色就必须使用 Authenticator 应用注册 MFA。 完成 MFA 注册以后，管理员在每次登录时都需要执行 MFA。

如果组织在脚本或代码中使用这些帐户，请考虑将其替换为 [托管标识](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。

若要启用此策略并保护管理员，请执行以下操作：

1. 以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户** 。

2. 浏览到“Azure Active Directory” > “条件访问”。

3. 在策略列表中，选择“基线策略:对管理员要求 MFA”。

4. 将“启用策略”设置为“立即使用策略”。 

5. 选择“保存” **** 。

启用此策略后，将在登录时提示具有上述管理员角色的用户提供其他安全信息并配置移动应用。 完成此操作后，他们将能够登录到相应的云服务。

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>步骤三：启用“最终用户保护”基线策略

“最终用户保护”基线策略保护目录中的所有用户。 启用此策略以后，所有用户就必须在 14 天内注册 Azure MFA。 注册后，系统将仅在出现存在风险的登录尝试期间提示用户进行 MFA，此行为未来将针对合作伙伴租户有所更改。 系统会阻止被盗用的用户帐户，直至用户重置密码并消除风险为止。

策略“基线策略：最终用户保护”已预先配置。当你在 Azure 门户中导航到“条件访问”边栏选项卡时，会在顶部看到它。

若要启用此策略并保护用户，请执行以下操作：

1. 以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户** 。

2. 浏览到“Azure Active Directory” > “条件访问”。

3. 在策略列表中，选择“基线策略:最终用户保护(预览)”。

4. 将“启用策略”设置为“立即使用策略”。 

5. 选择“保存” **** 。

启用此策略后，将在登录时提示所有用户提供其他安全信息并配置移动应用。 完成此操作后，他们将能够登录到相应的云服务。

>[!NOTE]
>在合作伙伴安全要求强制实施之前，系统将仅基于风险提示未被“对管理员要求 MFA”基线策略涵盖的用户进行 MFA。