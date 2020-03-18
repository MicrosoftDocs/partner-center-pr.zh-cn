---
title: 对合作伙伴租户强制执行 MFA | 合作伙伴中心
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解对合作伙伴租户强制执行 MFA 将如何有助于保护对客户资源的访问。 包括示例方案。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: high
ms.openlocfilehash: bf57b489f84540e50e28df5568391818f50c79d4
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340185"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>为合作伙伴租户强制执行多重身份验证 (MFA)

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
  - 直接计费
  - 间接提供商
  - 间接经销商
- 所有顾问

**相应的用户**
-    所有支持的用户，包括来宾用户

这些合作伙伴将需要针对以下部分完成 MFA 验证：

- [合作伙伴中心面板](#partner-center-dashboard)（目标定为 2020 年日历年第 2 季度）
- [合作伙伴中心 API](#partner-center-api)（目标定为 2020 年日历年第 2 季度）
- [合作伙伴委派的管理](#partner-delegated-administration)（从 2019 年 11 月 18 日起）

此功能的目的是帮助合作伙伴保护他们对客户资源的访问，防止凭据遭到泄露。

## <a name="partner-center-dashboard"></a>合作伙伴中心面板
合作伙伴中心面板中的某些页面将受到 MFA 的保护，包括：

* “客户”选项卡下的所有页面。 
* “支持”>“客户请求”选项卡下的所有页面。 

如果你要尝试访问任一这些页面并且之前尚未完成 MFA 验证，则需要执行此操作。

以下用户类型有权访问这些受 MFA 保护的页面，并且会受到此功能的影响，包括：

* 管理员代理
* 销售代理
* 支持人员代理

为了说明验证的工作原理，请考虑以下两个示例。

**示例 1：合作伙伴已实现 Azure AD MFA**
1.    Jane 在 CSP Contoso 工作。 Contoso 已使用 Azure AD MFA 为他们 Contoso 合作伙伴租户下的所有用户实现了 MFA。
2.    Jane 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 Jane 重定向到 Azure AD 以进行登录。
3.    由于 Contoso 设置的现有 Azure AD MFA，Jane 需要完成 MFA 验证。 成功完成登录和 MFA 验证后，Jane 会被重定向回合作伙伴中心面板概览页面。
4.    Jane 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 Jane 在之前登录期间已经完成了 MFA 验证，因此，Jane 可以访问受 MFA 保护的页面，无需再次进行 MFA 验证。

**示例 2：合作伙伴已使用联合身份验证实现了第三方 MFA**
1. Trent 在云解决方案提供商 Wingtip 工作。 Wingtip 已使用第三方 MFA（通过联合身份验证与 Azure AD 相集成）为他们 Wingtip 合作伙伴租户下的所有用户实现了 MFA。
2. Trent 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 Trent 重定向到 Azure AD 以进行登录。
3. 由于 Wingtip 设置了联合身份验证，因此 Azure AD 会将 Trent 重定向到联合身份验证标识提供程序以完成登录和 MFA 验证。 成功完成登录和 MFA 验证后，Trent 会被重定向回 Azure AD，然后再回到合作伙伴中心面板概览页面。
4. Trent 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 Trent 在之前登录期间已经完成了 MFA 验证，因此，Trent 可以访问受 MFA 保护的页面，无需再次进行 MFA 验证。

**示例 3：合作伙伴未实现 MFA**
1. John 在云解决方案提供商 Fabrikam 工作。 Fabrikam 没有为 Fabrikam 合作伙伴租户下的任何用户实现 MFA。
2. John 启动了一个新的浏览器会话并导航到合作伙伴中心面板概览页面（此页面不受 MFA 保护）。 合作伙伴中心将 John 重定向到 Azure AD 以进行登录。
3. 由于 Fabrikam 尚未实现 MFA，因此 John 不需要完成 MFA 验证。 成功完成登录后，John 会被重定向回合作伙伴中心面板概览页面。
4. John 尝试访问合作伙伴中心中任一受 MFA 保护的页面。 由于 John 未完成 MFA 验证，因此，合作伙伴中心将 John 重定向到 Azure AD 以完成 MFA 验证。 由于这是 John 第一次需要完成 MFA，John 还被要求使用 Microsoft Authenticator 应用注册 MFA。 在成功完成 MFA 注册和 MFA 验证后，John 现在可以访问受 MFA 保护的页面。

## <a name="partner-center-api"></a>合作伙伴中心 API

合作伙伴中心 API 同时支持“仅应用”身份验证和应用+用户身份验证。 使用应用+用户身份验证时，合作伙伴中心将要求进行 MFA 验证。 更具体地说，当合作伙伴应用程序想将 API 请求发送到合作伙伴中心时，它必须在请求的授权标头中包含一个访问令牌。 当合作伙伴中心收到带有使用应用+用户身份验证获得的访问令牌的 API 请求时，合作伙伴中心将检查身份验证方法引用 (AMR) 声明中是否存在“MFA”值。   你可以使用 JWT 解码器来验证访问令牌是否包含所需的身份验证方法引用 (AMR) 值：

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
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
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

## <a name="partner-delegated-administration"></a>合作伙伴委派的管理

### <a name="using-service-portals"></a>使用服务门户

合作伙伴帐户（包括管理员代理和支持人员代理）可以使用他们的委派管理员权限来通过 Microsoft Online Services 门户、命令行接口 (CLI) 和 API（使用的是应用+用户身份验证）管理客户资源。

当使用“合作伙伴委派管理员权限”来访问 Microsoft Online Services 门户时，这些门户中的众多门户都需要合作伙伴帐户以相互方式与设置为身份验证上下文的客户 Azure Active Directory 租户进行身份验证 - 合作伙伴帐户需要登录客户租户。

当 Azure Active Directory 收到此类身份验证请求时，它将要求合作伙伴帐户完成 MFA 验证。 可以使用两种用户体验，具体取决于合作伙伴帐户是托管标识还是联合身份标识：

- 如果合作伙伴帐户是托管标识，Azure Active Directory 将直接提示用户完成 MFA 验证。  如果合作伙伴帐户之前尚未通过 Azure Active Directory 注册 MFA，系统则将要求用户首先[完成 MFA 注册](#mfa-registration-experience)。

- 如果合作伙伴帐户是联合身份标识，体验则取决于合作伙伴管理员在 Azure Active Directory 中配置联合验证的方式。  在 Azure Active Directory 中设置联合验证时，合作伙伴管理员可以向 Azure Active Directory 指示联合身份验证标识提供程序是否支持 MFA。 如果支持，Azure Active Directory 会将用户重定向到联合身份验证标识提供程序以完成 MFA 验证。 否则，Azure Active Directory 将直接提示用户完成 MFA 验证。 如果合作伙伴帐户之前尚未通过 Azure Active Directory 注册 MFA，系统则将要求用户首先[完成 MFA 注册](#mfa-registration-experience)。

整体体验与最终客户租户为它的管理员实现了 MFA 的方案类似。 例如，客户租户启用了 [Azure AD 安全默认设置](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，这要求具有管理权限的所有帐户通过 MFA 验证登录到客户租户，包括管理员代理和支持人员代理。 出于测试目的，合作伙伴可以在客户租户中启用 [Azure AD 安全默认设置](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，然后尝试使用合作伙伴委派的管理权限来访问客户租户。

> [!NOTE]
> 并非所有 Microsoft Online Service 门户都需要合作伙伴帐户在使用合作伙伴委派的管理员权限访问客户资源时登录到客户租户。 相反，它们只要求合作伙伴帐户登录到合作伙伴租户。 Exchange 管理中心就是一个例子。 随着时间的推移，我们希望这些门户要求合作伙伴帐户在使用合作伙伴委派的管理员权限时登录到客户租户。

### <a name="using-service-apis"></a>使用服务 API
某些 Microsoft Online Services API（例如 Azure 资源管理器、Azure AD Graph 和 Microsoft Graph等）支持合作伙伴使用合作伙伴委派的管理员权限以编程方式管理客户资源。 若要通过这些 API 来利用合作伙伴委派的管理员权限，合作伙伴应用程序必须在 API 请求授权标头中包含访问令牌，此访问令牌是让合作伙伴用户帐户通过 Azure AD 与设置为身份验证上下文的客户 Azure AD 进行身份验证所获取的。 合作伙伴应用程序要求合作伙伴用户帐户登录客户租户。

当 Azure AD 收到此类身份验证请求时，Azure AD 将要求合作伙伴用户帐户完成 MFA 验证。 如果合作伙伴用户帐户之前尚未注册 MFA，系统将提示此用户帐户首先完成 MFA 注册。

使用合作伙伴委派的管理员权限与这些 API 集成的所有合作伙伴应用程序会受到此功能的影响。 确保合作伙伴应用程序可以继续使用这些 API，不会发生中断：

- 合作伙伴必须避免将非交互式用户身份验证方法与 Azure AD 配合使用才能获取访问令牌。 使用非交互式用户身份验证方法时（例如[密码流](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)），Azure AD 将无法提示用户完成 MFA 验证。 合作伙伴必须改用交互式用户身份验证方法，例如 [OpenID Connect 流](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code)。
- 在使用交互式用户身份验证方法期间，合作伙伴应使用已启用了 MFA 的合作伙伴用户帐户。 或者，在 Azure AD 提示时，合作伙伴可以在登录期间完成 MFA 注册和 MFA 验证。
- 这与最终客户租户为它的管理员实现了 MFA 的情况类似。 例如，客户租户启用了 [Azure AD 安全默认设置](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，这要求具有管理权限的所有用户帐户通过 MFA 验证登录到客户租户，包括管理员代理和支持人员代理。 出于测试目的，合作伙伴可以在客户租户中启用 [Azure AD 安全默认设置](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，然后尝试使用合作伙伴委派的管理权限以编程方式访问客户租户。

### <a name="mfa-registration-experience"></a>MFA 注册体验
在 MFA 验证期间，如果合作伙伴帐户之前尚未注册 MFA，Azure AD 将提示此用户首先完成 MFA 注册：

![MFA 注册步骤 1](images/MfaRegistration1.png)

单击“下一步”后，系统将要求用户从验证方法列表中进行选择（包括电话、短信和 Authenticator 应用）。 

![MFA 注册步骤 2](images/MfaRegistration2.png)

成功注册后，用户需要根据所选择的验证完成 MFA 验证。



## <a name="request-for-technical-exception"></a>请求技术例外

如果合作伙伴遇到与 Microsoft Online Services 相关的技术问题并且没有可行的解决方案或暂时解决方法，他们可以申请技术例外以取消 MFA 验证。 在执行此操作之前，请查看以下部分：

 - [合作伙伴报告的常见问题列表](#list-of-common-issues-reported-by-partners)
 - [如何提交请求技术例外](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>合作伙伴报告的常见问题列表
在申请技术例外之前，请查看由其他合作伙伴报告的常见问题列表以了解这些问题是否是请求技术例外的有效理由。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>问题 1：合作伙伴需要更多的时间来为他们的合作伙伴代理实现 MFA
合作伙伴尚未为他们的合作伙伴代理实现 MFA 或者正在实现过程中，这些代理需要使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户以管理客户资源。 合作伙伴需要更多的时间来完成 MFA 实现。 此问题能否成为请求技术例外的有效理由？

**答案**：不能。 合作伙伴需要制定计划来为他们的用户实现 MFA，从而避免中断。

> [!NOTE]
> 即使合作伙伴尚未为他们的合作伙伴代理实现 MFA，合作伙伴代理仍然可以使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户，只要在登录到客户租户期间出现提示时他们可以完成 MFA 注册和 MFA 验证。 完成 MFA 注册不会自动为用户启用 MFA。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>问题 2：合作伙伴尚未为未使用委派管理员权限的用户帐户实现 MFA
某一合作伙伴在他们的合作伙伴租户中拥有用户，这些用户不需要使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户以管理客户资源。 合作伙伴正在为这些用户实现 MFA，需要更多的时间才能完成。 此问题能否成为请求技术例外的有效理由？

**答案**：不能。 由于这些用户帐户不使用合作伙伴委派的管理权限来管理客户资源，他们将不需要登录到客户租户。 他们不受 Azure AD 要求在登录到客户租户期间进行 MFA 验证的影响。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>问题 3：合作伙伴尚未为用户服务帐户实现 MFA
某一合作伙伴在他们的合作伙伴租户中拥有一些用户帐户，这些帐户由设备作为服务帐户使用。 这些是低特权帐户，这些帐户不需要使用合作伙伴委派的管理权限来访问合作伙伴中心或 Microsoft Online Services 门户以管理客户资源。 此问题能否成为请求技术例外的有效理由？

**答案**：不能。 由于这些用户帐户不使用合作伙伴委派的管理权限来管理客户资源，他们将不需要登录到客户租户。 他们不受 Azure AD 要求在登录到客户租户期间进行 MFA 验证的影响。

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>问题 4：合作伙伴无法使用 MS Authenticator 应用来实现 MFA
合作伙伴具有“清理办公桌”政策，不允许员工将个人移动设备带到工作区。 在无法使用个人移动设备的情况下，员工无法安装 MS Authenticator 应用，这是 Azure AD 基线策略支持的唯一 MFA 验证。 此问题能否成为请求技术例外的有效理由？

**答案**：不能，这不是请求技术例外的有效理由。 合作伙伴应考虑以下替代方法，使他们的员工仍然可以在访问合作伙伴中心时完成 MFA 验证：
- 除了 MS Authenticator 应用外，Azure AD 基线策略还可用于第三方兼容的身份验证器应用，此类应用可能受到运行 Microsoft Windows 的 Windows 计算机的支持。
- 合作伙伴还可以注册 Azure AD Premium 或第三方 MFA 解决方案（与 Azure AD 兼容），此类解决方案可以提供其他验证方法。

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>问题 5：由于使用的是旧式身份验证协议，合作伙伴无法实现 MFA
某一合作伙伴的某些合作伙伴代理仍然在使用旧式身份验证协议，这与 MFA 不兼容。 例如，用户仍然在使用 Outlook 2010，此程序基于的是旧式身份验证协议。 为这些合作伙伴代理启用 MFA 将中断旧式身份验证协议的使用。

**答案**：不能，这不是请求技术例外的有效理由。 由于潜在的安全隐患问题，强烈建议合作伙伴避免使用旧式身份协议，因为不能通过 MFA 验证来保护这些协议并且这些协议更容易出现凭据泄露的问题。 如果无法避免使用旧式身份验证协议，合作伙伴应考虑注册支持使用应用程序密码的 Azure AD Premium。 应用程序密码是系统生成的一次性密码，通常比人为生成的密码更强。 通过使用应用程序密码，合作伙伴可以为他们的用户实现 MFA，同时回退到仅适用于旧式身份验证协议的应用程序密码。

> [!NOTE]
> 即使合作伙伴尚未为他们的合作伙伴代理实现 MFA，合作伙伴代理仍然可以使用合作伙伴委派的管理权限来访问 Microsoft Online Services 门户，只要在登录到客户租户期间出现提示时他们可以完成 MFA 注册和 MFA 验证。 完成 MFA 注册不会自动为用户启用 MFA。

#### <a name="issue-6-partner-is-using-exchange-online-powershell-that-does-not-support-mfa"></a>问题 6：合作伙伴正在使用不支持 MFA 的 Exchange Online PowerShell
合作伙伴正在使用带有合作伙伴委派的管理权限的 Exchange Online PowerShell 来代表他们的客户管理 Exchange Online 服务。 hange Online PowerShell 不支持 MFA。 如果合作伙伴为他们的用户实现 MFA，那么这些用户将无法再访问 Exchange Online PowerShell。 此问题能否成为请求技术例外的有效理由？

**答案**：能，此问题可能会被认为是请求技术例外的有效理由。 现有[支持合作伙伴委派的权限的 Exchange Online PowerShell 模块](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)不需要合作伙伴用户登录到客户租户，因此此类用户不受需要 MFA 验证的 Azure AD 影响。 但是，它不与 MFA 兼容。 Microsoft Exchange Online 团队正在开发一个同时支持合作伙伴委派的管理权限和 MFA 的新 PowerShell 模块。 在新的 PowerShell 模块可用之前，合作伙伴无法为需要使用现有 PowerShell 模块的用户实现 MFA。 如果这些用户在访问其他 Microsoft Online Services 时因在跨租户登录期间 Azure AD 要求进行 MFA 验证而遇到了问题，合作伙伴可以请求技术例外来取消 MFA 验证。

> [!NOTE]
> 即使合作伙伴无法为需要访问 Exchange Online PowerShell 模块的用户实现 MFA，这些用户仍然可以使用合作伙伴委派的管理权限来访问 Microsoft Online Services 以管理客户资源，只要在登录到客户租户期间出现提示时他们可以完成 MFA 注册和 MFA 验证即可。 完成 MFA 注册不会自动为用户启用 MFA，因此，不会影响对 Exchange Online PowerShell 模块的访问。

#### <a name="issue-7-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>问题 7：合作伙伴实现了 Azure AD 无法识别的第三方 MFA
合作伙伴使用第三方 MFA 解决方案为他们的用户实现了 MFA。 但是，合作伙伴无法正确配置第三方 MFA 解决方案来中继至在用户身份验证期间已完成 MFA 验证的 Azure AD。 这能否成为请求技术例外的有效理由？

**答案**：能，此问题可能会被认为是请求技术例外的有效理由。 提交请求技术例外时，请与第三方 MFA 解决方案提供商确认无法配置此 MFA 解决方案来将 authenticationmethodsreferences 声明（带有值 multipleauthn）传递给 Azure AD，以此来指示在用户身份验证期间已完成 MFA 验证。   提交请求技术例外时，必须提供所用的第三方 MFA 解决方案的详细信息，并指出集成方法（例如通过联合身份验证或使用 Azure AD 自定义控制）。

### <a name="how-to-submit-a-request-for-technical-exception"></a>如何提交请求技术例外

提交请求技术例外：

1. 以全局管理员或管理员代理的身份登录到合作伙伴中心。
2. 通过导航到“支持” > “合作伙伴支持请求”并单击“新请求”来创建新的合作伙伴服务请求。   
4. 在“MFA 和安全应用程序模型”主题下，选择“提交技术例外请求”来作为问题类型。  
6. 提供提交技术例外服务请求所需的详细信息，然后单击“提交”。 

Microsoft 可能需要花费长达三个工作日的时间来响应技术例外请求。
