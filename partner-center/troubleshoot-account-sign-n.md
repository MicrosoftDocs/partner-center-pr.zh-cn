---
title: 设置合作伙伴中心帐户或 MPN 续订问题的疑难解答
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查合作伙伴中心的注册问题
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1d850663224469f24d5d4442e33cc17c1bb6704
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220235"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="bb09c-103">帐户设置或 MPN 续订问题的疑难解答</span><span class="sxs-lookup"><span data-stu-id="bb09c-103">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="bb09c-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="bb09c-104">**Applies to**</span></span>

- <span data-ttu-id="bb09c-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="bb09c-105">Partner Center</span></span>
 
<span data-ttu-id="bb09c-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="bb09c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="bb09c-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bb09c-107">Global admin</span></span>
- <span data-ttu-id="bb09c-108">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="bb09c-108">MPN partner admin</span></span> 
 
<span data-ttu-id="bb09c-109">下面是有关在设置合作伙伴中心帐户时出现的常见问题的一些建议。</span><span class="sxs-lookup"><span data-stu-id="bb09c-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="bb09c-110">如果要从合作伙伴成员中心进行迁移并且无法编辑任何公司信息字段，会发生什么情况</span><span class="sxs-lookup"><span data-stu-id="bb09c-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="bb09c-111">如果你的公司已在合作伙伴中心（ (说 CSP 帐户) ）中存在，则会出现这种情况–你将显示一个只读屏幕，该屏幕将显示有关你的公司的所有信息，因为它存在于合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="bb09c-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="bb09c-112">你无法更改此屏幕上的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bb09c-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="bb09c-113">这是由设计决定的，而不是错误。</span><span class="sxs-lookup"><span data-stu-id="bb09c-113">This is by design and not an error.</span></span>

<span data-ttu-id="bb09c-114">选择 " **接受** 并 **继续** " 继续。</span><span class="sxs-lookup"><span data-stu-id="bb09c-114">Select **Accept** and **Continue** to proceed.</span></span>

## <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="bb09c-115">你正在尝试注册或从合作伙伴成员中心迁移，但收到了一条错误消息，指出 IT 部门已关闭 " **注册合作伙伴中心**"。</span><span class="sxs-lookup"><span data-stu-id="bb09c-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="bb09c-116">你会看到此消息，因为已禁用病毒用户或在 Azure AD 租户上禁用病毒注册。</span><span class="sxs-lookup"><span data-stu-id="bb09c-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="bb09c-117">Azure AD 帐户的全局管理员可以通过运行以下 PowerShell 命令来启用所需的功能：</span><span class="sxs-lookup"><span data-stu-id="bb09c-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="bb09c-118">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="bb09c-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="bb09c-119">有关详细信息，请阅读 [自助注册](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="bb09c-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="bb09c-120">你忘记了密码</span><span class="sxs-lookup"><span data-stu-id="bb09c-120">You forgot your password</span></span>

<span data-ttu-id="bb09c-121">如果忘记了密码，请在登录页面上选择 " **无法访问帐户？** " 链接，以重置密码，或要求全局管理员为你分配新凭据。</span><span class="sxs-lookup"><span data-stu-id="bb09c-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="bb09c-122">在 "告诉我们公司的情况" 屏幕上，收到 "出现错误" 错误</span><span class="sxs-lookup"><span data-stu-id="bb09c-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="bb09c-123">如果你在公司电话号码中无意中使用特殊字符、空格或国家/地区代码，则通常会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="bb09c-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="bb09c-124">在 "电话号码" 字段中输入的值最多只能包含10个字符。</span><span class="sxs-lookup"><span data-stu-id="bb09c-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

## <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="bb09c-125">你正在尝试通过信用卡完成购买，但你收到一条错误消息，指出 "你的订单已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="bb09c-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="bb09c-126">请验证你的信息</span><span class="sxs-lookup"><span data-stu-id="bb09c-126">Please verify your information”</span></span>

<span data-ttu-id="bb09c-127">你应始终插入与信用卡相对应的地址，而不是与你的法律实体对应的地址。</span><span class="sxs-lookup"><span data-stu-id="bb09c-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="bb09c-128">此外，请确保邮政编码正确，并对应于所使用的地址。</span><span class="sxs-lookup"><span data-stu-id="bb09c-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="bb09c-129">要从脱机支付切换到联机付款方式</span><span class="sxs-lookup"><span data-stu-id="bb09c-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="bb09c-130">您将需要使用首选付款方式取消原始订单和重新购买。</span><span class="sxs-lookup"><span data-stu-id="bb09c-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="bb09c-131">若要取消订单：</span><span class="sxs-lookup"><span data-stu-id="bb09c-131">To cancel an order:</span></span>

1. <span data-ttu-id="bb09c-132">在仪表板中选择 " **成员资格产品** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="bb09c-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="bb09c-133">选择 **取消顺序**</span><span class="sxs-lookup"><span data-stu-id="bb09c-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="bb09c-134">将显示一个确认窗口，您必须确认才能取消初始订单。</span><span class="sxs-lookup"><span data-stu-id="bb09c-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
