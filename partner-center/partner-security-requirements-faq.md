---
title: 合作伙伴安全要求常见问题解答
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 关于合作伙伴安全要求的常见问题，例如具体有哪些要求、合作伙伴应如何实施这些要求，以及你如何知道自己是否满足这些要求。
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f60b6e2624bd4f9020181a936842bdb46db8aa9
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133042"
---
# <a name="common-questions-about-partner-security-requirements"></a>合作伙伴安全要求的常见问题

**适用于**

- 合作伙伴中心

**相应的用户**

- 所有支持的用户，包括来宾用户


本文回答了有关[合作伙伴安全要求](partner-security-requirements.md)的一些常见问题。

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>什么是合作伙伴安全要求？合作伙伴为什么应实施它们？

提供更大力度的持续性安全和隐私保护是我们的首要任务，并且我们会继续帮助合作伙伴保护他们的客户和租户。 我们不断看到各种主要与身份泄露事件相关的安全攻击，其方法越来越复杂，其数量越来越多。 为了通过整体防御策略来阻止安全攻击，预防性的控制至关重要，因此我们于 2019 年引入了[强制性安全要求](partner-security-requirements.md)。 参与云解决方案提供商 (CSP) 计划的所有合作伙伴、控制面板供应商和顾问必须实施这些要求以保持合规性。

### <a name="what-are-the-key-timelines-and-milestones"></a>关键的时间线和里程碑有哪些？

与这些安全要求相关的条款（包括时间线和里程碑）已包含在 [Microsoft 合作伙伴协议](microsoft-partner-agreement.md)中。 为了保持参与 CSP 计划的合规性，你将需要尽快实施这些安全要求。

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>如果我没有实施这些合作伙伴安全要求会发生什么情况？

Microsoft 合作伙伴协议要求你为用户帐户强制实施多重身份验证，并采用安全应用程序模型与合作伙伴中心 API 交互。 

不遵循这些安全做法的合作伙伴可能无法在 CSP 计划中进行交易，也不能使用委托管理权限来管理客户租户。

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>安全要求是否适用于所有地理区域？

是，安全要求适用于所有地理区域。 强烈建议所有通过主权云（Microsoft Cloud for US Government、德国 Microsoft 云）处理事务的合作伙伴立即行动起来，履行这些安全要求。 但是，这些合作伙伴目前并不需要满足这些安全要求。 Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>是否可以让某个帐户例外？

否，对于强制实施多重身份验证 (MFA) 这一要求，任何用户帐户都不能例外。 考虑到合作伙伴会有很高的特权，因此 Microsoft 合作伙伴协议要求针对合作伙伴租户中的每个用户帐户强制实施多重身份验证。

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>如何才能知道自己是否满足合作伙伴安全要求？

你需要完成以下步骤：

- 你需要满足[合作伙伴安全要求](partner-security-requirements.md)中列出的所有要求。
- 需要确保合作伙伴租户中的所有用户帐户都已实施多重身份验证。

