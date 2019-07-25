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
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a><span data-ttu-id="30ed9-104">有关合作伙伴安全要求的常见问题</span><span class="sxs-lookup"><span data-stu-id="30ed9-104">Frequently asked questions about the partner security requirements</span></span>

<span data-ttu-id="30ed9-105">本文包含有关[合作伙伴安全要求](partner-security-requirements.md)的一些常见问题解答。</span><span class="sxs-lookup"><span data-stu-id="30ed9-105">This article contains some frequently asked questions for the [partner security requirements](partner-security-requirements.md).</span></span> <span data-ttu-id="30ed9-106">可在[此处](http://assetsprod.microsoft.com/security-requirements-faq.pdf)找到常见问题的综合列表。</span><span class="sxs-lookup"><span data-stu-id="30ed9-106">You can find a comprehensive list of frequently asked questions [here](http://assetsprod.microsoft.com/security-requirements-faq.pdf).</span></span>

## <a name="conditional-access"></a><span data-ttu-id="30ed9-107">条件访问</span><span class="sxs-lookup"><span data-stu-id="30ed9-107">Conditional Access</span></span>

### <a name="can-conditional-access-be-used"></a><span data-ttu-id="30ed9-108">是否可以使用条件访问？</span><span class="sxs-lookup"><span data-stu-id="30ed9-108">Can conditional access be used?</span></span>

<span data-ttu-id="30ed9-109">是的, 你可以使用条件性访问来为你的合作伙伴租户中的每个用户 (包括服务帐户) 强制实施 MFA。</span><span class="sxs-lookup"><span data-stu-id="30ed9-109">Yes, you can use conditional access to enforce MFA for each user, including service accounts, in your partner tenant.</span></span> <span data-ttu-id="30ed9-110">但是, 考虑到成为合作伙伴, 我们需要确保每个用户对每个单个身份验证都具有 MFA 质询。</span><span class="sxs-lookup"><span data-stu-id="30ed9-110">However, given the highly privileged nature of being a partner we need to ensure that each user has an MFA challenge for every single authentication.</span></span> <span data-ttu-id="30ed9-111">这意味着你将无法利用条件访问的功能, 这种功能会绕过 MFA 的要求。</span><span class="sxs-lookup"><span data-stu-id="30ed9-111">This means you will not be able to leverage feature of conditional access that circumvent the requirement for MFA.</span></span>

## <a name="multi-factor-authentication"></a><span data-ttu-id="30ed9-112">多重身份验证</span><span class="sxs-lookup"><span data-stu-id="30ed9-112">Multi-Factor Authentication</span></span>

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a><span data-ttu-id="30ed9-113">我的客户是否受合作伙伴安全要求的限制？</span><span class="sxs-lookup"><span data-stu-id="30ed9-113">Are my customers subject to the partner security requirements?</span></span>

<span data-ttu-id="30ed9-114">不需要, 不需要为客户的 Azure AD 租户中的每个用户强制实施 MFA。</span><span class="sxs-lookup"><span data-stu-id="30ed9-114">No, it is not required that you enforce MFA for each user in your customer's Azure AD tenants.</span></span> <span data-ttu-id="30ed9-115">但建议您与每个客户合作, 确定如何最好地保护他们的用户。</span><span class="sxs-lookup"><span data-stu-id="30ed9-115">However, it is recommended that you work with each customer to determine how best to protect their users.</span></span>

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a><span data-ttu-id="30ed9-116">应用密码是否可与基线保护策略一起使用？</span><span class="sxs-lookup"><span data-stu-id="30ed9-116">Can app passwords be used with the baseline protection policies?</span></span>

<span data-ttu-id="30ed9-117">是的, 可以使用[应用密码](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)。</span><span class="sxs-lookup"><span data-stu-id="30ed9-117">Yes, [app passwords](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) can be used.</span></span> <span data-ttu-id="30ed9-118">你应查看使用[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)记录的应用密码的注意事项, 以确定是否支持你的需求。</span><span class="sxs-lookup"><span data-stu-id="30ed9-118">You should review the considerations for using app passwords documented [here](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) to determine if they are supported for your need.</span></span>

### <a name="can-any-user-be-excluded-from-this-requirement"></a><span data-ttu-id="30ed9-119">是否可以从此要求中排除任何用户？</span><span class="sxs-lookup"><span data-stu-id="30ed9-119">Can any user be excluded from this requirement?</span></span> 

<span data-ttu-id="30ed9-120">不需要, 你的合作伙伴租户中的每个用户 (包括服务帐户) 都需要使用 MFA 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="30ed9-120">No, each user, including service accounts, in your partner tenant will be required to authenticate using MFA.</span></span>

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a><span data-ttu-id="30ed9-121">合作伙伴安全要求是否适用于集成沙盒？</span><span class="sxs-lookup"><span data-stu-id="30ed9-121">Do the partner security requirements apply to the integration sandbox?</span></span>

<span data-ttu-id="30ed9-122">是, 合作伙伴安全要求适用于集成沙盒。</span><span class="sxs-lookup"><span data-stu-id="30ed9-122">Yes, the partner security requirements apply to the integration sandbox.</span></span> <span data-ttu-id="30ed9-123">这意味着, 你将需要为 integration 沙盒租户中的用户实现适当的 MFA 解决方案。</span><span class="sxs-lookup"><span data-stu-id="30ed9-123">This means you will need to implement the appropriate MFA solution for users in the integration sandbox tenant.</span></span> <span data-ttu-id="30ed9-124">建议你实现基线保护策略来提供 MFA。</span><span class="sxs-lookup"><span data-stu-id="30ed9-124">It is recommended that you implement the baseline protection policies to provide MFA.</span></span>

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a><span data-ttu-id="30ed9-125">如何实现配置紧急访问 (中断玻璃) 帐户？</span><span class="sxs-lookup"><span data-stu-id="30ed9-125">How do I configure an emergency access (break glass) account?</span></span>

<span data-ttu-id="30ed9-126">它被认为是创建一个或两个紧急访问帐户, 以防止无意中锁定 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="30ed9-126">It considered best practice to create one or two emergency access accounts to prevent being inadvertently locked out of your Azure AD tenant.</span></span> <span data-ttu-id="30ed9-127">对于合作伙伴安全要求, 每个用户都需要使用 MFA 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="30ed9-127">With respect to the partner security requirements, it is required that each user authenticate using MFA.</span></span> <span data-ttu-id="30ed9-128">因此, 这意味着你将需要修改紧急访问帐户的定义。</span><span class="sxs-lookup"><span data-stu-id="30ed9-128">So, this means you will need to modify the definition of an emergency access account.</span></span> <span data-ttu-id="30ed9-129">它可以是利用第三方解决方案进行 MFA 的帐户。</span><span class="sxs-lookup"><span data-stu-id="30ed9-129">It could be an account that is leveraging a third-party solution for MFA.</span></span>

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a><span data-ttu-id="30ed9-130">来宾用户将受合作伙伴安全要求的影响？</span><span class="sxs-lookup"><span data-stu-id="30ed9-130">How will guest users be impacted by the partner security requirements?</span></span>

<span data-ttu-id="30ed9-131">访问合作伙伴租户中的资源时, 来宾用户需要使用 MFA 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="30ed9-131">Guest users will be required to authenticate using MFA, when accessing resources in your partner tenant.</span></span> <span data-ttu-id="30ed9-132">合作伙伴安全要求将不会对来宾用户访问其自己租户中的资源产生任何影响。</span><span class="sxs-lookup"><span data-stu-id="30ed9-132">The partner security requirements will have no impact on the guest user will accessing resources in their own tenant.</span></span>

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a><span data-ttu-id="30ed9-133">如果我使用的是第三方解决方案 Active Directory 需要联合身份验证服务 (ADFS) 吗？</span><span class="sxs-lookup"><span data-stu-id="30ed9-133">If I am using a third-party solution is Active Directory Federation Service (ADFS) required?</span></span> 

<span data-ttu-id="30ed9-134">不是, 如果使用的是第三方解决方案, 则不需要 Active Directory 联合身份验证服务 (ADFS)。</span><span class="sxs-lookup"><span data-stu-id="30ed9-134">No, it is not required to have Active Directory Federation Service (ADFS) if you are using a third-party solution.</span></span> <span data-ttu-id="30ed9-135">建议你与解决方案的供应商合作确定其解决方案的要求。</span><span class="sxs-lookup"><span data-stu-id="30ed9-135">It is recommended that you work with the vendor of the solution determine what the requirements for their solution are.</span></span>

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a><span data-ttu-id="30ed9-136">是否需要启用基线保护策略？</span><span class="sxs-lookup"><span data-stu-id="30ed9-136">Is it a requirement to enable the baseline protection policies?</span></span>

<span data-ttu-id="30ed9-137">不需要, 不需要启用基线保护策略。</span><span class="sxs-lookup"><span data-stu-id="30ed9-137">No, it is not required that you enable the baseline protection policies.</span></span> <span data-ttu-id="30ed9-138">唯一的要求是在合作伙伴租户中为每个用户 (包括服务帐户) 强制执行 MFA。</span><span class="sxs-lookup"><span data-stu-id="30ed9-138">The only requirement is that you enforce MFA for each user, including service accounts, in your partner tenant.</span></span>

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a><span data-ttu-id="30ed9-139">通过实现基线保护策略提供了哪些验证选项？</span><span class="sxs-lookup"><span data-stu-id="30ed9-139">What verification options are provided through the implementation of the baseline protection policies?</span></span> 

<span data-ttu-id="30ed9-140">对于通过实现基线保护策略而提供的 MFA 版本, 唯一可用的验证选项是验证器应用。</span><span class="sxs-lookup"><span data-stu-id="30ed9-140">With respect to the version of MFA that is available through the implementation of the baseline protection polices, the only verification option available is an authenticator app.</span></span> <span data-ttu-id="30ed9-141">使用电话呼叫和短信消息被视为不太安全。</span><span class="sxs-lookup"><span data-stu-id="30ed9-141">The use of a phone call and text message message is considered less secure.</span></span> <span data-ttu-id="30ed9-142">因此, 这些选项无法通过此版本的 MFA 获得。</span><span class="sxs-lookup"><span data-stu-id="30ed9-142">So, these options are not available through this version of MFA.</span></span>

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a><span data-ttu-id="30ed9-143">Azure AD Connect 所使用的服务帐户是否受合作伙伴安全要求的影响？</span><span class="sxs-lookup"><span data-stu-id="30ed9-143">Will the service account used by Azure AD Connect be impacted by the partner security requirements?</span></span>

<span data-ttu-id="30ed9-144">不会, Azure AD Connect 使用的服务帐户将不受合作伙伴安全要求的影响。</span><span class="sxs-lookup"><span data-stu-id="30ed9-144">No, the service account used by Azure AD Connect will not be impacted by the partner security requirements.</span></span> <span data-ttu-id="30ed9-145">如果由于强制 MFA 而导致 Azure AD Connect 遇到问题, 请通过 Microsoft 支持提出技术支持请求。</span><span class="sxs-lookup"><span data-stu-id="30ed9-145">If you experience an issue with Azure AD Connect as result of enforcing MFA, then open a technical support request with Microsoft support.</span></span>
