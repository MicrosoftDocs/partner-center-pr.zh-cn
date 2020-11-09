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
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381403"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="73aaa-104">帐户设置或 MPN 续订问题的疑难解答</span><span class="sxs-lookup"><span data-stu-id="73aaa-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="73aaa-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="73aaa-105">**Applies to**</span></span>

- <span data-ttu-id="73aaa-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="73aaa-106">Partner Center</span></span>
 
<span data-ttu-id="73aaa-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="73aaa-107">**Appropriate roles**</span></span>

- <span data-ttu-id="73aaa-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="73aaa-108">Global admin</span></span>
- <span data-ttu-id="73aaa-109">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="73aaa-109">MPN partner admin</span></span> 
 
<span data-ttu-id="73aaa-110">下面是有关在设置合作伙伴中心帐户时出现的常见问题的一些建议。</span><span class="sxs-lookup"><span data-stu-id="73aaa-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="73aaa-111">如果要从合作伙伴成员中心进行迁移并且无法编辑任何公司信息字段，会发生什么情况</span><span class="sxs-lookup"><span data-stu-id="73aaa-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="73aaa-112">如果你的公司已在合作伙伴中心中存在， (说 CSP 帐户) ，你会看到一个只读屏幕。</span><span class="sxs-lookup"><span data-stu-id="73aaa-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="73aaa-113">此屏幕将显示在合作伙伴中心存在的有关公司的所有信息。</span><span class="sxs-lookup"><span data-stu-id="73aaa-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="73aaa-114">无法更改此屏幕上的详细信息。</span><span class="sxs-lookup"><span data-stu-id="73aaa-114">You can't change the details on this screen.</span></span> <span data-ttu-id="73aaa-115">这是由设计决定的，而不是错误。</span><span class="sxs-lookup"><span data-stu-id="73aaa-115">This is by design and not an error.</span></span>

<span data-ttu-id="73aaa-116">选择 " **接受** 并 **继续** " 继续。</span><span class="sxs-lookup"><span data-stu-id="73aaa-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="73aaa-117">如果 IT 部门已关闭 **合作伙伴中心的注册** ，</span><span class="sxs-lookup"><span data-stu-id="73aaa-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="73aaa-118">你会看到此消息，因为已禁用病毒用户，或者是因为 Azure AD 租户上禁用了病毒注册。</span><span class="sxs-lookup"><span data-stu-id="73aaa-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="73aaa-119">Azure AD 帐户的全局管理员可以通过运行以下 PowerShell 命令来启用所需的功能：</span><span class="sxs-lookup"><span data-stu-id="73aaa-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="73aaa-120">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="73aaa-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="73aaa-121">有关详细信息，请阅读 [自助注册](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="73aaa-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="73aaa-122">你忘记了密码</span><span class="sxs-lookup"><span data-stu-id="73aaa-122">You forgot your password</span></span>

<span data-ttu-id="73aaa-123">如果忘记了密码，请在登录页上选择 " **无法访问帐户？** " 链接。</span><span class="sxs-lookup"><span data-stu-id="73aaa-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="73aaa-124">此选项可让你重置密码或请求全局管理员为你分配新凭据。</span><span class="sxs-lookup"><span data-stu-id="73aaa-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="73aaa-125">在 "告诉我们你的公司" 屏幕上，你会看到 "出现错误" 错误</span><span class="sxs-lookup"><span data-stu-id="73aaa-125">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="73aaa-126">如果你无意中在公司电话号码中使用特殊字符、空格或国家/地区代码，则会出现此错误消息。</span><span class="sxs-lookup"><span data-stu-id="73aaa-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="73aaa-127">在 "电话号码" 字段中输入的值最多只能包含10个字符。</span><span class="sxs-lookup"><span data-stu-id="73aaa-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="73aaa-128">你的信用卡购买将收到一条错误消息，指出 "你的订单已被拒绝。</span><span class="sxs-lookup"><span data-stu-id="73aaa-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="73aaa-129">请验证你的信息</span><span class="sxs-lookup"><span data-stu-id="73aaa-129">Please verify your information”</span></span>


<span data-ttu-id="73aaa-130">始终使用与您的信用卡相对应的地址，而不是您的法律实体。</span><span class="sxs-lookup"><span data-stu-id="73aaa-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="73aaa-131">此外，请确保邮政编码正确，并对应于所使用的地址。</span><span class="sxs-lookup"><span data-stu-id="73aaa-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="73aaa-132">要从脱机支付切换到联机付款方式</span><span class="sxs-lookup"><span data-stu-id="73aaa-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="73aaa-133">您将需要使用首选付款方式取消原始订单和重新购买。</span><span class="sxs-lookup"><span data-stu-id="73aaa-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="73aaa-134">若要取消订单：</span><span class="sxs-lookup"><span data-stu-id="73aaa-134">To cancel an order:</span></span>

1. <span data-ttu-id="73aaa-135">在仪表板中选择 " **成员资格产品** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="73aaa-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="73aaa-136">选择 **取消顺序**</span><span class="sxs-lookup"><span data-stu-id="73aaa-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="73aaa-137">将显示一个确认窗口，您必须确认才能取消初始订单。</span><span class="sxs-lookup"><span data-stu-id="73aaa-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="73aaa-138">后续步骤</span><span class="sxs-lookup"><span data-stu-id="73aaa-138">Next steps</span></span>

- [<span data-ttu-id="73aaa-139">管理合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="73aaa-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="73aaa-140">如何读取帐单和侦测文件</span><span class="sxs-lookup"><span data-stu-id="73aaa-140">How to read your bill and recon file</span></span>](read-your-bill.md)
