---
title: 合作伙伴安全要求常见问题解答 |合作伙伴中心
ms.topic: article
ms.date: 07/18/2019
description: 有关合作伙伴安全要求的常见问题
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820598"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>有关合作伙伴安全要求的常见问题

本文包含有关[合作伙伴安全要求](partner-security-requirements.md)的一些常见问题解答。

## <a name="partner-security-requirements"></a>合作伙伴安全要求

### <a name="what-are-the-new-partner-security-requirements"></a>新的合作伙伴安全要求有哪些？

为保护我们的合作伙伴和客户, 我们要求合作伙伴立即执行以下操作:  

1. **为合作伙伴租户中的所有用户启用多重身份验证 (MFA)** 。 合作伙伴租户中的所有用户必须使用多重身份验证 (MFA), 才能登录到 Microsoft 商业云服务, 或通过合作伙伴中心或 Api 在 CSP 中进行交易。 通过启用基线保护策略 MFA, 无需为合作伙伴租户的所有用户提供费用。

2. **采用安全应用程序模型框架**。 与 Microsoft API (如 Azure 资源管理器、Microsoft Graph 和合作伙伴中心 API) 集成的所有合作伙伴都必须采用安全的应用程序模型框架, 以避免在启用基线策略时对其集成的任何中断。 
 
启用多重身份验证 (MFA) 并采用安全的应用程序模型框架, 可帮助保护你的基础结构, 并保护客户的数据免受潜在的安全风险, 例如识别盗窃或其他欺诈事件。  

### <a name="which-partners-need-to-meet-the-requirements"></a>哪些合作伙伴需要满足这些要求？

这些要求适用于以下合作伙伴组:
- 参与云解决方案提供商 (CSP) 计划并使用 Microsoft 商业云服务进行约束力的所有合作伙伴组织
  - 直销合作伙伴
  - 间接提供商
  - 间接经销商
- 所有控制面板供应商
- 所有 Advisor 计划合作伙伴  

所有合作伙伴都不需要在8月1日生效的情况下, 通过主权云 (世纪、美国政府和德国) 约束力所有合作伙伴。 但是, 我们强烈建议使用主权云的所有合作伙伴都将立即采取这些新的安全要求。 Microsoft 将提供更多有关未来的主权云安全要求的详细信息。

### <a name="what-are-the-key-timelines-and-milestones"></a>关键时间线和里程碑有哪些？

与这些安全要求关联的条款将立即添加到云解决方案提供商计划指南。 你将需要实现这些安全要求, 使其符合你在8月 1 2019 日生效的 CSP 计划中的参与。 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>如果我不执行任何操作, 会发生什么情况？

在强制执行这些合作伙伴安全要求后, 无法遵守这些安全措施和义务的合作伙伴将无法在云解决方案提供商计划中进行处理, 也无法在使用委派管理权限的情况下管理客户租户。 我们正在制定要求的强制实施日期, 并将使用详细信息通知合作伙伴。

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Microsoft 为何强制实施这些新要求？
客户和合作伙伴的安全和隐私是 Microsoft 的头等大事。 我们会继续看到更复杂、不断增加的安全攻击, 主要与身份泄露事件相关。 由于预防控制在整体防御策略中扮演着关键角色来阻止安全攻击, 因此我们将开始强制实施一组必需的安全要求, 以帮助保护合作伙伴及其客户。

### <a name="does-this-apply-to-all-geographies"></a>这是否适用于所有地理区域？

是的, 这适用于所有地域。 我们强烈建议所有合作伙伴通过主权云 (世纪、美国政府和德国) 约束力, 并立即采取这些新的安全要求。 不过, 这些合作伙伴不需要满足8月1日生效的新安全要求。 Microsoft 将提供更多有关未来的主权云安全要求的详细信息。

## <a name="required-actions"></a>必需的操作

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>需要执行哪些关键操作来满足要求？  
CSP 计划中的所有合作伙伴 (直接帐单、间接提供商和间接经销商)、顾问和控制面板供应商都必须满足要求。

