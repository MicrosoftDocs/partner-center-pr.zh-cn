---
title: 排查设置 合作伙伴中心帐户或 MPN 续订问题
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查尝试在注册时合作伙伴中心。 解答解决了付款方式、忘记密码等难题。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431753"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="2b2aa-104">排查帐户设置或 MPN 续订问题</span><span class="sxs-lookup"><span data-stu-id="2b2aa-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="2b2aa-105">**适当的角色**：全局管理员|MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="2b2aa-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="2b2aa-106">下面是一些建议，用于排查设置帐户时出现的合作伙伴中心问题。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="2b2aa-107">如果从公司迁移Partner Membership Center无法编辑任何公司信息字段，会发生什么情况</span><span class="sxs-lookup"><span data-stu-id="2b2aa-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="2b2aa-108">例如，如果你的公司已在 合作伙伴中心 (，云解决方案提供商 (CSP) 帐户) - 将显示一个只读屏幕。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="2b2aa-109">此屏幕将显示有关公司的所有信息，因为它存在于合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="2b2aa-110">不能更改此屏幕上的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-110">You can't change the details on this screen.</span></span> <span data-ttu-id="2b2aa-111">这是设计使的，不是错误。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-111">This is by design and not an error.</span></span>

<span data-ttu-id="2b2aa-112">若要继续，请选择 **"接受"，** 然后选择"继续 **"。**</span><span class="sxs-lookup"><span data-stu-id="2b2aa-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="2b2aa-113">如果 IT 部门已关闭注册 **合作伙伴中心**</span><span class="sxs-lookup"><span data-stu-id="2b2aa-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="2b2aa-114">你会看到此消息，因为病毒用户被禁用，或者因为病毒性注册在 AD Azure Active Directory (上) 禁用。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="2b2aa-115">帐户的全局管理员Azure AD运行以下 PowerShell 命令来启用所需的功能：</span><span class="sxs-lookup"><span data-stu-id="2b2aa-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="2b2aa-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="2b2aa-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="2b2aa-117">有关详细信息，请阅读 [自助注册](/azure/active-directory/users-groups-roles/directory-self-service-signup)。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="2b2aa-118">忘记了密码</span><span class="sxs-lookup"><span data-stu-id="2b2aa-118">You forgot your password</span></span>

<span data-ttu-id="2b2aa-119">如果忘记了密码，请在登录页上选择"**无法访问你的帐户？"。**</span><span class="sxs-lookup"><span data-stu-id="2b2aa-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="2b2aa-120">此选项允许你重置密码或要求全局管理员分配新凭据。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="2b2aa-121">在"告诉我们关于你的公司"屏幕上，你收到"出现问题"错误</span><span class="sxs-lookup"><span data-stu-id="2b2aa-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="2b2aa-122">如果无意中在公司电话号码中使用了特殊字符、空格或国家/地区代码，通常会显示此错误消息。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="2b2aa-123">在"电话号码"字段中输入的值最多只能包含 10 个字符。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="2b2aa-124">信用卡购买收到一条错误消息，指出"你的订单被拒绝。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="2b2aa-125">请验证你的信息"</span><span class="sxs-lookup"><span data-stu-id="2b2aa-125">Please verify your information”</span></span>


<span data-ttu-id="2b2aa-126">始终使用与信用卡相对应的地址，而不是法定实体。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="2b2aa-127">此外，请确保邮政编码正确，并对应于你使用的地址。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="2b2aa-128">你想要从脱机付款切换到联机付款方式</span><span class="sxs-lookup"><span data-stu-id="2b2aa-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="2b2aa-129">需要取消原始订单，然后使用首选付款方式重新购买。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="2b2aa-130">取消订单：</span><span class="sxs-lookup"><span data-stu-id="2b2aa-130">To cancel an order:</span></span>

1. <span data-ttu-id="2b2aa-131">在"合作伙伴中心"仪表板中，选择" **成员资格产品/服务"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="2b2aa-132">选择 **"取消订单"**</span><span class="sxs-lookup"><span data-stu-id="2b2aa-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="2b2aa-133">将出现一个确认窗口，必须确认才能取消初始订单。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2b2aa-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2b2aa-134">Next steps</span></span>

- [<span data-ttu-id="2b2aa-135">管理合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="2b2aa-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="2b2aa-136">如何读取帐单和对帐文件</span><span class="sxs-lookup"><span data-stu-id="2b2aa-136">How to read your bill and recon file</span></span>](read-your-bill.md)
