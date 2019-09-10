---
title: 合作伙伴安全要求 | 合作伙伴中心
ms.topic: article
ms.date: 08/30/2019
description: 了解对参与云解决方案提供商计划的顾问和合作伙伴的安全要求。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: c95ec38f928ca4032ffecebaf25f23e87d10c079
ms.sourcegitcommit: de3cdc792b6b4bbc64d1288d371623d79d535205
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/03/2019
ms.locfileid: "70215651"
---
# <a name="partner-security-requirements"></a>合作伙伴安全要求

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
  - 直接计费
  - 间接提供商
  - 间接经销商
- 所有控制面板供应商
- 所有顾问

增强隐私保护和安全性是我们优先关注的事项。 我们知道，最好的防御措施是防患于未然，链条的强度取决于其最弱的一环。 因此，我们需要生态系统中的所有人都行动起来，确保将安全保护措施实施到位。 为了保护合作伙伴和客户，我们引入了一系列强制性安全要求，针对那些参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴。

从 2019 年 8 月 1 日开始，所有合作伙伴都必须对其合作伙伴租户中的所有用户（包括服务帐户）强制实施多重身份验证。

> [!NOTE]
> 强烈建议所有通过主权云（世纪互联、Microsoft Cloud for US Government、德国 Microsoft 云）进行事务处理的合作伙伴立即行动起来，履行这些安全要求。 但是，这些合作伙伴不是必须满足这些新的在 2019 年 8 月 1 日生效的安全要求。 Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。

与合作伙伴安全要求相关的条款已添加到[云解决方案提供商计划指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)中。 从 2019 年 8 月 1 日起，所有参与云解决方案提供商计划的合作伙伴都应遵守这些条款。 由于与顾问相关，因此会实施相同的合同要求。

一旦我们强制实施这些安全要求，不实施这些强制性要求的合作伙伴将不能在云解决方案提供商计划中进行事务处理，也不能利用委托管理权限来管理客户租户。 我们准备针对这些要求确定一个严格的强制实施日期，并且会将该日期和相关详细信息告知合作伙伴。

## <a name="what-actions-do-i-need-to-take"></a>我需要采取什么行动？

考虑到合作伙伴会有很高的特权，因此我们需要确保在每位用户每次进行身份验证时都对其进行 MFA 质询。 可以通过下述方式之一来实现这一点：