1. **为所有用户强制实施 MFA**

    CSP 计划、顾问和控制面板供应商的所有合作伙伴都需要为其合作伙伴租户中的所有用户强制实施 MFA。 为此, 可以启用 "[要求对管理员使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)"、"[最终用户保护基准](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)" 和任何将来的基准策略。 基准策略提供的功能将继续发展, 以确保合作伙伴和客户免受不断变化的安全威胁。 因此, 请务必查看[基准策略文档](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)以了解详细信息。

    - 请[参阅基准策略:要求对管理员](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)进行 mfa, 详细了解如何启用 "对管理员使用 mfa" 基准策略。
    - 请[参阅基准策略:有关如何启用](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)最终用户保护基线策略的详细信息, 请最终用户保护。
    - 了解[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)的概念。

    其他注意事项:

    - 间接提供商需要与间接经销商合作, 以便加入合作伙伴中心 (如果尚未这样做), 并鼓励其经销商满足要求。
    - 使用[Microsoft Authenticator 应用程序](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)的唯一验证方法将 Azure MFA 免费提供给合作伙伴租户中的所有用户。
    - 如果需要其他方法 (如短信或电子邮件), 可通过[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) sku 获取其他验证方法。
    - 合作伙伴还可以在访问 Microsoft 商业云服务时, 根据每个用户的情况利用第三方 MFA 解决方案。

