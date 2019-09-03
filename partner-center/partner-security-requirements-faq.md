---
title: 合作伙伴安全要求常见问题解答 | 合作伙伴中心
ms.topic: article
ms.date: 08/23/2019
description: 关于合作伙伴安全要求的常见问题解答
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: 54ac919aeadec85b941e0dce9b1556df843e5fcb
ms.sourcegitcommit: 435634c55c3d20a42083c0a58d96c7f6b8ec0a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/26/2019
ms.locfileid: "70020537"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>关于合作伙伴安全要求的常见问题解答

本文包含[合作伙伴安全要求](partner-security-requirements.md)的一些常见问题解答。

## <a name="partner-security-requirements"></a>合作伙伴安全要求

### <a name="what-are-the-new-partner-security-requirements"></a>新的合作伙伴安全要求是什么？

为了保护我们的合作伙伴和你的客户，我们要求合作伙伴立即采取以下措施：  

1. **为合作伙伴租户中的所有用户启用多重身份验证 (MFA)** 。 在登录到 Microsoft 商业云服务时，或者通过合作伙伴中心或 API 在云解决方案提供商处进行交易时，合作伙伴租户中的所有用户必须使用多重身份验证 (MFA)。 启用基线保护策略以后，合作伙伴租户的所有用户就可以免费使用 MFA。

2. **采用安全应用程序模型框架**。 所有集成 Microsoft API（例如 Azure 资源管理器、Microsoft Graph、合作伙伴中心 API）的合作伙伴必须采用安全应用程序模型框架，以免在启用基线策略时对其集成造成中断。

启用多重身份验证 (MFA) 和采用安全应用程序模型框架将有助于保护你的基础结构与客户数据免受身份盗窃或其他欺诈事件等潜在安全风险的影响。  

### <a name="which-partners-need-to-meet-the-requirements"></a>哪些合作伙伴需要满足这些要求？

这些要求针对以下合作伙伴组：

- 参与云解决方案提供商 (CSP) 计划的所有合作伙伴组织，这些组织使用 Microsoft 商业云服务进行交易
  - 直接计费合作伙伴
  - 间接提供商
  - 间接经销商
- 所有控制面板供应商
- 所有顾问计划合作伙伴  

所有通过主权云（世纪互联、Microsoft Cloud for US Government、德国 Microsoft 云）进行交易的合作伙伴不是必须履行 8 月 1 日生效的新安全要求。 但是，我们强烈建议所有使用主权云的合作伙伴立即行动起来，履行这些新的安全要求。 Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。

### <a name="what-are-the-key-timelines-and-milestones"></a>关键的时间线和里程碑有哪些？

与这些安全要求相关的条款会立即添加到[云解决方案提供商计划指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)中。 参与云解决方案提供商计划时，若要合规，你必须履行 2019 年 8 月 1 日生效的这些安全要求。

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>如果我不采取任何措施，会发生什么情况？

一旦我们强制实施这些合作伙伴安全要求，未能遵循这些安全做法和义务要求的合作伙伴将不能在云解决方案提供商计划中进行交易，也不能利用委托管理权限来管理客户租户。 我们准备针对这些要求确定一个强制实施日期，并且会将该日期和相关详细信息告知合作伙伴。

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>如果我没有在 2019 年 8 月 1 日之前根据这个新的安全要求实施 MFA，会发生什么情况？

与[云解决方案提供商计划指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)中的这些安全要求相关的条款已经从 2019 年 8 月 1 日开始生效。 所有参与云解决方案提供商计划的合作伙伴都应按要求履行这些条款并保护其业务。 一旦我们在不远的将来开始严格地强制实施合作伙伴安全要求，不遵循这些安全做法的合作伙伴可能无法在云解决方案提供商计划中进行交易，也不能利用委托管理权限来管理客户租户。 我们会确定一个强制实施日期，很快就会将该日期告知合作伙伴。

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>为何 Microsoft 要强制实施这些新要求？

客户和合作伙伴的安全和隐私是 Microsoft 最优先关注的事情。 我们不断看到各种主要与身份泄露事件相关的安全攻击，其方法越来越复杂，其数量越来越多。 若要通过整体防御策略来阻止安全攻击，预防性的控制至关重要，因此我们将开始实施一系列强制性安全要求，以便对合作伙伴及其客户进行保护。

### <a name="does-this-apply-to-all-geographies"></a>这是否适用于所有地区？

