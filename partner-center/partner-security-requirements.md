---
title: 合作伙伴安全要求 |合作伙伴中心
ms.topic: article
ms.date: 07/18/2019
description: 了解参与云解决方案提供商计划的顾问和合作伙伴的安全要求。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: 0ce8a8dd5a58d1647c8d9e53dec0d0bbf7fe6592
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "68313927"
---
# <a name="partner-security-requirements"></a>合作伙伴安全要求

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
  - 直接帐单
  - 间接提供程序
  - 间接经销商
- 所有控制面板供应商
- 所有顾问

更高的隐私保护和安全性是我们的头等大事。 我们知道最好的防御措施并不像我们的最弱链接一样强大。 这就是为什么我们需要生态系统中的每个人都能行动, 并确保它们具有适当的安全保护。 为帮助保护合作伙伴和客户, 我们为参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴引入了一组必需的安全要求。

从2019年8月1日起, 所有合作伙伴都需要为其合作伙伴租户中的所有用户 (包括服务帐户) 强制实施多重身份验证。

> [!NOTE]
> 我们强烈建议所有合作伙伴通过主权云 (世纪、美国政府和德国) 约束力, 并立即采取这些新的安全要求。 但是, 在2019年8月1日生效, 这些合作伙伴不需要满足新安全要求。 Microsoft 将提供更多有关未来的主权云安全要求的详细信息。

与合作伙伴安全要求关联的条款已添加到[云解决方案提供商计划指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)。 自2019年8月1日起, 所有参与云解决方案提供商计划的合作伙伴都应遵守这些条款。 与顾问相关的是, 相同的合同要求就位。

在强制实施这些要求后, 不实现必需安全要求的合作伙伴将无法在云解决方案提供商计划中进行处理, 也不能使用委派管理权限来管理客户租户。 我们正在制定要求的技术实施日期, 并将使用详细信息通知合作伙伴。

## <a name="what-actions-do-i-need-to-take"></a>需要执行哪些操作？

考虑到成为合作伙伴, 我们需要确保每个用户都对每个单个身份验证都具有 MFA 质询。 这可以通过以下方式之一完成

