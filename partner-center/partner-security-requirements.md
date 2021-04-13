---
title: 合作伙伴安全要求
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 引入合作伙伴安全要求，以启用多重身份验证 (MFA) 并采用安全应用程序模型框架。
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087053"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>使用合作伙伴中心或合作伙伴中心 API 的安全要求

**相应的角色**

- 所有合作伙伴中心用户

本文介绍了针对参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴的强制性安全要求，以及身份验证选项和其他安全注意事项。 隐私保护和安全性是我们优先关注的事项。 我们知道，最好的防御措施是防患于未然，链条的强度取决于其最弱的一环。 因此，我们需要生态系统中的所有人都行动起来，确保将安全保护措施实施到位。

## <a name="mandatory-security-requirements"></a>强制性安全要求

不实施这些强制性要求的合作伙伴将不能在云解决方案提供商计划中处理事务，也不能使用委托的管理权限来管理客户租户。 另外，不实施安全要求的合作伙伴可能有无法参与计划的风险。 与合作伙伴安全要求相关的条款已添加到 Microsoft 合作伙伴协议中。 由于与顾问相关，因此会实施相同的合同要求。

为了保护你和你的客户，我们要求合作伙伴立即采取以下措施：  

1. **为合作伙伴租户中的所有用户帐户启用多重身份验证 (MFA)** 。 必须为合作伙伴租户中的所有用户帐户启用 MFA。 在登录到 Microsoft 商业云服务时，或者通过合作伙伴中心或 API 在云解决方案提供商计划中进行事务处理时，用户必须接受 MFA。

2. **采用安全应用程序模型框架**。 所有集成合作伙伴中心 API 的合作伙伴必须对任何应用和用户身份验证模型应用程序采用[安全应用程序模型框架](/partner-center/develop/enable-secure-app-model)。

    > [!IMPORTANT]
    > 强烈建议合作伙伴实现安全应用程序模型，以便集成 Microsoft API（例如 Azure 资源管理器或 Microsoft Graph）或利用自动化时（例如使用用户凭据的 PowerShell），避免在强制实施 MFA 时出现任何中断。

这些安全要求将有助于保护你的基础结构与客户数据免受身份盗用或其他欺诈事件等潜在安全风险的影响。  

## <a name="implementing-multi-factor-authentication"></a>实施多重身份验证

若要符合合作伙伴安全要求，必须为合作伙伴租户中的每个用户帐户实施并强制执行多重身份验证。 可通过下述方法之一完成此操作：

