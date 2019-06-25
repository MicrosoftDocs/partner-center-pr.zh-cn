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
# <a name="partner-security-requirements"></a><span data-ttu-id="de29e-104">合作伙伴的安全要求</span><span class="sxs-lookup"><span data-stu-id="de29e-104">Partner Security Requirements</span></span>

<span data-ttu-id="de29e-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="de29e-105">**Applies to**</span></span>

- <span data-ttu-id="de29e-106">云解决方案提供商计划中的所有合作伙伴</span><span class="sxs-lookup"><span data-stu-id="de29e-106">All partners in the Cloud Solution Provider program</span></span>
  - <span data-ttu-id="de29e-107">直接的帐单</span><span class="sxs-lookup"><span data-stu-id="de29e-107">Direct bill</span></span>
  - <span data-ttu-id="de29e-108">间接提供商</span><span class="sxs-lookup"><span data-stu-id="de29e-108">Indirect provider</span></span>
  - <span data-ttu-id="de29e-109">间接经销商</span><span class="sxs-lookup"><span data-stu-id="de29e-109">Indirect reseller</span></span>
- <span data-ttu-id="de29e-110">所有控件面板供应商</span><span class="sxs-lookup"><span data-stu-id="de29e-110">All Control Panel Vendors</span></span>
- <span data-ttu-id="de29e-111">所有顾问</span><span class="sxs-lookup"><span data-stu-id="de29e-111">All Advisors</span></span>

<span data-ttu-id="de29e-112">安全和隐私的客户和合作伙伴是 microsoft 的头等大事。</span><span class="sxs-lookup"><span data-stu-id="de29e-112">Security and privacy of customers and partners are top priorities for Microsoft.</span></span> <span data-ttu-id="de29e-113">我们继续看到越来越多的更复杂的安全攻击，主要与遭到入侵的标识。</span><span class="sxs-lookup"><span data-stu-id="de29e-113">We continue to see an increasing number of more sophisticated security attacks, primarily related to compromised identities.</span></span> <span data-ttu-id="de29e-114">预防性控制整个防御策略以阻止安全攻击中扮演着重要角色，我们将开始强制执行一系列必需的安全要求，以帮助保护合作伙伴和客户。</span><span class="sxs-lookup"><span data-stu-id="de29e-114">As preventive controls play a key role in an overall defense strategy to thwart security attacks, we will start enforcing a set of mandatory security requirements to help protect partners and their customers.</span></span>

> [!NOTE]
> <span data-ttu-id="de29e-115">我们强烈建议所有合作伙伴通过主权云 (21Vianet，美国政府区域和德国) 事务处理操作，并立即采用这些新的安全要求。</span><span class="sxs-lookup"><span data-stu-id="de29e-115">We strongly recommend that all partners transacting through a sovereign cloud (21Vianet, US Government, and Germany) act and adopt these new security requirements immediately.</span></span> <span data-ttu-id="de29e-116">但是，这些合作伙伴不需要满足年 7 月 1 日生效的新安全要求。</span><span class="sxs-lookup"><span data-stu-id="de29e-116">However, these partners are not required to meet the new security requirements effective July 1st.</span></span> <span data-ttu-id="de29e-117">Microsoft 将提供有关在将来实施主权云这些安全性要求的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-117">Microsoft will provide additional details regarding the enforcement of these security requirements for sovereign clouds in the future.</span></span>

## <a name="overview-of-the-requirements"></a><span data-ttu-id="de29e-118">要求概述</span><span class="sxs-lookup"><span data-stu-id="de29e-118">Overview of the requirements</span></span>