2. **采用安全应用程序模型框架**

    使用任何 Api (例如 Azure 资源管理器、Microsoft Graph、合作伙伴中心 API 等) 开发了自定义集成的所有合作伙伴或使用 PowerShell 等工具实现的自定义自动化都需要采用[安全的应用程序模型](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)与 Microsoft 云服务集成的框架。 如果不这样做, 可能会由于 MFA 部署导致中断。 以下资源提供了有关如何采用模型的概述和指导。

    - [安全应用程序模型概述](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [合作伙伴中心:安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP 计划中的合作伙伴: 用于启用安全应用程序模型的 .NET 示例代码](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [CSP 计划中的合作伙伴:用于启用安全应用程序模型的 Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [合作伙伴中心身份验证文档](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    如果你使用的是 "控制面板", 则需要咨询供应商以了解如何采用安全应用程序模型框架。

    控制面板供应商需要作为控制面板供应商[加入](https://docs.microsoft.com/partner-center/enroll-as-cpv)合作伙伴中心, 并立即开始实现此要求。 请参阅合作伙伴中心: [保护应用程序模型](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)框架。 控制面板供应商必须接受并管理 CSP 合作伙伴的同意而不是凭据, 并清除所有现有的 CSP 合作伙伴的凭据。

## <a name="multi-factor-authentication"></a>多重身份验证

### <a name="what-is-mfa"></a>什么是 MFA？

多重身份验证 (MFA) 是一种安全机制, 但通过多个必需的安全和验证过程对个人进行身份验证。 它的工作方式是需要以下两种或多种身份验证方法:

- 您知道的信息（通常为密码）
- 您拥有的东西（不易被复制的受信任设备，如电话）
- 您的特征（生物识别）

### <a name="what-are-baseline-protection-policies"></a>什么是基准保护策略？ 

[Microsoft 基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)(当前预览) 是一组预定义策略, 可帮助组织防范多种常见攻击。 这些常见攻击包括密码喷涂、重播和网络钓鱼。 所有版本的 Azure Active Directory 都提供基准策略。 Microsoft 将这些基准保护策略提供给所有人, 因为基于身份的攻击已经在过去几年的时间上升。 这些策略的目标是确保所有组织都启用了一个基线级别 "安全", 而无需额外付费。

> [!NOTE]
> Microsoft 基线策略和相关功能将继续发展, 以更好地保护合作伙伴和客户免受不断变化的安全威胁。 基本策略可能会有一些命名和分类更改。 我们强烈建议你直接访问基线策略页面, 以查看最新信息。

### <a name="what-baseline-policies-must-i-enable"></a>我必须启用哪些基准策略？

如果打算利用当前的基线保护策略为合作伙伴租户中的每个用户提供 MFA, 则必须启用 "[要求对管理员使用 mfa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) " 和 "[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)" 基准策略。 这些基准保护策略将满足合作伙伴租户中每个用户的 MFA 要求, 且仅适用于通过移动设备使用 Microsoft Authenticator 应用的合作伙伴。

"[需要对管理员的 MFA" 基准策略](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)可用于合作伙伴目录中的管理用户,[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线策略用于保护合作伙伴租户中的非管理员用户。 启用这些策略将要求用户注册 MFA。 用户成功注册后, 系统会根据策略的条件, 在登录尝试期间提示用户进行 MFA。 基准策略提供的功能将继续发展, 以确保合作伙伴和客户免受不断变化的安全威胁。 因此, 请务必查看[基准策略文档](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)以了解详细信息。

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>如何实现启用 "需要对管理员进行 MFA" 策略？ 

可以通过 Azure 管理门户启用 "需要针对管理员的 MFA" 基准策略。 请[参阅基准策略:需要针对管理员](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)的 MFA, 详细了解如何启用此基准策略。

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>如何实现启用最终用户保护策略吗？

可以通过 Azure 管理门户启用最终用户保护基准策略。 请[参阅基准策略:有关如何启用](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)此基线策略的详细信息, 请最终用户保护。

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>是否自动启用基线策略？ 

否, 若要启用这些策略, 作为全局管理员、安全管理员或条件访问管理员角色成员的用户将需要将策略配置为立即使用策略。

### <a name="what-is-the-cost-of-enabling-mfa"></a>启用 MFA 的成本是多少？

Microsoft 不需要通过实现[管理](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略, 即可免费提供 mfa。 通过此版本的 MFA 提供的唯一验证选项是[Microsoft Authenticator 应用](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。 如果需要电话呼叫或短信, 则需要购买[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)许可证。 或者, 你可以利用第三方解决方案为你的合作伙伴租户中的每个用户提供 MFA –在这种情况下, 你有责任确保你的 MFA 解决方案受到强制, 并且符合你的要求。

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>如果我已经有了 MFA 解决方案, 需要执行哪些操作？

通过这些安全要求, 合作伙伴租户中的用户在访问 Microsoft 商业云服务时将需要使用 MFA 进行身份验证。 可以使用第三方解决方案来满足这些要求。 Microsoft 不再向独立标识提供者提供验证测试, 以与 Azure Active Directory 兼容。 如果你想要测试你的产品的互操作性, 请参阅这些[准则](https://www.microsoft.com/download/details.aspx?id=56843)。

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>可以使用哪种验证方法对 MFA 进行身份验证？

Microsoft 不需要通过实现[管理](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略, 即可免费提供 mfa。 通过此版本的 MFA 提供的唯一验证选项是[Microsoft Authenticator 应用](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。 如果需要电话呼叫或短信, 则需要购买[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)许可证。 或者, 你可以利用第三方解决方案为你的合作伙伴租户中的每个用户提供 MFA –在这种情况下, 你有责任确保你的 MFA 解决方案受到强制, 并且符合你的要求。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>我使用多个合作伙伴租户来处理。 我是否需要对它们实施 MFA？

是的, 你将需要为与 CSP 计划或 Advisor 计划关联的每个 Azure Active Directory 租户强制执行 MFA。 如果计划购买 Azure Active Directory Premium 许可证, 则必须为每个 Azure Active Directory 租户中的用户购买许可证。

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>我的合作伙伴租户中的每个用户是否需要强制执行 MFA？ 

对于 "管理员" 和 "[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)" 的 "[要求 mfa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) " 基线保护策略将为合作伙伴租户中的每个用户强制实施 mfa。 如果你使用这些策略来提供 MFA 并使用[Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)应用程序, 则无需购买任何其他许可证。 否则, 你将需要购买适当的解决方案, 以便向合作伙伴租户中的每个用户提供 MFA。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>我是 Microsoft 的直接帐单合作伙伴。 需要执行哪些操作？

直接帐单云解决方案提供商合作伙伴必须为其合作伙伴租户中的每个用户强制实施 MFA。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>我是一个间接经销商, 只是通过分销商来处理。 是否仍需要执行此操作？

所有间接经销商都需要为其合作伙伴租户中的每个用户强制实施 MFA。 这是间接经销商必须执行的操作。

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>我不使用合作伙伴中心 API。 是否仍需要实现 MFA？

是的, 此安全要求适用于所有用户, 包括合作伙伴租户中的合作伙伴管理员用户和最终用户。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>哪些第三方供应商提供与 Azure Active Directory 兼容的 MFA 解决方案？

有许多独立的 MFA 解决方案检查, 如[Gartner](https://www.gartner.com/en/webinars/3881781)。 查看 MFA 供应商和解决方案时, 合作伙伴必须确保他们选择的解决方案与 Azure Active Directory 兼容。

Microsoft 不再向独立标识提供者提供验证测试, 以与 Azure Active Directory 兼容。 如果你想要测试你的产品的互操作性, 请参阅这些[准则](https://www.microsoft.com/download/details.aspx?id=56843)。

有关详细信息, 请参阅[Azure AD 联合兼容性列表](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>如何在集成沙盒中测试 MFA？

应为集成沙盒租户启用 "管理员" 和 "[最终用户" 保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线策略[要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 。 通过此策略, 租户中的每个用户都需要使用 MFA 进行身份验证。

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>启用 MFA 后如何与客户的租户进行交互？ 

否。 履行这些安全要求不会影响你管理客户的方式。 你执行委派的管理操作的能力不会中断。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>我的客户是否受合作伙伴安全要求的限制？

不需要, 不需要为客户的 Azure AD 租户中的每个用户强制实施 MFA。 但建议您与每个客户合作, 确定如何最好地保护他们的用户。

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>应用密码是否可与基线保护策略一起使用？

是的, 可以使用[应用密码](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)。 你应查看使用[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)记录的应用密码的注意事项, 以确定是否支持你的需求。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>是否可以从此要求中排除任何用户？ 

不需要, 你的合作伙伴租户中的每个用户 (包括服务帐户) 都需要使用 MFA 进行身份验证。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>合作伙伴安全要求是否适用于集成沙盒？

是, 合作伙伴安全要求适用于集成沙盒。 这意味着, 你将需要为 integration 沙盒租户中的用户实现适当的 MFA 解决方案。 建议你实现基线保护策略来提供 MFA。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>如何实现配置紧急访问 (中断玻璃) 帐户？

它被认为是创建一个或两个紧急访问帐户, 以防止无意中锁定 Azure AD 租户。 对于合作伙伴安全要求, 每个用户都需要使用 MFA 进行身份验证。 因此, 这意味着你将需要修改紧急访问帐户的定义。 它可以是利用第三方解决方案进行 MFA 的帐户。

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>来宾用户将受合作伙伴安全要求的影响？

访问合作伙伴租户中的资源时, 来宾用户需要使用 MFA 进行身份验证。 合作伙伴安全要求将不会对来宾用户访问其自己租户中的资源产生任何影响。

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>如果我使用的是第三方解决方案 Active Directory 需要联合身份验证服务 (ADFS) 吗？ 

不是, 如果使用的是第三方解决方案, 则不需要 Active Directory 联合身份验证服务 (ADFS)。 建议你与解决方案的供应商合作确定其解决方案的要求。

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>是否需要启用基线保护策略？

不需要, 不需要启用基线保护策略。 唯一的要求是在合作伙伴租户中为每个用户 (包括服务帐户) 强制执行 MFA。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>是否可以使用条件性访问来满足 MFA 要求？

是的, 你可以使用条件性访问来为你的合作伙伴租户中的每个用户 (包括服务帐户) 强制实施 MFA。 但是, 考虑到成为合作伙伴, 我们需要确保每个用户对每个单个身份验证都具有 MFA 质询。 这意味着你将无法利用条件访问的功能, 这种功能会绕过 MFA 的要求。

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>通过实现基线保护策略提供了哪些验证选项？ 

对于通过实现基线保护策略而提供的 MFA 版本, 唯一可用的验证选项是验证器应用。 使用电话呼叫和短信消息被视为不太安全。 因此, 这些选项无法通过此版本的 MFA 获得。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect 所使用的服务帐户是否受合作伙伴安全要求的影响？

不会, Azure AD Connect 使用的服务帐户将不受合作伙伴安全要求的影响。 如果由于强制 MFA 而导致 Azure AD Connect 遇到问题, 请通过 Microsoft 支持提出技术支持请求。

## <a name="secure-application-model"></a>安全应用程序模型

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>谁应该采用安全的应用程序模型来满足这些要求？

Microsoft 正在介绍一种安全且可扩展的框架, 用于验证利用多重身份验证的云解决方案提供商 (CSP) 合作伙伴和控制面板供应商 (CPV)。 有关详细信息, 请参阅[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 使用任何 Api (例如 Azure 资源管理器、Microsoft Graph、合作伙伴中心 API 等) 开发了自定义集成的所有合作伙伴或使用 PowerShell 等工具实现的自定义自动化都需要采用[安全的应用程序模型](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)与 Microsoft 云服务集成的框架。

### <a name="what-is-the-secure-application-model"></a>安全应用程序模型是什么？

Microsoft 正在介绍一种安全且可扩展的框架, 用于验证利用多重身份验证的云解决方案提供商 (CSP) 合作伙伴和控制面板供应商 (CPV)。 有关详细信息, 请参阅[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。  

### <a name="how-do-i-implement-the-secure-application-model"></a>如何实现实现安全的应用程序模型？

使用任何 Api (例如 Azure 资源管理器、Microsoft Graph、合作伙伴中心 API 等) 开发了自定义集成的所有合作伙伴或使用 PowerShell 等工具实现的自定义自动化都需要采用[安全的应用程序模型](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)与 Microsoft 云服务集成的框架。 如果不这样做, 可能会由于 MFA 部署导致中断。 以下资源提供了有关如何采用模型的概述和指导。

- [安全应用程序模型概述](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心:安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP 计划中的合作伙伴: 用于启用安全应用程序模型的 .NET 示例代码](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [CSP 计划中的合作伙伴:用于启用安全应用程序模型的 Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [合作伙伴中心身份验证文档](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

如果你使用的是 "控制面板", 则需要咨询供应商以了解如何采用安全应用程序模型框架。

控制面板供应商需要作为控制面板供应商[加入](https://docs.microsoft.com/partner-center/enroll-as-cpv)合作伙伴中心, 并立即开始实现此要求。 请参阅合作伙伴中心: [保护应用程序模型](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)框架。 控制面板供应商必须接受并管理 CSP 合作伙伴的同意而不是凭据, 并清除所有现有的 CSP 合作伙伴的凭据。

### <a name="who-is-a-control-panel-vendor-cpv"></a>谁是控制面板供应商 (CPV)？ 
控制面板供应商是一个独立的软件供应商, 可开发供 CSP 合作伙伴用于集成合作伙伴中心 Api 的应用。 控制面板供应商不是可直接访问合作伙伴中心仪表板或 Api 的 CSP 合作伙伴。 可在[合作伙伴中心获取详细说明:安全应用程序模型](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)指南。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>安全应用程序模型是否只需要为合作伙伴中心 API/SDK 实现？ 

一旦启用 "*需要对管理员的 MFA* " 和 "*最终用户保护*" 基线策略, 每个用户都需要使用多重身份验证进行身份验证。 这意味着, 你将需要为每个 API、CLI 和 PowerShell 模块 (例如 Azure、Azure AD、MS Online、合作伙伴中心等) 实现安全的应用程序模型, 该模块旨在以非交互方式运行, 并依赖于用户凭据的使用来进行身份验证。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>我使用的是自动化工具, 如 PowerShell。 如何实现实现安全的应用程序模型？  

如果你的自动化旨在以非交互方式运行, 并依赖于用户凭据进行身份验证, 则你将需要实现安全的应用程序模型。 请参阅[安全应用程序模型 |合作伙伴中心 PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) , 指导如何实现此框架。  请注意, 并非所有自动化工具都提供使用访问令牌进行身份验证的功能。 如果需要帮助了解需要进行哪些更改, 请在[合作伙伴中心安全指南](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)组中发布一条消息。

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>在执行许可过程时, 应用程序管理员应提供哪些用户凭据？ 

建议使用已被分配了最低特权权限的服务帐户。 对于合作伙伴中心 API, 这意味着你应该使用已分配有 "销售代理" 或 "管理代理" 角色的帐户。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>为什么在执行许可过程时, 应用程序管理员应不提供全局管理员用户凭据？

最佳做法是尽可能使用最低特权标识, 因为这样可以降低风险。 不建议使用具有全局管理员权限的帐户, 因为这将提供比所需权限更多的权限

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>我是一个 CSP 合作伙伴。 如何实现知道我的控制面板供应商 (CPV) 是否正在实施解决方案？ 

对于使用控制面板供应商 (CPV) 解决方案来处理云解决方案提供商 (CSP) 计划的合作伙伴, 你有责任咨询你的 CPV。 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>我是一个 CPV。 如何实现注册？ 

若要注册为控制面板供应商 (CPV), 请按照[此处](https://docs.microsoft.com/partner-center/enroll-as-cpv)提供的指南进行操作。

若要接收注册链接, CPVs 必须联系[CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) , 并为 Microsoft 员工赞助商提供与 CPV 的业务关系或了解其业务。 例如, 合作伙伴开发经理 (PDM)。

在合作伙伴中心注册并注册应用程序后, 你将有权访问合作伙伴中心 Api。 如果你是新的 CPV, 则会通过合作伙伴中心通知收到你的沙盒信息。 完成注册为 Microsoft CPV 并接受 CPV 协议后, 可以:

1. 管理多租户应用程序 (将应用程序添加到 Azure 门户、在合作伙伴中心注册和取消注册应用程序)。 注意：CPVs 必须将其应用程序注册到合作伙伴中心, 才能获得合作伙伴中心 Api 的授权。 将应用程序单独添加到 Azure 门户不会为合作伙伴中心 Api 授权 CPV 应用程序。
2. 查看并管理你的 CPV 配置文件。
3. 查看并管理需要访问 CPV 功能的用户。 CPV 可以拥有的唯一角色是全局管理员。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>我使用的是合作伙伴中心 SDK。 SDK 会自动采用安全应用程序模型吗？ 

不需要, 你将需要遵循[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)中提供的指导原则。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>是否可以使用未启用 MFA 的帐户为安全应用程序模型生成刷新令牌？

是的, 可以使用未强制 MFA 的帐户生成刷新令牌。 但是, 不应执行此操作, 因为使用未启用 MFA 的帐户生成的任何令牌将无法访问资源, 因为需要进行 MFA。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>如果启用 MFA, 应用程序应该如何获取访问令牌？

你将需要遵循[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf), 其中提供了有关如何执行此操作的详细信息, 同时遵守新的安全要求。 可在[此处](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)找到 .net 示例代码和 [Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>作为 CPV, 我是否在 CPV 租户或 CSP 合作伙伴的租户中创建 Azure AD 应用程序？

CPV 需要在与注册为 CPV 的租户中创建 Azure Active Directory 应用程序。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>我是使用仅应用身份验证的 CSP。 是否需要进行任何更改？

仅限应用的身份验证不受影响, 因为未使用用户凭据来请求访问令牌。 如果共享用户凭据, 控制面板供应商 (CPVs) 必须采用[安全的应用程序模型框架](http://assetsprod.microsoft.com/secure-application-model-guide.pdf), 并清除任何现有的合作伙伴凭据。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV 可以使用仅限应用的身份验证样式来获取访问令牌？

否, 控制面板供应商合作伙伴无法利用仅限应用的身份验证样式来代表合作伙伴请求访问令牌。 它们应实现安全的应用程序模型, 该模型使用 "应用 + 用户身份验证" 样式。

## <a name="key-resources"></a>关键资源

### <a name="how-to-get-started"></a>如何开始

- [合作伙伴安全要求: 循序渐进指南](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- 将你的问题和反馈定向到此[合作伙伴中心安全指南组](https://aka.ms/MPCSecurityGuidance)。
- 参加未来的合作伙伴办公时间和网络研讨会。 请在[此处查看详细的计划和资源](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)。

### <a name="resources-for-enabling-mfa"></a>用于启用 MFA 的资源

- 了解[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)的概念。
- 请[参阅基准策略:要求对管理员](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)进行 mfa, 详细了解如何启用 "对管理员使用 mfa" 基准策略。
- 请[参阅基准策略:有关如何启用](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)最终用户保护基线策略的详细信息, 请最终用户保护。

### <a name="resources-for-adopting-secure-application-model"></a>采用安全应用程序模型的资源

- [安全应用程序模型概述](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心:安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP 计划中的合作伙伴: 用于启用安全应用程序模型的 .NET 示例代码](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [CSP 计划中的合作伙伴:用于启用安全应用程序模型的 Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [合作伙伴中心身份验证文档](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>支持

### <a name="where-can-i-ask-get-support"></a>在哪里可以请求获取支持？

此外, 若要支持使用资源来满足安全要求, 如果你具有对合作伙伴 (ASfP) 的高级支持, 请与你的服务帐户经理联系;对于合作伙伴协议 (PSfP) 的顶级支持, 请与你的服务客户经理和技术客户经理联系。

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>如何在启用基线策略时获得帮助？

- 合作伙伴可以利用 MPN 权益提供的建议时间获取更多有关如何实现安全要求的详细指导。
- Azure Active Directory 的技术产品支持选项可通过 MPN 权益获得。 有权访问活动的 ASfP 或 PSfP 协议的合作伙伴可以与其关联的客户经理 (SAM/TAM) 合作, 以最大程度地了解可用的选项。
- 可以通过[合作伙伴中心服务请求](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)访问合作伙伴中心的基准策略实现支持。 选择 " *MFA & 保护应用程序模型*作为主题。

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>如何实现获取技术信息以采用安全的应用程序模型框架？ 

Azure Active Directory 的技术产品支持选项可通过 MPN 权益获得。 有权访问 active ASfP 或 PSfP 订阅的合作伙伴可以与其关联的帐户管理器 (SAM/TAM) 一起使用, 以最大程度地了解可用的选项。

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>在哪里可以找到有关技术常见问题的详细信息？ 

可在[此处](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)找到有关技术常见问题的信息。