- 实现 [Azure Active Directory (Azure AD) 安全默认值](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)。 详见[下一节](#security-defaults)。

- 为每个用户帐户购买 Azure Active Directory Premium。 有关详细信息，请参阅[规划 Azure AD 多重身份验证部署](/azure/active-directory/authentication/howto-mfa-getstarted)。

- 使用第三方解决方案为合作伙伴租户中的每个用户帐户强制实施 MFA。 要确保解决方案将提供预期的解决办法，请参阅[如何强制实施安全要求](#how-the-requirements-are-enforced)。

> [!NOTE]
> 虽然多重身份验证不是主权云（Microsoft Cloud for US Government、德国 Microsoft 云）的协议要求的，但我们仍强烈建议你履行这些安全要求。

### <a name="security-defaults"></a>安全性默认设置

合作伙伴可选择用于实现 MFA 要求的选项之一是在 Azure AD 中启用安全默认值。 安全默认值提供基本的安全级别，无需额外付费。 启用安全默认值之前，请查看如何使用 Azure AD 为组织启用 MFA，并查看以下关键注意事项。

- 已采用基线策略的合作伙伴需采取行动过渡到安全性默认设置。

- 安全默认值是预览版基线策略的正式版替代品。 一旦合作伙伴启用了安全默认值，他们就不再能够启用基线策略。

- 使用安全性默认设置时，所有策略都会一次性启用。

- 对于使用[条件访问](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)的合作伙伴，[安全默认值将不可用](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)。

- 我们目前不阻止旧式身份验证。 但是，由于大多数与已泄露标识相关的事件都来自于使用旧身份验证的登录尝试，因此建议合作伙伴脱离这些早期协议。

- Azure AD Connect 同步帐户已从安全默认值中排除。

有关详细信息，请阅读[组织的 Azure AD 多重身份验证概述](/azure/active-directory/authentication/concept-mfa-get-started)和[什么是安全默认值？](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)。

> [!NOTE]
> Azure AD 安全性默认设置是从简化的基线保护策略演进过来的。 如果你已启用基线保护策略，强烈建议你启用[安全默认值](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)。

## <a name="implementation-considerations"></a>实现注意事项

由于这些要求适用于合作伙伴租户中的所有用户帐户，因此你需要考虑一些事项以确保顺利进行部署。 例如，确定 Azure AD 中不能执行 MFA 的用户帐户，以及组织中不支持新式身份验证的应用程序和设备。

建议在执行任何操作之前完成以下验证。 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>你是否有不支持使用新式身份验证的应用程序或设备？

强制实施 MFA 时，系统会阻止旧式身份验证协议（例如 IMAP、POP3、SMTP 等）的使用，因为这些协议不支持 MFA。 为了解决此限制问题，可以使用[应用密码](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)功能，确保应用程序或设备仍然会进行身份验证。 请查看[应用密码使用注意事项](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)，确定应用密码是否可以在你的环境中使用。

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>你是否有拥有与你的合作伙伴租户关联的许可证的 Office 365 用户？

建议你在实现任何解决方案之前，确定合作伙伴租户中的用户所使用的 Microsoft Office 版本。 用户可能会在使用 Outlook 之类的应用程序时遇到连接问题。 在强制实施 MFA 之前，必须确保使用的是 Outlook 2013 SP1 或更高版本，且组织已启用新式身份验证。 有关详细信息，请参阅[在 Exchange Online 中启用新式身份验证](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)。 

若要为运行 Windows 且已安装 Microsoft Office 2013 的设备启用新式身份验证，需创建两个注册表项。 请参阅[在 Windows 设备上启用适用于 Office 2013 的新式身份验证](/office365/admin/security-and-compliance/enable-modern-authentication)。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>是否有策略阻止用户在工作时使用其移动设备？

必须确定任何阻止员工在工作时使用移动设备的公司策略，因为它会影响你实现的具体的 MFA 解决方案。 有的解决方案（例如通过实施 [Azure AD 安全性默认设置](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)提供的解决方案）仅允许使用 Authenticator 应用进行验证。 如果组织的某项策略阻止使用移动设备，则请考虑以下选项之一：

- 部署可以在安全系统上运行的基于时间的一次性密码 (TOTP) 应用程序。

- 实现第三方解决方案，为合作伙伴租户中的每个用户帐户强制实施 MFA，以便提供最适当的验证选项。

- 为受影响的用户购买 [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) 许可证。

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>你有哪种自动化或集成来利用用户凭据进行身份验证？

由于我们对合作伙伴目录中的每位用户（包括服务帐户）强制实施 MFA，因此任何使用用户凭据进行身份验证的自动化或集成都会受影响。 因此，必须确定在这些情况下使用的是什么帐户。 请查看以下列表，了解要考虑的示例应用程序或服务：

- 控制面板，用于代表客户预配资源

- 与任何用于客户发票（由于与 CSP 计划相关）和支持的平台的集成

- 使用 Az、AzureRM、Azure AD、MS Online 和其他模块的 PowerShell 脚本

以上列表并不完整。 因此，必须对环境中使用用户凭据进行身份验证的任何应用程序或服务进行完整的评估。 在可能情况下，应该按[安全应用程序模型框架](/partner-center/develop/enable-secure-app-model)中的指南（不同于 MFA 的要求）进行操作。

## <a name="accessing-your-environment"></a>访问环境

若要更好地了解哪个帐户或用户在进行身份验证时没有受到 MFA 质询，建议查看登录活动。 可通过 Azure Active Directory Premium 使用登录报告。 有关此主题的详细信息，请参阅 [Azure Active Directory 门户中的登录活动报告](/azure/active-directory/reports-monitoring/concept-sign-ins)。 如果你没有 Azure Active Directory Premium 或正打算通过 PowerShell 获取此登录活动，则需要使用[合作伙伴中心 PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) 模块中的 [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet。

## <a name="how-the-requirements-are-enforced"></a>如何强制实施这些要求

合作伙伴安全要求先后由 Azure AD 和合作伙伴中心强制实施，方法是：检查是否存在 MFA 声明，以便确定是否进行了 MFA 验证。 从 2019 年 11 月 18 日开始，Microsoft 激活了针对合作伙伴租户的其他安全保护措施（以前称为“技术强制措施”）。

激活后，合作伙伴租户中的用户在执行任何管理员代表 (AOBO) 操作、访问合作伙伴中心门户或调用合作伙伴中心 API 时都会被要求完成 MFA 验证。 有关详细信息，请参阅[为合作伙伴租户强制执行多重身份验证 (MFA)](partner-security-requirements-mandating-mfa.md)。 

尚未满足这些要求的合作伙伴应尽快实施这些措施，以免出现业务中断。 如果使用 Azure Active Directory 多重身份验证或 Azure AD 安全默认值，则不需要执行任何其他操作。

如果使用的是第三方 MFA 解决方案，可能会出现 MFA 声明未发出的情况。 如果缺少该声明，则 Azure AD 无法确定身份验证请求是否受到了 MFA 的质询。 若要了解如何验证解决方案是否发出了预期的声明，请阅读[测试合作伙伴安全要求](/powershell/partnercenter/test-partner-security-requirements)。 

> [!IMPORTANT]
> 如果第三方解决方案未发出预期的声明，则需咨询开发该解决方案的供应商，以确定应该采取哪些措施。

## <a name="resources-and-samples"></a>资源和示例

请查看以下资源来获取支持和示例代码：

- [合作伙伴中心安全指导组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)：合作伙伴中心安全指导组社区是一个网上社区，你可在这里了解即将发生的活动并就你可能遇到的任何问题提问。
- [合作伙伴中心 .NET 示例](https://github.com/microsoft/partner-center-dotnet-samples)：这个 GitHub 存储库包含使用 .NET 开发的示例，用于演示如何实现安全应用程序模型框架。
- [合作伙伴中心 Java 示例](https://github.com/microsoft/partner-center-java-samples)：这个 GitHub 存储库包含使用 Java 开发的示例，用于演示如何实现安全应用程序模型框架。
- [合作伙伴中心 PowerShell - 多重身份验证](/powershell/partnercenter/multi-factor-auth)：这篇关于多重身份验证的文章详细介绍了如何使用 PowerShell 实现安全应用程序模型框架。

## <a name="next-steps"></a>后续步骤

- [为合作伙伴租户强制执行多重身份验证 (MFA)](partner-security-requirements-mandating-mfa.md)