<span data-ttu-id="de29e-119">所有合作伙伴参与云解决方案提供商计划、 控制面板供应商和顾问合作伙伴都需要为每个用户在其合作伙伴租户中强制实施多重身份验证 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="de29e-119">All partners who are participating in the Cloud Solution Provider program, Control Panel Vendors, and Advisor partners are required to enforce Multi-Factor Authentication (MFA) for each user in their partner tenant.</span></span> <span data-ttu-id="de29e-120">这可以通过启用两个[Azure Active Directory 基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)。</span><span class="sxs-lookup"><span data-stu-id="de29e-120">This can be done by enabling two [Azure Active Directory baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).</span></span> <span data-ttu-id="de29e-121">基线策略是一组预定义策略来帮助保护组织针对许多常见的攻击。</span><span class="sxs-lookup"><span data-stu-id="de29e-121">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="de29e-122">这些常见的攻击可以包含密码喷射、 重播和网页仿冒欺诈。</span><span class="sxs-lookup"><span data-stu-id="de29e-122">These common attacks can include password spray, replay, and phishing.</span></span> <span data-ttu-id="de29e-123">所有版本的 Azure Active Directory 中提供了基线策略。</span><span class="sxs-lookup"><span data-stu-id="de29e-123">Baseline policies are available in all editions of Azure Active Directory.</span></span> <span data-ttu-id="de29e-124">Microsoft 向这些基线保护策略提供每个人都因为基于标识的攻击已过去几年的上升。</span><span class="sxs-lookup"><span data-stu-id="de29e-124">Microsoft is making these baseline protection policies available to everyone because identity-based attacks have been on the rise over the last few years.</span></span>

<span data-ttu-id="de29e-125">下表所述，应启用的两个基线策略。</span><span class="sxs-lookup"><span data-stu-id="de29e-125">The two baseline policies that should be enabled are described in the table below.</span></span>

|<span data-ttu-id="de29e-126">**策略**</span><span class="sxs-lookup"><span data-stu-id="de29e-126">**Policy**</span></span>| |
|-----|-----|
|<span data-ttu-id="de29e-127">**适用于管理员要求 MFA**</span><span class="sxs-lookup"><span data-stu-id="de29e-127">**Require MFA for admins**</span></span>|<span data-ttu-id="de29e-128">启用管理员策略需要 MFA，将要求管理员角色的用户注册 MFA 使用身份验证器应用。</span><span class="sxs-lookup"><span data-stu-id="de29e-128">Enabling the Require MFA for admins policy, will require users in the administrator roles  to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="de29e-129">MFA 注册完成后，管理员将需要执行 MFA，每次登录。</span><span class="sxs-lookup"><span data-stu-id="de29e-129">Once MFA registration is complete, administrators will need to perform MFA every time they sign-in.</span></span>|
|<span data-ttu-id="de29e-130">**最终用户保护**</span><span class="sxs-lookup"><span data-stu-id="de29e-130">**End user protection**</span></span>|<span data-ttu-id="de29e-131">最终用户保护是基于风险的 MFA 基线策略保护的目录中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="de29e-131">End user protection is a risk-based MFA baseline policy that protects all users in a directory.</span></span> <span data-ttu-id="de29e-132">如果启用此策略要求所有用户注册 MFA 使用身份验证器应用。</span><span class="sxs-lookup"><span data-stu-id="de29e-132">Enabling this policy requires all users to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="de29e-133">14 天，此后它们将无法登录，直到在注册 MFA，用户可以忽略 MFA 注册提示。</span><span class="sxs-lookup"><span data-stu-id="de29e-133">Users can ignore the MFA registration prompt for 14 days, after which they will be blocked from signing in until they register for MFA.</span></span> <span data-ttu-id="de29e-134">一旦注册 MFA，用户将会提示进行 MFA 仅在有风险的登录尝试。</span><span class="sxs-lookup"><span data-stu-id="de29e-134">Once registered for MFA, users will be prompted for MFA only during risky sign-in attempts.</span></span> <span data-ttu-id="de29e-135">重置其密码和已关闭风险事件之前，将阻止用户帐户泄露。</span><span class="sxs-lookup"><span data-stu-id="de29e-135">Compromised user accounts are blocked until their password is reset and risk events have been dismissed.</span></span>|

