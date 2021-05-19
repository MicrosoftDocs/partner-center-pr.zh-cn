---
title: 信用额度强制执行
ms.topic: how-to
ms.date: 05/11/2021
description: 了解信用限制及其计算方式。 包含常见问题解答。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148102"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="dff7f-104">信用限制实施 (CLE) </span><span class="sxs-lookup"><span data-stu-id="dff7f-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="dff7f-105">**适当的角色**：计费管理员</span><span class="sxs-lookup"><span data-stu-id="dff7f-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="dff7f-106">信用限制及其工作原理</span><span class="sxs-lookup"><span data-stu-id="dff7f-106">Your credit limit and how it works</span></span>

<span data-ttu-id="dff7f-107">信用限制是指作为合作伙伴可以用来在合作伙伴中心购买产品或订阅的最大 (，以美元为) 。</span><span class="sxs-lookup"><span data-stu-id="dff7f-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="dff7f-108">如果超出了信用额度，则无法进行新的购买，直到进行了充足的付款。</span><span class="sxs-lookup"><span data-stu-id="dff7f-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="dff7f-109">现有订阅将继续不间断地继续。</span><span class="sxs-lookup"><span data-stu-id="dff7f-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="dff7f-110">信用限制适用于 Azure 计划、Azure 预订、软件、Marketplace、Azure 145 P、Office 和 Dynamics 产品中的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="dff7f-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="dff7f-111">信用限制不适用于续订和持续消耗。</span><span class="sxs-lookup"><span data-stu-id="dff7f-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="dff7f-112">在载入期间，我们会在租户级别分配信用限制。</span><span class="sxs-lookup"><span data-stu-id="dff7f-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="dff7f-113">我们基于预测收入、购买技能和付款历史记录。</span><span class="sxs-lookup"><span data-stu-id="dff7f-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="dff7f-114">然后，使用以下公式来计算可用余额：</span><span class="sxs-lookup"><span data-stu-id="dff7f-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="dff7f-115">**[信用限制– (传入购买 + 未付的未付款发票 + 未开票费用–超额支付) ]**</span><span class="sxs-lookup"><span data-stu-id="dff7f-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="dff7f-116">常见问题</span><span class="sxs-lookup"><span data-stu-id="dff7f-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="dff7f-117">我的信用额度是否设置为租户或全局级别？</span><span class="sxs-lookup"><span data-stu-id="dff7f-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="dff7f-118">租户级别。</span><span class="sxs-lookup"><span data-stu-id="dff7f-118">The tenant level.</span></span> <span data-ttu-id="dff7f-119">例如，假设您从美国、加拿大和日本进行操作。</span><span class="sxs-lookup"><span data-stu-id="dff7f-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="dff7f-120">如果加拿大租户达到其信用额度，则当租户尝试在合作伙伴中心购买时，会收到通知。</span><span class="sxs-lookup"><span data-stu-id="dff7f-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="dff7f-121">其他租户将不会受到影响。</span><span class="sxs-lookup"><span data-stu-id="dff7f-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="dff7f-122">如果我超过了信用限制，是否可以继续使用完全访问权限为现有客户和订阅提供服务？</span><span class="sxs-lookup"><span data-stu-id="dff7f-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="dff7f-123">是。</span><span class="sxs-lookup"><span data-stu-id="dff7f-123">Yes.</span></span> <span data-ttu-id="dff7f-124">客户的现有订阅将继续进行，而不会中断。</span><span class="sxs-lookup"><span data-stu-id="dff7f-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="dff7f-125">但是，不能为客户购买新订阅。</span><span class="sxs-lookup"><span data-stu-id="dff7f-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="dff7f-126">直接计费合作伙伴和间接提供商是否同时应用了 CLE？</span><span class="sxs-lookup"><span data-stu-id="dff7f-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="dff7f-127">是的，这两者均适用。</span><span class="sxs-lookup"><span data-stu-id="dff7f-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="dff7f-128">提交付款以恢复帐户后，何时可以购买更多订阅？</span><span class="sxs-lookup"><span data-stu-id="dff7f-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="dff7f-129">假设 Microsoft 已收到继续进行信用检查过程的所有要求，你应该能够在付款后 24 小时内恢复购买。</span><span class="sxs-lookup"><span data-stu-id="dff7f-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="dff7f-130">如何检查信用额度？</span><span class="sxs-lookup"><span data-stu-id="dff7f-130">How can I check my credit limit?</span></span>

<span data-ttu-id="dff7f-131">请联系 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 查看信用额度限制，并获取有关最近购买的信息。</span><span class="sxs-lookup"><span data-stu-id="dff7f-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="dff7f-132">存在争议的发票是否计入信用额度限制？</span><span class="sxs-lookup"><span data-stu-id="dff7f-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="dff7f-133">是。</span><span class="sxs-lookup"><span data-stu-id="dff7f-133">Yes.</span></span> <span data-ttu-id="dff7f-134">但是，可以通过 联系 Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="dff7f-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="dff7f-135">如果我向 写入了 ，多久就会听到回信 ucmwrcsp@microsoft.com ？</span><span class="sxs-lookup"><span data-stu-id="dff7f-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="dff7f-136">应在 24 小时内收到响应。</span><span class="sxs-lookup"><span data-stu-id="dff7f-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="dff7f-137">Microsoft 使用什么条件来设置合作伙伴的信用额度限制？</span><span class="sxs-lookup"><span data-stu-id="dff7f-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="dff7f-138">我们根据预测的收入、购买能力以及付款历史记录来确定信用额度限制。</span><span class="sxs-lookup"><span data-stu-id="dff7f-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="dff7f-139">新商务体验当前是否强制实施了信用额度限制？</span><span class="sxs-lookup"><span data-stu-id="dff7f-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="dff7f-140">是。</span><span class="sxs-lookup"><span data-stu-id="dff7f-140">Yes.</span></span> <span data-ttu-id="dff7f-141">信用额度适用于所有云解决方案提供商计划和合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="dff7f-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="dff7f-142">我的组织即将达到其信用额度限制时，谁会收到通知？</span><span class="sxs-lookup"><span data-stu-id="dff7f-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="dff7f-143">组织的 Finance Account Should 联系人应收到通知。</span><span class="sxs-lookup"><span data-stu-id="dff7f-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dff7f-144">后续步骤</span><span class="sxs-lookup"><span data-stu-id="dff7f-144">Next steps</span></span>

[<span data-ttu-id="dff7f-145">计费基础知识</span><span class="sxs-lookup"><span data-stu-id="dff7f-145">Billing basics</span></span>](./billing-basics.md)
