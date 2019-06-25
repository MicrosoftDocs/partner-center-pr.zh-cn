---
title: 合作伙伴的安全要求 |合作伙伴中心
ms.topic: article
ms.date: 06/25/2019
description: 了解有关顾问和参与云解决方案提供商计划的合作伙伴的安全要求。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory、 云解决方案提供商、 云解决方案提供商，则程序 CSP、 控件面板供应商联系，CPV、 多重身份验证，MFA，安全应用程序模型、 安全的应用程序模型、 安全性
ms.localizationpriority: medium
ms.openlocfilehash: de1452ce14c8343e2e05dcc65a7a6c05259576c5
ms.sourcegitcommit: ca7f000a58575fa9a089693256c095120dde3c5d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2019
ms.locfileid: "67346996"
---
# <a name="partner-security-requirements"></a>合作伙伴的安全要求

**适用于**

- 云解决方案提供商计划中的所有合作伙伴
  - 直接的帐单
  - 间接提供商
  - 间接经销商
- 所有控件面板供应商
- 所有顾问

安全和隐私的客户和合作伙伴是 microsoft 的头等大事。 我们继续看到越来越多的更复杂的安全攻击，主要与遭到入侵的标识。 预防性控制整个防御策略以阻止安全攻击中扮演着重要角色，我们将开始强制执行一系列必需的安全要求，以帮助保护合作伙伴和客户。

> [!NOTE]
> 我们强烈建议所有合作伙伴通过主权云 (21Vianet，美国政府区域和德国) 事务处理操作，并立即采用这些新的安全要求。 但是，这些合作伙伴不需要满足年 7 月 1 日生效的新安全要求。 Microsoft 将提供有关在将来实施主权云这些安全性要求的其他详细信息。

## <a name="overview-of-the-requirements"></a>要求概述

所有合作伙伴参与云解决方案提供商计划、 控制面板供应商和顾问合作伙伴都需要为每个用户在其合作伙伴租户中强制实施多重身份验证 (MFA)。 这可以通过启用两个[Azure Active Directory 基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)。 基线策略是一组预定义策略来帮助保护组织针对许多常见的攻击。 这些常见的攻击可以包含密码喷射、 重播和网页仿冒欺诈。 所有版本的 Azure Active Directory 中提供了基线策略。 Microsoft 向这些基线保护策略提供每个人都因为基于标识的攻击已过去几年的上升。

下表所述，应启用的两个基线策略。

|**策略**| |
|-----|-----|
|**适用于管理员要求 MFA**|启用管理员策略需要 MFA，将要求管理员角色的用户注册 MFA 使用身份验证器应用。 MFA 注册完成后，管理员将需要执行 MFA，每次登录。|
|**最终用户保护**|最终用户保护是基于风险的 MFA 基线策略保护的目录中的所有用户。 如果启用此策略要求所有用户注册 MFA 使用身份验证器应用。 14 天，此后它们将无法登录，直到在注册 MFA，用户可以忽略 MFA 注册提示。 一旦注册 MFA，用户将会提示进行 MFA 仅在有风险的登录尝试。 重置其密码和已关闭风险事件之前，将阻止用户帐户泄露。|

启用这些策略后，每个用户将能够利用 Azure MFA，且不另外收费。 如果使用第三方解决方案，然后需要访问 Microsoft 商业云服务时为每个用户强制实施 MFA。

> [!IMPORTANT]
> 对于合作伙伴目录中的每个用户，将强制执行 MFA，因为会影响任何自动化或利用用户凭据的集成。 若要解决这种影响将需要修改的方式自动化或集成连接到 Microsoft 商业云服务。 如果要连接到该服务支持基于身份验证令牌，则我们建议你实现[保护应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)。

## <a name="what-actions-do-i-need-to-take"></a>我需要执行哪些操作？ 

