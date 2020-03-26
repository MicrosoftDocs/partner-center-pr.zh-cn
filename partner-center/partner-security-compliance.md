---
title: 合作伙伴安全要求状态 | 合作伙伴中心
ms.date: 10/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解为了提高云解决方案提供商计划中的顾问、控制面板供应商以及合作伙伴的安全性而需满足的全新强制性要求。
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: high
ms.topic: conceptual
ms.openlocfilehash: 2fc0926f2277cea8eebd7157af44338aabfaa94c
ms.sourcegitcommit: e98684319d8f9bfc2cadad77fd7c51d7aa32c419
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "80136318"
---
# <a name="partner-security-requirements-status"></a>合作伙伴安全要求状态

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
  - 直接计费
  - 间接提供商
  - 间接经销商
- 所有控制面板供应商
- 所有顾问

**相应的用户**
-    所有支持的用户，包括来宾用户

增强隐私保护和安全性是我们优先关注的事项。 我们知道，最好的防御措施是防患于未然，链条的强度取决于其最弱的一环。 因此，我们需要生态系统中的所有人都行动起来，确保将安全保护措施实施到位。 为了保护合作伙伴和客户，我们引入了一系列强制性安全要求，针对那些参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴。

从 2019 年 8 月 1 日开始，所有合作伙伴都必须对其合作伙伴租户中的所有用户（包括服务帐户）强制实施多重身份验证。 有关新安全策略的详细信息，请阅读[合作伙伴安全要求](partner-security-requirements.md)。

我们需要确保每位用户在每次身份验证时都回应 MFA 质询。 可以通过下述方式之一来实现这一点：

- 实施 Azure AD Premium，确保对每位用户强制实施 MFA
- 实施 [Azure AD 安全性默认设置](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- 实施第三方解决方案，确保对每位用户强制实施 MFA

## <a name="partner-security-requirements-status"></a>合作伙伴安全要求状态

此报告可让你通过某种方式了解自己的不足之处，以此确认自己的安全要求状态。 跟踪结果会定期更新。

>[!NOTE]
>只有合作伙伴中心才支持“合作伙伴安全要求状态”报告。 Microsoft Cloud for US Government 或 Microsoft Cloud Germany 不提供此报告。 强烈建议所有通过主权云（世纪互联、Microsoft Cloud for US Government、德国 Microsoft 云）进行事务处理的合作伙伴立即履行这些安全要求。 但是，这些合作伙伴不是必须满足这些新的在 2019 年 8 月 1 日生效的安全要求。 Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。

## <a name="multi-factor-authentication-mfa-report"></a>多重身份验证 (MFA) 报告

合作伙伴中心 MFA 报告根据云解决方案提供商租户的 MFA 配置和合作伙伴中心活动，提供两种类型的指标，从而提供对合作伙伴 MFA 实施情况的见解： 

### <a name="mfa-configuration-on-a-csp-tenant"></a>云解决方案提供商租户上的 MFA 配置

此指标与每日捕获并报告的云解决方案提供商租户上的 MFA 配置相关。 它使用这些 [MFA 选项](https://aka.ms/partner-mfa-get-started)中的任意一个来度量强制实施了 MFA 的已启用用户帐户的百分比。 例如：

- Contoso 是一个云解决方案提供商合作伙伴，其租户中有 110 个用户帐户，这些帐户中有 10 个处于禁用状态。 
- 在剩余的 100 个用户帐户中，有 90 个已使用提供的 [MFA 选项](https://aka.ms/partner-mfa-get-started)强制实施了 MFA。 因此，该指标显示 90%。 

### <a name="partner-center-activities-with-mfa"></a>在实施了 MFA 的情况下进行的合作伙伴中心活动

每当员工登录到合作伙伴中心来完成工作，或者在合作伙伴中心通过 API 获取或发送数据时，其安全状态将受到质询和跟踪。 你的应用程序以及任何控制面板供应商应用程序也会受到安全状态跟踪。 显示的状态是过去 7 天的状态。

#### <a name="mfa-verification-completed-by-users"></a>用户完成的 MFA 验证

此指标与合作伙伴中心仪表板中的活动相关。 它度量已完成 MFA 验证的用户执行的操作百分比。 例如：

- Contoso 是一家 CSP 合作伙伴，它有两名管理代理：Jane 和 John。
- 在第一天，Jane 在未完成 MFA 验证的情况下登录到了合作伙伴中心仪表板，并执行了 3 项操作。
- 在第二天，John 在未完成 MFA 验证的情况下登录到了合作伙伴中心仪表板，并执行了 5 项操作。
- 在第三天，Jane 在完成 MFA 验证的情况下登录到了合作伙伴中心仪表板，并执行了 2 项操作。
- 在剩余的 4 天，这两名代理未执行任何操作。
- 在 7 天内共执行了 10 项操作，其中，有 2 项操作是用户在已完成 MFA 验证的情况下执行的。 因此，指标显示 20%。

#### <a name="appuser-authentication"></a>应用+用户身份验证

此指标与使用应用+用户身份验证发出的合作伙伴中心 API 请求的用法相关。 它度量结合 MFA 声明使用访问令牌发出的 API 请求百分比。 例如：

- Fabrikam 是一家 CSP 合作伙伴，它的某个 CSP 应用程序混合使用了应用+用户身份验证和仅限应用的身份验证方法。
- 第一天，该应用程序发出了 3 个 API 请求，这些请求是在未完成 MFA 验证的情况下，通过应用+用户身份验证方法获取的访问令牌提供支持的。
- 第二天，该应用程序发出了 5 个 API 请求，这些请求是由使用仅限应用的身份验证获取的访问令牌提供支持的。
- 第三天，该应用程序发出了 2 个 API 请求，这些请求是在已完成 MFA 验证的情况下，使用应用+用户身份验证方法获取的访问令牌提供支持的。
- 在剩余的 4 天里，这两名代理未执行任何操作。
- 指标中会忽略第二天发出的，由通过仅限应用的身份验证获取的访问令牌提供支持的 5 个 API 请求，因为该身份验证方法未使用用户凭据。 在剩余的 5 个操作中，有 2 个操作是在已完成 MFA 验证的情况下通过获取的访问令牌提供支持的。 因此，指标显示 40%。

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>如果 MFA 报告中的指标不是 100% 该怎么办

对于已实施 MFA 的合作伙伴，合作伙伴中心 MFA 报告中的指标可能不是 100%。 若要了解原因，请考虑以下几个因素。

> [!NOTE]
> 需要咨询组织中熟悉标识管理以及合作伙伴租户 MFA 实施方案的人员。

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>是否对合作伙伴租户实施了 MFA？

如果没有，则首先需要对合作伙伴租户实施 MFA。 有关如何实施 MFA 的详细信息，请参阅[合作伙伴安全要求](partner-security-requirements.md)一文。

### <a name="have-you-only-recently-completed-mfa-implementation"></a>是否只是最近才完成了 MFA 的实施？

指标是每日计算的，考虑过去 7 天内执行的操作。 如果你只是最近才对合作伙伴租户完成了 MFA 的实施，指标可能不是 100%。

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>是否从 MFA 实施方案中排除了一些用户帐户？

了解当前的 MFA 实施方案是包括所有用户帐户，还是只包括一部分用户帐户。 有些 MFA 解决方案基于策略且支持用户排除，而有些则可能要求按用户显式启用 MFA。 确认未从当前 MFA 实施方案中排除任何用户。 对于已排除的任何用户帐户，他们登录合作伙伴中心来执行与云解决方案提供商相关的任何活动，都可能导致指标不是 100%。

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>是否仅在满足特定的条件时才需要 MFA？

了解当前的实施方案是否仅在特定的条件下强制实施 MFA。 某些 MFA 解决方案具有灵活性，允许仅在满足特定的条件（例如，用户从未知的设备或位置进行访问）时 才强制实施 MFA。 如果为某个用户启用了 MFA，但该用户在访问合作伙伴中心时不一定要完成 MFA 验证，则可能会导致指标不是 100%。

>[!NOTE]
>对于已使用 Azure AD 安全性默认设置实施了 MFA 的合作伙伴，请务必注意，对于非管理员用户帐户，会根据风险强制实施多重身份验证。 仅当用户尝试进行有风险的登录（例如，从不同的位置登录）时，系统才会提示他们完成 MFA。 此外，用户有长达 14 天的时间来注册 MFA。 在这 14 天内，未完成 MFA 注册的用户不会受到 MFA 验证的质询。 因此，对于已使用 Azure AD 安全性默认设置实施了 MFA 的合作伙伴，指标可能不是 100%，这在预料之中。

### <a name="are-you-using-3rd-party-mfa-solution"></a>是否在使用第三方 MFA 解决方案？

如果使用第三方 MFA 解决方案，请确定如何将它与 Azure AD 集成。 一般情况下，有两种方法：联合与自定义控制：

* **标识联合** - 当 Azure AD 收到身份验证请求时，Azure AD 会将用户重定向到联合的标识提供者进行身份验证。 身份验证成功后，联合的标识提供者会将用户重定向回到 Azure AD，并提供一个 SAML 令牌。 为使 Azure AD 能够识别到该用户在对联合的标识提供者进行身份验证时已完成 MFA 验证，该 SAML 令牌必须包含 *authenticationmethodsreferences*  声明（值为 *multipleauthn*）。 检查联合的标识提供者是否支持发出此类声明。 如果是，请检查联合的标识提供者是否已配置为提供此项支持。 如果缺少声明，Azure AD（因而也包括合作伙伴中心）将不知道用户已完成 MFA 验证，这可能会导致指标不是 100%。

* **自定义控制** - 无法使用 Azure AD 自定义控制来确定用户是否已通过第三方 MFA 解决方案完成了 MFA 验证。 因此，对于 Azure AD（因而也包括合作伙伴中心）而言，通过自定义控制完成 MFA 验证的任何用户始终看上去并未完成 MFA 验证。 如果可能，我们建议在与 Azure AD 集成时改用标识联合，而不要使用自定义控制。

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>确定哪些用户在未完成 MFA 的情况下登录到了合作伙伴中心

确定哪些用户在未完成 MFA 验证的情况下登录到了合作伙伴中心，并根据当前的 MFA 实施方案对其进行验证，可能会有帮助。 可以使用 [Azure AD 登录报告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)来确定用户是否已完成 MFA 验证。 Azure AD 登录报告目前仅适用于订阅了 Azure AD Premium 或任何包含 Azure AD Premium 的 O365 SKU（例如 EMS）的合作伙伴。

**详细信息**

- [合作伙伴中心安全指导组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [合作伙伴中心安全要求](partner-security-requirements.md)
- [合作伙伴中心安全要求常见问题解答](partner-security-requirements-faq.md)