- 实现 Azure AD Premium，确保为每位用户强制实施 MFA
- 实现[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- 实现第三方解决方案，确保为每位用户强制实施 MFA

> [!IMPORTANT]
> 严格实施这些要求以后，每一项身份验证都必须进行 MFA 质询。 你将无法使用条件访问的任何功能来避免在访问 Microsoft 商业云服务时使用 MFA 进行身份验证。

### <a name="considerations"></a>注意事项

由于这些要求适用于合作伙伴租户中的所有用户（包括服务帐户），因此需要遵守一些注意事项，确保顺利进行部署。 这些注意事项包括确定 Azure AD 中不能执行 MFA 的用户，以及组织所使用的不支持新式身份验证的应用程序和设备。

建议在执行任何操作之前确定以下事项：

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>你是否有进行身份验证时不支持使用 MFA 的应用程序或设备？

强制实施 MFA 时，系统会阻止旧版身份验证协议（例如 IMAP、POP3、SMTP 等）的使用，因为这些协议不支持 MFA。 为了解决此限制问题，可以使用名为[应用密码](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)的功能，确保应用程序或设备仍然能够进行身份验证。 你应该查看[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)记录的应用密码使用注意事项，确定应用密码是否可以在你的环境中使用。

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>你是否有用户使用通过与合作伙伴租户相关联的许可证获得的 Office 365？

在实现任何解决方案之前，建议你确定合作伙伴租户中的用户所使用的 Microsoft Office 版本。 在采取任何行动之前，请参阅 [Office 365 部署的多重身份验证计划](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)。 用户可能会在使用 Outlook 之类的应用程序时遇到连接问题。 在强制实施 MFA 之前，必须确保使用的是 Outlook 2013 SP1 或更高版本，且组织已启用新式身份验证。 有关详细信息，请参阅[在 Exchange Online 中启用新式身份验证](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)。

若要为任何运行 Windows 且已安装 Microsoft Office 2013 的设备启用新式身份验证，需创建两个注册表项。 请参阅[在 Windows 设备上启用适用于 Office 2013 的新式身份验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。

> [!IMPORTANT]
> 如果已为用户启用 Azure AD MFA，但他们有一些运行 Office 2013 的设备未启用新式身份验证，则他们需要在这些设备上使用应用密码。 若要详细了解应用密码以及应该在何时、何处以何种方式使用它们，可参阅：[应用密码与 Azure 多重身份验证](https://go.microsoft.com/fwlink/p/?LinkId=528178)。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>是否有策略阻止用户在工作时使用其移动设备？

必须确定任何阻止员工在工作时使用移动设备的公司策略，因为它会影响你实现的具体的 MFA 解决方案。 有的 MFA 解决方案（例如通过实施[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)提供的解决方案）仅允许使用 Authenticator 应用进行验证。 如果组织的某项策略阻止使用移动设备，则应考虑以下选项之一：

- 部署可以在安全系统上运行的基于时间的一次性密码 (TOTP) 应用程序
- 实现第三方解决方案，为合作伙伴租户中的每位用户强制实施 MFA，以便提供最适当的验证选项
- 为受影响的用户购买 [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) 许可证

对 FIDO 安全密钥的使用支持已经列入基线保护策略的路线图。 添加支持后，即可利用 FIDO 安全密钥进行双重身份验证。 在此之前，只能使用 Authenticator 应用。

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>你有什么样的利用用户凭据进行身份验证的自动化或集成？

由于此要求是对合作伙伴目录中的每位用户（包括服务帐户）强制实施 MFA，因此任何利用用户凭据进行身份验证的自动化或集成都会受影响。 因此，必须确定在这些情况下使用的是什么帐户。 下面是一个列表，其中包含应该考虑的应用程序或服务的示例：

- 控制面板，用于代表客户预配资源
- 与任何用于客户发票（由于与 CSP 计划相关）和支持的平台的集成
- 利用 Az、AzureRM、Azure AD、MS Online 等模块的 PowerShell 脚本

以上列表并不完整。 因此，必须对环境中利用用户凭据进行身份验证的任何应用程序或服务进行完整的评估。 在可能情况下，应该按[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)中的指南（不同于 MFA 的要求）进行操作。 下面是其他资源，介绍如何实现安全应用程序模型框架：

- [Partner Center .NET Samples](https://github.com/microsoft/partner-center-dotnet-samples)（合作伙伴中心 .NET 示例） - 此 GitHub 存储库包含使用 .NET 开发的示例，用于演示如何实现安全应用程序模型框架。
- [合作伙伴中心 Java 示例](https://github.com/microsoft/partner-center-java-samples) - 此 GitHub 存储库包含使用 Java 开发的示例，用于演示如何实现安全应用程序模型框架。
- [合作伙伴中心 PowerShell - 安全应用程序模型](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) - 这是一篇详述如何使用 PowerShell 实现安全应用程序模型框架的文章。
- [合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - 这是一个在线社区，你可以在其中了解即将发生的事件并提问任何问题。

### <a name="enforcing-mfa-for-all-users"></a>对所有用户强制实施 MFA

此部分介绍如何使用[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)为合作伙伴租户中的每位用户（包括服务帐户）强制实施 MFA。 如果打算使用 Azure AD Premium，则请执行[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)记录的步骤。

> [!NOTE]
> 可以使用与 Azure AD 兼容的第三方解决方案为所有用户（包括服务帐户）强制实施 MFA。 请参阅供应商文档，更详细地了解应该如何实现此解决方案。

基线保护策略是一组预定义的策略，可帮助组织防范许多常见攻击。 这些常见攻击可能包括密码喷射、重播和钓鱼。 基线保护策略在所有版本的 Azure Active Directory 中提供。 Microsoft 会将这些基线保护策略提供给所有人，从而让客户和合作伙伴可以实施最佳安全做法。

下表介绍了应该启用的两种基线保护策略。

|**策略**| |
|-----|-----|
|**对管理员要求 MFA**|启用“对管理员要求 MFA”策略以后，担任管理员角色的用户就必须使用 Authenticator 应用注册 MFA。 完成 MFA 注册以后，管理员在每次登录时都需要执行 MFA。|
|**最终用户保护**|“最终用户保护”是一种基于风险的 MFA 基线保护策略，用于保护目录中的所有用户。 启用此策略以后，所有用户就必须使用 Authenticator 应用注册 MFA。 用户可以忽略 MFA 注册提示 14 天，此期限过后系统会阻止用户登录，直至用户注册 MFA 为止。 注册 MFA 以后，系统仅在检测到风险登录尝试时提示用户进行 MFA。 系统会阻止被盗用的用户帐户，直至用户重置密码并消除风险事件为止。|

启用这些策略后，每位用户就能够使用 Azure MFA，通过 Authenticator 应用进行验证，不需额外付费。

#### <a name="configure-self-service-password-reset"></a>配置自助式密码重置

自助式密码重置 (SSPR) 是一项 Azure Active Directory 功能，该功能允许用户重置其密码而不需联系其支持团队。 用户必须主动或被动注册自助式密码重置，然后才能使用此服务。 在注册期间，用户可以选择其组织启用的一个或多个身份验证方法。

启用[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略以后，系统会阻止被盗用的任何用户帐户，直至用户重置密码并消除风险事件为止。 考虑到这一点，建议每位全局管理员用户通过以下操作注册 SSPR，防止被系统阻止进入。

1. 浏览到 [SSPR 设置页](https://aka.ms/ssprsetup)
2. 输入用户名和密码
3. 配置至少一个验证选项。当你重置密码时，系统会使用这些选项进行身份验证。  

如果某个帐户被盗用，管理员需采取措施还原受影响用户的访问权限。 请参阅[取消阻止用户的步骤](#recovering-compromised-accounts)，详细了解取消阻止用户的过程。

#### <a name="require-mfa-for-admins"></a>对管理员要求 MFA

“对管理员要求 MFA”基线策略要求对以下目录角色进行 MFA，这些角色是特权最高的 Azure Active Directory 角色： 

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
2. 浏览到“Azure Active Directory”   >   “条件访问”。
3. 在策略列表中，选择“基线策略:  对管理员要求 MFA”。
4. 将“启用策略”设置为“立即使用策略”。  
5. 单击“保存”。 ****

> [!WARNING]
> 在启用此策略之前，请确保用户使用的不是旧版身份验证协议。 实施此策略以后，系统会阻止旧版身份验证。

> [!IMPORTANT]
> 这是已知问题，会影响你使用委派的管理权限连接到 Exchange Online PowerShell。 如果使用该 PowerShell 模块，请在启用此策略之前查看 [Exchange Online PowerShell](#exchange-online-powershell) 已知问题。

#### <a name="end-user-protection"></a>最终用户保护

“最终用户保护”基线策略保护目录中的所有用户。 启用此策略以后，所有用户就必须在 14 天内注册 Azure MFA。 注册以后，系统仅在检测到风险登录尝试时提示用户进行 MFA。 系统会阻止被盗用的用户帐户，直至用户重置密码并消除风险为止。

“基线策略:  最终用户保护”策略已预先配置。当你在 Azure 门户中导航到“条件访问”边栏选项卡时，会在顶部看到它。

若要启用此策略并保护用户，请执行以下操作：

1. 以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户**。
2. 浏览到“Azure Active Directory”   >   “条件访问”。
3. 在策略列表中，选择“基线策略:  最终用户保护(预览)”。
4. 将“启用策略”设置为“立即使用策略”。  
5. 单击“保存”。 ****

> [!WARNING]
> 在启用此策略之前，请确保用户使用的不是旧版身份验证协议。 实施此策略以后，系统会阻止旧版身份验证。

> [!IMPORTANT]
> 这是已知问题，会影响你使用委派的管理权限连接到 Exchange Online PowerShell。 如果使用该 PowerShell 模块，请在启用此策略之前查看 [Exchange Online PowerShell](#exchange-online-powershell) 已知问题。

## <a name="assessing-your-environment"></a>评估环境

根据当前的一项合作伙伴安全要求，你必须为合作伙伴租户中的每位用户强制实施 MFA。 由于此要求可以通过许多不同的方法来履行，因此可能难以评估是否需要执行额外的操作。 可以使用 Azure Active Directory 审核日志和 [Microsoft 安全功能分数](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)之类的工具，以便评估是否需要执行额外的操作才能通过 MFA 来保护租户。 Microsoft 正在合作伙伴中心构建一项体验，用于针对 MFA 和安全应用程序模型要求进行快速的符合性检查。

Microsoft 安全功能分数提供强大的可视化功能、与其他 Microsoft 产品集成的功能、将你的分数与其他公司的分数进行比较的功能、按类别筛选的功能，等等。 可以使用此工具在组织中完成安全改进操作，并跟踪分数历史记录。 此分数也可反映第三方解决方案何时解决了建议的改进操作问题。

![Microsoft 安全功能分数](images/security/secure-score.png)

> [!NOTE]
> 系统可能需要长达 24 小时的时间才能反映你可以执行的用于改进 Microsoft 安全功能分数的操作。

Microsoft 安全功能分数只是以数字方式体现你的安全态势。 若要更好地了解哪个帐户或用户在进行身份验证时没有受到 MFA 质询，建议查询 Azure Active Directory 审核日志。 为此，可以使用 [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) 模块和下面的脚本。 这样会生成一个报表，该报表详细说明了过去一天内发生的哪些身份验证尝试没有受到 MFA 质询。

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

运行以上脚本以后，即可在 report.csv 文件中获取详细信息。 该文件将包含一个列表，列表中的身份验证尝试是过去一天内发生的，相关用户没有受到 MFA 质询。 你需要查看每个条目，确定其是否为预期的行为，必要时采取行动。

![评估报表](images/security/assessment-report.png)

## <a name="common-issues"></a>常见问题

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

在启用基线策略以后，你可能会发现自己的自动化或集成遇到如下所示的异常：

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

发生此异常的原因是，你在使用用户凭据进行身份验证，而现在需要的是 MFA。 若要解决此异常问题，需要使用访问令牌进行身份验证。 有关详细信息，请参阅[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。

>[!IMPORTANT]
>大多数新式 API 和 PowerShell 模块支持使用访问令牌进行身份验证的功能。 不过，也有一些目前不支持此功能。 如果需要他人帮你确定你尝试使用的 API 或 PowerShell 模块是否支持使用访问令牌进行身份验证，则请在[合作伙伴中心安全指南组](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)社区发布消息。

#### <a name="aadsts700082"></a>AADSTS700082

一旦实现安全应用程序模型框架，则可能会在生成初始刷新令牌 90 天后收到以下异常：

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

就 Azure Active Directory 来说，刷新令牌的最长生存期为 90 天。 若要解决此错误，需生成新的刷新令牌并将其安全地存储。 请注意，可以通过编程方式更新此刷新令牌，因为每次向 Azure Active Directory 请求访问令牌时，都会返回新的刷新令牌。 可以实现适当的逻辑，在安全存储的刷新令牌过期之前更新它。

有关详细信息，请参阅 [Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

### <a name="recovering-compromised-accounts"></a>恢复被盗用的帐户

为了保护客户，Microsoft 的泄漏凭据服务会查找公开可用的用户名/密码对。 如果这些用户名/密码对与某位用户匹配，我们会立即对该帐户进行保护。 如果确定用户的凭据泄漏，则会将其确认为被盗用用户。 系统会阻止这些用户登录，直至其密码被重置。

被分配 Azure AD Premium 许可证的用户可以通过自助式密码重置 (SSPR) 来还原访问权限，前提是该功能已在用户的目录中启用。 没有高级许可证却被系统阻止的用户必须联系管理员，让其执行手动密码重置并消除标记的用户风险事件。

#### <a name="steps-to-unblock-a-user"></a>取消阻止用户的步骤

检查用户的登录日志，确认用户是否已被策略阻止。

1. 管理员需登录到 **Azure 门户**，导航到 **“Azure Active Directory”**  >   “用户”，单击用户的名称，然后导航到“登录”。
2. 若要对被阻止的用户启动密码重置，管理员需导航到“Azure Active Directory”   >   “已标记为存在风险的用户”
3. 单击其帐户已被阻止的用户，查看有关此用户的最近登录活动的信息。
4. 单击“重置密码”，分配一个临时密码，该密码必须在下次登录时更改。
5. 单击“清除所有事件”，重置用户的风险分数。

用户现在可以登录并重置其密码，然后访问应用程序。

## <a name="known-issues"></a>已知问题

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

强制实施 MFA 以后，合作伙伴将无法利用其委派的管理权限和 Exchange Online PowerShell 对其客户执行操作。 有关此限制的详细信息，请参阅[使用多重身份验证连接到 Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)。

若要规避此限制，可以创建一个新帐户，但不使用它来执行交互式身份验证。 建议使用 [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) 来创建此新帐户，然后执行初始配置。 以下 PowerShell 可以用来创建并配置此帐户：

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

下次通过 PowerShell 连接到 Exchange Online 时，请使用此帐户，它会按预期运行。

> [!IMPORTANT]
> 合作伙伴在强制实施 MFA 以后利用其委派的管理权限和 Exchange Online PowerShell 对其客户执行操作的功能将在以后推出。 在此之前，应使用此解决方法。

## <a name="resources-and-support"></a>资源和支持

可以通过[合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)查找其他资源，并了解即将发生的事件，例如技术办公时间。 请参阅[常见问题解答](partner-security-requirements-faq.md)文档，详细了解相关要求。