若要确保伙伴中的每个用户受到保护，需要启用[适用于管理员要求使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)并[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线策略。 在启用这些策略之前, 务必理解他们执行的操作以及它们将如何影响任何自动化或集成和你的用户。

### <a name="considerations"></a>注意事项

由于安全要求将应用于合作伙伴目录中的所有用户，几个注意事项需要进行，以确保顺利完成部署。 这些注意事项包括标识不能或不应执行 MFA，以及应用程序和由你的组织不支持新式身份验证的客户端的 Azure Active Directory 中的用户。

#### <a name="legacy-protocols"></a>旧协议

邮件客户端使用旧式身份验证协议 （IMAP、 SMTP、 POP3、 等） 进行身份验证请求。 这些协议不支持 MFA。 大部分看到由 Microsoft 帐户破坏而引起不良参与方执行攻击试图绕过 MFA 的旧协议。 为了确保登录到合作伙伴目录中的帐户时需要 MFA 和不良参与方不能绕过 MFA，这些安全要求将阻止旧版协议中的所有身份验证请求。

### <a name="enabling-the-baseline-policies"></a>启用基线策略

请参阅[实现合作伙伴安全要求教程](tutorials/partner-security-requirements.yml)有关基线策略的实现提供引导式体验。  

#### <a name="require-mfa-for-admins"></a>适用于管理员要求 MFA

*管理员要求使用 MFA*基准策略要求使用 MFA 进行以下目录角色，被视为最高特权的 Azure Active Directory 角色：

- 全局管理员
- SharePoint 管理员
- Exchange 管理员
- 条件性访问管理员
- 安全管理员
- 支持管理员 / 密码管理员
- 帐务管理员
- 用户管理员

启用管理员策略需要 MFA，时更高版本的九个管理员角色将需要使用身份验证器应用的 mfa 注册。 MFA 注册完成后，管理员将需要执行每次登录的 MFA。

如果你的组织中的脚本或代码中使用这些帐户，请考虑将它们替换为 [托管标识](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。

若要启用此策略并保护你的管理员：

1. 登录到 **Azure 门户** 作为全局管理员、 安全管理员或条件性访问管理员。
2. 浏览到**Azure Active Directory** > **条件性访问**。
3. 在策略列表中，选择**基准策略：适用于管理员要求 MFA**。
4. 设置**启用策略**到**立即使用策略**。
5. 单击 **保存**。

    ![适用于管理员要求 MFA](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> 启用此策略之前，请确保你的用户不使用传统的身份验证协议。 请参阅文章[如何：阻止到 Azure Active Directory 条件性访问与传统的身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use)有关详细信息。

> [!IMPORTANT]
> 没有已知的问题，影响您连接到 Exchange Online PowerShell 使用委派管理权限的能力。 请参阅[Exchange Online PowerShell](#exchange-online-powershell)已知问题之前启用此策略，如果您使用此 PowerShell 模块。

#### <a name="end-user-protection"></a>最终用户保护

最终用户保护基线策略保护的目录中的所有用户。 如果启用此策略要求所有用户在 14 天内注册 Azure MFA。 注册后，用户将会提示进行 MFA 仅在有风险的登录尝试。 密码重置和风险上诉之前，将阻止用户帐户泄露。

策略**基准策略：最终用户保护**预配置，此时将显示在顶部导航到在 Azure 门户中的条件性访问边栏选项卡时。

若要启用此策略并保护你的用户：

1. 登录到 **Azure 门户** 作为全局管理员、 安全管理员或条件性访问管理员。
2. 浏览到**Azure Active Directory** > **条件性访问**。
3. 在策略列表中，选择**基准策略：最终用户保护 （预览版）** 。
4. 设置**启用策略**到**立即使用策略**。
5. 单击 **保存**。

    ![最终用户保护](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> 启用此策略之前，请确保你的用户不使用传统的身份验证协议。 请参阅文章[如何：阻止到 Azure Active Directory 条件性访问与传统的身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use)有关详细信息。

> [!IMPORTANT]
> 没有已知的问题，影响您连接到 Exchange Online PowerShell 使用委派管理权限的能力。 请参阅[Exchange Online PowerShell](#exchange-online-powershell)已知问题之前启用此策略，如果您使用此 PowerShell 模块。

## <a name="common-issues"></a>常见问题

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

启用后基线策略，可能会发现你的自动化或集成遇到类似于下面的异常

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

此异常的原因是要进行身份验证使用用户凭据，MFA 目前所需。 若要解决此异常，您将需要使用访问令牌进行身份验证。 请参阅[保护应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)有关详细信息。

>[!IMPORTANT]
>大多数新式 Api 和 PowerShell 模块支持能够使用身份验证的访问令牌。 但是，有一些当前不支持此功能。 如果你需要帮助确定如果您尝试利用 API 或 PowerShell 模块支持使用访问令牌的身份验证，然后将消息发布在[合作伙伴中心安全指南组](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)社区。

#### <a name="aadsts700082"></a>AADSTS700082

实现安全应用程序模型框架后就可能会收到以下异常 90 天后生成了初始的刷新令牌

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

对于 Azure Active Directory 进行刷新的最长生存期令牌为 90 天。 若要解决此错误，将需要生成并安全地将存储新的刷新令牌。 请注意可以以编程方式更新刷新令牌，因为与 Azure Active Directory 访问令牌的每个请求返回一个新的刷新令牌。 您可以实现相应的逻辑以安全地存储的刷新令牌过期之前进行更新。

请参阅[Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)有关详细信息。

## <a name="known-issues"></a>已知问题

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

启用 MFA 后合作伙伴不能利用其委派管理权限与 Exchange Online PowerShell，若要对其客户执行各种操作。 请参阅[连接到使用多重身份验证的 Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)有关此限制的详细信息。

## <a name="resources-and-support"></a>资源和支持

通过[合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)可以将查找其他资源并了解即将开展的活动，例如技术工作时间。 请参阅[方面的常见问题](http://assetsprod.microsoft.com/security-requirements-faq.pdf)文档，了解有关要求的详细信息。

### <a name="developers"></a>开发人员

- [启用安全的应用程序模型](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [合作伙伴中心.NET 示例](https://github.com/microsoft/partner-center-dotnet-samples)
- [合作伙伴中心的 Java 示例](https://github.com/microsoft/partner-center-java-samples)
- [合作伙伴中心 PowerShell 实现安全应用程序模型](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
