---
title: 合作伙伴安全要求 | 合作伙伴中心
ms.topic: article
ms.date: 10/11/2019
description: 了解对参与云解决方案提供商计划的顾问和合作伙伴的安全要求。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 云解决方案提供商, 云解决方案提供商计划, CSP, 控制面板供应商, CPV, 多重身份验证, MFA, 安全应用程序模型, 安全应用模型, 安全性
ms.localizationpriority: high
ms.openlocfilehash: b09588387d3b4f0f3f726a700245999c89755199
ms.sourcegitcommit: 9dd6f1ee0ebc132442126340c9df8cf7e3e1d3ad
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "72425201"
---
# <a name="partner-security-requirements"></a><span data-ttu-id="39dd1-104">合作伙伴安全要求</span><span class="sxs-lookup"><span data-stu-id="39dd1-104">Partner Security Requirements</span></span>

<span data-ttu-id="39dd1-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="39dd1-105">**Applies to**</span></span>

- <span data-ttu-id="39dd1-106">云解决方案提供商计划中的所有合作伙伴</span><span class="sxs-lookup"><span data-stu-id="39dd1-106">All partners in the Cloud Solution Provider program</span></span>
  - <span data-ttu-id="39dd1-107">直接计费</span><span class="sxs-lookup"><span data-stu-id="39dd1-107">Direct bill</span></span>
  - <span data-ttu-id="39dd1-108">间接提供商</span><span class="sxs-lookup"><span data-stu-id="39dd1-108">Indirect provider</span></span>
  - <span data-ttu-id="39dd1-109">间接经销商</span><span class="sxs-lookup"><span data-stu-id="39dd1-109">Indirect reseller</span></span>
- <span data-ttu-id="39dd1-110">所有控制面板供应商</span><span class="sxs-lookup"><span data-stu-id="39dd1-110">All Control Panel Vendors</span></span>
- <span data-ttu-id="39dd1-111">所有顾问</span><span class="sxs-lookup"><span data-stu-id="39dd1-111">All Advisors</span></span>

<span data-ttu-id="39dd1-112">增强隐私保护和安全性是我们优先关注的事项。</span><span class="sxs-lookup"><span data-stu-id="39dd1-112">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="39dd1-113">我们知道，最好的防御措施是防患于未然，链条的强度取决于其最弱的一环。</span><span class="sxs-lookup"><span data-stu-id="39dd1-113">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="39dd1-114">因此，我们需要生态系统中的所有人都行动起来，确保将安全保护措施实施到位。</span><span class="sxs-lookup"><span data-stu-id="39dd1-114">That is why we need everyone in our ecosystem to act and ensure they have appropriate security protections in place.</span></span> <span data-ttu-id="39dd1-115">为了保护合作伙伴和客户，我们引入了一系列强制性安全要求，针对那些参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="39dd1-115">To help safeguard partners and customers, we are introducing a set of mandatory security requirements for Advisors, Control Panel Vendors, and partners participating in the Cloud Solution Provider program.</span></span>

## <a name="overview"></a><span data-ttu-id="39dd1-116">概述</span><span class="sxs-lookup"><span data-stu-id="39dd1-116">Overview</span></span>

<span data-ttu-id="39dd1-117">从 2019 年 8 月 1 日开始，所有合作伙伴都必须对其合作伙伴租户中的所有用户帐户强制实施多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-117">Starting August 1, 2019 all partners are required to enforce multi-factor authentication for all user accounts in their partner tenant.</span></span> <span data-ttu-id="39dd1-118">与合作伙伴安全要求相关的条款已添加到[云解决方案提供商计划指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)中。</span><span class="sxs-lookup"><span data-stu-id="39dd1-118">The terms associated with the partner security requirements have been added to the [Cloud Solution Provider program guide](https://go.microsoft.com/fwlink/p/?LinkId=617100).</span></span> <span data-ttu-id="39dd1-119">由于与顾问相关，因此会实施相同的合同要求。</span><span class="sxs-lookup"><span data-stu-id="39dd1-119">As it relates to Advisors the same contractual requirements will be in place.</span></span>

> [!NOTE]
> <span data-ttu-id="39dd1-120">强烈建议所有通过主权云（世纪互联、Microsoft Cloud for US Government、德国 Microsoft 云）进行事务处理的合作伙伴立即行动起来，履行这些安全要求。</span><span class="sxs-lookup"><span data-stu-id="39dd1-120">We strongly recommend that all partners transacting through a sovereign cloud (21Vianet, US Government, and Germany) act and adopt these security requirements immediately.</span></span> <span data-ttu-id="39dd1-121">但是，这些合作伙伴不是必须满足这些在 2019 年 8 月 1 日生效的安全要求。</span><span class="sxs-lookup"><span data-stu-id="39dd1-121">However, these partners are not required to meet the  security requirements effective August 1, 2019.</span></span> <span data-ttu-id="39dd1-122">Microsoft 会在以后更详细地说明如何强制实施这些针对主权云的安全要求。</span><span class="sxs-lookup"><span data-stu-id="39dd1-122">Microsoft will provide additional details regarding the enforcement of these security requirements for sovereign clouds in the future.</span></span>

<span data-ttu-id="39dd1-123">一旦我们强制实施这些安全要求，不实施这些强制性要求的合作伙伴将不能在云解决方案提供商计划中进行事务处理，也不能利用委托管理权限来管理客户租户。</span><span class="sxs-lookup"><span data-stu-id="39dd1-123">Partners who do not implement the mandatory security requirements will not be able to transact in the Cloud Solution Provider program or manage customer tenants leveraging delegate admin rights, once these requirements are enforced.</span></span>

## <a name="actions-that-you-need-to-take"></a><span data-ttu-id="39dd1-124">需要采取的措施</span><span class="sxs-lookup"><span data-stu-id="39dd1-124">Actions that you need to take</span></span>

<span data-ttu-id="39dd1-125">若要符合合作伙伴安全要求，你必须为合作伙伴租户中的每个用户帐户强制实施多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-125">To comply with the partner security requirements you must enforce multi-factor authentication for each user account in your partner tenant.</span></span> <span data-ttu-id="39dd1-126">可以通过下述方式之一来实现这一点</span><span class="sxs-lookup"><span data-stu-id="39dd1-126">This can be accomplished through one of the way following ways</span></span>

- <span data-ttu-id="39dd1-127">实现 Azure Active Directory 提供的[对管理员要求 MFA](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 和[最终用户保护](/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基线保护策略功能，不需额外付费</span><span class="sxs-lookup"><span data-stu-id="39dd1-127">Implementing the [Require MFA for admins](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) and [End user protection](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) baseline protection policies feature from Azure Active Directory at no additional cost</span></span>
- <span data-ttu-id="39dd1-128">为每个用户帐户购买 Azure Active Directory Premium。</span><span class="sxs-lookup"><span data-stu-id="39dd1-128">Purchasing Azure Active Directory Premium for each user account.</span></span> <span data-ttu-id="39dd1-129">有关详细信息，请参阅[规划基于云的 Azure 多重身份验证部署](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)。</span><span class="sxs-lookup"><span data-stu-id="39dd1-129">See [Planning a cloud-based Azure Multi-Factor Authentication deployment](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted) for more information.</span></span>
- <span data-ttu-id="39dd1-130">使用第三方解决方案为合作伙伴租户中的每个用户帐户强制实施多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-130">Using a third-party solution to enforce multi-factor authentication for each user account in your partner tenant.</span></span> <span data-ttu-id="39dd1-131">请参阅[如何强制实施安全要求](#how-the-requirements-will-be-enforced)，更详细地了解如何确保解决方案会提供预期的信息。</span><span class="sxs-lookup"><span data-stu-id="39dd1-131">See [how the security requirements will be enforced](#how-the-requirements-will-be-enforced) for more details to ensure the solution will provide the expected information.</span></span>

### <a name="consideration"></a><span data-ttu-id="39dd1-132">注意事项</span><span class="sxs-lookup"><span data-stu-id="39dd1-132">Consideration</span></span>

<span data-ttu-id="39dd1-133">由于这些要求适用于合作伙伴租户中的所有用户帐户，因此需要遵守一些注意事项，确保顺利进行部署。</span><span class="sxs-lookup"><span data-stu-id="39dd1-133">Because these requirements apply to all user accounts in your partner tenant, there are several considerations that need to be made to ensure a smooth deployment.</span></span> <span data-ttu-id="39dd1-134">这些注意事项包括确定 Azure Active Directory 中不能执行多重身份验证的用户帐户，以及组织所使用的不支持新式身份验证的应用程序和设备。</span><span class="sxs-lookup"><span data-stu-id="39dd1-134">These considerations include identifying user accounts in Azure Active Directory that cannot perform multi-factor authentication, as well as applications and devices used by your organization that do not support modern authentication.</span></span>

<span data-ttu-id="39dd1-135">建议在执行任何操作之前确定以下事项：</span><span class="sxs-lookup"><span data-stu-id="39dd1-135">Prior to performing any action, it is recommended that you identify the following</span></span>

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a><span data-ttu-id="39dd1-136">你是否有不支持使用新式身份验证的应用程序或设备？</span><span class="sxs-lookup"><span data-stu-id="39dd1-136">Do you have an application or device that does not support the use of modern authentication?</span></span>

<span data-ttu-id="39dd1-137">强制实施多重身份验证时，系统会阻止旧版身份验证协议（例如 IMAP、POP3、SMTP 等）的使用，因为这些协议不支持多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-137">When you enforce multi-factor authentication legacy authentication use protocols such as IMAP, POP3, SMTP, etc. will be blocked because these protocols do not support multi-factor authentication.</span></span> <span data-ttu-id="39dd1-138">为了解决此限制问题，可以使用名为[应用密码](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)的功能，确保应用程序或设备仍然能够进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-138">To address this limitation a feature known as [app passwords](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) can be used to ensure the application or device can still authenticate.</span></span> <span data-ttu-id="39dd1-139">你应该查看[此处](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)记录的应用密码使用注意事项，确定应用密码是否可以在你的环境中使用。</span><span class="sxs-lookup"><span data-stu-id="39dd1-139">You should review the considerations for using app passwords documented [here](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) to determine if they can be used in your environment.</span></span>

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a><span data-ttu-id="39dd1-140">你是否有用户使用通过与合作伙伴租户相关联的许可证获得的 Office 365？</span><span class="sxs-lookup"><span data-stu-id="39dd1-140">Do you have users using Office 365 provided by licenses associated with your partner tenant?</span></span>

<span data-ttu-id="39dd1-141">在实现任何解决方案之前，建议你确定合作伙伴租户中的用户所使用的 Microsoft Office 版本。</span><span class="sxs-lookup"><span data-stu-id="39dd1-141">Prior to implementing any solution, it is recommended that you determine what version of Microsoft Office is being used by users in your partner tenant.</span></span> <span data-ttu-id="39dd1-142">在采取任何行动之前，请参阅 [Office 365 部署的多重身份验证计划](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)。</span><span class="sxs-lookup"><span data-stu-id="39dd1-142">Review [plan for multi-factor authentication for Office 365 Deployments](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) before taking any action.</span></span> <span data-ttu-id="39dd1-143">用户可能会在使用 Outlook 之类的应用程序时遇到连接问题。</span><span class="sxs-lookup"><span data-stu-id="39dd1-143">There is a chance your users will experience connectivity issues with applications like Outlook.</span></span> <span data-ttu-id="39dd1-144">在强制实施多重身份验证之前，必须确保使用的是 Outlook 2013 SP1 或更高版本，且组织已启用新式身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-144">Before enforcing multi-factor authentication, it is important to ensure that Outlook 2013 SP1, or later, is being used and that your organization has modern authentication enabled.</span></span> <span data-ttu-id="39dd1-145">有关详细信息，请参阅[在 Exchange Online 中启用新式身份验证](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="39dd1-145">See [Enable modern authentication in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) for more information.</span></span>

<span data-ttu-id="39dd1-146">若要为任何运行 Windows 且已安装 Microsoft Office 2013 的设备启用新式身份验证，需创建两个注册表项。</span><span class="sxs-lookup"><span data-stu-id="39dd1-146">To enable modern authentication for any devices running Windows, that have Microsoft Office 2013 installed, you will need to create two registry keys.</span></span> <span data-ttu-id="39dd1-147">请参阅[在 Windows 设备上启用适用于 Office 2013 的新式身份验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="39dd1-147">See [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a><span data-ttu-id="39dd1-148">是否有策略阻止用户在工作时使用其移动设备？</span><span class="sxs-lookup"><span data-stu-id="39dd1-148">Is there a policy preventing any of your users from using their mobile devices while working?</span></span>

<span data-ttu-id="39dd1-149">必须确定任何阻止员工在工作时使用移动设备的公司策略，因为它会影响你实现的具体的多重身份验证解决方案。</span><span class="sxs-lookup"><span data-stu-id="39dd1-149">It is important to identify any corporate policy that prevents employees from using mobile devices while working because it will influence what multi-factor authentication solution you implement.</span></span> <span data-ttu-id="39dd1-150">有的解决方案（例如通过实施[基线保护策略](/azure/active-directory/conditional-access/concept-baseline-protection)提供的解决方案）仅允许使用 Authenticator 应用进行验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-150">There are solutions, such as the one provided through the implementation of [baseline protection policies](/azure/active-directory/conditional-access/concept-baseline-protection), that only allow the use of an authenticator app for verification.</span></span> <span data-ttu-id="39dd1-151">如果组织的某项策略阻止使用移动设备，则应考虑以下选项之一：</span><span class="sxs-lookup"><span data-stu-id="39dd1-151">In the event your organization has a policy that prevent the use of mobile devices, then you should consider one of the following options</span></span>

- <span data-ttu-id="39dd1-152">部署可以在安全系统上运行的基于时间的一次性密码 (TOTP) 应用程序</span><span class="sxs-lookup"><span data-stu-id="39dd1-152">Deploy a time-based one-time base password (TOTP) application that can run on secure system</span></span>
- <span data-ttu-id="39dd1-153">实现第三方解决方案，为合作伙伴租户中的每个用户帐户强制实施多重身份验证，以便提供最适当的验证选项</span><span class="sxs-lookup"><span data-stu-id="39dd1-153">Implement a third-party solution that enforces multi-factor authentication for each user account in the partner tenant that provides the most appropriate verification option</span></span>
- <span data-ttu-id="39dd1-154">为受影响的用户购买 [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) 许可证</span><span class="sxs-lookup"><span data-stu-id="39dd1-154">Purchase [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) licenses for the impacted users</span></span>

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a><span data-ttu-id="39dd1-155">你有什么样的利用用户凭据进行身份验证的自动化或集成？</span><span class="sxs-lookup"><span data-stu-id="39dd1-155">What automation or integration do you have that leverages user credentials for authentication?</span></span>

<span data-ttu-id="39dd1-156">由于此要求是对合作伙伴目录中的每位用户（包括服务帐户）强制实施 MFA，因此任何利用用户凭据进行身份验证的自动化或集成都会受影响。</span><span class="sxs-lookup"><span data-stu-id="39dd1-156">Since the requirement is to enforce MFA for each user, including service accounts, in your partner directory any automation or integration that leverages user credentials for authentication will be impacted.</span></span> <span data-ttu-id="39dd1-157">因此，必须确定在这些情况下使用的是什么帐户。</span><span class="sxs-lookup"><span data-stu-id="39dd1-157">So, it important that you identify what accounts are being used in these situations.</span></span> <span data-ttu-id="39dd1-158">下面是一个列表，其中包含应该考虑的应用程序或服务的示例：</span><span class="sxs-lookup"><span data-stu-id="39dd1-158">The following is a list of examples of applications or services that should be considered</span></span>

- <span data-ttu-id="39dd1-159">控制面板，用于代表客户预配资源</span><span class="sxs-lookup"><span data-stu-id="39dd1-159">Control panel used to provision resources on behalf of your customers</span></span>
- <span data-ttu-id="39dd1-160">与任何用于客户发票（由于与 CSP 计划相关）和支持的平台的集成</span><span class="sxs-lookup"><span data-stu-id="39dd1-160">Integration with any platform that is used for invoicing (as it relates to the CSP program) and supporting your customers</span></span>
- <span data-ttu-id="39dd1-161">利用 Az、AzureRM、Azure AD、MS Online 等模块的 PowerShell 脚本</span><span class="sxs-lookup"><span data-stu-id="39dd1-161">PowerShell scripts that utilize the Az, AzureRM, Azure AD, MS Online, etc. modules</span></span>

<span data-ttu-id="39dd1-162">以上列表并不完整。</span><span class="sxs-lookup"><span data-stu-id="39dd1-162">The above list is not comprehensive.</span></span> <span data-ttu-id="39dd1-163">因此，必须对环境中利用用户凭据进行身份验证的任何应用程序或服务进行完整的评估。</span><span class="sxs-lookup"><span data-stu-id="39dd1-163">So, it important that you perform a complete assessment of any application or service in your environment that leverages user credentials for authentication.</span></span> <span data-ttu-id="39dd1-164">在可能情况下，应该按[安全应用程序模型框架](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)中的指南（不同于多重身份验证的要求）进行操作。</span><span class="sxs-lookup"><span data-stu-id="39dd1-164">To contend with the requirement for multi-factor authentication, you should implement the guidance in the [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) where possible.</span></span>

## <a name="accessing-your-environment"></a><span data-ttu-id="39dd1-165">访问环境</span><span class="sxs-lookup"><span data-stu-id="39dd1-165">Accessing your environment</span></span>

<span data-ttu-id="39dd1-166">若要更好地了解哪个帐户或用户在进行身份验证时没有受到多重身份验证质询，建议查询 Azure Active Directory 审核日志。</span><span class="sxs-lookup"><span data-stu-id="39dd1-166">To better understand what or who is authenticating without being challenged for multi-factor authentication, it is recommended to query the Azure Active Directory audit logs.</span></span> <span data-ttu-id="39dd1-167">为此，可以使用 [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) 模块和下面的脚本。</span><span class="sxs-lookup"><span data-stu-id="39dd1-167">This can be accomplished using the [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) module and the script below.</span></span> <span data-ttu-id="39dd1-168">这样会生成一个报表，该报表详细说明了过去一天内发生的哪些身份验证尝试没有受到多重身份验证质询。</span><span class="sxs-lookup"><span data-stu-id="39dd1-168">It will generate a report that provides insight into what authentication attempts have occurred over the past day that were not challenged for multi-factor authentication.</span></span>

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false -and $_.loginSucceeded -eq $true} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

<span data-ttu-id="39dd1-169">运行以上脚本以后，即可在 report.csv 文件中获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="39dd1-169">After running the above script, the details will be available in the report.csv file.</span></span> <span data-ttu-id="39dd1-170">该文件将包含一个列表，列表中的身份验证尝试是过去一天内发生的，相关用户没有受到 MFA 质询。</span><span class="sxs-lookup"><span data-stu-id="39dd1-170">It will contain a list of authentication attempts that have occurred over the last day where the user was not challenged for MFA.</span></span> <span data-ttu-id="39dd1-171">你需要查看每个条目，确定其是否为预期的行为，必要时采取行动。</span><span class="sxs-lookup"><span data-stu-id="39dd1-171">You will need to review each entry to determine if this is the expected behavior and act if necessary.</span></span>

![评估报表](images/security/assessment-report.png)

## <a name="how-the-requirements-will-be-enforced"></a><span data-ttu-id="39dd1-173">将如何强制实施这些要求</span><span class="sxs-lookup"><span data-stu-id="39dd1-173">How the requirements will be enforced</span></span>

<span data-ttu-id="39dd1-174">合作伙伴安全要求将先后由 Azure Active Directory 和合作伙伴中心强制实施，方法是：检查是否存在 MFA 声明，以便确定是否进行了多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="39dd1-174">The partner security requirements will be enforced by Azure Active Directory, and in turn Partner Center, by checking for the presence of the MFA claim to identify that multi-factor authentication verification has taken place.</span></span> <span data-ttu-id="39dd1-175">如果使用 Azure 多重身份验证或基线保护策略，则不需执行任何其他操作。</span><span class="sxs-lookup"><span data-stu-id="39dd1-175">If you are using Azure Multi-Factor Authentication or the baseline protection policies, then there are no additional actions you need to take.</span></span>

<span data-ttu-id="39dd1-176">使用第三方多重身份验证解决方案时，可能会出现 MFA 声明未发出的情况。</span><span class="sxs-lookup"><span data-stu-id="39dd1-176">When using a third-party multi-factor authentication solution, there is a chance the MFA claim may not be issued.</span></span> <span data-ttu-id="39dd1-177">如果缺少该声明，则 Azure Active Directory 无法确定身份验证请求是否受到了多重身份验证的质询。</span><span class="sxs-lookup"><span data-stu-id="39dd1-177">If this claim is missing Azure Active Directory will not be able determine if the authentication request was challenged by multi-factor authentication.</span></span> <span data-ttu-id="39dd1-178">若要了解如何验证解决方案是否发出了预期的声明，请参阅[测试合作伙伴安全要求](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)。</span><span class="sxs-lookup"><span data-stu-id="39dd1-178">See [Testing the Partner Security Requirements](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) for information on how to verify your solution is issuing the expected claim.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="39dd1-179">如果第三方解决方案未发出预期的声明，则需咨询开发该解决方案的供应商，以确定应该采取哪些措施。</span><span class="sxs-lookup"><span data-stu-id="39dd1-179">If your third-party solution does not issue the expected claim, then you will need to work with the vendor who developed the solution to determine what actions should be taken.</span></span>

## <a name="resources-and-support"></a><span data-ttu-id="39dd1-180">资源和支持</span><span class="sxs-lookup"><span data-stu-id="39dd1-180">Resources and support</span></span>

<span data-ttu-id="39dd1-181">下面是提供支持和示例代码的资源</span><span class="sxs-lookup"><span data-stu-id="39dd1-181">The following are resources where you can find support and sample code</span></span>

- <span data-ttu-id="39dd1-182">[合作伙伴中心安全指南组社区](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - 这是一个在线社区，你可以在其中了解即将发生的事件并提问任何问题。</span><span class="sxs-lookup"><span data-stu-id="39dd1-182">[Partner Center Security Guidance Group community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - This is online community where you can learn about upcoming events and ask any questions that you might have.</span></span>
- <span data-ttu-id="39dd1-183">[Partner Center .NET Samples](https://github.com/microsoft/partner-center-dotnet-samples)（合作伙伴中心 .NET 示例） - 此 GitHub 存储库包含使用 .NET 开发的示例，用于演示如何实现安全应用程序模型框架。</span><span class="sxs-lookup"><span data-stu-id="39dd1-183">[Partner Center .NET Samples](https://github.com/microsoft/partner-center-dotnet-samples) - This GitHub repository contains samples, developed using .NET, that will demonstrate how you can implement the Secure Application Model framework.</span></span>
- <span data-ttu-id="39dd1-184">[合作伙伴中心 Java 示例](https://github.com/microsoft/partner-center-java-samples) - 此 GitHub 存储库包含使用 Java 开发的示例，用于演示如何实现安全应用程序模型框架。</span><span class="sxs-lookup"><span data-stu-id="39dd1-184">[Partner Center Java Samples](https://github.com/microsoft/partner-center-java-samples) - This GitHub repository contains samples, developed using Java, that will demonstrate how you can implement the Secure Application Model framework.</span></span>
- <span data-ttu-id="39dd1-185">[合作伙伴中心 PowerShell - 多重身份验证](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) - 这是一篇详述如何使用 PowerShell 实现安全应用程序模型框架的文章。</span><span class="sxs-lookup"><span data-stu-id="39dd1-185">[Partner Center PowerShell - Multi-Factor Authentication](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) - This is an article that provides details on how to implement the Secure Application Model framework using PowerShell.</span></span>
