---
title: 为合作伙伴租户强制执行多重身份验证 (MFA)
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解对合作伙伴租户强制执行 MFA 将如何有助于保护对客户资源的访问。 包括示例方案。
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b6985054e927dd777d61ae30bd435ab4c6c4ea8c
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133095"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>为合作伙伴租户强制执行多重身份验证 (MFA)

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
- 所有控制面板供应商
- 所有顾问

**受影响的角色**

- 管理员代理
- 销售代理
- 支持人员代理
- 帐务管理员
- 全局管理员

本文提供了在合作伙伴中心强制执行多重身份验证 (MFA) 的详细示例和指导。 此功能的目的是帮助合作伙伴保护他们对客户资源的访问，防止凭据遭到泄露。 合作伙伴必须为其合作伙伴租户中的所有用户帐户（包括来宾用户）强制实施 MFA。 将针对以下方面强制这些用户完成 MFA 验证：

- [合作伙伴中心仪表板](#partner-center-dashboard)
- [合作伙伴中心 API](#partner-center-api)
- [合作伙伴委派的管理](#partner-delegated-administration)

提供更大力度的持续性安全和隐私保护是我们的首要任务，并且我们会继续帮助合作伙伴保护他们的客户和租户。 参与云解决方案提供商 (CSP) 计划的所有合作伙伴、控制面板供应商 (CPV) 和顾问都应实施[合作伙伴安全要求](partner-security-requirements.md)以保持合规性。

为帮助合作伙伴保护其业务和客户免受身份盗用和未经授权的访问，我们为合作伙伴租户激活了额外的安全保护措施，以强制执行并验证 MFA。 

## <a name="partner-center-dashboard"></a>合作伙伴中心面板

合作伙伴中心面板中的某些页面将受到 MFA 的保护，包括：

- “客户”选项卡下的所有页面，例如可以通过以下 URL 访问的所有页面： https://partner.microsoft.com/commerce/*
- “支持”>“客户请求”选项卡下的所有页面，例如通过 https://partner.microsoft.com/dashboard/support/csp/customers/* 访问的页面
- 计费页面

下表显示了哪些用户类型有权访问这些受 MFA 保护的页面（因此会受到此功能的影响）。


| 受 MFA 保护的页面       | 管理员代理      |  销售代理     |   支持人员代理     | 全局管理员      |  帐务管理员     | 
|---    |---    |---    |---    |---    |---    |
| “客户”选项卡下的所有页面      |   x    |    x   |  x     |       |       |
| “支持”>“客户请求”选项卡下的所有页面     | x      |       |    x   |       |       |
| 计费页面     |   x    |       |       |    x   |   x    |

如果你要尝试访问任一这些页面并且之前尚未完成 MFA 验证，则需要执行此操作。 合作伙伴中心的其他页面（例如“概览”页面、“服务运行状况状态”检查页面）不需要 MFA。

## <a name="verification-examples"></a>验证示例

为了说明验证在合作伙伴中心面板的工作原理，我们列举了以下示例。

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>示例 1：合作伙伴已实现 Azure AD MFA

1. Jane 在 CSP Contoso 工作。 Contoso 已使用 Azure Active Directory (Azure AD) MFA 为其 Contoso 合作伙伴租户下的所有用户实现了 MFA。

2. Jane 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 Jane 重定向到 Azure AD 以进行登录。

3. 由于 Contoso 设置的现有 Azure AD MFA，Jane 需要完成 MFA 验证。 成功完成登录和 MFA 验证后，Jane 会被重定向回合作伙伴中心面板概览页面。

4. Jane 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 Jane 在之前登录期间已经完成了 MFA 验证，因此，Jane 可以访问受 MFA 保护的页面，无需再次进行 MFA 验证。

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>示例 2：合作伙伴已使用联合身份验证实现了第三方 MFA

1. Trent 在云解决方案提供商 Wingtip 工作。 Wingtip 已使用第三方 MFA（通过联合身份验证与 Azure AD 相集成）为他们 Wingtip 合作伙伴租户下的所有用户实现了 MFA。

2. Trent 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 Trent 重定向到 Azure AD 以进行登录。

3. 由于 Wingtip 设置了联合身份验证，因此 Azure AD 会将 Trent 重定向到联合身份验证标识提供程序以完成登录和 MFA 验证。 成功完成登录和 MFA 验证后，Trent 会被重定向回 Azure AD，然后再回到合作伙伴中心面板概览页面。

4. Trent 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 Trent 在之前登录期间已经完成了 MFA 验证，因此，Trent 可以访问受 MFA 保护的页面，无需再次进行 MFA 验证。

### <a name="example-3-partner-hasnt-implemented-mfa"></a>示例 3：合作伙伴未实现 MFA

1. John 在云解决方案提供商 Fabrikam 工作。 Fabrikam 没有为 Fabrikam 合作伙伴租户下的任何用户实现 MFA。

2. John 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 John 重定向到 Azure AD 以进行登录。

3. 由于 Fabrikam 尚未实现 MFA，因此 John 不需要完成 MFA 验证。 成功完成登录后，John 会被重定向回合作伙伴中心面板概览页面。

4. John 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 John 未完成 MFA 验证，因此，合作伙伴中心将 John 重定向到 Azure AD 以完成 MFA 验证。 由于这是 John 第一次需要完成 MFA，John 还被要求[注册 MFA](#mfa-registration-experience)。 在成功完成 MFA 注册和 MFA 验证后，John 现在可以访问受 MFA 保护的页面。

5. 在 Fabrikam 为任何用户实现 MFA 之前的某一天，John 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 John 重定向到了 Azure AD 以进行登录，没有提示他要完成 MFA。 

6. John 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 John 未完成 MFA 验证，因此，合作伙伴中心将 John 重定向到 Azure AD 以完成 MFA 验证。 由于 John 已注册了 MFA，因此这次只要求他完成 MFA 验证即可。

> [!NOTE]
>操作：公司管理员有[三个选项](partner-security-requirements.md#implementing-multi-factor-authentication)来实现 MFA。

## <a name="partner-center-api"></a>合作伙伴中心 API

合作伙伴中心 API 同时支持“仅应用”身份验证和“应用+用户”身份验证。 

使用应用+用户身份验证时，合作伙伴中心将要求进行 MFA 验证。 更具体地说，当合作伙伴应用程序想将 API 请求发送到合作伙伴中心时，它必须在请求的授权标头中包含一个访问令牌。 

> [!NOTE]
>[安全应用程序模型框架](/partner-center/develop/enable-secure-app-model)是一种可缩放的框架，用于在你调用合作伙伴中心 API 时通过 Microsoft Azure MFA 体系结构对 CSP 合作伙伴和 CPV 进行身份验证。 在对租户启用 MFA 之前，需要实现此框架。 

当合作伙伴中心收到带有使用“应用+用户”身份验证获得的访问令牌的 API 请求时，合作伙伴中心 API 将检查身份验证方法引用 (AMR) 声明中是否存在“MFA”值 。 你可以使用 JWT 解码器来验证访问令牌是否包含所需的身份验证方法引用 (AMR) 值：

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

如果值存在，合作伙伴中心则会得出已完成 MFA 验证的结论并处理 API 请求。 如果值不存在，合作伙伴中心 API 将拒绝请求，并返回以下响应：

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

当使用“仅应用”身份验证时，支持“仅应用”身份验证的 API 将继续运行，而无需 MFA。

## <a name="partner-delegated-administration"></a>合作伙伴委派的管理

合作伙伴帐户（包括管理员代理和支持人员代理）可以使用他们的合作伙伴委派管理员权限来通过 Microsoft Online Services 门户、命令行接口 (CLI) 和 API（使用的是“应用+用户”身份验证）管理客户资源。

### <a name="using-service-portals"></a>使用服务门户

当使用“合作伙伴委派管理员权限(代表管理员)”来访问 Microsoft Online Services 门户时，这些门户中的许多门户都需要合作伙伴帐户以交互方式与设置为身份验证上下文的客户 Azure AD 租户进行身份验证 - 合作伙伴帐户需要登录客户租户。

当 Azure AD 收到此类身份验证请求时，它将要求合作伙伴帐户完成 MFA 验证。 可以使用两种用户体验，具体取决于合作伙伴帐户是托管标识还是联合身份标识：

- 如果合作伙伴帐户是托管标识，Azure AD 将直接提示用户完成 MFA 验证。 如果合作伙伴帐户之前尚未通过 Azure AD 注册 MFA，系统将要求用户首先[完成 MFA 注册](#mfa-registration-experience)。

- 如果合作伙伴帐户是联合身份标识，体验将取决于合作伙伴管理员在 Azure AD 中配置联合验证的方式。 在 Azure AD 中设置联合验证时，合作伙伴管理员可以向 Azure AD 指示联合身份验证标识提供程序是否支持 MFA。 如果支持，Azure AD 会将用户重定向到联合身份验证标识提供程序以完成 MFA 验证。 否则，Azure AD 将直接提示用户完成 MFA 验证。 如果合作伙伴帐户之前尚未通过 Azure AD 注册 MFA，系统将要求用户首先[完成 MFA 注册](#mfa-registration-experience)。

整体体验与最终客户租户为它的管理员实现了 MFA 的方案类似。 例如，客户租户启用了 [Azure AD 安全默认设置](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，这要求具有管理权限的所有帐户通过 MFA 验证登录到客户租户，包括管理员代理和支持人员代理。 出于测试目的，合作伙伴可以在客户租户中启用 [Azure AD 安全默认设置](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，然后尝试使用合作伙伴委派的管理权限来访问客户租户。

> [!NOTE]
> 并非所有 Microsoft Online Service 门户都需要合作伙伴帐户在使用合作伙伴委派的管理员权限访问客户资源时登录到客户租户。 相反，它们只要求合作伙伴帐户登录到合作伙伴租户。 Exchange 管理中心就是一个例子。 随着时间的推移，我们希望这些门户要求合作伙伴帐户在使用合作伙伴委派的管理员权限时登录到客户租户。

### <a name="using-service-apis"></a>使用服务 API

某些 Microsoft Online Services API（例如 Azure 资源管理器、Azure AD Graph 和 Microsoft Graph等）支持合作伙伴使用合作伙伴委派的管理员权限以编程方式管理客户资源。 若要通过这些 API 来利用合作伙伴委派的管理员权限，合作伙伴应用程序必须在 API 请求授权标头中包含访问令牌，此访问令牌是让合作伙伴用户帐户通过 Azure AD 与设置为身份验证上下文的客户 Azure AD 进行身份验证所获取的。 合作伙伴应用程序要求合作伙伴用户帐户登录客户租户。

当 Azure AD 收到此类身份验证请求时，Azure AD 将要求合作伙伴用户帐户完成 MFA 验证。 如果合作伙伴用户帐户之前尚未注册 MFA，系统将提示此用户帐户首先完成 MFA 注册。

使用合作伙伴委派的管理员权限与这些 API 集成的所有合作伙伴应用程序会受到此功能的影响。 确保合作伙伴应用程序可以继续使用这些 API，不会发生中断：

- 合作伙伴必须避免将非交互式用户身份验证方法与 Azure AD 配合使用才能获取访问令牌。 使用非交互式用户身份验证方法时（例如[密码流](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)），Azure AD 将无法提示用户完成 MFA 验证。 合作伙伴必须改用交互式用户身份验证方法，例如 [OpenID Connect 流](/azure/active-directory/develop/v1-protocols-openid-connect-code)。

- 在使用交互式用户身份验证方法期间，合作伙伴应使用已启用了 MFA 的合作伙伴用户帐户。 或者，在 Azure AD 提示时，合作伙伴可以在登录期间完成 MFA 注册和 MFA 验证。

- 这与最终客户租户为它的管理员实现了 MFA 的情况类似。 例如，客户租户启用了 [Azure AD 安全默认设置](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，这要求具有管理权限的所有用户帐户通过 MFA 验证登录到客户租户，包括管理员代理和支持人员代理。 出于测试目的，合作伙伴可以在客户租户中启用 [Azure AD 安全默认设置](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，然后尝试使用合作伙伴委派的管理权限以编程方式访问客户租户。

### <a name="mfa-registration-experience"></a>MFA 注册体验

在 MFA 验证期间，如果合作伙伴帐户之前尚未注册 MFA，Azure AD 将提示此用户首先完成 MFA 注册：

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA 注册步骤 1":::

单击“下一步”后，系统将要求用户从验证方法列表中进行选择。

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA 注册步骤 2":::

成功注册后，用户需要根据所选择的验证完成 MFA 验证。
 
## <a name="list-of-common-issues"></a>常见问题列表

在申请 MFA 要求的[技术例外](#how-to-submit-a-request-for-technical-exception)之前，请查看由其他合作伙伴报告的常见问题列表以了解你的请求是否有效。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>问题 1：合作伙伴需要更多的时间来为他们的合作伙伴代理实现 MFA
合作伙伴尚未为他们的合作伙伴代理实现 MFA 或者正在实现过程中，这些代理需要使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户以管理客户资源。 合作伙伴需要更多的时间来完成 MFA 实现。 此问题能否成为请求技术例外的有效理由？

**答案** ：不能。 合作伙伴需要制定计划来为他们的用户实现 MFA，从而避免中断。

> [!NOTE]
> 即使合作伙伴尚未为他们的合作伙伴代理实现 MFA，合作伙伴代理仍然可以使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户，只要在登录到客户租户期间出现提示时他们可以完成 MFA 注册和 MFA 验证。 完成 MFA 注册不会自动为用户启用 MFA。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>问题 2：合作伙伴尚未为未使用委派管理员权限的用户帐户实现 MFA
某一合作伙伴在他们的合作伙伴租户中拥有用户，这些用户不需要使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户以管理客户资源。 合作伙伴正在为这些用户实现 MFA，需要更多的时间才能完成。 此问题能否成为请求技术例外的有效理由？

**答案** ：不能。 由于这些用户帐户不使用合作伙伴委派的管理权限来管理客户资源，因此他们将不需要登录到客户租户。 他们不受 Azure AD 要求在登录到客户租户期间进行 MFA 验证的影响。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>问题 3：合作伙伴尚未为用户服务帐户实现 MFA
某一合作伙伴在他们的合作伙伴租户中拥有一些用户帐户，这些帐户由设备作为服务帐户使用。 这些是低特权帐户，这些帐户不需要使用合作伙伴委派的管理权限来访问合作伙伴中心或 Microsoft Online Services 门户以管理客户资源。 此问题能否成为请求技术例外的有效理由？

**答案** ：不能。 由于这些用户帐户不使用合作伙伴委派的管理权限来管理客户资源，因此他们将不需要登录到客户租户。 他们不受 Azure AD 要求在登录到客户租户期间进行 MFA 验证的影响。

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>问题 4：合作伙伴无法使用 MS Authenticator 应用来实现 MFA
合作伙伴具有“清理办公桌”政策，不允许员工将个人移动设备带到工作区。 在无法使用个人移动设备的情况下，员工无法安装 MS Authenticator 应用，这是 Azure AD 安全默认设置支持的唯一 MFA 验证。 此问题能否成为请求技术例外的有效理由？

**答案** ：不能，这不是请求技术例外的有效理由。 合作伙伴应考虑以下替代方法，使他们的员工仍然可以在访问合作伙伴中心时完成 MFA 验证：
- 合作伙伴还可以注册 Azure AD Premium 或第三方 MFA 解决方案（与 Azure AD 兼容），此类解决方案可以提供其他验证方法。

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>问题 5：由于使用的是旧式身份验证协议，合作伙伴无法实现 MFA
某一合作伙伴的某些合作伙伴代理仍然在使用旧式身份验证协议，这与 MFA 不兼容。 例如，用户仍然在使用 Outlook 2010，此程序基于的是旧式身份验证协议。 为这些合作伙伴代理启用 MFA 将中断旧式身份验证协议的使用。

**答案** ：不能，这不是请求技术例外的有效理由。 由于潜在的安全隐患问题，强烈建议合作伙伴避免使用旧式身份协议，因为不能通过 MFA 验证来保护这些协议并且这些协议更容易出现凭据泄露的问题。 如果无法避免使用旧式身份验证协议，合作伙伴应考虑注册支持使用应用程序密码的 Azure AD Premium。 应用程序密码是系统生成的一次性密码，通常比人为生成的密码更强。 通过使用应用程序密码，合作伙伴可以为他们的用户实现 MFA，同时回退到仅适用于旧式身份验证协议的应用程序密码。

阅读[基本身份验证和 Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) 的相关文章以了解关于支持 Outlook 的旧式身份验证的最新计划，同时关注 [Exchange 团队博客](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange)以获取最新的资讯。 

> [!NOTE]
> 即使合作伙伴尚未为他们的合作伙伴代理实现 MFA，合作伙伴代理仍然可以使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户，只要在登录到客户租户期间出现提示时他们可以完成 MFA 注册和 MFA 验证。 完成 MFA 注册不会自动为用户启用 MFA。

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>问题 6：合作伙伴实现了 Azure AD 无法识别的第三方 MFA
合作伙伴使用第三方 MFA 解决方案为他们的用户实现了 MFA。 但是，合作伙伴无法正确配置第三方 MFA 解决方案来中继至在用户身份验证期间已完成 MFA 验证的 Azure AD。 这能否成为请求技术例外的有效理由？

**答案** ：能，此问题可能会被认为是请求技术例外的有效理由。 提交请求技术例外时，请与第三方 MFA 解决方案提供商确认无法配置此 MFA 解决方案来将 authenticationmethodsreferences 声明（带有值 multipleauthn）传递给 Azure AD，以此来指示在用户身份验证期间已完成 MFA 验证 。 提交请求技术例外时，必须提供所用的第三方 MFA 解决方案的详细信息，指出集成方法（例如通过联合身份验证或使用 Azure AD 自定义控制），并在技术例外请求中提供以下信息作为支持文档：

- 第三方 MFA 配置。

- 由启用了第三方 MFA 的帐户运行的[测试合作伙伴安全要求](/powershell/partnercenter/test-partner-security-requirements)的结果。

- 你正在使用或计划使用的第三方 MFA 解决方案的采购订单。

## <a name="how-to-submit-a-request-for-technical-exception"></a>如何提交请求技术例外

如果合作伙伴遇到与 Microsoft Online Services 相关的技术问题并且没有可行的解决方案或暂时解决方法，他们可以申请技术例外以取消 MFA 验证。 在此之前，请查看上一节中的[常见问题列表](#list-of-common-issues)。

提交请求技术例外：

1. 以全局管理员或管理员代理的身份登录到合作伙伴中心。

2. 通过导航到“支持” > “合作伙伴支持请求”并单击“新请求”来创建新的合作伙伴服务请求。  

3. 在搜索框中搜索“MFA - 请求例外”；或从“类别”中选择“CSP”，然后从“主题”中选择“帐户、加入、访问”，接着从子主题中选择“MFA - 请求例外”，再选择“下一步”    。

4. 提供提交技术例外服务请求所需的详细信息，然后单击“提交”。

Microsoft 可能在最长三个工作日的时间内响应技术例外请求。

## <a name="next-steps"></a>后续步骤

 - [合作伙伴安全要求状态](partner-security-compliance.md)