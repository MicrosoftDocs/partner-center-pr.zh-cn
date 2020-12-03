---
title: 管理客户的 Azure 保留
description: 了解如何管理客户的 Azure 保留，包括如何取消预订、交换预订或请求退款。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: c377fca3e38161258c836d14202ac4db21484526
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534754"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a><span data-ttu-id="77e29-103">为客户管理、取消、交换或退款 Microsoft Azure 预订</span><span class="sxs-lookup"><span data-stu-id="77e29-103">Manage, cancel, exchange, or refund Microsoft Azure reservations for customers</span></span>

<span data-ttu-id="77e29-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="77e29-104">**Appropriate roles**</span></span>

- <span data-ttu-id="77e29-105">管理员代理</span><span class="sxs-lookup"><span data-stu-id="77e29-105">Admin agent</span></span>
- <span data-ttu-id="77e29-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="77e29-106">Global admin</span></span>
- <span data-ttu-id="77e29-107">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="77e29-107">Helpdesk agent</span></span>
- <span data-ttu-id="77e29-108">销售代理</span><span class="sxs-lookup"><span data-stu-id="77e29-108">Sales agent</span></span>
- <span data-ttu-id="77e29-109">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="77e29-109">User management admin</span></span>

<span data-ttu-id="77e29-110">本文介绍如何管理客户的 Azure 保留，包括如何取消预订、交换预订或请求退款。</span><span class="sxs-lookup"><span data-stu-id="77e29-110">This article explains how to manage Azure reservations for a customer, including how to cancel a reservation, exchange a reservation, or request a refund.</span></span>

