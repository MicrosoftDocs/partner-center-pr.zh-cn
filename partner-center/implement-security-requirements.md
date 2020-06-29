---
title: 实现合作伙伴安全要求
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何为用户实现必要的安全要求
author: LauraBrenner
ms.author: labrenne
keywords: 安全性
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133260"
---
# <a name="implement-the-partner-security-requirements"></a><span data-ttu-id="df09a-104">实现合作伙伴安全要求</span><span class="sxs-lookup"><span data-stu-id="df09a-104">Implement the partner security requirements</span></span>

<span data-ttu-id="df09a-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="df09a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="df09a-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-106">Global admin</span></span>

<span data-ttu-id="df09a-107">客户和合作伙伴的安全和隐私是 Microsoft 首要关注的重点。</span><span class="sxs-lookup"><span data-stu-id="df09a-107">Security and privacy of customers and partners are top priorities for Microsoft.</span></span> <span data-ttu-id="df09a-108">我们不断看到有越来越多更为复杂的安全攻击在发生，这些安全攻击主要与身份遭到泄露相关。</span><span class="sxs-lookup"><span data-stu-id="df09a-108">We continue to see an increasing number of more sophisticated security attacks, primarily related to compromised identities.</span></span> <span data-ttu-id="df09a-109">若要通过整体防御策略来阻止安全攻击，预防性的控制至关重要，因此我们将开始实施一系列强制性安全要求，以便对合作伙伴及其客户进行保护。</span><span class="sxs-lookup"><span data-stu-id="df09a-109">As preventive controls play a key role in an overall defense strategy to thwart security attacks, we will start enforcing a set of mandatory security requirements to help protect partners and their customers.</span></span>

<span data-ttu-id="df09a-110">本教程将介绍合作伙伴安全要求的详细信息，并介绍如何满足这些要求以及对合作伙伴目录中的用户所产生的影响。</span><span class="sxs-lookup"><span data-stu-id="df09a-110">Through this tutorial you will learn more about the partner security requirements, how to fulfill them, and the impact to users in your partner directory.</span></span>

<span data-ttu-id="df09a-111">所有参与云解决方案提供商计划的合作伙伴、控制面板供应商和顾问合作伙伴都需要对他们合作伙伴租户中的每位用户强制实施多重身份验证 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="df09a-111">All partners who are participating in the Cloud Solution Provider program, Control Panel Vendors, and Advisor partners are required to enforce Multi-Factor Authentication (MFA) for each user in their partner tenant.</span></span> <span data-ttu-id="df09a-112">这一实施可以通过启用两种 [Azure Active Directory 基线策略](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)来完成。</span><span class="sxs-lookup"><span data-stu-id="df09a-112">This enforcement can be done by enabling two [Azure Active Directory baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).</span></span> <span data-ttu-id="df09a-113">基线策略是一组预定义的策略，用于帮助组织防范许多常见攻击。</span><span class="sxs-lookup"><span data-stu-id="df09a-113">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="df09a-114">这些常见攻击可能包括密码喷射、重播和钓鱼。</span><span class="sxs-lookup"><span data-stu-id="df09a-114">These common attacks can include password spray, replay, and phishing.</span></span> <span data-ttu-id="df09a-115">基线策略在所有版本的 Azure Active Directory 中提供。</span><span class="sxs-lookup"><span data-stu-id="df09a-115">Baseline policies are available in all editions of Azure Active Directory.</span></span> <span data-ttu-id="df09a-116">Microsoft 会将这些基线保护策略提供给所有人，因为基于身份的攻击在过去几年呈上升趋势。</span><span class="sxs-lookup"><span data-stu-id="df09a-116">Microsoft is making these baseline protection policies available to everyone because identity-based attacks have been on the rise over the last few years.</span></span>

<span data-ttu-id="df09a-117">以下过程描述了如何启用两个必需的基线策略：</span><span class="sxs-lookup"><span data-stu-id="df09a-117">The procedures below describe the process of enabling the two necessary baseline policies:</span></span>

- <span data-ttu-id="df09a-118">**对管理员要求 MFA** 启用“对管理员要求 MFA”策略后，担任管理员角色的用户需要使用 Authenticator 应用来注册 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-118">**Require MFA for admins**  Enabling the Require MFA for admins policy will require users in the administrator roles to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="df09a-119">完成 MFA 注册以后，管理员在每次登录时都需要执行 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-119">Once MFA registration is complete, administrators will need to perform MFA every time they sign-in.</span></span>

- <span data-ttu-id="df09a-120">**最终用户保护** “最终用户保护”是一种基于风险的 MFA 基线策略，用于保护目录中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="df09a-120">**End user protection**  End user protection is a risk-based MFA baseline policy that protects all users in a directory.</span></span> <span data-ttu-id="df09a-121">启用此策略以后，所有用户就必须使用 Authenticator 应用注册 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-121">Enabling this policy requires all users to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="df09a-122">用户可以忽略 MFA 注册提示 14 天，此期限过后系统会阻止用户登录，直至用户注册 MFA 为止。</span><span class="sxs-lookup"><span data-stu-id="df09a-122">Users can ignore the MFA registration prompt for 14 days, after which they will be blocked from signing in until they register for MFA.</span></span> <span data-ttu-id="df09a-123">注册 MFA 以后，系统仅在检测到风险登录尝试时提示用户进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-123">Once registered for MFA, users will be prompted for MFA only during risky sign-in attempts.</span></span> <span data-ttu-id="df09a-124">系统会阻止被盗用的用户帐户，直至用户重置密码并消除风险事件为止。</span><span class="sxs-lookup"><span data-stu-id="df09a-124">Compromised user accounts are blocked until their password is reset and risk events have been dismissed.</span></span>

<span data-ttu-id="df09a-125">启用这些策略后，每位用户都能够使用 Azure MFA，无需额外成本。</span><span class="sxs-lookup"><span data-stu-id="df09a-125">Once these policies are enabled, each user will be able to utilize Azure MFA at no additional cost.</span></span> <span data-ttu-id="df09a-126">如果你使用的是第三方解决方案，则需要在每位用户访问 Microsoft 商业云服务时对他们强制实施 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-126">If you are using a third-party solution, then you are required to enforce MFA for each user when accessing Microsoft Commercial cloud services.</span></span>

>[!NOTE]
><span data-ttu-id="df09a-127">由于将对合作伙伴目录中的每位用户强制实施 MFA，因此利用用户凭据的所有自动化或集成都将受到影响。</span><span class="sxs-lookup"><span data-stu-id="df09a-127">Since MFA will be enforced for every user in the partner directory, there will be an impact to any automation or integration that utilizes user credentials.</span></span> <span data-ttu-id="df09a-128">若要消除这种影响，你需要修改将自动化或集成连接到 Microsoft 商业云服务的方式。</span><span class="sxs-lookup"><span data-stu-id="df09a-128">To address this impact, you will need to modify the way your automation or integration connects to Microsoft commercial cloud services.</span></span> <span data-ttu-id="df09a-129">如果所连接的服务支持基于令牌的身份验证，我们建议你实现[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)。</span><span class="sxs-lookup"><span data-stu-id="df09a-129">If the service you are connecting to supports token-based authentication, then it is recommended that you implement the [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).</span></span>

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a><span data-ttu-id="df09a-130">步骤一：阻止任何现有的旧版身份验证协议</span><span class="sxs-lookup"><span data-stu-id="df09a-130">Step one: Block any existing legacy authentication protocols</span></span>

<span data-ttu-id="df09a-131">启用“对管理员和最终用户保护要求 MFA”前，请确保用户未使用旧版身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="df09a-131">Before you enable the Require MFA for admins and End user protection policies, ensure that your users are not using legacy authentication protocols.</span></span> <span data-ttu-id="df09a-132">请参阅[如何：使用条件访问阻止向 Azure AD 进行旧身份验证](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use)一文以了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="df09a-132">See the article [How to: Block legacy authentication to Azure AD with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) for more information.</span></span>

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a><span data-ttu-id="df09a-133">步骤二：启用“对管理员要求 MFA”基线策略</span><span class="sxs-lookup"><span data-stu-id="df09a-133">Step two: Enable the Require MFA for admins baseline policy</span></span>

<span data-ttu-id="df09a-134">“对管理员要求 MFA”基线策略要求对以下目录角色实施 MFA，这些角色被认为是具有最高特权的 Azure AD 角色：</span><span class="sxs-lookup"><span data-stu-id="df09a-134">The Require MFA for admin baseline policy requires MFA for the following directory roles, considered to be the most privileged Azure AD roles:</span></span>

- <span data-ttu-id="df09a-135">全局管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-135">Global administrator</span></span>
- <span data-ttu-id="df09a-136">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-136">SharePoint administrator</span></span>
- <span data-ttu-id="df09a-137">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-137">Exchange administrator</span></span>
- <span data-ttu-id="df09a-138">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-138">Conditional access administrator</span></span>
- <span data-ttu-id="df09a-139">安全管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-139">Security administrator</span></span>
- <span data-ttu-id="df09a-140">支持管理员/密码管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-140">Helpdesk administrator/Password administrator</span></span>
- <span data-ttu-id="df09a-141">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-141">Billing administrator</span></span>
- <span data-ttu-id="df09a-142">用户管理员</span><span class="sxs-lookup"><span data-stu-id="df09a-142">User administrator</span></span>

<span data-ttu-id="df09a-143">启用“对管理员要求 MFA”策略以后，以上九种管理员角色就必须使用 Authenticator 应用注册 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-143">Upon enabling the Require MFA for admins policy, the above nine administrator roles will be required to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="df09a-144">完成 MFA 注册以后，管理员在每次登录时都需要执行 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-144">Once MFA registration is complete, administrators will need to perform MFA every single time they sign-in.</span></span>

<span data-ttu-id="df09a-145">如果组织在脚本或代码中使用这些帐户，请考虑将其替换为 [托管标识](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。</span><span class="sxs-lookup"><span data-stu-id="df09a-145">If your organization has these accounts in use in scripts or code, consider replacing them with [managed identities](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).</span></span>

<span data-ttu-id="df09a-146">若要启用此策略并保护管理员，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="df09a-146">To enable this policy and protect your administrators:</span></span>

1. <span data-ttu-id="df09a-147">以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户** 。</span><span class="sxs-lookup"><span data-stu-id="df09a-147">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="df09a-148">浏览到“Azure Active Directory” > “条件访问”。</span><span class="sxs-lookup"><span data-stu-id="df09a-148">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="df09a-149">在策略列表中，选择“基线策略:对管理员要求 MFA”。</span><span class="sxs-lookup"><span data-stu-id="df09a-149">In the list of policies, select **Baseline policy: Require MFA for admins**.</span></span>

4. <span data-ttu-id="df09a-150">将“启用策略”设置为“立即使用策略”。 </span><span class="sxs-lookup"><span data-stu-id="df09a-150">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="df09a-151">选择“保存” \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="df09a-151">Select **Save**.</span></span>

<span data-ttu-id="df09a-152">启用此策略后，将在登录时提示具有上述管理员角色的用户提供其他安全信息并配置移动应用。</span><span class="sxs-lookup"><span data-stu-id="df09a-152">Once you’ve enabled this policy, users in the above administrator roles will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="df09a-153">完成此操作后，他们将能够登录到相应的云服务。</span><span class="sxs-lookup"><span data-stu-id="df09a-153">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a><span data-ttu-id="df09a-154">步骤三：启用“最终用户保护”基线策略</span><span class="sxs-lookup"><span data-stu-id="df09a-154">Step three: Enable the End user protection baseline policy</span></span>

<span data-ttu-id="df09a-155">“最终用户保护”基线策略保护目录中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="df09a-155">The End user protection baseline policy protects all users in a directory.</span></span> <span data-ttu-id="df09a-156">启用此策略以后，所有用户就必须在 14 天内注册 Azure MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-156">Enabling this policy requires all users to register for Azure MFA within 14 days.</span></span> <span data-ttu-id="df09a-157">注册后，系统将仅在出现存在风险的登录尝试期间提示用户进行 MFA，此行为未来将针对合作伙伴租户有所更改。</span><span class="sxs-lookup"><span data-stu-id="df09a-157">Once registered, users will be prompted for MFA only during risky sign-in attempts, this behavior will change for partner tenants in the future.</span></span> <span data-ttu-id="df09a-158">系统会阻止被盗用的用户帐户，直至用户重置密码并消除风险为止。</span><span class="sxs-lookup"><span data-stu-id="df09a-158">Compromised user accounts are blocked until password reset and risk dismissal.</span></span>

<span data-ttu-id="df09a-159">策略“基线策略：最终用户保护”已预先配置。当你在 Azure 门户中导航到“条件访问”边栏选项卡时，会在顶部看到它。</span><span class="sxs-lookup"><span data-stu-id="df09a-159">The policy Baseline policy: End user protection comes pre-configured and will show up at the top when you navigate to the Conditional Access blade in Azure portal.</span></span>

<span data-ttu-id="df09a-160">若要启用此策略并保护用户，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="df09a-160">To enable this policy and protect your users:</span></span>

1. <span data-ttu-id="df09a-161">以全局管理员、安全管理员或条件访问管理员身份登录到 **Azure 门户** 。</span><span class="sxs-lookup"><span data-stu-id="df09a-161">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="df09a-162">浏览到“Azure Active Directory” > “条件访问”。</span><span class="sxs-lookup"><span data-stu-id="df09a-162">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="df09a-163">在策略列表中，选择“基线策略:最终用户保护(预览)”。</span><span class="sxs-lookup"><span data-stu-id="df09a-163">In the list of policies, select **Baseline policy: End user protection (preview)**.</span></span>

4. <span data-ttu-id="df09a-164">将“启用策略”设置为“立即使用策略”。 </span><span class="sxs-lookup"><span data-stu-id="df09a-164">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="df09a-165">选择“保存” \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="df09a-165">Select **Save**.</span></span>

<span data-ttu-id="df09a-166">启用此策略后，将在登录时提示所有用户提供其他安全信息并配置移动应用。</span><span class="sxs-lookup"><span data-stu-id="df09a-166">Once you’ve enabled this policy, all users will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="df09a-167">完成此操作后，他们将能够登录到相应的云服务。</span><span class="sxs-lookup"><span data-stu-id="df09a-167">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

>[!NOTE]
><span data-ttu-id="df09a-168">在合作伙伴安全要求强制实施之前，系统将仅基于风险提示未被“对管理员要求 MFA”基线策略涵盖的用户进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="df09a-168">Until the partner security requirements are enforced, users who are not covered by the Require MFA for admins baseline policy will only be prompted for MFA based on risk.</span></span>