<span data-ttu-id="de29e-136">启用这些策略后，每个用户将能够利用 Azure MFA，且不另外收费。</span><span class="sxs-lookup"><span data-stu-id="de29e-136">When these policies are enabled, each user will be able to utilize Azure MFA at no additional cost.</span></span> <span data-ttu-id="de29e-137">如果使用第三方解决方案，然后需要访问 Microsoft 商业云服务时为每个用户强制实施 MFA。</span><span class="sxs-lookup"><span data-stu-id="de29e-137">If you are using a third-party solution, then you are required to enforce MFA for each user when accessing Microsoft Commercial cloud services.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="de29e-138">对于合作伙伴目录中的每个用户，将强制执行 MFA，因为会影响任何自动化或利用用户凭据的集成。</span><span class="sxs-lookup"><span data-stu-id="de29e-138">Since MFA will be enforced for every user in the partner directory, there will be an impact to any automation or integration that utilizes user credentials.</span></span> <span data-ttu-id="de29e-139">若要解决这种影响将需要修改的方式自动化或集成连接到 Microsoft 商业云服务。</span><span class="sxs-lookup"><span data-stu-id="de29e-139">To address this impact you will need to modify the way your automation or integration connects to Microsoft commercial cloud services.</span></span> <span data-ttu-id="de29e-140">如果要连接到该服务支持基于身份验证令牌，则我们建议你实现[保护应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)。</span><span class="sxs-lookup"><span data-stu-id="de29e-140">If the service you are connecting to supports token based authentication, then it is recommended that you implement the [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).</span></span>

## <a name="what-actions-do-i-need-to-take"></a><span data-ttu-id="de29e-141">我需要执行哪些操作？</span><span class="sxs-lookup"><span data-stu-id="de29e-141">What actions do I need to take?</span></span> 

