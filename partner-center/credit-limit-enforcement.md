---
title: 信用限制实施
ms.topic: how-to
ms.date: 05/11/2021
description: 了解信用限制及其计算方式。 包含常见问题解答。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819203"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="d8915-104">信用限制实施 (CLE) </span><span class="sxs-lookup"><span data-stu-id="d8915-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="d8915-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="d8915-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d8915-106">计费管理员</span><span class="sxs-lookup"><span data-stu-id="d8915-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="d8915-107">信用限制及其工作原理</span><span class="sxs-lookup"><span data-stu-id="d8915-107">Your credit limit and how it works</span></span>

<span data-ttu-id="d8915-108">信用限制是指作为合作伙伴可以用来在合作伙伴中心购买产品或订阅的最大 (，以美元为) 。</span><span class="sxs-lookup"><span data-stu-id="d8915-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="d8915-109">如果超出了信用额度，则无法进行新的购买，直到进行了充足的付款。</span><span class="sxs-lookup"><span data-stu-id="d8915-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="d8915-110">现有订阅将继续不间断地继续。</span><span class="sxs-lookup"><span data-stu-id="d8915-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="d8915-111">信用限制适用于 Azure 计划、Azure 预订、软件、Marketplace、Azure 145 P、Office 和 Dynamics 产品中的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="d8915-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="d8915-112">信用限制不适用于续订和持续消耗。</span><span class="sxs-lookup"><span data-stu-id="d8915-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="d8915-113">在载入期间，我们会在租户级别分配信用限制。</span><span class="sxs-lookup"><span data-stu-id="d8915-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="d8915-114">我们基于预测收入、购买技能和付款历史记录。</span><span class="sxs-lookup"><span data-stu-id="d8915-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="d8915-115">然后，使用以下公式来计算可用余额：</span><span class="sxs-lookup"><span data-stu-id="d8915-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="d8915-116">**[信用限制– (传入购买 + 未付的未付款发票 + 未开票费用–超额支付) ]**</span><span class="sxs-lookup"><span data-stu-id="d8915-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="d8915-117">常见问题</span><span class="sxs-lookup"><span data-stu-id="d8915-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="d8915-118">我的信用额度是否设置为租户或全局级别？</span><span class="sxs-lookup"><span data-stu-id="d8915-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="d8915-119">租户级别。</span><span class="sxs-lookup"><span data-stu-id="d8915-119">The tenant level.</span></span> <span data-ttu-id="d8915-120">例如，假设您从美国、加拿大和日本进行操作。</span><span class="sxs-lookup"><span data-stu-id="d8915-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="d8915-121">如果加拿大租户达到其信用额度，则当租户尝试在合作伙伴中心购买时，会收到通知。</span><span class="sxs-lookup"><span data-stu-id="d8915-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="d8915-122">其他租户将不会受到影响。</span><span class="sxs-lookup"><span data-stu-id="d8915-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="d8915-123">如果我超过了信用限制，是否可以继续使用完全访问权限为现有客户和订阅提供服务？</span><span class="sxs-lookup"><span data-stu-id="d8915-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="d8915-124">是的。</span><span class="sxs-lookup"><span data-stu-id="d8915-124">Yes.</span></span> <span data-ttu-id="d8915-125">你的客户的现有订阅将继续进行而不中断。</span><span class="sxs-lookup"><span data-stu-id="d8915-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="d8915-126">但是，你不能为客户购买新的订阅。</span><span class="sxs-lookup"><span data-stu-id="d8915-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="d8915-127">CLE 是否适用于直属客户和间接提供商？</span><span class="sxs-lookup"><span data-stu-id="d8915-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="d8915-128">是的，它适用于这两种情况。</span><span class="sxs-lookup"><span data-stu-id="d8915-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="d8915-129">提交我的付款以恢复我的帐户后，我可以在何时购买更多订阅？</span><span class="sxs-lookup"><span data-stu-id="d8915-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="d8915-130">你应能够在你的付款24小时内恢复购买，假设 Microsoft 已收到继续信用检查过程的所有要求。</span><span class="sxs-lookup"><span data-stu-id="d8915-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="d8915-131">如何检查信用额度？</span><span class="sxs-lookup"><span data-stu-id="d8915-131">How can I check my credit limit?</span></span>

<span data-ttu-id="d8915-132">联系 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 以查看信用限制并获取有关最近购买的信息。</span><span class="sxs-lookup"><span data-stu-id="d8915-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="d8915-133">是否有针对信用额度的争议计数的发票？</span><span class="sxs-lookup"><span data-stu-id="d8915-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="d8915-134">是的。</span><span class="sxs-lookup"><span data-stu-id="d8915-134">Yes.</span></span> <span data-ttu-id="d8915-135">不过，您可以在上与 Microsoft 联系 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 以解决此问题。</span><span class="sxs-lookup"><span data-stu-id="d8915-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="d8915-136">如果我要写入，会多久再收到 ucmwrcsp@microsoft.com ？</span><span class="sxs-lookup"><span data-stu-id="d8915-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="d8915-137">你的响应应在24小时内。</span><span class="sxs-lookup"><span data-stu-id="d8915-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="d8915-138">Microsoft 用于设置合作伙伴信用限制的条件是什么？</span><span class="sxs-lookup"><span data-stu-id="d8915-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="d8915-139">我们根据预测收入、购买技能和付款历史记录来确定信用限制。</span><span class="sxs-lookup"><span data-stu-id="d8915-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="d8915-140">当前是否在新的商业体验上强制实施信用限制？</span><span class="sxs-lookup"><span data-stu-id="d8915-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="d8915-141">是的。</span><span class="sxs-lookup"><span data-stu-id="d8915-141">Yes.</span></span> <span data-ttu-id="d8915-142">信用限制适用于合作伙伴中心的所有 CSP 计划和产品。</span><span class="sxs-lookup"><span data-stu-id="d8915-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="d8915-143">如果组织接近信用限制，谁会收到通知？</span><span class="sxs-lookup"><span data-stu-id="d8915-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="d8915-144">组织的财务帐户应付帐款联系人应收到通知。</span><span class="sxs-lookup"><span data-stu-id="d8915-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d8915-145">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d8915-145">Next steps</span></span>

[<span data-ttu-id="d8915-146">计费基础知识</span><span class="sxs-lookup"><span data-stu-id="d8915-146">Billing basics</span></span>](./billing-basics.md)
