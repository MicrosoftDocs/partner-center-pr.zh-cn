---
title: 合作伙伴租户的强制 MFA |合作伙伴中心
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解合作伙伴租户的强制 MFA 如何帮助保护对客户资源的访问。 包括示例方案。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: 46d485f8d3edf916fce478812c6d8243909e4ed4
ms.sourcegitcommit: a620880aad1f5f8a4274a0ec3f257056363082e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2020
ms.locfileid: "76723484"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>合作伙伴租户的强制执行多重身份验证（MFA）

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
  - 直接计费
  - 间接提供商
  - 间接经销商
- 所有顾问

**适当的用户**
-   所有已启用的用户（包括来宾用户）

这些合作伙伴将需要完成以下领域的 MFA 验证：

- [合作伙伴中心仪表板](#partner-center-dashboard)（面向 H1 CY2020）
- [合作伙伴中心 API](#partner-center-api) （面向 H1 CY2020）
- [合作伙伴委派管理](#partner-delegated-administration)（从2019年11月18日起）

此功能的目的是帮助合作伙伴保护其对客户资源的访问，防止凭据泄露。

## <a name="partner-center-dashboard"></a>合作伙伴中心仪表板
合作伙伴中心仪表板中的某些页面将受到 MFA 保护，包括：

* "**客户**" 选项卡下的所有页。
* **支持 > 客户请求**"选项卡下的所有页面。

如果尝试访问任何这些页面，并且之前未完成 MFA 验证，则需要执行此操作。

以下用户类型有权访问这些受 MFA 保护的页面，因此受此功能影响，其中包括：

* 管理代理
* 销售代理
* 支持人员代理

为了说明这种方法的工作原理，请考虑以下两个示例。

**示例1：合作伙伴已实现 Azure AD MFA**
1.  Jane 适用于 CSP Contoso。 Contoso 已使用 Azure AD MFA 实现了 Contoso 合作伙伴租户下的所有用户的 MFA。
2.  Jane 在她的工作站上启动了一个新的浏览器会话，并导航到 "合作伙伴中心" 面板的 "概述" 页（不受 MFA 保护）。 合作伙伴中心将 Jane 重定向到 Azure AD，以便登录。
3.  由于 Contoso 的现有 Azure AD MFA 设置，需要 Jane 来完成 MFA 验证。 成功登录和 MFA 验证后，Jane 会重定向回合作伙伴中心仪表板概述页。
4.  Jane 尝试访问合作伙伴中心的一个受 MFA 保护的页面。 由于 Jane 在先前登录期间已完成了 MFA 验证，因此 Jane 可以访问受 MFA 保护的页面，而无需再次进行 MFA 验证。

**示例2：合作伙伴已使用联合身份验证实现第三方 MFA**
1. Trent 适用于 CSP Wingtip。 Wingtip 已使用第三方 MFA 为 Wingtip partner 租户下的所有用户实现了 MFA，该用户通过联合身份验证与 Azure AD 集成。
2. 在他的工作站上，Trent 将启动一个新的浏览器会话，并导航到 "合作伙伴中心" 面板的 "概述" 页（不受 MFA 保护）。 合作伙伴中心将 Justin 重定向到 Azure AD，以便登录。
3. 由于 Wingtip 具有设置联合身份验证，因此 Azure AD 重定向 Trent 到联合标识提供程序，以完成登录和 MFA 验证。 成功登录和 MFA 验证后，Trent 将重定向回 Azure AD，然后重定向到合作伙伴中心仪表板概述页。
4. Justin 尝试访问合作伙伴中心的一个受 MFA 保护的页面。 由于 Trent 在之前登录时已经完成了 MFA 验证，Trent 可以访问受 MFA 保护的页面，而无需再次进行 MFA 验证。

**示例3：合作伙伴未实现 MFA**
1. John 适用于 CSP Fabrikam。 Fabrikam 未为 Fabrikam 合作伙伴租户下的任何用户实现 MFA。
2. John 在他的工作站上启动了一个新的浏览器会话，并导航到 "合作伙伴中心" 面板的 "概述" 页（这不受 MFA 保护）。 合作伙伴中心将 John 重定向到 Azure AD，以便登录。
3. 由于 Fabrikam 尚未实现 MFA，因此 John 不需要完成 MFA 验证。 成功登录后，John 会重定向回合作伙伴中心仪表板概述页。
4. John 尝试访问合作伙伴中心的某个受 MFA 保护的页面。 由于 John 未完成 MFA 验证，因此合作伙伴中心将 John 重定向到 Azure AD 以完成 MFA 验证。 由于这是完成 MFA 所需的第一次 John，因此还请求 John 使用 Microsoft Authenticator 应用注册 MFA。 在成功进行 MFA 注册和 MFA 验证后，John 现在可以访问受 MFA 保护的页。

## <a name="partner-center-api"></a>合作伙伴中心 API

合作伙伴中心 API 支持仅限应用的身份验证和应用 + 用户身份验证。 使用 "应用 + 用户身份验证" 时，合作伙伴中心需要进行 MFA 验证。 更具体地讲，当合作伙伴应用程序要将 API 请求发送到合作伙伴中心时，它必须在请求的 Authorization 标头中包含一个访问令牌。 当合作伙伴中心接收到使用应用 + 用户身份验证获取的访问令牌的 API 请求时，合作伙伴中心 API 会检查*身份验证方法引用（AMR）* 声明中是否存在*MFA*值。 您可以使用 JWT 解码器来验证访问令牌是否包含所需的身份验证方法引用（AMR）值：

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

如果值存在，伙伴中心将结束 MFA 验证已完成并处理 API 请求。 如果值不存在，则合作伙伴中心 API 将拒绝请求，并提供以下响应：

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>合作伙伴委托管理

### <a name="using-service-portals"></a>使用服务门户

合作伙伴帐户（包括管理代理和支持人员代理）可以使用其合作伙伴委派的管理员权限通过 Microsoft Online Services 门户、命令行接口（CLI）和 Api （使用应用 + 用户身份验证）来管理客户资源。

当使用 "合作伙伴委派的管理员" 权限来管理客户资源时，如果访问 Microsoft Online Services 门户，其中许多门户都需要合作伙伴帐户以交互方式进行身份验证，客户 Azure Active Directory 租户设置为身份验证上下文-需要合作伙伴帐户登录到客户租户。

当 Azure Active Directory 收到此类身份验证请求时，它将需要合作伙伴帐户来完成 MFA 验证。 有两个可能的用户体验，具体取决于合作伙伴帐户是托管标识还是联合身份：

- 如果合作伙伴帐户是**托管**标识，Azure Active Directory 会直接提示用户完成 MFA 验证。 如果合作伙伴帐户尚未注册 Azure Active Directory 之前的 MFA，则系统将要求用户首先[完成 mfa 注册](#mfa-registration-experience)。

- 如果合作伙伴帐户是**联合**身份，则体验取决于伙伴管理员如何在 Azure Active Directory 中配置联合。 在 Azure Active Directory 中设置联合时，合作伙伴管理员可以指示 Azure Active Directory 联合标识提供者是否支持 MFA。 如果是这样，Azure Active Directory 会将用户重定向到联合标识提供者，以完成 MFA 验证。 否则，Azure Active Directory 会直接提示用户完成 MFA 验证。 如果合作伙伴帐户尚未注册 Azure Active Directory 之前的 MFA，则系统将要求用户首先[完成 mfa 注册](#mfa-registration-experience)。

总体体验非常类似于最终客户租户为其管理员实现了 MFA 的方案。 例如，客户租户已[为管理员启用 Azure AD 基准策略-MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，这要求具有管理权限的所有帐户通过 mfa 验证登录到客户租户，包括管理代理和支持人员代理。 出于测试目的，合作伙伴可以为客户租户中的 "[管理员" 策略启用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) ，然后尝试使用 "合作伙伴委托管理" 权限来访问客户租户。

> [!NOTE]
> 并非所有 Microsoft Online Service 门户都需要合作伙伴帐户在使用合作伙伴委派的管理员权限访问客户资源时登录到客户租户。 相反，他们只要求合作伙伴帐户登录到合作伙伴租户。 例如，Exchange 管理中心。 随着时间的推移，我们希望这些门户要求合作伙伴帐户在使用合作伙伴委派的管理员特权时登录到客户租户。

### <a name="using-service-apis"></a>使用服务 Api
某些 Microsoft Online Services Api （例如，Azure 资源管理器、Azure AD Graph、Microsoft Graph 等）支持使用合作伙伴委派的管理员权限的合作伙伴来以编程方式管理客户资源。 若要利用这些 Api 来利用合作伙伴委派的管理员权限，合作伙伴应用程序必须在 API 请求授权标头中包含访问令牌，其中访问令牌通过使用 Azure AD 进行身份验证的合作伙伴用户帐户来获取，客户 Azure AD 设置为身份验证上下文。 合作伙伴应用程序需要使用合作伙伴用户帐户登录到客户租户。

Azure AD 收到（例如身份验证请求）时，Azure AD 将需要合作伙伴用户帐户来完成 MFA 验证。 如果伙伴用户帐户以前未注册 MFA，则系统会提示用户帐户首先完成 MFA 注册。

使用合作伙伴委派的管理员权限与这些 Api 集成的所有合作伙伴应用程序都受此功能的影响。 确保合作伙伴的应用程序可以继续使用这些 Api，而不会发生中断：

- 合作伙伴必须避免将非交互式用户身份验证方法与 Azure AD 配合使用才能获取访问令牌。 使用非交互式用户身份验证方法（例如[密码流](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)）时，Azure AD 将无法提示用户完成 MFA 验证。 合作伙伴必须改用交互用户身份验证方法，例如[OpenID connect flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) 。
- 在交互式用户身份验证方法中，伙伴应该使用已启用 MFA 的合作伙伴用户帐户。 或者，在 Azure AD 系统提示时，合作伙伴可以在登录期间完成 MFA 注册和 MFA 验证。
- 这非常类似于最终客户租户已为其管理员实现了 MFA 的方案。 例如，客户租户已[为管理员启用 Azure AD 基准策略-MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，这要求具有管理权限的所有用户帐户通过 mfa 验证登录到客户租户，包括管理代理和支持人员代理。 出于测试目的，合作伙伴可以为客户租户中的 "[管理员" 策略启用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) ，然后尝试使用 "合作伙伴委托管理" 权限以编程方式访问客户租户。

### <a name="mfa-registration-experience"></a>MFA 注册体验
在 MFA 验证期间，如果合作伙伴帐户之前尚未注册 MFA，Azure AD 将提示用户首先完成 MFA 注册：

![MFA 注册步骤1](images/MfaRegistration1.png)

单击 "**下一步**" 后，系统将要求用户从一系列验证方法（包括电话、短信和验证器应用）中进行选择。

![MFA 注册步骤2](images/MfaRegistration2.png)

成功注册后，用户需要根据用户选择的验证完成 MFA 验证。



## <a name="request-for-technical-exception"></a>请求技术异常

如果合作伙伴遇到 Microsoft Online Services 的技术问题，但没有可行的解决方案或解决方法，则合作伙伴可申请技术例外以取消 MFA 验证。 在执行此操作之前，请查看以下部分：

 - [合作伙伴报告的常见问题列表](#list-of-common-issues-reported-by-partners)
 - [如何提交技术异常请求](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>合作伙伴报告的常见问题列表
在应用技术异常之前，请查看其他合作伙伴报告的常见问题列表，以了解这些问题是否是技术异常的有效原因。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>问题1：合作伙伴需要更多时间来实现其合作伙伴代理的 MFA
合作伙伴尚未启动或仍处于为其合作伙伴代理实现 MFA 的过程，这些客户需要使用合作伙伴委派管理权限来管理客户资源。 合作伙伴需要更多时间来完成 MFA 实现。 这是否是技术异常的有效原因？

**答**：否。 合作伙伴需要计划为其用户实现 MFA，以避免中断。

> [!NOTE]
> 即使合作伙伴尚未实现其合作伙伴代理的 MFA，伙伴代理仍可使用合作伙伴委派管理权限访问 Microsoft Online Services 门户，前提是他们可以完成 MFA 注册和 MFA 验证当登录到客户租户时出现提示。 完成 MFA 注册不会自动为用户启用 MFA。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>问题2：合作伙伴尚未对不使用委派的管理员权限的用户帐户实施 MFA
合作伙伴在其合作伙伴租户中有一些用户，这些用户不需要访问 Microsoft Online Services 门户即可使用合作伙伴委派管理权限来管理客户资源。 合作伙伴正在为这些用户实现 MFA，需要更多时间才能完成。 这是否是技术异常的有效原因？

**答**：否。 由于这些用户帐户不使用合作伙伴委派管理权限来管理客户资源，因此他们不需要登录到客户租户。 它们不受 Azure AD 要求在登录到客户租户期间进行 MFA 验证。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>问题3：合作伙伴尚未为用户服务帐户实现 MFA
合作伙伴在其合作伙伴租户中提供了一些用户帐户，由设备用作服务帐户。 这些帐户通常是低特权帐户，无需访问合作伙伴中心或 Microsoft 联机服务门户即可使用合作伙伴委派管理权限来管理客户资源。 这是否是技术异常的有效原因？

**答**：否。 由于这些用户帐户不使用合作伙伴委派管理权限来管理客户资源，因此他们不需要登录到客户租户。 它们不受 Azure AD 要求在登录到客户租户期间进行 MFA 验证。

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>问题4：合作伙伴无法使用 MS 验证器应用实现 MFA
合作伙伴具有 "清洁办公桌" 策略，不允许员工将其个人移动设备带入其工作区。 在不访问其个人移动设备的情况下，员工无法安装 MS 身份验证器应用，这是 Azure AD 基准策略支持的唯一 MFA 验证。 这是否是技术异常的有效原因？

**答**：不能，这不是一个用于技术异常的有效原因。 合作伙伴应考虑以下替代方法，以便在访问合作伙伴中心时，其员工仍可以完成 MFA 验证：
- 除了 MS 验证器应用外，Azure AD 基准策略还可与第三方兼容的身份验证器应用（可能是运行 Microsoft Windows 的 Windows 计算机）一起使用。
- 合作伙伴还可以注册 Azure AD Premium 或第三方 MFA 解决方案（与 Azure AD 兼容），该解决方案可以提供其他验证方法。

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>问题5：由于使用旧式身份验证协议，伙伴无法实现 MFA
合作伙伴的某些合作伙伴代理仍在使用旧式身份验证协议，而不是 MFA 兼容。 例如，用户仍在使用基于旧身份验证协议的 Outlook 2010。 为这些伙伴代理启用 MFA 将中断旧身份验证协议的使用。

**答**：不能，这不是一个用于技术异常的有效原因。 由于不能使用 MFA 验证来保护这些协议，因此强烈建议合作伙伴避免使用旧的身份验证协议，并且更容易受到凭据泄露。 如果不再使用旧的身份验证协议，则合作伙伴应考虑注册 Azure AD Premium，以支持使用应用程序密码。 应用程序密码是由系统生成的一次性密码，通常比用户生成的密码更强。 通过使用应用程序密码，合作伙伴可以为其用户实现 MFA，同时回退到仅适用于旧身份验证协议的应用程序密码。

> [!NOTE]
> 即使合作伙伴尚未实现其合作伙伴代理的 MFA，伙伴代理仍可使用合作伙伴委派管理权限访问 Microsoft Online Services 门户，前提是他们可以完成 MFA 注册和 MFA 验证当登录到客户租户时出现提示。 完成 MFA 注册不会自动为用户启用 MFA。

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>问题6：合作伙伴使用的是不支持 MFA 的 Exchange Online PowerShell
合作伙伴将使用带有合作伙伴委派管理权限的 Exchange Online PowerShell 代表其客户管理 Exchange Online 服务。 Exchange Online PowerShell 不支持 MFA。 如果合作伙伴为其用户实现 MFA，则这些用户将无法再访问 Exchange Online PowerShell。 这是否是技术异常的有效原因？

**答**：是的，这可能被视为技术异常的一个有效原因。 [支持合作伙伴委派管理的现有 Exchange Online PowerShell 模块](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)不需要合作伙伴用户登录到客户租户，因此不受 AZURE AD 需要 MFA 验证的影响。 但是，它不与 MFA 兼容。 Microsoft Exchange Online 团队正在开发一个新的 PowerShell 模块，该模块支持伙伴委托管理特权和 MFA。 在新的 PowerShell 模块可用之前，对于需要使用现有 PowerShell 模块的用户，合作伙伴无法实现 MFA。 如果这些用户在访问其他 Microsoft Online Services 时遇到困难，因为 Azure AD 要求在跨租户登录期间进行 MFA 验证，则合作伙伴可以请求技术例外来禁止 MFA 验证。

> [!NOTE]
> 即使合作伙伴无法为需要访问 Exchange Online PowerShell 模块的用户实现 MFA，这些用户仍可以访问 Microsoft Online Services，以使用所提供的合作伙伴委派管理权限来管理客户资源当登录到客户租户时，他们可以在出现提示时完成 MFA 注册和 MFA 验证。 完成 MFA 注册不会自动为用户启用 MFA，因此不会影响对 Exchange Online PowerShell 模块的访问。

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>问题7：合作伙伴已实现 Azure AD 无法识别的第三方 MFA
合作伙伴已使用第三方 MFA 解决方案为其用户实现了 MFA。 但是，合作伙伴无法正确配置第三方 MFA 解决方案来中继，以 Azure AD 在用户身份验证期间已完成 MFA 验证。 这是否是技术异常的有效原因？

**答**：是的，这可能被视为技术异常的一个有效原因。 提交针对技术异常的请求之前，请使用第三方 MFA 解决方案提供商确认 MFA 解决方案无法配置为将*authenticationmethodsreferences*声明（使用值*multipleauthn*）传递到 Azure AD，以指示在用户身份验证期间已完成 mfa 验证。 提交有关技术异常的请求时，请提供使用的第三方 MFA 解决方案的详细信息，并指示集成方法（例如，通过联合身份验证或使用 Azure AD 自定义控件）。

### <a name="how-to-submit-a-request-for-technical-exception"></a>如何提交技术异常请求

提交技术例外请求：

1. 以全局管理员或管理员代理的身份登录到合作伙伴中心。
2. 通过导航到**支持** > **合作伙伴支持请求**并单击 "**新建请求**" 来创建新的合作伙伴服务请求。
4. 在**MFA 和安全应用程序模型**主题下，select**提交技术例外请求**作为问题类型。
6. 提供请求的详细信息以提交技术异常的服务请求，然后单击 "**提交**"。

Microsoft 可能最多需要3个工作日来提供对技术例外请求的响应。