为了帮助确定你可以采取行动的关键领域，我们提供了[安全要求状态报告](https://partner.microsoft.com/commerce/security/compliance)，该报告可通过合作伙伴中心获得。

有关状态报告的详细信息，请参阅[合作伙伴安全要求状态](partner-security-compliance.md)。

## <a name="required-actions"></a>必需的措施

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>我需要采取哪些主要措施才能满足这些要求？

CSP 计划中的所有合作伙伴（直接计费合作伙伴、间接提供商和间接经销商）、顾问和控制面板供应商必须满足这些要求。

1. **对所有用户强制实施 MFA**

    云解决方案提供商计划中的所有合作伙伴、顾问和控制面板供应商必须针对其合作伙伴租户中的所有用户强制实施 MFA。

    其他注意事项：

    - 间接提供商若要加入合作伙伴中心（如果尚未加入），则需与间接经销商展开合作，并要求自己的经销商满足这些要求。
    - Azure MFA 是通过 Azure AD 安全默认设置免费提供给合作伙伴租户中所有用户的，唯一的验证方法是使用支持基于时间的一次性密码 (TOTP) 的身份验证器应用程序。
    - 如果需要其他验证方法（例如电话呼叫或短信），可以通过 [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU 使用这些方法。
    - 在访问 Microsoft 商业云服务时，合作伙伴也可以对每个帐户使用第三方 MFA 解决方案。

2. **采用安全应用程序模型框架**

    所有使用任意 API（例如，Azure 资源管理器、Microsoft Graph、合作伙伴中心 API，等等）开发了自定义集成或使用 PowerShell 之类的工具实施了自定义自动化的合作伙伴必须采用[安全应用程序模型框架](/partner-center/develop/enable-secure-app-model)，以便集成 Microsoft 云服务。 否则可能会因 MFA 部署而造成中断。 以下资源提供有关如何采用此模型的概述和指南。

    - [安全应用程序模型概述](/partner-center/develop/enable-secure-app-model)
    - [合作伙伴中心：安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 .NET 示例代码](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 Java 示例代码](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [合作伙伴中心身份验证文档](/partner-center/develop/partner-center-authentication)
    - [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](/powershell/partnercenter/multi-factor-auth)

    如果你使用的是控制面板，请与供应商协商采用安全应用程序模型框架的事宜。

    控制面板供应商必须以控制面板供应商身份[加入](enroll-as-cpv.md)合作伙伴中心并立即开始实施此要求。 请参阅[合作伙伴中心：安全应用程序模型框架](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制面板供应商必须接受并管理云解决方案提供商合作伙伴的许可而非凭据，并清除所有现有的云解决方案提供商合作伙伴的凭据。

## <a name="multi-factor-authentication"></a>多重身份验证

### <a name="what-is-multi-factor-authentication-mfa"></a>什么是多重身份验证 (MFA)？

MFA 是一种安全机制，单个用户可以使用该机制通过多个必需的安全和验证过程进行身份验证。 该方法需要使用下列身份验证方式中的两种或更多种来发挥作用：

- 您知道的信息（通常为密码）
- 用户具有的某样东西（无法轻易复制的可信设备，如电话）
- 自身的特征（生物辨识系统）

### <a name="what-is-the-cost-of-enabling-mfa"></a>启用 MFA 的费用是多少？

Microsoft 允许用户实施 Azure AD 安全性默认设置，以这种方式免费提供 MFA。 通过此版 MFA 提供的唯一验证选项是身份验证器应用程序。 如果需要电话呼叫或短信，则需购买 [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) 许可证。 也可利用第三方解决方案为你合作伙伴租户中的每名用户提供 MFA - 在这种情况下，你需要负责确保强制实施 MFA 解决方案并且确保你是合规的。

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>如果已经有了 MFA 解决方案，我需要采取什么措施？

根据这些安全要求，合作伙伴租户中的用户在访问 Microsoft 商业云服务时必须使用 MFA 进行身份验证。 可以使用第三方解决方案来履行这些要求。 Microsoft 不再向独立的标识提供者提供是否符合 Azure Active Directory 的验证测试。 若要测试产品的互操作性，请参阅这些[准则](https://www.microsoft.com/download/details.aspx?id=56843)。

> [!IMPORTANT]
> 如果使用的是第三方解决方案，请务必验证该解决方案是否会发出包含 MFA 值的身份验证方法引用 (AMR) 声明。 若要详细了解如何验证第三方解决方案是否发出所需的声明，请参阅[测试合作伙伴安全要求](/powershell/partnercenter/test-partner-security-requirements)。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>我使用多个合作伙伴租户进行交易。 我是否需要对其都进行 MFA？

是的，你需要对每个与 CSP 计划或顾问计划相关联的 Azure Active Directory 租户强制实施 MFA。 若要购买 Azure Active Directory Premium 许可证，则必须为每个 Azure Active Directory 租户中的用户购买一个 Azure Active Directory 许可证。 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>是否需要为合作伙伴租户中的每个用户帐户强制实施 MFA？

是的，每个用户都需要强制实施 MFA。 但是，如果你使用的是 Azure AD 安全默认设置，则不需执行任何其他操作，因为该功能为所有用户帐户强制实施 MFA。 启用安全默认设置是一种用于确保用户帐户符合 MFA 要求的免费且简单的方式，并且在强制实施 MFA 后不会受影响。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>我是 Microsoft 的直接计费合作伙伴。 我需要做些什么？

直接计费云解决方案提供商合作伙伴必须为其合作伙伴租户中的每个用户强制实施 MFA。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>我是间接经销商，只通过分销商进行交易。 我是否仍然需要启用 MFA？

所有间接经销商都必须为其合作伙伴租户中的每个用户强制实施 MFA。 间接经销商必须启用 MFA。

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>我不使用合作伙伴中心 API。 我是否仍然需要进行 MFA？

是的，此安全要求针对所有用户，包括合作伙伴租户中的合作伙伴管理员用户和最终用户。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>哪些第三方供应商提供与 Azure Active Directory 兼容的 MFA 解决方案？

评审 MFA 供应商和解决方案时，合作伙伴必须确保所选解决方案兼容 Azure Active Directory。

Microsoft 不再向独立的标识提供者提供是否符合 Azure Active Directory 的验证测试。 若要测试产品的互操作性，请参阅这些[准则](https://www.microsoft.com/download/details.aspx?id=56843)。

有关详细信息，请参阅 [Azure AD 联合身份验证兼容性列表](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>如何在集成沙盒中测试 MFA？

应该启用 Azure AD 安全性默认设置功能，也可利用某个使用联合身份验证的第三方解决方案。

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>启用 MFA 是否会影响我与客户的租户交互？

不能。 履行这些安全要求不会影响你管理客户。 你执行委派管理操作的权限不会受影响。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>我的客户是否需遵循合作伙伴安全要求？

否。不是必须为客户的 Azure AD 租户中的每个用户强制实施 MFA。 不过，建议你与每个客户协商确定如何才能最好地保护其用户。

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>是否有用户可以不遵守 MFA 要求？

否。合作伙伴租户中的每个用户（包括服务帐户）都必须使用 MFA 进行身份验证。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>合作伙伴安全要求是否适用于集成沙盒？

是的，合作伙伴安全要求适用于集成沙盒。 这意味着，你需要为集成沙盒租户中的用户实施适当的 MFA 解决方案。 建议实施提供 MFA 所需的 Azure AD 安全性默认设置。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>如何配置紧急访问（不受限）帐户？

最佳做法是创建一两个紧急访问帐户，防止自己被意外锁定在 Azure AD 租户外。 根据合作伙伴安全要求，每个用户都必须使用 MFA 进行身份验证。 此要求意味着你需要修改紧急访问帐户的定义。 它可以是利用第三方解决方案进行 MFA 的帐户。

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>如果我使用第三方解决方案，是否必须使用 Active Directory 联合身份验证服务 (ADFS)？

否。如果你使用第三方解决方案，Active Directory 联合身份验证服务 (ADFS) 则不是必需的。 建议你与解决方案供应商协商，确定其解决方案的要求。

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>是否必须启用 Azure AD 安全性默认设置？

否，不是必须启用 Azure AD 安全性默认设置。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>是否可以使用条件访问来满足 MFA 要求？

是的，可以使用条件访问为合作伙伴租户中的每个用户（包括服务帐户）强制实施 MFA。 但是，考虑到合作伙伴会有很高的特权，因此我们需要确保在每位用户每次进行身份验证时都对其进行 MFA 质询。 这意味着，如果条件访问的某些功能需要规避 MFA 要求，你就无法使用它们。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect 使用的服务帐户是否会受合作伙伴安全要求的影响？

否。Azure AD Connect 使用的服务帐户不会受合作伙伴安全要求的影响。 如果你在强制实施 MFA 时遇到 Azure AD Connect 问题，则请向 Microsoft 支持部门提交技术支持请求。

## <a name="secure-application-model"></a>安全应用程序模型

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>谁应该采用安全应用程序模型来满足这些要求？

Microsoft 引入了一个安全且可缩放的框架，用于对使用多重身份验证的云解决方案提供商 (CSP) 合作伙伴和控制面板供应商 (CPV) 进行身份验证。 有关详细信息，请参阅[安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 所有使用任意 API（例如，Azure 资源管理器、Microsoft Graph、合作伙伴中心 API，等等）开发了自定义集成或使用 PowerShell 之类的工具实施了自定义自动化的合作伙伴必须采用[安全应用程序模型框架](/partner-center/develop/enable-secure-app-model)，以便集成 Microsoft 云服务。

### <a name="what-is-the-secure-application-model"></a>安全应用程序模型是什么？

Microsoft 引入了一个安全且可缩放的框架，用于对使用多重身份验证的云解决方案提供商 (CSP) 合作伙伴和控制面板供应商 (CPV) 进行身份验证。 有关详细信息，请参阅[安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。  

### <a name="how-do-i-implement-the-secure-application-model"></a>如何实现安全应用程序模型？

所有使用任意 API（例如，Azure 资源管理器、Microsoft Graph、合作伙伴中心 API，等等）开发了自定义集成或使用 PowerShell 之类的工具实施了自定义自动化的合作伙伴必须采用[安全应用程序模型框架](/partner-center/develop/enable-secure-app-model)，以便集成 Microsoft 云服务。 否则可能会因 MFA 部署而造成中断。 以下资源提供有关如何采用此模型的概述和指南。

- [安全应用程序模型概述](/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心：安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 .NET 示例代码](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 Java 示例代码](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [合作伙伴中心身份验证文档](/partner-center/develop/partner-center-authentication)
- [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](/powershell/partnercenter/multi-factor-auth)

如果你使用的是控制面板，则需与供应商协商采用安全应用程序模型框架的事宜。

控制面板供应商必须以控制面板供应商身份[加入](enroll-as-cpv.md)合作伙伴中心并立即开始实施此要求。 请参阅[合作伙伴中心：安全应用程序模型框架](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制面板供应商必须接受并管理云解决方案提供商合作伙伴的许可而非凭据，并清除所有现有的云解决方案提供商合作伙伴的凭据。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>是否只需为合作伙伴中心 API/SDK 实现安全应用程序模型？

对所有用户帐户强制实施多重身份验证会影响任何旨在以非交互方式运行的自动化或集成。 虽然根据合作伙伴安全要求，必须为合作伙伴中心 API 启用安全应用程序模型，但可以利用它来解决对自动化和集成进行双重身份验证的需求。

>[!Note] 
>被访问的资源需要支持基于访问令牌的身份验证。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>我使用 PowerShell 之类的自动化工具。 如何实现安全应用程序模型？

如果你的自动化旨在以非交互方式运行并且依赖于用户凭据进行身份验证，则需实现安全应用程序模型。 请参阅[安全应用程序模型 | 合作伙伴中心 PowerShell](/powershell/partnercenter/multi-factor-auth)，获取有关如何实现此框架的指南。  

>[!Note] 
>并非所有自动化工具都提供使用访问令牌进行身份验证的功能。 如果不了解需要进行哪些更改，请在[合作伙伴中心安全指南](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)组中发布消息。 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>执行许可过程时，应用程序管理员应该提供哪些用户凭据？

建议使用一个所分配的特权最少的服务帐户。 就合作伙伴中心 API 来说，你应该使用分配有“销售代理”或“管理员代理”角色的帐户。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>为何应用程序管理员在执行许可过程时不应该提供全局管理员用户凭据？

最佳做法是使用最低权限的标识。  这会降低风险。 建议不要使用具有全局管理员特权的帐户，因为这样会使提供的权限超出所需的权限。

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>我是云解决方案提供商合作伙伴。 我如何才能知道我的控制面板供应商 (CPV) 是否正在实现解决方案？

作为使用控制面板供应商 (CPV) 解决方案在云解决方案提供商 (CSP) 计划中交易的合作伙伴，你有责任咨询你的 CPV。

### <a name="who-is-a-control-panel-vendor-cpv"></a>谁是控制面板供应商 (CPV)？

控制面板供应商是独立软件供应商，其开发的应用可供云解决方案提供商合作伙伴用来与合作伙伴中心 API 集成。 控制面板供应商不是可以直接访问合作伙伴中心面板或 API 的 CSP 合作伙伴。 详细说明在[合作伙伴中心：安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)中提供。

### <a name="i-am-a-cpv-how-do-i-enroll"></a>我是 CPV。 如何注册？

若要注册为控制面板供应商 (CPV)，请按[此处](enroll-as-cpv.md)提供的指南操作。

CPV 必须与 [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) 联系才能收到注册链接，并需要提供一位与 CPV 有业务关系或了解其业务的 Microsoft 员工发起人。 例如，合作伙伴开发经理 (PDM)。

加入合作伙伴中心并注册应用程序以后即可访问合作伙伴中心 API。 如果你是新的 CPV，则将通过合作伙伴中心通知接收沙盒信息。 注册为 Microsoft CPV 并接受 CPV 协议以后，即可执行以下操作：

1. 管理多租户应用程序（向 Azure 门户添加应用程序、在合作伙伴中心注册和取消注册应用程序）。

   >[!Note]
   >CPV 必须在合作伙伴中心注册其应用程序，然后才会获得使用合作伙伴中心 API 的授权。 只是将应用程序添加到 Azure 门户并不会为 CPV 应用程序授予使用合作伙伴中心 API 的权限。

1. 查看和管理 CPV 配置文件。

1. 查看和管理需访问 CPV 功能的用户。 CPV 只能具有“全局管理员”角色。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>我使用合作伙伴中心 SDK。 SDK 是否会自动采用安全应用程序模型？

否。你需要按[安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)中提供的指南操作。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>对于有未启用 MFA 的帐户的安全应用程序模型，我是否可以生成一个刷新令牌？

是的，可以使用未强制实施 MFA 的帐户来生成刷新令牌。 但是，你不应该这样做， 因为使用未启用 MFA 的帐户生成的任何令牌都无法访问资源，这是 MFA 的要求。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>如果我们启用 MFA，我的应用程序应该如何获取访问令牌？

你需要按照[安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)操作，该指南详述了如何在遵循新安全要求的同时这样做。 可以在[此处](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)找到 .NET 示例代码，在[此处](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)找到 Java 示例代码。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>作为 CPV，我是在 CPV 租户中还是在云解决方案提供商合作伙伴租户中创建 Azure AD 应用程序？

CPV 需在与其注册（以 CPV 身份）相关联的租户中创建 Azure Active Directory 应用程序。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>我是使用“仅应用”身份验证的云解决方案提供商。 我是否需要进行任何更改？

“仅应用”身份验证不受影响，因为用户凭据不用于请求访问令牌。 如果用户凭据是共享的，则控制面板供应商 (CPV) 必须采用[安全应用程序模型框架](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)并清除他们现有的任何合作伙伴凭据。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>作为 CPV，我是否可以利用“仅应用”身份验证模式来获取访问令牌？

否，控制面板供应商合作伙伴不能利用“仅应用”身份验证模式代表合作伙伴来请求访问令牌。 他们应该实现安全应用程序模型，以便利用“应用 + 用户”身份验证模式。

## <a name="technical-enforcement"></a>技术实施

### <a name="what-is-the-activation-of-security-safeguards"></a>什么是激活安全保护措施？

参与云解决方案提供商 (CSP) 计划的所有合作伙伴、控制面板供应商 (CPV) 和顾问应实施强制性安全要求以保持合规性。

为了提供额外的保护，Microsoft 已经开始激活安全保护措施了，通过强制执行多重身份验证 (MFA) 来阻止未经授权的访问，从而帮助合作伙伴保障其租户及其客户的安全。  

我们已成功完成了为所有合作伙伴租户的“代表管理员(AOBO)”功能激活保护措施。 为了进一步保护合作伙伴和客户，以 2020 年（日历年）第 2 季度为起点，我们将开始针对 CSP 中的合作伙伴中心交易激活保护措施，帮助合作伙伴保护其业务和客户免受身份盗窃相关事件的影响。

有关详细信息，请访问[为合作伙伴租户强制执行多重身份验证 (MFA)](partner-security-requirements-mandating-mfa.md) 页面。

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>我使用的是第三方 MFA 解决方案，但我遭到阻止，该怎么办？

为了验证访问资源的帐户是否已受到多重身份验证的质询，我们需要检查[身份验证方法引用](https://tools.ietf.org/html/rfc8176)声明，查看其中是否列出了 MFA。 某些第三方解决方案不会发出此声明，或者不包含 MFA 值。 如果缺少该声明或者未列出 MFA 值，则无法确定身份验证的帐户是否受到了多重身份验证的质询。 需要咨询第三方解决方案的供应商，以确定需要采取哪些措施来使解决方案发出身份验证方法引用声明。

如果你不确定自己的第三方解决方案是否发出所需的声明，请参阅[测试合作伙伴安全要求](/powershell/partnercenter/test-partner-security-requirements)。

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA 阻止我使用 AOBO 为客户提供支持，该怎么办？

合作伙伴安全要求的技术实施将会检查身份验证的帐户是否已受到多重身份验证的质询。 如果该帐户未受到质询，系统则会将你重定向到登录页面并且会再次提示你进行身份验证。 请在此[为合作伙伴租户强制执行多重身份验证 (MFA)](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) 文档中查看其他体验和指南。 如果你的域不是联合域，那么在成功完成身份验证后，系统会提示你设置多重身份验证。 设置完成后，你就可以使用 AOBO 对客户进行管理。 如果你的域是联合域，则需要确保帐户受到多重身份验证的质询。

## <a name="security-defaults-transition"></a>安全默认设置过渡

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>如何从基线策略过渡到安全默认设置或其他 MFA 解决方案？

Azure Active Directory (Azure AD)[“基线”策略将被删除并被替换](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults)为“安全默认设置”，这是一组适用于你和你客户的更全面的保护策略。 [安全默认设置](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)有助于保护组织免受与身份盗窃相关的安全攻击。

如果你尚未从基线策略过渡到安全默认设置策略或[其他 MFA 实现选项](partner-security-requirements.md#implementing-multi-factor-authentication)，你的多重身份验证 (MFA) 实现则会因基线策略的停用而被删除。 你合作伙伴租户中执行受 MFA 保护的操作的任何用户将被要求完成 MFA 验证。 在[此处](partner-security-requirements-mandating-mfa.md)查看更多详细的指南。
若要保持合规性并最大程度地减少中断，请执行以下操作之一：

- 过渡到安全默认设置
    - 安全默认设置策略是合作伙伴可选择用于实现 MFA 的选项之一。 它提供基本的安全级别，无需额外付费即可启用。
    - 了解如何使用 Azure AD 为组织启用 MFA，并查看[安全默认设置关键注意事项](partner-security-requirements.md#security-defaults)。
    - 如果安全默认设置符合你的业务需求，则启用它。
- 过渡到条件访问
    - 如果安全默认设置策略不满足你的需求，则启用条件访问。 有关详细信息，请查看“Azure AD 条件访问”文档。

## <a name="key-resources"></a>重要资源

### <a name="how-to-get-started"></a>如何开始使用

- [合作伙伴安全要求：分步指南](partner-security-requirements.md)。
- 请将你的问题和反馈发布到此[合作伙伴中心安全指南组](https://aka.ms/MPCSecurityGuidance)。
- 参加即将召开的 Partner Office Hours 和网络研讨会。 请[在此处查看详细的计划和资源](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)。

### <a name="resources-for-adopting-secure-application-model"></a>采用安全应用程序模型的资源

- [安全应用程序模型概述](/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心：安全应用程序模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 .NET 示例代码](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [云解决方案提供商计划中的合作伙伴：用于启用安全应用程序模型的 Java 示例代码](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [合作伙伴中心身份验证文档](/partner-center/develop/partner-center-authentication)
- [合作伙伴中心 PowerShell 多重身份验证 (MFA) 文档](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>支持

### <a name="where-can-i-get-support"></a>我可以在哪里获得支持？

如需获得满足安全要求的支持资源，而且你有合作伙伴高级支持 (ASfP)，请联系服务帐户管理员；如需获得合作伙伴协议高级支持 (PSfP)，请联系服务帐户管理员和技术帐户管理员。

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>如何获取有助于我采用安全应用程序模型框架的技术信息和支持？

可以通过 MPN 权益获取 Azure Active Directory 的技术产品支持选项。 能够访问活动 ASfP 或 PSfP 订阅的合作伙伴可以咨询相关的帐户管理员 (SAM/TAM)，这样可以最好地了解可用选项。

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>如果我无法再访问合作伙伴中心，那么该如何联系支持部门？

如果你由于 MFA 问题失去访问权限，请联系你租户的全局管理员。 你的内部 IT 部门将能够告诉你全局管理员是谁。 

如果你忘记了密码，请阅读[无法登录](unable-to-sign-in.md)来获得帮助。

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>在哪里可以找到常见技术问题的详细信息？

有关常见技术问题的信息，请参阅[针对使用合作伙伴中心或合作伙伴中心 API 的合作伙伴安全要求](partner-security-requirements.md)