- 实现 Azure AD Premium 并确保为每个用户强制实施 MFA
- 实现[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- 实现第三方解决方案, 并确保为每个用户强制实施 MFA

> [!IMPORTANT]
> 在从技术上强制实施这些要求后, 每次身份验证都必须具有 MFA 质询。 在访问 Microsoft 商业云服务时, 你将不能使用条件性访问的任何功能来避免使用 MFA 进行身份验证。

### <a name="considerations"></a>注意事项

由于这些要求适用于你的合作伙伴租户中的所有用户 (包括服务帐户), 因此需要考虑几个注意事项来确保顺利部署。 这些注意事项包括: 标识不能执行 MFA 的 Azure AD 中的用户, 以及不支持新式身份验证的组织使用的应用程序和设备。

在执行任何操作之前, 建议你确定以下各项:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>在进行身份验证时, 你的应用程序或设备是否不支持使用 MFA？

当你强制执行 MFA 旧身份验证时, 将阻止使用 IMAP、POP3、SMTP 等协议, 因为这些协议不支持 MFA。 若要解决此限制, 可使用称为 "[应用密码](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)" 的功能来确保应用程序或设备仍可进行身份验证。 你应查看使用[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)记录的应用密码的注意事项, 以确定是否可以在你的环境中使用它们。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>是否有策略阻止任何用户在工作时使用其移动设备？

在工作时, 必须标识阻止员工使用移动设备的任何公司策略, 因为这会影响你实现的 MFA 解决方案。 有一些 MFA 解决方案, 如通过实现[基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)提供的解决方案, 只允许使用验证器应用进行验证。 如果你的组织具有阻止使用移动设备的策略, 则应查看为受影响的用户购买[Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) , 或者可以实现第三方解决方案, 以提供最适当的验证选.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>使用用户凭据进行身份验证的自动化或集成有哪些？

由于要求是在合作伙伴目录中强制执行每个用户的 MFA (包括服务帐户), 因此, 利用用户凭据进行身份验证的任何自动化或集成都将受到影响。 因此, 务必要确定在这些情况下使用了哪些帐户。 下面列出了应考虑的应用程序或服务示例

- 用于代表客户预配资源的控制面板
- 与用于开票的任何平台 (与 CSP 计划相关) 和支持客户的集成
- 使用 Az、AzureRM、Azure AD、MS Online 等模块的 PowerShell 脚本

以上列表并不全面。 因此, 对环境中使用用户凭据进行身份验证的任何应用程序或服务执行完整评估非常重要。 若要与 MFA 的要求争用, 应尽可能在[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)中实施指导。 下面是可帮助你了解安全应用程序模型框架如何实现的其他资源

- [合作伙伴中心 .Net 示例](https://github.com/microsoft/partner-center-dotnet-samples)-此 GitHub 存储库包含使用 .net 开发的示例, 这些示例将演示如何实现安全的应用程序模型框架。
- [合作伙伴中心 Java 示例](https://github.com/microsoft/partner-center-java-samples)-此 GitHub 存储库包含使用 Java 开发的示例, 这些示例将演示如何实现安全的应用程序模型框架。
- [合作伙伴中心 PowerShell-安全应用程序模型](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)-这篇文章提供了有关如何使用 PowerShell 实现安全应用程序模型框架的详细信息。
- [合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)-这是在线社区, 你可以在其中了解即将到来的事件, 并询问你可能遇到的任何问题。

### <a name="enforcing-mfa-for-all-users"></a>为所有用户强制实施 MFA

本部分将介绍如何使用[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)对合作伙伴租户中的每个用户 (包括服务帐户) 强制实施 MFA。 如果计划使用 Azure AD Premium, 请按照[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)所述的步骤进行操作。

> [!NOTE]
> 与 Azure AD 兼容的第三方解决方案可用于为所有用户 (包括服务帐户) 强制执行 MFA。 有关应如何实现解决方案的详细信息, 请参阅供应商提供的文档。

基线保护策略是一组预定义策略, 可帮助组织防范多种常见攻击。 这些常见攻击包括密码喷涂、重播和网络钓鱼。 所有版本的 Azure Active Directory 都提供了基线保护策略。 Microsoft 使所有人都能使用这些基准保护策略, 进一步使客户和合作伙伴能够实现一流的安全实践。

下表介绍了应启用的两个基线保护策略。

|**策略**| |
|-----|-----|
|**需要对管理员的 MFA**|如果启用 "要求对管理员使用 MFA" 策略, 将要求管理员角色中的用户注册使用验证器应用的 MFA。 完成 MFA 注册后, 管理员在每次登录时都需要执行 MFA。|
|**最终用户保护**|最终用户保护是一种基于风险的 MFA 基线保护策略, 可保护目录中的所有用户。 如果启用此策略, 则要求所有用户注册使用验证器应用的 MFA。 用户可以忽略14天的 MFA 注册提示, 超过此时间后, 它们将被阻止登录, 直到他们注册 MFA。 为 MFA 注册后, 用户仅在有风险的登录尝试期间才会提示用户进行 MFA。 受损的用户帐户会被阻止, 直到其密码重置和消除了风险事件。|

启用这些策略后, 每个用户都将能够使用验证器应用的 Azure MFA, 无需额外付费。

#### <a name="configure-self-service-password-reset"></a>配置自助服务密码重置

自助服务密码重置 (SSPR) 是一项 Azure Active Directory 功能, 使用户能够重置其密码, 而无需联系其支持团队。 在使用服务之前, 用户必须注册以进行自助密码重置。 注册过程中, 用户选择一个或多个由其组织启用的身份验证方法。

当启用 "[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)" 基线保护策略时, 任何已泄露的用户帐户将被阻止, 直到其密码被重置且风险事件已消除。 考虑到这一点, 建议每个用户 (即全局管理员) 执行以下操作来注册 SSPR, 使其不会被锁定。

1. 浏览到 " [SSPR 安装" 页](https://aka.ms/ssprsetup)
2. 输入用户名和密码
3. 至少配置一个将用于验证重置密码的验证选项。  

当某个帐户遭到入侵时, 管理员将需要采取措施来还原受影响用户的访问权限。 有关取消阻止用户的过程的详细信息, 请参阅[取消阻止用户的步骤](#recovering-compromised-accounts)。

#### <a name="require-mfa-for-admins"></a>需要对管理员的 MFA

"*需要对管理员的 mfa 进行管理*基准策略" 需要针对以下目录角色的 mfa, 并将其视为最特权的 Azure Active Directory 角色:

- 全局管理员
- SharePoint 管理员
- Exchange 管理员
- 条件访问管理员
- 安全管理员
- 支持人员管理员/密码管理员
- 帐务管理员
- 用户管理员

启用 "要求对管理员使用 MFA" 策略后, 将需要使用验证器应用为 MFA 注册以上九个管理员角色。 完成 MFA 注册后, 管理员将需要在每次登录时执行 MFA。

如果你的组织在脚本或代码中使用这些帐户, 请考虑将它们替换为 [托管标识](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。

若要启用此策略并保护管理员:

1. 以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户** 。
2. 浏览到**Azure Active Directory** > **条件性访问**。
3. 在策略列表中, 选择 **"基准策略":需要对管理员**进行 MFA。
4. 将 "**启用策略**" 设置为 "**立即使用策略**"。
5. 单击 " **保存**"。

> [!WARNING]
> 启用此策略之前, 请确保用户未使用旧身份验证协议。 通过实现此策略, 将阻止旧身份验证。

> [!IMPORTANT]
> 存在一个已知问题, 它会影响你使用委派的管理权限连接到 Exchange Online PowerShell 的能力。 如果使用此 PowerShell 模块, 请参阅[Exchange Online PowerShell](#exchange-online-powershell)已知问题, 启用此策略。

#### <a name="end-user-protection"></a>最终用户保护

最终用户保护基线策略保护目录中的所有用户。 如果启用此策略, 则需要所有用户在14天内注册 Azure MFA。 注册后, 仅在有风险的登录尝试期间, 系统才会提示用户进行 MFA。 在密码重置和风险消除之前, 会阻止泄露的用户帐户。

策略**基线策略:当你导航**到 Azure 门户中的 "条件性访问" 边栏选项卡时, 最终用户保护会预配置, 并显示在顶部。

若要启用此策略并保护用户:

1. 以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户** 。
2. 浏览到**Azure Active Directory** > **条件性访问**。
3. 在策略列表中, 选择 **"基准策略":最终用户保护 (预览版)** 。
4. 将 "**启用策略**" 设置为 "**立即使用策略**"。
5. 单击 " **保存**"。

> [!WARNING]
> 启用此策略之前, 请确保用户未使用旧身份验证协议。 通过实现此策略, 将阻止旧身份验证。

> [!IMPORTANT]
> 存在一个已知问题, 这会影响你使用委派的管理权限连接到 Exchange Online PowerShell 的能力。 如果使用此 PowerShell 模块, 请参阅[Exchange Online PowerShell](#exchange-online-powershell)已知问题, 启用此策略。

## <a name="common-issues"></a>常见问题

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

启用基线策略后, 你可能会发现你的自动化或集成遇到如下所示的异常

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

发生此异常的原因是你正在使用用户凭据进行身份验证, 而 MFA 现在是必需的。 若要解决此异常, 你将需要使用访问令牌进行身份验证。 有关详细信息, 请参阅[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。

>[!IMPORTANT]
>大多数新式 Api 和 PowerShell 模块都支持使用访问令牌进行身份验证的功能。 但是, 有一些当前不支持此功能。 如果你需要帮助来确定尝试使用的 API 或 PowerShell 模块是否支持使用访问令牌进行身份验证, 请在[合作伙伴中心安全指南组](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)社区中发布一条消息。

#### <a name="aadsts700082"></a>AADSTS700082

一旦实现了安全应用程序模型框架, 在生成初始刷新令牌后, 可能会收到以下异常90天

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

对于 Azure Active Directory 刷新令牌的最长生存期为90天。 若要解决此错误, 你将需要生成并安全地存储新的刷新令牌。 请注意, 可以通过编程方式更新刷新令牌, 因为每个 Azure Active Directory 请求都将返回一个新的刷新令牌。 可以实现相应的逻辑, 以便在安全存储的刷新令牌过期之前对其进行更新。

有关详细信息, 请参阅[Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

### <a name="recovering-compromised-accounts"></a>恢复受损帐户

为了帮助保护我们的客户, Microsoft 泄漏的凭据服务将查找公开提供的用户名/密码对。 如果这些用户与我们的用户之一匹配, 我们将帮助你立即保护该帐户。 标识为具有泄漏的凭据的用户将被确认为已泄露。 这些用户在重置其密码之前将被阻止登录。

如果已在目录中启用功能, 则分配有 Azure AD Premium 许可证的用户可以通过自助服务密码重置 (SSPR) 还原访问权限。 如果用户不具有被阻止的高级许可证, 则必须与管理员联系以执行手动密码重置, 并关闭标记用户风险事件。

#### <a name="steps-to-unblock-a-user"></a>取消阻止用户的步骤

通过检查用户的登录日志来确认该用户已被该策略阻止。

1. 管理员需要登录到**Azure 门户**并导航到**Azure Active Directory** > **用户**> 单击用户的名称并导航到 "登录"。
2. 若要在被阻止的用户上启动密码重置, 管理员需要 > 导航到已**标记为有风险 Azure Active Directory 用户**
3. 单击其帐户被阻止的用户, 查看有关用户最近登录活动的信息。
4. 单击 "重置密码", 分配在下一次登录时必须更改的临时密码。
5. 单击 "消除所有事件" 以重置用户的风险评分。

用户现在可以登录、重置其密码并访问应用程序。

## <a name="known-issues"></a>已知问题

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

启用 MFA 后, 合作伙伴将无法使用 Exchange Online PowerShell 的委派管理权限来对其客户执行操作。 有关此限制的详细信息, 请参阅[使用多重身份验证连接到 Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) 。

## <a name="resources-and-support"></a>资源和支持

通过[合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance), 你可以找到更多的资源, 并了解即将发生的事件, 例如技术办公室的工作时间。 若要详细了解要求, 请参阅[常见问题](http://assetsprod.microsoft.com/security-requirements-faq.pdf)文档。