是的，这适用于所有地区。 强烈建议所有通过主权云（世纪互联、Microsoft Cloud for US Government、德国 Microsoft 云）进行事务处理的合作伙伴立即行动起来，履行这些安全要求。 但是，这些合作伙伴不是必须满足这些新的在 8 月 1 日生效的安全要求。 Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>是否可以让某个帐户例外？

否，对于强制实施 MFA 这一要求，任何帐户都不能例外。 考虑到合作伙伴会有很高的特权，因此[云解决方案提供商计划指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)要求针对合作伙伴租户中的每个帐户强制实施 MFA。

## <a name="required-actions"></a>必需的措施

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>我需要采取哪些主要措施才能满足这些要求？

云解决方案提供商计划中的所有合作伙伴（直接计费合作伙伴、间接提供商和间接经销商）、顾问和控制面板供应商必须满足这些要求。

1. **对所有用户强制实施 MFA**

    云解决方案提供商计划中的所有合作伙伴、顾问和控制面板供应商必须针对其合作伙伴租户中的所有用户强制实施 MFA。 这可以通过启用[“对管理员要求 MFA”策略](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)、[“最终用户保护”基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)以及任何未来的基线策略来实现。 基线策略提供的功能会持续改进，确保合作伙伴和客户免受不断变化的安全威胁的危害。 因此，请参阅[基线策略文档](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)以了解详细信息，这很重要。

    - 请参阅[基线策略：对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，详细了解如何启用“对管理员要求 MFA”基线策略。
    - 请参阅[基线策略：最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)，详细了解如何启用“最终用户保护”基线策略。
    - 了解[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)的概念。

    其他注意事项：

    - 间接提供商若要加入合作伙伴中心（如果尚未加入），则需与间接经销商展开合作，并要求自己的经销商满足这些要求。
    - Azure MFA 通过基线策略免费提供给合作伙伴租户中的所有用户，唯一的验证方法是使用 [Microsoft Authenticator 应用](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。
    - 如果需要其他验证方法（例如短信或电子邮件），则可通过 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU 使用这些方法。
    - 在访问 Microsoft 商业云服务时，合作伙伴也可以针对每个用户使用第三方 MFA 解决方案。

2. **采用安全应用程序模型框架**

    所有使用任意 API（例如，Azure 资源管理器、Microsoft Graph、合作伙伴中心 API，等等）开发了自定义集成或使用 PowerShell 之类的工具实施了自定义自动化的合作伙伴必须采用[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)，以便集成 Microsoft 云服务。 否则可能会因 MFA 部署而造成中断。 以下资源提供有关如何采用此模型的概述和指南。

    - [安全应用程序模型概述](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [合作伙伴中心：安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 .NET 示例代码](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [合作伙伴中心身份验证文档](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    如果使用控制面板，则需与供应商协商采用安全应用程序模型框架的事宜。

    控制面板供应商必须以控制面板供应商身份[加入](https://docs.microsoft.com/partner-center/enroll-as-cpv)合作伙伴中心并立即开始实施此要求。 请参阅[合作伙伴中心：安全应用程序模型框架](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制面板供应商必须接受并管理云解决方案提供商合作伙伴的许可而非凭据，并清除所有现有的云解决方案提供商合作伙伴的凭据。

## <a name="multi-factor-authentication"></a>多重身份验证

### <a name="what-is-multi-factor-authentication-mfa"></a>什么是多重身份验证 (MFA)？

MFA 是一种安全机制，单个用户可以使用该机制通过多个必需的安全和验证过程进行身份验证。 该方法需要使用下列身份验证方式中的两种或更多种来发挥作用：

- 您知道的信息（通常为密码）
- 您拥有的东西（不易被复制的受信任设备，如电话）
- 您的特征（生物识别）

### <a name="what-are-baseline-protection-policies"></a>什么是基线保护策略？

[Microsoft 基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)（目前为预览版）是一组预定义的策略，可帮助组织防范许多常见攻击。 这些常见攻击可能包括密码喷射、重播和钓鱼。 基线策略在所有版本的 Azure Active Directory 中提供。 Microsoft 会将这些基线保护策略提供给所有人，因为基于身份的攻击在过去几年呈上升趋势。 这些策略的目标是确保所有组织在不额外付费的情况下可以启用基本的安全措施。

> [!NOTE]
> Microsoft 基线策略和相关的功能会持续改进，更好地保护合作伙伴和客户免受不断变化的安全威胁的危害。 可能很快会对基线策略进行一些命名和分类更改。 强烈建议你直接访问基线策略页，以便查看最新信息。

### <a name="what-baseline-policies-must-i-enable"></a>必须启用哪些基线策略？

如果打算利用当前的基线保护策略为合作伙伴租户中的每个用户提供 MFA，则必须启用[对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线策略。 这些基线保护策略会为合作伙伴租户中的每个用户免费履行 MFA 要求，前提是合作伙伴通过移动设备使用 Microsoft Authenticator 应用。

[“对管理员要求 MFA”基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)用于保护合作伙伴目录中的管理用户，[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线策略用于保护合作伙伴租户中的非管理用户。 若要启用这些策略，用户必须注册 MFA。 用户成功注册以后，系统会在用户尝试登录时根据策略要求提示用户进行 MFA。 基线策略提供的功能会持续改进，确保合作伙伴和客户免受不断变化的安全威胁的危害。 因此，请参阅[基线策略文档](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)以了解详细信息，这很重要。

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>如何启用“对管理员要求 MFA”策略？

可以通过 Azure 管理门户启用“对管理员要求 MFA”基线策略。 请参阅[基线策略：对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，详细了解如何启用此基线策略。

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>如何启用“最终用户保护”策略？

可以通过 Azure 管理门户启用“最终用户保护”基线策略。 请参阅[基线策略：最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)，详细了解如何启用此基线策略。

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>是否会自动启用基线策略？

否。若要启用这些策略，属于全局管理员、安全管理员或条件访问管理员角色成员的用户需要将策略配置为“立即使用策略”。

### <a name="what-is-the-cost-of-enabling-mfa"></a>启用 MFA 的费用是多少？

Microsoft 允许用户实施[对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略，以这种方式免费提供 MFA。 通过此版 MFA 提供的唯一验证选项是 [Microsoft Authenticator 应用](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。 如果需要电话呼叫或短信，则需购买 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 许可证。 也可利用第三方解决方案为合作伙伴租户中的每个用户提供 MFA – 在这种情况下，你必须负责确保强制实施 MFA 解决方案而且你符合相关规范。

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>如果已经有了 MFA 解决方案，我需要采取什么措施？

根据这些安全要求，合作伙伴租户中的用户在访问 Microsoft 商业云服务时必须使用 MFA 进行身份验证。 可以使用第三方解决方案来履行这些要求。 Microsoft 不再向独立的标识提供者提供是否符合 Azure Active Directory 的验证测试。 若要测试产品的互操作性，请参阅这些[准则](https://www.microsoft.com/download/details.aspx?id=56843)。

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>我可以使用什么验证方法进行 MFA？

Microsoft 允许用户实施[对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略，以这种方式免费提供 MFA。 通过此版 MFA 提供的唯一验证选项是 [Microsoft Authenticator 应用](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。 如果需要电话呼叫或短信，则需购买 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 许可证。 也可利用第三方解决方案为合作伙伴租户中的每个用户提供 MFA – 在这种情况下，你必须负责确保强制实施 MFA 解决方案而且你符合相关规范。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>我使用多个合作伙伴租户进行交易。 我是否需要对其都进行 MFA？

是的，需要对每个与云解决方案提供商计划或顾问计划相关联的 Azure Active Directory 租户强制实施 MFA。 如果打算购买 Azure Active Directory Premium 许可证，则必须为每个 Azure Active Directory 租户中的用户购买一个许可证。

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>是否需要为合作伙伴租户中的每个用户强制实施 MFA？*

[对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略将为合作伙伴租户中的每个用户强制实施 MFA。 如果利用这些策略来提供 MFA，并且使用的是 [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) 应用程序，则不需购买任何其他的许可证， 而只需购买适当的解决方案，为合作伙伴租户中的每个用户提供 MFA 即可。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>我是 Microsoft 的直接计费合作伙伴。 我需要做些什么？

直接计费云解决方案提供商合作伙伴必须为其合作伙伴租户中的每个用户强制实施 MFA。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>我是间接经销商，只通过分销商进行交易。 我是否仍然需要这样做？

所有间接经销商都必须为其合作伙伴租户中的每个用户强制实施 MFA。 这是间接经销商必须执行的操作。

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>我不使用合作伙伴中心 API。 我是否仍然需要进行 MFA？

是的，此安全要求针对所有用户，包括合作伙伴租户中的合作伙伴管理员用户和最终用户。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>哪些第三方供应商提供与 Azure Active Directory 兼容的 MFA 解决方案？

有许多 MFA 解决方案线上独立调查报告，例如 [Gartner](https://www.gartner.com/en/webinars/3881781) 报告。 评审 MFA 供应商和解决方案时，合作伙伴必须确保所选解决方案兼容 Azure Active Directory。

Microsoft 不再向独立的标识提供者提供是否符合 Azure Active Directory 的验证测试。 若要测试产品的互操作性，请参阅这些[准则](https://www.microsoft.com/download/details.aspx?id=56843)。

有关详细信息，请参阅 [Azure AD 联合身份验证兼容性列表](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>如何在集成沙盒中测试 MFA？

应该为集成沙盒租户启用[对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 和[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略。 启用此策略以后，租户中的每个用户就必须使用 MFA 进行身份验证。

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>启用 MFA 是否会影响我与客户的租户交互？

否。 履行这些安全要求不会影响你管理客户。 你执行委派管理操作的权限不会受影响。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>我的客户是否需遵循合作伙伴安全要求？

否。不是必须为客户的 Azure AD 租户中的每个用户强制实施 MFA。 不过，建议你与每个客户协商确定如何才能最好地保护其用户。

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>是否可以将应用密码与基线保护策略配合使用？

是的，[应用密码](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)可以这样使用。 你应该查看[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)记录的应用密码使用注意事项，确定应用密码是否符合你的需求。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>是否有用户可以不遵守此要求？

否。合作伙伴租户中的每个用户（包括服务帐户）都必须使用 MFA 进行身份验证。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>合作伙伴安全要求是否适用于集成沙盒？

是的，合作伙伴安全要求适用于集成沙盒。 这意味着，你需要为集成沙盒租户中的用户实施适当的 MFA 解决方案。 建议实施提供 MFA 所需的基线保护策略。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>如何配置紧急访问（不受限）帐户？

最佳做法是创建一两个紧急访问帐户，防止自己被意外锁定在 Azure AD 租户外面。 根据合作伙伴安全要求，每个用户都必须使用 MFA 进行身份验证。 因此，这意味着你需要修改紧急访问帐户的定义。 它可以是利用第三方解决方案进行 MFA 的帐户。

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>合作伙伴安全要求对来宾用户的影响如何？

来宾用户在访问合作伙伴租户中的资源时，必须使用 MFA 进行身份验证。 当来宾用户访问自己租户中的资源时，合作伙伴安全要求对其没有影响。

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>如果我使用第三方解决方案，是否必须使用 Active Directory 联合身份验证服务 (ADFS)？

否。如果你使用第三方解决方案，Active Directory 联合身份验证服务 (ADFS) 不是必需的。 建议你与解决方案供应商协商，确定其解决方案的要求。

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>是否必须启用基线保护策略？

否。不一定要启用基线保护策略。 唯一要求是为合作伙伴租户中的每个用户（包括服务帐户）强制实施 MFA。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>是否可以使用条件访问来满足 MFA 要求？

是的，可以使用条件访问为合作伙伴租户中的每个用户（包括服务帐户）强制实施 MFA。 但是，考虑到合作伙伴会有很高的特权，因此我们需要确保在每位用户每次进行身份验证时都对其进行 MFA 质询。 这意味着，你将无法使用条件访问的那些规避 MFA 要求的功能。

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>哪些验证选项是通过实施基线保护策略提供的？

至于实施基线保护策略时可以使用的 MFA 版本，我们只能说，唯一可用的验证选项是一个验证器应用。 使用电话呼叫和短信不太安全。 因此，此版 MFA 不提供这些选项。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect 使用的服务帐户是否会受合作伙伴安全要求的影响？

否。Azure AD Connect 使用的服务帐户不会受合作伙伴安全要求的影响。 如果你在强制实施 MFA 时遇到 Azure AD Connect 问题，则请向 Microsoft 支持部门提交技术支持请求。

## <a name="secure-application-model"></a>安全应用程序模型

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>谁应该采用安全应用程序模型来满足这些要求？

Microsoft 引入了一个安全且可缩放的框架，用于对使用多重身份验证的云解决方案提供商 (CSP) 合作伙伴和控制面板供应商 (CPV) 进行身份验证。 有关详细信息，请参阅[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 所有使用任意 API（例如，Azure 资源管理器、Microsoft Graph、合作伙伴中心 API，等等）开发了自定义集成或使用 PowerShell 之类的工具实施了自定义自动化的合作伙伴必须采用[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)，以便集成 Microsoft 云服务。

### <a name="what-is-the-secure-application-model"></a>安全应用程序模型是什么？

Microsoft 引入了一个安全且可缩放的框架，用于对使用多重身份验证的云解决方案提供商 (CSP) 合作伙伴和控制面板供应商 (CPV) 进行身份验证。 有关详细信息，请参阅[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。  

### <a name="how-do-i-implement-the-secure-application-model"></a>如何实现安全应用程序模型？

所有使用任意 API（例如，Azure 资源管理器、Microsoft Graph、合作伙伴中心 API，等等）开发了自定义集成或使用 PowerShell 之类的工具实施了自定义自动化的合作伙伴必须采用[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)，以便集成 Microsoft 云服务。 否则可能会因 MFA 部署而造成中断。 以下资源提供有关如何采用此模型的概述和指南。

- [安全应用程序模型概述](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心：安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 .NET 示例代码](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [合作伙伴中心身份验证文档](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

如果使用控制面板，则需与供应商协商采用安全应用程序模型框架的事宜。

控制面板供应商必须以控制面板供应商身份[加入](https://docs.microsoft.com/partner-center/enroll-as-cpv)合作伙伴中心并立即开始实施此要求。 请参阅[合作伙伴中心：安全应用程序模型框架](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制面板供应商必须接受并管理云解决方案提供商合作伙伴的许可而非凭据，并清除所有现有的云解决方案提供商合作伙伴的凭据。

### <a name="who-is-a-control-panel-vendor-cpv"></a>谁是控制面板供应商 (CPV)？

控制面板供应商是独立软件供应商，其开发的应用可供云解决方案提供商合作伙伴用来与合作伙伴中心 API 集成。 控制面板供应商不是可以直接访问合作伙伴中心仪表板或 API 的云解决方案提供商合作伙伴。 详细说明在[合作伙伴中心：安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)中提供。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>是否只需为合作伙伴中心 API/SDK 实现安全应用程序模型？

启用“对管理员要求 MFA”  和“最终用户保护”  基线保护策略以后，每位用户都必须使用多重身份验证进行身份验证。 这意味着，你需要针对每个旨在以非交互方式运行并且依赖于使用用户凭据进行身份验证的 API、CLI 和 PowerShell 模块（例如，Azure、Azure AD、MS Online、合作伙伴中心，等等）实现安全应用程序模型。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>我使用 PowerShell 之类的自动化工具。 如何实现安全应用程序模型？

如果自动化旨在以非交互方式运行并且依赖于用户凭据进行身份验证，则需实现安全应用程序模型。 请参阅[安全应用程序模型 | 合作伙伴中心 PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5)，获取有关如何实现此框架的指南。  请注意，并非所有自动化工具都提供使用访问令牌进行身份验证的功能。 如果不了解需要进行哪些更改，请在[合作伙伴中心安全指南](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)组发布消息。

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>执行许可过程时，应用程序管理员应该提供哪些用户凭据？

建议使用一个所分配的特权最少的服务帐户。 就合作伙伴中心 API 来说，这意味着，你应该使用一个分配了“销售代理”或“管理员代理”角色的帐户。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>为何应用程序管理员在执行许可过程时不应该提供全局管理员用户凭据？

最佳做法是使用最低特权标识，这样可以降低风险。 建议不要使用具有全局管理员特权的帐户，因为这样一来，提供的权限会超出需要。

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>我是云解决方案提供商合作伙伴。 我如何才能知道我的控制面板供应商 (CPV) 是否正在实现解决方案？

作为使用控制面板供应商 (CPV) 解决方案在云解决方案提供商 (CSP) 计划中交易的合作伙伴，你有责任咨询你的 CPV。

### <a name="i-am-a-cpv-how-do-i-enroll"></a>我是 CPV。 如何注册？

若要注册为控制面板供应商 (CPV)，请按[此处](https://docs.microsoft.com/partner-center/enroll-as-cpv)提供的指南操作。

CPV 必须与 [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) 联系并提供一位与 CPV 有业务关系或了解其业务的 Microsoft 员工赞助商，然后才能收到注册链接。 例如，合作伙伴开发经理 (PDM)。

加入合作伙伴中心并注册应用程序以后，即可访问合作伙伴中心 API。 如果你是新 CPV，则可通过合作伙伴中心通知接收沙盒信息。 注册为 Microsoft CPV 并接受 CPV 协议以后，即可执行以下操作：

1. 管理多租户应用程序（向 Azure 门户添加应用程序、在合作伙伴中心注册和取消注册应用程序）。 注意：CPV 必须在合作伙伴中心注册其应用程序，然后才会获得使用合作伙伴中心 API 的授权。 只是将应用程序添加到 Azure 门户并不会为 CPV 应用程序授予使用合作伙伴中心 API 的权限。
2. 查看和管理 CPV 配置文件。
3. 查看和管理需访问 CPV 功能的用户。 CPV 可以有的唯一角色是全局管理员。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>我使用合作伙伴中心 SDK。 SDK 是否会自动采用安全应用程序模型？

否。你需要按[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)中提供的指南操作。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>对于有帐户未启用 MFA 的安全应用程序模型，我是否可以生成一个刷新令牌？

是的，可以使用未强制实施 MFA 的帐户来生成刷新令牌。 但是，你不应该这样做，因为使用未启用 MFA 的帐户生成的任何令牌都无法访问资源，这是 MFA 的要求。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>如果我们启用 MFA，我的应用程序应该如何获取访问令牌？

你需要按照[安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)操作，该指南详述了如何在遵循新安全要求的同时这样做。 可以在[此处](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)找到 .NET 示例代码，在[此处](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)找到 Java 示例代码。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>作为 CPV，我是在 CPV 租户中还是在云解决方案提供商合作伙伴租户中创建 Azure AD 应用程序？

CPV 需在与其注册（以 CPV 身份）相关联的租户中创建 Azure Active Directory 应用程序。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>我是使用“仅应用”身份验证的云解决方案提供商。 我是否需要进行任何更改？

“仅应用”身份验证不受影响，因为用户凭据不用于请求访问令牌。 如果用户凭据是共享的，则控制面板供应商 (CPV) 必须采用[安全应用程序模型框架](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)并清除他们现有的任何合作伙伴凭据。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>作为 CPV，我是否可以利用“仅应用”身份验证模式来获取访问令牌？

否，控制面板供应商合作伙伴不能利用“仅应用”身份验证模式代表合作伙伴来请求访问令牌。 他们应该实现安全应用程序模型，以便利用“应用 + 用户”身份验证模式。

## <a name="key-resources"></a>重要资源

### <a name="how-to-get-started"></a>如何开始使用

- [合作伙伴安全要求：分步指南](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- 请将你的问题和反馈发布到此[合作伙伴中心安全指南组](https://aka.ms/MPCSecurityGuidance)。
- 参加即将召开的 Partner Office Hours 和网络研讨会。 请[在此处查看详细的计划和资源](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)。

### <a name="resources-for-enabling-mfa"></a>启用 MFA 的资源

- 了解[基线保护策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)的概念。
- 请参阅[基线策略：对管理员要求 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，详细了解如何启用“对管理员要求 MFA”基线策略。
- 请参阅[基线策略：最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)，详细了解如何启用“最终用户保护”基线策略。

### <a name="resources-for-adopting-secure-application-model"></a>采用安全应用程序模型的资源

- [安全应用程序模型概述](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心：安全应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 .NET 示例代码](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 Java 示例代码](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [合作伙伴中心身份验证文档](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>支持

### <a name="where-can-i-get-support"></a>我可以在哪里获得支持？

如需获得满足安全要求的支持资源，而且你有合作伙伴高级支持 (ASfP)，请联系服务帐户管理员；如需获得合作伙伴协议高级支持 (PSfP)，请联系服务帐户管理员和技术帐户管理员。

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>我如何获得基线策略启用方面的帮助？

- 合作伙伴可以利用 MPN 权益的咨询时间获取有关如何实施安全要求的更详细指南。
- 可以通过 MPN 权益获取 Azure Active Directory 的技术产品支持选项。 能够访问活动 ASfP 或 PSfP 协议的合作伙伴可以咨询相关的帐户管理员 (SAM/TAM)，这样可以最好地了解可用选项。
- 可以通过[合作伙伴中心服务请求](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)访问合作伙伴中心的基线策略实施支持。 选择“MFA 和安全应用程序模型”作为主题。 

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>如何获取有助于我采用安全应用程序模型框架的技术信息和支持？

可以通过 MPN 权益获取 Azure Active Directory 的技术产品支持选项。 能够访问活动 ASfP 或 PSfP 订阅的合作伙伴可以咨询相关的帐户管理员 (SAM/TAM)，这样可以最好地了解可用选项。

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>在哪里可以找到常见技术问题的详细信息？

可以在[此处](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)找到常见技术问题的信息。
