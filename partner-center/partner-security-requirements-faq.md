---
title: 合作伙伴安全要求常见问题解答 |合作伙伴中心
ms.topic: article
ms.date: 07/18/2019
description: 有关合作伙伴安全要求的常见问题
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315546"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>有关合作伙伴安全要求的常见问题

本文包含有关[合作伙伴安全要求](partner-security-requirements.md)的一些常见问题解答。 可在[此处](http://assetsprod.microsoft.com/security-requirements-faq.pdf)找到常见问题的综合列表。

## <a name="conditional-access"></a>条件访问

### <a name="can-conditional-access-be-used"></a>是否可以使用条件访问？

是的, 你可以使用条件性访问来为你的合作伙伴租户中的每个用户 (包括服务帐户) 强制实施 MFA。 但是, 考虑到成为合作伙伴, 我们需要确保每个用户对每个单个身份验证都具有 MFA 质询。 这意味着你将无法利用条件访问的功能, 这种功能会绕过 MFA 的要求。

## <a name="multi-factor-authentication"></a>多重身份验证

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

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>通过实现基线保护策略提供了哪些验证选项？ 

对于通过实现基线保护策略而提供的 MFA 版本, 唯一可用的验证选项是验证器应用。 使用电话呼叫和短信消息被视为不太安全。 因此, 这些选项无法通过此版本的 MFA 获得。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect 所使用的服务帐户是否受合作伙伴安全要求的影响？

不会, Azure AD Connect 使用的服务帐户将不受合作伙伴安全要求的影响。 如果由于强制 MFA 而导致 Azure AD Connect 遇到问题, 请通过 Microsoft 支持提出技术支持请求。
