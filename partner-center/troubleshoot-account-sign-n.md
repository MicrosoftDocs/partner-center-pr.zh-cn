---
title: 设置合作伙伴中心帐户或 MPN 续订问题的疑难解答
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查试图注册伙伴中心时遇到的问题。 通过支付方法、忘记密码等解决问题。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d80651c4e5e4afb476dada388f23c118e0bdf25
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768697"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="6d573-104">帐户设置或 MPN 续订问题的疑难解答</span><span class="sxs-lookup"><span data-stu-id="6d573-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="6d573-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="6d573-105">**Appropriate roles**</span></span>

- <span data-ttu-id="6d573-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="6d573-106">Global admin</span></span>
- <span data-ttu-id="6d573-107">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="6d573-107">MPN partner admin</span></span> 
 
<span data-ttu-id="6d573-108">下面是有关在设置合作伙伴中心帐户时出现的常见问题的一些建议。</span><span class="sxs-lookup"><span data-stu-id="6d573-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="6d573-109">如果要从合作伙伴成员中心进行迁移并且无法编辑任何公司信息字段，会发生什么情况</span><span class="sxs-lookup"><span data-stu-id="6d573-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="6d573-110">如果你的公司已在合作伙伴中心中存在 (例如，) CSP 帐户–你将会看到一个只读屏幕。</span><span class="sxs-lookup"><span data-stu-id="6d573-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="6d573-111">此屏幕将显示在合作伙伴中心存在的有关公司的所有信息。</span><span class="sxs-lookup"><span data-stu-id="6d573-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="6d573-112">无法更改此屏幕上的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6d573-112">You can't change the details on this screen.</span></span> <span data-ttu-id="6d573-113">这是由设计决定的，而不是错误。</span><span class="sxs-lookup"><span data-stu-id="6d573-113">This is by design and not an error.</span></span>

<span data-ttu-id="6d573-114">选择 " **接受** 并 **继续** " 继续。</span><span class="sxs-lookup"><span data-stu-id="6d573-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="6d573-115">如果 IT 部门已关闭 **合作伙伴中心的注册**，</span><span class="sxs-lookup"><span data-stu-id="6d573-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="6d573-116">你会看到此消息，因为已禁用病毒用户，或者是因为 Azure AD 租户上禁用了病毒注册。</span><span class="sxs-lookup"><span data-stu-id="6d573-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="6d573-117">Azure AD 帐户的全局管理员可以通过运行以下 PowerShell 命令来启用所需的功能：</span><span class="sxs-lookup"><span data-stu-id="6d573-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="6d573-118">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="6d573-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="6d573-119">有关详细信息，请阅读 [自助服务注册](/azure/active-directory/users-groups-roles/directory-self-service-signup)。</span><span class="sxs-lookup"><span data-stu-id="6d573-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="6d573-120">你忘记了密码</span><span class="sxs-lookup"><span data-stu-id="6d573-120">You forgot your password</span></span>

<span data-ttu-id="6d573-121">如果忘记了密码，请在登录页上选择 " **无法访问帐户？** " 链接。</span><span class="sxs-lookup"><span data-stu-id="6d573-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="6d573-122">此选项可让你重置密码或请求全局管理员为你分配新凭据。</span><span class="sxs-lookup"><span data-stu-id="6d573-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="6d573-123">在 "告诉我们你的公司" 屏幕上，你会看到 "出现错误" 错误</span><span class="sxs-lookup"><span data-stu-id="6d573-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="6d573-124">如果你无意中在公司电话号码中使用特殊字符、空格或国家/地区代码，则会出现此错误消息。</span><span class="sxs-lookup"><span data-stu-id="6d573-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="6d573-125">在 "电话号码" 字段中输入的值最多只能包含10个字符。</span><span class="sxs-lookup"><span data-stu-id="6d573-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="6d573-126">你的信用卡购买将收到一条错误消息，指出 "你的订单已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="6d573-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="6d573-127">请验证你的信息</span><span class="sxs-lookup"><span data-stu-id="6d573-127">Please verify your information”</span></span>


<span data-ttu-id="6d573-128">始终使用与您的信用卡相对应的地址，而不是您的法律实体。</span><span class="sxs-lookup"><span data-stu-id="6d573-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="6d573-129">此外，请确保邮政编码正确，并对应于所使用的地址。</span><span class="sxs-lookup"><span data-stu-id="6d573-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="6d573-130">要从脱机支付切换到联机付款方式</span><span class="sxs-lookup"><span data-stu-id="6d573-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="6d573-131">您将需要使用首选付款方式取消原始订单和重新购买。</span><span class="sxs-lookup"><span data-stu-id="6d573-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="6d573-132">若要取消订单：</span><span class="sxs-lookup"><span data-stu-id="6d573-132">To cancel an order:</span></span>

1. <span data-ttu-id="6d573-133">在仪表板中选择 " **成员资格产品** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="6d573-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="6d573-134">选择 **取消顺序**</span><span class="sxs-lookup"><span data-stu-id="6d573-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="6d573-135">将显示一个确认窗口，您必须确认才能取消初始订单。</span><span class="sxs-lookup"><span data-stu-id="6d573-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6d573-136">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6d573-136">Next steps</span></span>

- [<span data-ttu-id="6d573-137">管理合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="6d573-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="6d573-138">如何读取帐单和侦测文件</span><span class="sxs-lookup"><span data-stu-id="6d573-138">How to read your bill and recon file</span></span>](read-your-bill.md)