> [!NOTE]
> <span data-ttu-id="77e29-111">本文仅适用于云解决方案提供商 (CSP) 计划中的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="77e29-111">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="77e29-112">使用其他订阅类型的客户 (例如，即用即付、个人、Microsoft 客户协议或企业协议订阅) 应改为阅读 [此 Azure 保留文档](/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="77e29-112">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="77e29-113">若要在购买后管理客户的 Azure 预订，请选择要在合作伙伴中心管理的客户和预订，然后在 Azure 门户中对预订进行更改。</span><span class="sxs-lookup"><span data-stu-id="77e29-113">To manage your customers' Azure reservations post-purchase, you'll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal.</span></span>

1. <span data-ttu-id="77e29-114">若要开始，请从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要管理其预留的客户。</span><span class="sxs-lookup"><span data-stu-id="77e29-114">To get started, select **Customers** from the Partner Center menu and then select the customer whose reservations you want to manage.</span></span> 

2. <span data-ttu-id="77e29-115">在客户的详细信息页面菜单上，选择 " **Azure 保留** "，然后选择要管理的特定预订。</span><span class="sxs-lookup"><span data-stu-id="77e29-115">On the customer's detail page menu, select **Azure reservations** and then select the specific reservation you want to manage.</span></span>  

3. <span data-ttu-id="77e29-116">在 " **操作**" 下，选择 " **管理** " 以前往 Azure 门户中的客户预订记录。</span><span class="sxs-lookup"><span data-stu-id="77e29-116">Under **Actions**, select **Manage** to go to the customer's reservation record in the Azure portal.</span></span> <span data-ttu-id="77e29-117">在预订详细信息页面上，执行以下步骤来完成任务。</span><span class="sxs-lookup"><span data-stu-id="77e29-117">On the reservation detail page, follow the steps below to complete tasks.</span></span>  

    | <span data-ttu-id="77e29-118">**Select**</span><span class="sxs-lookup"><span data-stu-id="77e29-118">**Select**</span></span>   | <span data-ttu-id="77e29-119">**To**</span><span class="sxs-lookup"><span data-stu-id="77e29-119">**To**</span></span>    |
    |:-----------------------------|:-----------------|
    | <span data-ttu-id="77e29-120">概述</span><span class="sxs-lookup"><span data-stu-id="77e29-120">**Overview**</span></span>   | <span data-ttu-id="77e29-121">查看客户预订的详细信息，包括到期日期、范围和利用率数据。</span><span class="sxs-lookup"><span data-stu-id="77e29-121">View details of a customer's reservation, including expiration date, scope, and utilization data.</span></span> <span data-ttu-id="77e29-122">**注意** 选择 **退款** 可以创建一个按比例退款的支持请求。</span><span class="sxs-lookup"><span data-stu-id="77e29-122">**NOTE** Select **Refund** to create a support request for a pro-rated refund.</span></span> <span data-ttu-id="77e29-123">选择 **兑换** 可以创建一个兑换未使用部分的预订期限的支持请求。</span><span class="sxs-lookup"><span data-stu-id="77e29-123">Select **Exchange** to create a support request to exchange the unused portion of your reservation term.</span></span>  
    | <span data-ttu-id="77e29-124">**(IAM) 的访问控制**</span><span class="sxs-lookup"><span data-stu-id="77e29-124">**Access Control (IAM)**</span></span>   | <span data-ttu-id="77e29-125">管理对客户预订信息的访问。</span><span class="sxs-lookup"><span data-stu-id="77e29-125">Manage access to the customer's reservation information.</span></span>|
    | <span data-ttu-id="77e29-126">**配置**</span><span class="sxs-lookup"><span data-stu-id="77e29-126">**Configuration**</span></span>   | <span data-ttu-id="77e29-127">更改保留的作用域和/或与之关联的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="77e29-127">Change the reservation's scope and/or the Azure subscription the reservation is associated with.</span></span>    |
    | <span data-ttu-id="77e29-128">**属性**</span><span class="sxs-lookup"><span data-stu-id="77e29-128">**Properties**</span></span>   | <span data-ttu-id="77e29-129">查看预订的属性并将其复制到剪贴板中保留 ID 和预留订单 ID。</span><span class="sxs-lookup"><span data-stu-id="77e29-129">View the reservation's properties and copy to the clipboard the reservation ID and reservation order ID.</span></span> <span data-ttu-id="77e29-130">**注意** 当你代表客户请求支持时，支持人员可能会要求你提供预订 ID 和预订订单 ID。</span><span class="sxs-lookup"><span data-stu-id="77e29-130">**NOTE** Support may ask you for the reservation ID and reservation order ID when you request support on behalf of a customer.</span></span>    |
    | <span data-ttu-id="77e29-131">**新建支持请求**</span><span class="sxs-lookup"><span data-stu-id="77e29-131">**New support request**</span></span>    | <span data-ttu-id="77e29-132">请求 Microsoft 支持人员提供帮助。</span><span class="sxs-lookup"><span data-stu-id="77e29-132">Request help from Microsoft Support.</span></span>   |
 
## <a name="cancel-or-exchange-a-reservation"></a><span data-ttu-id="77e29-133">取消或兑换预订</span><span class="sxs-lookup"><span data-stu-id="77e29-133">Cancel or exchange a reservation</span></span>

<span data-ttu-id="77e29-134">如果客户的业务需求发生了变化，则他们可能需要取消预订，并获得退款或交换预订的按比例支付的退款金额，以用于新预订的价格。</span><span class="sxs-lookup"><span data-stu-id="77e29-134">If at any point a customer's business needs change, they may want to cancel a reservation and get a refund or exchange a reservation's prorated refund amount to be used toward the price of a new reservation.</span></span>

<span data-ttu-id="77e29-135">在这两种情况下，Microsoft 将为你退款，这样你就可以通过客户管理生成的财务交易。</span><span class="sxs-lookup"><span data-stu-id="77e29-135">In both of these scenarios, Microsoft refunds the amount to you so that you can then manage the resulting financial transactions with your customers.</span></span> <span data-ttu-id="77e29-136">Microsoft 不会直接与客户联系，就计费、取消或退款。</span><span class="sxs-lookup"><span data-stu-id="77e29-136">Microsoft does not contact customers directly about billing, cancellations, or refunds.</span></span>

### <a name="how-cancellations-work"></a><span data-ttu-id="77e29-137">如何取消</span><span class="sxs-lookup"><span data-stu-id="77e29-137">How cancellations work</span></span>

<span data-ttu-id="77e29-138">客户可随时请求取消预留 (每年 $50000 的退款金额) 。</span><span class="sxs-lookup"><span data-stu-id="77e29-138">Customers can request to cancel a reservation at any time (refund amount capped at $50,000 per year).</span></span> <span data-ttu-id="77e29-139">取消预订后，客户可以返回 Azure 预订的剩余月份数，以提前终止费。</span><span class="sxs-lookup"><span data-stu-id="77e29-139">Canceling a reservation allows the customer to return the amount of the remaining months of an Azure reservation for an early termination fee.</span></span> <span data-ttu-id="77e29-140">剩余的按比例余额减去提前终止费，以使你的帐户获得退款。</span><span class="sxs-lookup"><span data-stu-id="77e29-140">The remaining prorated balance, minus the early termination fee, is refunded to your account so that you can refund the customer's account.</span></span> 

<span data-ttu-id="77e29-141">请参阅下面的 "取消详细信息和费用"。</span><span class="sxs-lookup"><span data-stu-id="77e29-141">See below for cancellation details and fees.</span></span>


|<span data-ttu-id="77e29-142">**取消日期**</span><span class="sxs-lookup"><span data-stu-id="77e29-142">**Cancellation date**</span></span><br> <span data-ttu-id="77e29-143"> (天) </span><span class="sxs-lookup"><span data-stu-id="77e29-143">(days)</span></span>   |<span data-ttu-id="77e29-144">**使用情况**</span><span class="sxs-lookup"><span data-stu-id="77e29-144">**Usage**</span></span>    |<span data-ttu-id="77e29-145">**额度**</span><span class="sxs-lookup"><span data-stu-id="77e29-145">**Credit**</span></span>  |<span data-ttu-id="77e29-146">**提前终止**</span><span class="sxs-lookup"><span data-stu-id="77e29-146">**Early termination**</span></span><br> <span data-ttu-id="77e29-147">费用</span><span class="sxs-lookup"><span data-stu-id="77e29-147">fee</span></span>    |<span data-ttu-id="77e29-148">**退款 cap**</span><span class="sxs-lookup"><span data-stu-id="77e29-148">**Refund cap**</span></span> | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|<span data-ttu-id="77e29-149">5个或更少</span><span class="sxs-lookup"><span data-stu-id="77e29-149">5 or fewer</span></span>                         | <span data-ttu-id="77e29-150">否</span><span class="sxs-lookup"><span data-stu-id="77e29-150">No</span></span>          | <span data-ttu-id="77e29-151">100%</span><span class="sxs-lookup"><span data-stu-id="77e29-151">100%</span></span>       | <span data-ttu-id="77e29-152">否</span><span class="sxs-lookup"><span data-stu-id="77e29-152">No</span></span>                              | <span data-ttu-id="77e29-153">$50000 USD</span><span class="sxs-lookup"><span data-stu-id="77e29-153">$50,000 USD</span></span>   |
|<span data-ttu-id="77e29-154">5个或更少</span><span class="sxs-lookup"><span data-stu-id="77e29-154">5 or fewer</span></span>                         | <span data-ttu-id="77e29-155">是</span><span class="sxs-lookup"><span data-stu-id="77e29-155">Yes</span></span>         | <span data-ttu-id="77e29-156">按比例</span><span class="sxs-lookup"><span data-stu-id="77e29-156">Pro-rated</span></span>  | <span data-ttu-id="77e29-157">否</span><span class="sxs-lookup"><span data-stu-id="77e29-157">No</span></span>                              | <span data-ttu-id="77e29-158">$50000 USD</span><span class="sxs-lookup"><span data-stu-id="77e29-158">$50,000 USD</span></span>   |
|<span data-ttu-id="77e29-159">超过5个</span><span class="sxs-lookup"><span data-stu-id="77e29-159">More than 5</span></span>                        | <span data-ttu-id="77e29-160">否</span><span class="sxs-lookup"><span data-stu-id="77e29-160">No</span></span>          | <span data-ttu-id="77e29-161">按比例</span><span class="sxs-lookup"><span data-stu-id="77e29-161">Pro-rated</span></span>  | <span data-ttu-id="77e29-162">12%</span><span class="sxs-lookup"><span data-stu-id="77e29-162">12%</span></span>                             | <span data-ttu-id="77e29-163">$50000 USD</span><span class="sxs-lookup"><span data-stu-id="77e29-163">$50,000 USD</span></span>   |
|<span data-ttu-id="77e29-164">超过5个</span><span class="sxs-lookup"><span data-stu-id="77e29-164">More than 5</span></span>                        | <span data-ttu-id="77e29-165">是</span><span class="sxs-lookup"><span data-stu-id="77e29-165">Yes</span></span>         | <span data-ttu-id="77e29-166">按比例</span><span class="sxs-lookup"><span data-stu-id="77e29-166">Pro-rated</span></span>  | <span data-ttu-id="77e29-167">12%</span><span class="sxs-lookup"><span data-stu-id="77e29-167">12%</span></span>                             | <span data-ttu-id="77e29-168">$50000 USD</span><span class="sxs-lookup"><span data-stu-id="77e29-168">$50,000 USD</span></span>   |

### <a name="how-exchanges-work"></a><span data-ttu-id="77e29-169">如何兑换</span><span class="sxs-lookup"><span data-stu-id="77e29-169">How exchanges work</span></span> 

<span data-ttu-id="77e29-170">如果客户想要购买不同于他们最初购买的预订，则他们可以请求交换。</span><span class="sxs-lookup"><span data-stu-id="77e29-170">If a customer wants to buy a different reservation than the one they originally bought from you, they can request an exchange.</span></span> <span data-ttu-id="77e29-171">交换预订可能是取消预订的极具吸引力的替代方法，因为它允许客户使用按比例支付的退款量来支付新预订的价格。</span><span class="sxs-lookup"><span data-stu-id="77e29-171">Exchanging a reservation can be an attractive alternative to canceling a reservation because it allows the customer to use the prorated refund amount toward the price of the new reservation.</span></span> 

<span data-ttu-id="77e29-172">按比例退款金额将贷记到你的帐户，以便为客户提供 exchange。</span><span class="sxs-lookup"><span data-stu-id="77e29-172">The prorated refund amount is credited to your account so that you can offer the customer an exchange.</span></span>

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a><span data-ttu-id="77e29-173">代表客户请求退款或兑换</span><span class="sxs-lookup"><span data-stu-id="77e29-173">Request a refund or exchange on behalf of a customer</span></span>

<span data-ttu-id="77e29-174">若要为代表客户的退款或 exchange 提供支持请求，请选择 "合作伙伴中心" 中的 "客户和预订"，然后在 Azure 门户中创建支持请求。</span><span class="sxs-lookup"><span data-stu-id="77e29-174">To file a support request for a refund or exchange on behalf of your customers, you'll select the customer and reservation in Partner Center, and then create the support request in the Azure portal.</span></span> 

>[!NOTE]
><span data-ttu-id="77e29-175">Microsoft 支持代理可能会要求你提供预订 ID 和预订订单 ID。</span><span class="sxs-lookup"><span data-stu-id="77e29-175">Microsoft Support agents may ask you to provide the reservation ID and reservation order ID.</span></span> <span data-ttu-id="77e29-176">你可以在 Azure 门户的保留 **属性** 页上找到此信息。</span><span class="sxs-lookup"><span data-stu-id="77e29-176">You can find this information on the reservation's **Properties** page in the Azure portal.</span></span>

1. <span data-ttu-id="77e29-177">若要开始，请从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要退款的客户。</span><span class="sxs-lookup"><span data-stu-id="77e29-177">To get started, select **Customers** from the Partner Center menu and then select the customer who wants a refund.</span></span> 

2. <span data-ttu-id="77e29-178">在客户的详细信息页上，选择 " **Azure 预订** "，然后选择客户希望获得退款的特定预订。</span><span class="sxs-lookup"><span data-stu-id="77e29-178">On the customer's detail page, select **Azure reservations** and then select the specific reservation the customer wants refunded.</span></span>  

3. <span data-ttu-id="77e29-179">在 " **操作**" 下，选择 " **退款** " 以前往 Azure 门户中的客户预订记录，并启动支持请求。</span><span class="sxs-lookup"><span data-stu-id="77e29-179">Under **Actions**, select **Refund** to go to the customer's reservation record in the Azure portal and initiate a support request.</span></span>  

4. <span data-ttu-id="77e29-180">在 **新建支持请求** 页上，请按照以下步骤来请求退款。</span><span class="sxs-lookup"><span data-stu-id="77e29-180">On the **New support request** page, follow the steps below to request a refund.</span></span> <span data-ttu-id="77e29-181">执行每个步骤后选择 **下一步**。</span><span class="sxs-lookup"><span data-stu-id="77e29-181">Select **Next** after each step.</span></span> 

   |<span data-ttu-id="77e29-182">**步骤**</span><span class="sxs-lookup"><span data-stu-id="77e29-182">**Step**</span></span>                    |<span data-ttu-id="77e29-183">**选择**</span><span class="sxs-lookup"><span data-stu-id="77e29-183">**Selections**</span></span>    |
   |:---------------------------|:-----------------|
   |<span data-ttu-id="77e29-184">**1基础知识**</span><span class="sxs-lookup"><span data-stu-id="77e29-184">**1 Basics**</span></span>                |<span data-ttu-id="77e29-185">问题类型：计费。</span><span class="sxs-lookup"><span data-stu-id="77e29-185">Issue type: Billing.</span></span>  |
   |<span data-ttu-id="77e29-186">**2 问题**</span><span class="sxs-lookup"><span data-stu-id="77e29-186">**2 Problem**</span></span>               |<span data-ttu-id="77e29-187">问题类型：预订管理。</span><span class="sxs-lookup"><span data-stu-id="77e29-187">Problem type: Reservation management.</span></span> <span data-ttu-id="77e29-188">类别：兑换和退款。</span><span class="sxs-lookup"><span data-stu-id="77e29-188">Category: Exchanges and refunds.</span></span> |
   |<span data-ttu-id="77e29-189">**3 联系人信息**</span><span class="sxs-lookup"><span data-stu-id="77e29-189">**3 Contact information**</span></span>   |<span data-ttu-id="77e29-190">选择首选项并输入所需的信息。</span><span class="sxs-lookup"><span data-stu-id="77e29-190">Select your preferences and enter the required information.</span></span> 

5. <span data-ttu-id="77e29-191">完成后，选择“创建”。</span><span class="sxs-lookup"><span data-stu-id="77e29-191">Select **Create** when done.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="77e29-192">Azure 预订资源</span><span class="sxs-lookup"><span data-stu-id="77e29-192">Azure reservations resources</span></span>

|<span data-ttu-id="77e29-193">**有关以下方面的信息**</span><span class="sxs-lookup"><span data-stu-id="77e29-193">**For information about**</span></span>   |<span data-ttu-id="77e29-194">**阅读此文**</span><span class="sxs-lookup"><span data-stu-id="77e29-194">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="77e29-195">云解决方案提供商计划中的 Azure 预订概述</span><span class="sxs-lookup"><span data-stu-id="77e29-195">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="77e29-196">销售 Microsoft Azure 预留实例</span><span class="sxs-lookup"><span data-stu-id="77e29-196">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="77e29-197">在合作伙伴中心为客户购买 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="77e29-197">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="77e29-198">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="77e29-198">Buy Azure reservations</span></span>](azure-reservations-buying.md) |
|<span data-ttu-id="77e29-199">确定正确的虚拟机大小，然后确认客户虚拟机使用情况</span><span class="sxs-lookup"><span data-stu-id="77e29-199">Determine the correct VM size and verify customer VM usage</span></span>   | [<span data-ttu-id="77e29-200">针对最大 Azure 预订利用率确定虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="77e29-200">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="77e29-201">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="77e29-201">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="77e29-202">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="77e29-202">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="77e29-203">为客户提供从为他们购买的订阅购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="77e29-203">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="77e29-204">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="77e29-204">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |