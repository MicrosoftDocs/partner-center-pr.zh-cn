---
title: 安全要求状态报告
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何通过安全要求状态报告和合作伙伴中心 MFA 报告来检查安全要求的合规性
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: d56b9675ea405b29190f68420037ea9a92f3d831
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086543"
---
# <a name="security-requirements-status-report"></a>安全要求状态报告

**相应的角色**
- CPV 管理员
- 全局管理员

本文介绍合作伙伴中心中的安全要求状态报告。 该报告提供有关合作伙伴租户中用户进行多重身份验证 (MFA) 的[合作伙伴安全要求](partner-security-requirements.md)的合规性指标。

要在[合作伙伴中心](https://partner.microsoft.com/dashboard)访问此报告，请转到“设置” > 帐户设置” > “安全要求状态”  。 该报告每天更新，反映过去七天的登录数据。

>[!NOTE]
>只有合作伙伴中心才支持安全要求状态报告。 Microsoft Cloud for US Government 或 Microsoft Cloud Germany 不提供此报告。 强烈建议所有通过主权云（Microsoft Cloud for US Government、德国 Microsoft 云）处理事务的合作伙伴立即履行这些安全要求。 但是，这些合作伙伴目前并不需要满足新的安全要求。 Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。

## <a name="security-status-metrics"></a>安全状态指标

此安全要求状态报告提供对合作伙伴 MFA 实现的见解，并提供有关合作伙伴租户中 MFA 配置和合作伙伴中心活动的指标。 以下部分详细介绍了这些指标。

### <a name="mfa-configuration-on-a-partner-tenant"></a>合作伙伴租户中的 MFA 配置

指标“使用此处列出的选项强制实施 MFA 的已启用用户帐户的百分比”：显示已强制实施 MFA 的合作伙伴租户中已启用用户帐户的百分比。 可以使用这些 [MFA 选项](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)之一来实现合规性。 每天都会捕获并报告此数据。 例如：

- Contoso 是一个云解决方案提供商合作伙伴，其租户中有 110 个用户帐户，这些用户帐户中有 10 个处于禁用状态。 
- 在剩余的 100 个用户帐户中，有 90 个已使用提供的 [MFA 选项](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)强制实施了 MFA。 因此，该指标显示 90%。 

### <a name="partner-center-requests-with-mfa"></a>在实施了 MFA 的情况下进行的合作伙伴中心请求

每当员工登录到合作伙伴中心来完成工作，或者在合作伙伴中心通过 API 获取或发送数据时，其安全状态将受到质询和跟踪。 你的应用程序以及任何控制面板供应商应用程序也会受到安全状态跟踪。 此数据显示在“在实施了 MFA 的情况下向合作伙伴中心发送的请求的百分比”下的指标中，并反映了过去七天的情况。

#### <a name="dashboard-mfa-verification"></a>面板 MFA 验证

“通过合作伙伴中心门户”这一指标与合作伙伴中心面板中的活动相关。 它度量已完成 MFA 验证的用户执行的操作百分比。 例如：

- Contoso 是一家 CSP 合作伙伴，它有两名管理代理：Jane 和 John。
- 在第一天，Jane 在未完成 MFA 验证的情况下登录到了合作伙伴中心仪表板，并执行了 3 项操作。
- 在第二天，John 在未完成 MFA 验证的情况下登录到了合作伙伴中心仪表板，并执行了 5 项操作。
- 在第三天，Jane 在完成 MFA 验证的情况下登录到了合作伙伴中心仪表板，并执行了 2 项操作。
- 在剩余的 4 天里，这两名代理未执行任何操作。
- 在 7 天内共执行了 10 项操作，其中有 2 项是用户在已完成 MFA 验证的情况下执行的。 因此，指标显示 20%。

使用“没有 MFA 的门户请求”文件来了解哪些用户未进行 MFA 验证便已登录到合作伙伴中心仪表板，及其在报告时段内进行最后一次访问的时间。

#### <a name="appuser-mfa-verification"></a>应用+用户 MFA 验证

“通过 API 或 SDK”这一指标与通过合作伙伴中心 API 请求进行的应用+用户身份验证有关。 它度量结合 MFA 声明使用访问令牌发出的 API 请求百分比。 例如：

- Fabrikam 是一家 CSP 合作伙伴，它的某个 CSP 应用程序混合使用了应用+用户身份验证和仅限应用的身份验证方法。
- 第一天，该应用程序发出了 3 个 API 请求，这些请求是在未完成 MFA 验证的情况下，通过应用+用户身份验证方法获取的访问令牌提供支持的。
- 第二天，该应用程序发出了 5 个 API 请求，这些请求是由使用仅限应用的身份验证获取的访问令牌提供支持的。
- 第三天，该应用程序发出了 2 个 API 请求，这些请求是由将“应用+用户”身份验证方法与 MFA 验证配合使用来获取的访问令牌提供支持的。
- 在剩余的 4 天里，这两名代理未执行任何操作。
- 指标中会忽略第二天发出的 5 个 API 请求（由通过仅限应用的身份验证获取的访问令牌提供支持），因为该身份验证方法未使用用户凭据。 在剩余的 5 个操作中，有 2 个操作是在已完成 MFA 验证的情况下通过获取的访问令牌提供支持的。 因此，指标显示 40%。

如果要了解哪些应用和用户活动导致此指标为非 100%，请使用文件：

- “API 请求摘要”来了解应用程序的总体 MFA 状态。
- “所有 API 请求”来了解租户的用户发出的每个 API 请求的详细信息，结果限制为最多 10000 个最新请求，以获得更好的下载体验。

## <a name="actions-for-mfa-status-below-100"></a>MFA 状态低于 100% 时采取的措施

一些实施了 MFA 的合作伙伴可能会发现报告指标低于 100%。 若要了解原因，请考虑以下几个因素。

> [!NOTE]
> 需要咨询组织中熟悉标识管理以及合作伙伴租户 MFA 实施方案的人员。

### <a name="implemented-mfa-for-your-partner-tenant"></a>对合作伙伴租户实施 MFA

你必须对合作伙伴租户实施 MFA 才能实现合规性。 有关如何实施 MFA 的详细信息，请参阅[使用合作伙伴中心或合作伙伴中心 API 的安全要求](partner-security-requirements.md)。

>[!NOTE]
> MFA 指标是每日计算的，并会将过去 7 天内执行的操作考虑在内。 如果你只是最近才对合作伙伴租户完成了 MFA 的实施，指标可能尚未显示 100%。

### <a name="verify-mfa-on-all-user-accounts"></a>验证所有用户帐户上的 MFA

了解当前的 MFA 实施方案是包括所有用户帐户，还是只包括一部分用户帐户。 有些 MFA 解决方案基于策略且支持用户排除，而有些则可能要求按用户显式启用 MFA。 确认未从当前 MFA 实施方案中排除任何用户。 对于已排除的任何用户帐户，他们登录合作伙伴中心来执行与云解决方案提供商、控制面板供应商或顾问相关的任何活动时，都可能导致指标不是 100%。

### <a name="review-your-mfa-conditions"></a>审查你的 MFA 条件

了解当前的实施方案是否仅在特定的条件下强制实施 MFA。 某些 MFA 解决方案具有灵活性，允许仅在满足特定的条件（例如，用户从未知的设备或位置进行访问）时 才强制实施 MFA。 如果为某个用户启用了 MFA，但该用户在访问合作伙伴中心时不一定要完成 MFA 验证，则可能会导致指标不是 100%。

>[!NOTE]
>对于已使用 Azure AD 安全性默认设置实施了 MFA 的合作伙伴，请务必注意，对于非管理员用户帐户，会根据风险强制实施多重身份验证。 仅当用户尝试进行有风险的登录（例如，从不同的位置登录）时，系统才会提示他们完成 MFA。 此外，用户有长达 14 天的时间来注册 MFA。 在这 14 天内，未完成 MFA 注册的用户不会受到 MFA 验证的质询。 因此，对于已使用 Azure AD 安全性默认设置实施了 MFA 的合作伙伴，指标可能不是 100%，这在预料之中。

### <a name="review-third-party-mfa-configurations"></a>审查第三方 MFA 配置

如果使用第三方 MFA 解决方案，请确定如何将它与 Azure AD 集成。 一般情况下，有两种方法：联合与自定义控制：

* **标识联合** - 当 Azure AD 收到身份验证请求时，Azure AD 会将用户重定向到联合的标识提供者进行身份验证。 身份验证成功后，联合的标识提供者会将用户重定向回到 Azure AD，并提供一个 SAML 令牌。 为使 Azure AD 能够识别到该用户在对联合的标识提供者进行身份验证时已完成 MFA 验证，该 SAML 令牌必须包含 *authenticationmethodsreferences*  声明（值为 *multipleauthn*）。 检查联合的标识提供者是否支持发出此类声明。 如果是，请检查联合的标识提供者是否已配置为提供此项支持。 如果缺少声明，Azure AD（因而也还有合作伙伴中心）将不知道用户已完成 MFA 验证，并且缺少声明可能会导致该指标无法达到 100%。

* **自定义控制** - Azure AD 自定义控制不能用来确定用户是否已通过第三方 MFA 解决方案完成了 MFA 验证。 因此，对于 Azure AD（因而也包括合作伙伴中心）而言，通过自定义控制完成 MFA 验证的任何用户始终看上去并未完成 MFA 验证。 如果可能，我们建议在与 Azure AD 集成时改用标识联合，而不要使用自定义控制。

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>确定哪些用户在未完成 MFA 的情况下登录到了合作伙伴中心

确定哪些用户在未完成 MFA 验证的情况下登录到了合作伙伴中心，并根据当前的 MFA 实施方案对其进行验证，可能会有帮助。 可以使用 [Azure AD 登录报告](/azure/active-directory/reports-monitoring/concept-sign-ins)来确定用户是否已完成 MFA 验证。 Azure AD 登录报告目前仅适用于订阅了 Azure AD Premium 或任何包含 Azure AD Premium 的 O365 SKU（例如 EMS）的合作伙伴。

## <a name="next-steps"></a>后续步骤

- [合作伙伴中心安全指导组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [合作伙伴中心安全要求](partner-security-requirements.md)
- [合作伙伴中心安全要求常见问题解答](partner-security-requirements-faq.md)