<span data-ttu-id="de29e-142">若要确保伙伴中的每个用户受到保护，需要启用[适用于管理员要求使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)并[最终用户保护](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线策略。</span><span class="sxs-lookup"><span data-stu-id="de29e-142">To ensure each user in the partner is protected, you are required to enable the [Require MFA for admins](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) and [End user protection](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) baseline policies.</span></span> <span data-ttu-id="de29e-143">在启用这些策略之前, 务必理解他们执行的操作以及它们将如何影响任何自动化或集成和你的用户。</span><span class="sxs-lookup"><span data-stu-id="de29e-143">Prior to enabling these policies, it is important to understand what they do and how they will impact any automation or integration and your users.</span></span>

### <a name="considerations"></a><span data-ttu-id="de29e-144">注意事项</span><span class="sxs-lookup"><span data-stu-id="de29e-144">Considerations</span></span>

<span data-ttu-id="de29e-145">由于安全要求将应用于合作伙伴目录中的所有用户，几个注意事项需要进行，以确保顺利完成部署。</span><span class="sxs-lookup"><span data-stu-id="de29e-145">Because the security requirements apply to all users in a partner directory, several considerations need to be made to ensure a smooth deployment.</span></span> <span data-ttu-id="de29e-146">这些注意事项包括标识不能或不应执行 MFA，以及应用程序和由你的组织不支持新式身份验证的客户端的 Azure Active Directory 中的用户。</span><span class="sxs-lookup"><span data-stu-id="de29e-146">These considerations include identifying users in Azure Active Directory that cannot or should not perform MFA, as well as applications and clients used by your organization that do not support modern authentication.</span></span>

#### <a name="legacy-protocols"></a><span data-ttu-id="de29e-147">旧协议</span><span class="sxs-lookup"><span data-stu-id="de29e-147">Legacy protocols</span></span>

<span data-ttu-id="de29e-148">邮件客户端使用旧式身份验证协议 （IMAP、 SMTP、 POP3、 等） 进行身份验证请求。</span><span class="sxs-lookup"><span data-stu-id="de29e-148">Legacy authentication protocols (IMAP, SMTP, POP3, etc.) are used by mail clients to make authentication requests.</span></span> <span data-ttu-id="de29e-149">这些协议不支持 MFA。</span><span class="sxs-lookup"><span data-stu-id="de29e-149">These protocols do not support MFA.</span></span> <span data-ttu-id="de29e-150">大部分看到由 Microsoft 帐户破坏而引起不良参与方执行攻击试图绕过 MFA 的旧协议。</span><span class="sxs-lookup"><span data-stu-id="de29e-150">Most of the account compromises seen by Microsoft are caused by bad actors performing attacks against legacy protocols attempting to bypass MFA.</span></span> <span data-ttu-id="de29e-151">为了确保登录到合作伙伴目录中的帐户时需要 MFA 和不良参与方不能绕过 MFA，这些安全要求将阻止旧版协议中的所有身份验证请求。</span><span class="sxs-lookup"><span data-stu-id="de29e-151">To ensure that MFA is required when logging into an account in a partner directory and bad actors are not able to bypass MFA, these security requirements will block all authentication requests from legacy protocols.</span></span>

### <a name="enabling-the-baseline-policies"></a><span data-ttu-id="de29e-152">启用基线策略</span><span class="sxs-lookup"><span data-stu-id="de29e-152">Enabling the baseline policies</span></span>

<span data-ttu-id="de29e-153">请参阅[实现合作伙伴安全要求教程](tutorials/partner-security-requirements.yml)有关基线策略的实现提供引导式体验。</span><span class="sxs-lookup"><span data-stu-id="de29e-153">See the [Implementing the partner security requirements tutorial](tutorials/partner-security-requirements.yml) for a guided experience regarding the implementation of the baseline policies.</span></span>  

#### <a name="require-mfa-for-admins"></a><span data-ttu-id="de29e-154">适用于管理员要求 MFA</span><span class="sxs-lookup"><span data-stu-id="de29e-154">Require MFA for admins</span></span>

<span data-ttu-id="de29e-155">*管理员要求使用 MFA*基准策略要求使用 MFA 进行以下目录角色，被视为最高特权的 Azure Active Directory 角色：</span><span class="sxs-lookup"><span data-stu-id="de29e-155">The *Require MFA for admin* baseline policy requires MFA for the following directory roles, considered to be the most privileged Azure Active Directory roles:</span></span>

- <span data-ttu-id="de29e-156">全局管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-156">Global administrator</span></span>
- <span data-ttu-id="de29e-157">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-157">SharePoint administrator</span></span>
- <span data-ttu-id="de29e-158">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-158">Exchange administrator</span></span>
- <span data-ttu-id="de29e-159">条件性访问管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-159">Conditional access administrator</span></span>
- <span data-ttu-id="de29e-160">安全管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-160">Security administrator</span></span>
- <span data-ttu-id="de29e-161">支持管理员 / 密码管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-161">Helpdesk administrator / Password administrator</span></span>
- <span data-ttu-id="de29e-162">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-162">Billing administrator</span></span>
- <span data-ttu-id="de29e-163">用户管理员</span><span class="sxs-lookup"><span data-stu-id="de29e-163">User administrator</span></span>

<span data-ttu-id="de29e-164">启用管理员策略需要 MFA，时更高版本的九个管理员角色将需要使用身份验证器应用的 mfa 注册。</span><span class="sxs-lookup"><span data-stu-id="de29e-164">Upon enabling the Require MFA for admins policy, the above nine administrator roles will be required to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="de29e-165">MFA 注册完成后，管理员将需要执行每次登录的 MFA。</span><span class="sxs-lookup"><span data-stu-id="de29e-165">Once MFA registration is complete, administrators will need to perform MFA every single time they sign-in.</span></span>

<span data-ttu-id="de29e-166">如果你的组织中的脚本或代码中使用这些帐户，请考虑将它们替换为 [托管标识](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。</span><span class="sxs-lookup"><span data-stu-id="de29e-166">If your organization has these accounts in use in scripts or code, consider replacing them with [managed identities](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).</span></span>

<span data-ttu-id="de29e-167">若要启用此策略并保护你的管理员：</span><span class="sxs-lookup"><span data-stu-id="de29e-167">To enable this policy and protect your administrators:</span></span>

1. <span data-ttu-id="de29e-168">登录到 **Azure 门户** 作为全局管理员、 安全管理员或条件性访问管理员。</span><span class="sxs-lookup"><span data-stu-id="de29e-168">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>
2. <span data-ttu-id="de29e-169">浏览到**Azure Active Directory** > **条件性访问**。</span><span class="sxs-lookup"><span data-stu-id="de29e-169">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>
3. <span data-ttu-id="de29e-170">在策略列表中，选择**基准策略：适用于管理员要求 MFA**。</span><span class="sxs-lookup"><span data-stu-id="de29e-170">In the list of policies, select **Baseline policy: Require MFA for admins**.</span></span>
4. <span data-ttu-id="de29e-171">设置**启用策略**到**立即使用策略**。</span><span class="sxs-lookup"><span data-stu-id="de29e-171">Set **Enable policy** to **Use policy immediately**.</span></span>
5. <span data-ttu-id="de29e-172">单击 **保存**。</span><span class="sxs-lookup"><span data-stu-id="de29e-172">Click **Save**.</span></span>

    ![适用于管理员要求 MFA](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> <span data-ttu-id="de29e-174">启用此策略之前，请确保你的用户不使用传统的身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="de29e-174">Before you enable this policy, make sure your users are not using legacy authentication protocols.</span></span> <span data-ttu-id="de29e-175">请参阅文章[如何：阻止到 Azure Active Directory 条件性访问与传统的身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use)有关详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-175">See the article [How to: Block legacy authentication to Azure Active Directory with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) for more information.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="de29e-176">没有已知的问题，影响您连接到 Exchange Online PowerShell 使用委派管理权限的能力。</span><span class="sxs-lookup"><span data-stu-id="de29e-176">There is a known issue, that impacts your ability to connect to Exchange Online PowerShell using delegated administrative privileges.</span></span> <span data-ttu-id="de29e-177">请参阅[Exchange Online PowerShell](#exchange-online-powershell)已知问题之前启用此策略，如果您使用此 PowerShell 模块。</span><span class="sxs-lookup"><span data-stu-id="de29e-177">See the [Exchange Online PowerShell](#exchange-online-powershell) known issue prior to enabling this policy if you using this PowerShell module.</span></span>

#### <a name="end-user-protection"></a><span data-ttu-id="de29e-178">最终用户保护</span><span class="sxs-lookup"><span data-stu-id="de29e-178">End user protection</span></span>

<span data-ttu-id="de29e-179">最终用户保护基线策略保护的目录中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="de29e-179">The End user protection baseline policy protects all users in a directory.</span></span> <span data-ttu-id="de29e-180">如果启用此策略要求所有用户在 14 天内注册 Azure MFA。</span><span class="sxs-lookup"><span data-stu-id="de29e-180">Enabling this policy requires all users to register for Azure MFA within 14 days.</span></span> <span data-ttu-id="de29e-181">注册后，用户将会提示进行 MFA 仅在有风险的登录尝试。</span><span class="sxs-lookup"><span data-stu-id="de29e-181">Once registered, users will be prompted for MFA only during risky sign-in attempts.</span></span> <span data-ttu-id="de29e-182">密码重置和风险上诉之前，将阻止用户帐户泄露。</span><span class="sxs-lookup"><span data-stu-id="de29e-182">Compromised user accounts are blocked until password reset and risk dismissal.</span></span>

<span data-ttu-id="de29e-183">策略**基准策略：最终用户保护**预配置，此时将显示在顶部导航到在 Azure 门户中的条件性访问边栏选项卡时。</span><span class="sxs-lookup"><span data-stu-id="de29e-183">The policy **Baseline policy: End user protection** comes pre-configured and will show up at the top when you navigate to the Conditional Access blade in Azure portal.</span></span>

<span data-ttu-id="de29e-184">若要启用此策略并保护你的用户：</span><span class="sxs-lookup"><span data-stu-id="de29e-184">To enable this policy and protect your users:</span></span>

1. <span data-ttu-id="de29e-185">登录到 **Azure 门户** 作为全局管理员、 安全管理员或条件性访问管理员。</span><span class="sxs-lookup"><span data-stu-id="de29e-185">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>
2. <span data-ttu-id="de29e-186">浏览到**Azure Active Directory** > **条件性访问**。</span><span class="sxs-lookup"><span data-stu-id="de29e-186">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>
3. <span data-ttu-id="de29e-187">在策略列表中，选择**基准策略：最终用户保护 （预览版）** 。</span><span class="sxs-lookup"><span data-stu-id="de29e-187">In the list of policies, select **Baseline policy: End user protection (preview)**.</span></span>
4. <span data-ttu-id="de29e-188">设置**启用策略**到**立即使用策略**。</span><span class="sxs-lookup"><span data-stu-id="de29e-188">Set **Enable policy** to **Use policy immediately**.</span></span>
5. <span data-ttu-id="de29e-189">单击 **保存**。</span><span class="sxs-lookup"><span data-stu-id="de29e-189">Click **Save**.</span></span>

    ![最终用户保护](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> <span data-ttu-id="de29e-191">启用此策略之前，请确保你的用户不使用传统的身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="de29e-191">Before you enable this policy, make sure your users are not using legacy authentication protocols.</span></span> <span data-ttu-id="de29e-192">请参阅文章[如何：阻止到 Azure Active Directory 条件性访问与传统的身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use)有关详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-192">See the article [How to: Block legacy authentication to Azure Active Directory with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) for more information.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="de29e-193">没有已知的问题，影响您连接到 Exchange Online PowerShell 使用委派管理权限的能力。</span><span class="sxs-lookup"><span data-stu-id="de29e-193">There is a known issues, that impacts your ability to connect to Exchange Online PowerShell using delegated administrative privileges.</span></span> <span data-ttu-id="de29e-194">请参阅[Exchange Online PowerShell](#exchange-online-powershell)已知问题之前启用此策略，如果您使用此 PowerShell 模块。</span><span class="sxs-lookup"><span data-stu-id="de29e-194">See the [Exchange Online PowerShell](#exchange-online-powershell) known issue prior to enabling this policy if you using this PowerShell module.</span></span>

## <a name="common-issues"></a><span data-ttu-id="de29e-195">常见问题</span><span class="sxs-lookup"><span data-stu-id="de29e-195">Common issues</span></span>

### <a name="azure-active-directory"></a><span data-ttu-id="de29e-196">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="de29e-196">Azure Active Directory</span></span>

#### <a name="aadsts50076"></a><span data-ttu-id="de29e-197">AADSTS50076</span><span class="sxs-lookup"><span data-stu-id="de29e-197">AADSTS50076</span></span>

<span data-ttu-id="de29e-198">启用后基线策略，可能会发现你的自动化或集成遇到类似于下面的异常</span><span class="sxs-lookup"><span data-stu-id="de29e-198">After enabling the baseline policies, you might find that your automation or integration is encountering an exception similar to the following</span></span>

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

<span data-ttu-id="de29e-199">此异常的原因是要进行身份验证使用用户凭据，MFA 目前所需。</span><span class="sxs-lookup"><span data-stu-id="de29e-199">The reason for this exception is that you are authenticating using user credentials and MFA is now required.</span></span> <span data-ttu-id="de29e-200">若要解决此异常，您将需要使用访问令牌进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="de29e-200">To address this exception, you will need to utilize an access token for authentication.</span></span> <span data-ttu-id="de29e-201">请参阅[保护应用程序模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)有关详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-201">See the [Secure Application Model guide](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) for more information.</span></span>

>[!IMPORTANT]
><span data-ttu-id="de29e-202">大多数新式 Api 和 PowerShell 模块支持能够使用身份验证的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="de29e-202">Most modern APIs and PowerShell modules support the ability to utilize an access token for authentication.</span></span> <span data-ttu-id="de29e-203">但是，有一些当前不支持此功能。</span><span class="sxs-lookup"><span data-stu-id="de29e-203">However, there are some that currently do not support this functionality.</span></span> <span data-ttu-id="de29e-204">如果你需要帮助确定如果您尝试利用 API 或 PowerShell 模块支持使用访问令牌的身份验证，然后将消息发布在[合作伙伴中心安全指南组](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)社区。</span><span class="sxs-lookup"><span data-stu-id="de29e-204">If you need help determining if the API or PowerShell module you are trying to leverage supports the use of an access token for authentication, then post a message on the [Partner Center Security Guidance Group](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) community.</span></span>

#### <a name="aadsts700082"></a><span data-ttu-id="de29e-205">AADSTS700082</span><span class="sxs-lookup"><span data-stu-id="de29e-205">AADSTS700082</span></span>

<span data-ttu-id="de29e-206">实现安全应用程序模型框架后就可能会收到以下异常 90 天后生成了初始的刷新令牌</span><span class="sxs-lookup"><span data-stu-id="de29e-206">Once you have implemented the Secure Application Model framework there is a chance you will receive the following exception 90 days after generating the initial refresh token</span></span>

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

<span data-ttu-id="de29e-207">对于 Azure Active Directory 进行刷新的最长生存期令牌为 90 天。</span><span class="sxs-lookup"><span data-stu-id="de29e-207">With respect to Azure Active Directory the maximum lifetime for a refresh token is 90 days.</span></span> <span data-ttu-id="de29e-208">若要解决此错误，将需要生成并安全地将存储新的刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="de29e-208">To address this error, you will need to generate and securely store a new refresh token.</span></span> <span data-ttu-id="de29e-209">请注意可以以编程方式更新刷新令牌，因为与 Azure Active Directory 访问令牌的每个请求返回一个新的刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="de29e-209">Note it is possible to update the refresh token programmatically because with each request to Azure Active Directory for an access token a new refresh token is returned.</span></span> <span data-ttu-id="de29e-210">您可以实现相应的逻辑以安全地存储的刷新令牌过期之前进行更新。</span><span class="sxs-lookup"><span data-stu-id="de29e-210">You can implement the appropriate logic to update the securely stored refresh token before it expires.</span></span>

<span data-ttu-id="de29e-211">请参阅[Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)有关详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-211">See [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) for more information.</span></span>

## <a name="known-issues"></a><span data-ttu-id="de29e-212">已知问题</span><span class="sxs-lookup"><span data-stu-id="de29e-212">Known issues</span></span>

### <a name="exchange-online-powershell"></a><span data-ttu-id="de29e-213">Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="de29e-213">Exchange Online PowerShell</span></span>

<span data-ttu-id="de29e-214">启用 MFA 后合作伙伴不能利用其委派管理权限与 Exchange Online PowerShell，若要对其客户执行各种操作。</span><span class="sxs-lookup"><span data-stu-id="de29e-214">When MFA is enabled partners will not be able to utilize their delegated administrative privileges with Exchange Online PowerShell to perform actions against their customers.</span></span> <span data-ttu-id="de29e-215">请参阅[连接到使用多重身份验证的 Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)有关此限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-215">See [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) for more information regarding this limitation.</span></span>

## <a name="resources-and-support"></a><span data-ttu-id="de29e-216">资源和支持</span><span class="sxs-lookup"><span data-stu-id="de29e-216">Resources and support</span></span>

<span data-ttu-id="de29e-217">通过[合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)可以将查找其他资源并了解即将开展的活动，例如技术工作时间。</span><span class="sxs-lookup"><span data-stu-id="de29e-217">Through the [Partner Center Security Guidance Group community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) you can will find additional resources and learn about upcoming events such as technical office hours.</span></span> <span data-ttu-id="de29e-218">请参阅[方面的常见问题](http://assetsprod.microsoft.com/security-requirements-faq.pdf)文档，了解有关要求的详细信息。</span><span class="sxs-lookup"><span data-stu-id="de29e-218">See the [frequently asked questions](http://assetsprod.microsoft.com/security-requirements-faq.pdf) document to learn more about the requirements.</span></span>

### <a name="developers"></a><span data-ttu-id="de29e-219">开发人员</span><span class="sxs-lookup"><span data-stu-id="de29e-219">Developers</span></span>

- [<span data-ttu-id="de29e-220">启用安全的应用程序模型</span><span class="sxs-lookup"><span data-stu-id="de29e-220">Enabling the Secure Application Model</span></span>](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [<span data-ttu-id="de29e-221">合作伙伴中心.NET 示例</span><span class="sxs-lookup"><span data-stu-id="de29e-221">Partner Center .NET Samples</span></span>](https://github.com/microsoft/partner-center-dotnet-samples)
- [<span data-ttu-id="de29e-222">合作伙伴中心的 Java 示例</span><span class="sxs-lookup"><span data-stu-id="de29e-222">Partner Center Java Samples</span></span>](https://github.com/microsoft/partner-center-java-samples)
- [<span data-ttu-id="de29e-223">合作伙伴中心 PowerShell 实现安全应用程序模型</span><span class="sxs-lookup"><span data-stu-id="de29e-223">Partner Center PowerShell implementing the Secure Application Model</span></span>](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
