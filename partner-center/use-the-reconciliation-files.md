---
title: 使用对帐文件 | 合作伙伴中心
description: 有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892138374f5730bdc10bdf07f75d0a8e3ef56bea
ms.sourcegitcommit: 2d3203dd5e2653af031a8009aa3b999a454acef5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2018
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="67fd4-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="67fd4-103">Use the reconciliation files</span></span>

**<span data-ttu-id="67fd4-104">适用于</span><span class="sxs-lookup"><span data-stu-id="67fd4-104">Applies to</span></span>**

-  <span data-ttu-id="67fd4-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="67fd4-105">Partner Center</span></span>
-  <span data-ttu-id="67fd4-106">美国政府 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="67fd4-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="67fd4-107">德国 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="67fd4-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="67fd4-108">有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。</span><span class="sxs-lookup"><span data-stu-id="67fd4-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="67fd4-109">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="67fd4-110">由合作伙伴列出明细</span><span class="sxs-lookup"><span data-stu-id="67fd4-110">Itemize by partner</span></span>


<span data-ttu-id="67fd4-111">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="67fd4-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="67fd4-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="67fd4-112">MPN ID</span></span></th>
<th><span data-ttu-id="67fd4-113">描述</span><span class="sxs-lookup"><span data-stu-id="67fd4-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="67fd4-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="67fd4-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="67fd4-115">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-116">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="67fd4-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="67fd4-117">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="67fd4-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="67fd4-118">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="67fd4-119">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="67fd4-120">若要查看或更新经销商，请在“合作伙伴中心”菜单中，选择“客户”<strong></strong>，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="67fd4-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="67fd4-121">在“客户”菜单中，选择“订阅”<strong></strong>，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="67fd4-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="67fd4-122">选择“更新”<strong></strong>以更改“经销商 (MPN ID)”<strong></strong>。</span><span class="sxs-lookup"><span data-stu-id="67fd4-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="67fd4-123">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="67fd4-124">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="67fd4-125">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="67fd4-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="67fd4-126">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="67fd4-126">License-based file fields</span></span>


<span data-ttu-id="67fd4-127">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="67fd4-128">列</span><span class="sxs-lookup"><span data-stu-id="67fd4-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="67fd4-129">描述</span><span class="sxs-lookup"><span data-stu-id="67fd4-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="67fd4-130">示例值</span><span class="sxs-lookup"><span data-stu-id="67fd4-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="67fd4-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="67fd4-132">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="67fd4-133">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="67fd4-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="67fd4-134">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="67fd4-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="67fd4-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="67fd4-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="67fd4-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="67fd4-137">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="67fd4-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="67fd4-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="67fd4-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="67fd4-139">OrderID</span></span></td>
<td><p><span data-ttu-id="67fd4-140">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="67fd4-141">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="67fd4-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="67fd4-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="67fd4-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="67fd4-144">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="67fd4-145">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="67fd4-146">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="67fd4-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="67fd4-147">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="67fd4-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="67fd4-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="67fd4-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="67fd4-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="67fd4-150">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="67fd4-151">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="67fd4-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="67fd4-152">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="67fd4-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="67fd4-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="67fd4-154">OfferID</span></span></td>
<td><p><span data-ttu-id="67fd4-155">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-155">Unique offer ID.</span></span> <span data-ttu-id="67fd4-156">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="67fd4-157"><b>注意</b>：此值与价目表中的产品/服务 ID 不匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="67fd4-158">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="67fd4-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="67fd4-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="67fd4-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="67fd4-161">唯一的持久型产品/服务 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="67fd4-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="67fd4-162"><b>注意</b>：此值与价目表中的产品/服务 ID 匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="67fd4-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="67fd4-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="67fd4-164">OfferName</span></span></td>
<td><p><span data-ttu-id="67fd4-165">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="67fd4-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="67fd4-166">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="67fd4-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="67fd4-168">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="67fd4-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="67fd4-169">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="67fd4-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="67fd4-170">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="67fd4-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="67fd4-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="67fd4-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="67fd4-173">订阅结束日期：12 个月 + 开始日期之后的 x 天（以便与合作伙伴帐单日期一致）或从续订日期算起的 12 个月。</span><span class="sxs-lookup"><span data-stu-id="67fd4-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="67fd4-174">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="67fd4-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="67fd4-175">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="67fd4-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="67fd4-176">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="67fd4-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="67fd4-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="67fd4-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="67fd4-179">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="67fd4-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="67fd4-180">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="67fd4-181">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="67fd4-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="67fd4-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="67fd4-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="67fd4-184">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="67fd4-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="67fd4-185">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="67fd4-186">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="67fd4-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="67fd4-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="67fd4-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="67fd4-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="67fd4-189">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-189">The type of charge or adjustment.</span></span> <span data-ttu-id="67fd4-190">请参阅<a href="#charge_types">映射发票与对帐文件之间的费用</a></span><span class="sxs-lookup"><span data-stu-id="67fd4-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="67fd4-191">请参阅<a href="#charge_types">映射发票与对帐文件之间的费用</a></span><span class="sxs-lookup"><span data-stu-id="67fd4-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="67fd4-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="67fd4-193">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="67fd4-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="67fd4-194">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="67fd4-195">6.82</span><span class="sxs-lookup"><span data-stu-id="67fd4-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-196">数量</span><span class="sxs-lookup"><span data-stu-id="67fd4-196">Quantity</span></span></td>
<td><p><span data-ttu-id="67fd4-197">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="67fd4-197">Number of seats.</span></span> <span data-ttu-id="67fd4-198">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="67fd4-199">2</span><span class="sxs-lookup"><span data-stu-id="67fd4-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-200">金额</span><span class="sxs-lookup"><span data-stu-id="67fd4-200">Amount</span></span></td>
<td><p><span data-ttu-id="67fd4-201">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="67fd4-201">Total of price for quantity.</span></span> <span data-ttu-id="67fd4-202">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="67fd4-203">13.32</span><span class="sxs-lookup"><span data-stu-id="67fd4-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="67fd4-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="67fd4-205">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="67fd4-206">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="67fd4-207">2.32</span><span class="sxs-lookup"><span data-stu-id="67fd4-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-208">小计</span><span class="sxs-lookup"><span data-stu-id="67fd4-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="67fd4-209">税前总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-209">Total before tax.</span></span> <span data-ttu-id="67fd4-210">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="67fd4-211">11</span><span class="sxs-lookup"><span data-stu-id="67fd4-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-212">税务</span><span class="sxs-lookup"><span data-stu-id="67fd4-212">Tax</span></span></td>
<td><p><span data-ttu-id="67fd4-213">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="67fd4-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="67fd4-214">0</span><span class="sxs-lookup"><span data-stu-id="67fd4-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="67fd4-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="67fd4-216">税后总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-216">Total after tax.</span></span> <span data-ttu-id="67fd4-217">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="67fd4-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="67fd4-218">11</span><span class="sxs-lookup"><span data-stu-id="67fd4-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-219">货币</span><span class="sxs-lookup"><span data-stu-id="67fd4-219">Currency</span></span></td>
<td><p><span data-ttu-id="67fd4-220">货币类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-220">Currency type.</span></span> <span data-ttu-id="67fd4-221">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="67fd4-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="67fd4-222">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="67fd4-223">EUR</span><span class="sxs-lookup"><span data-stu-id="67fd4-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="67fd4-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="67fd4-225">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="67fd4-226">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="67fd4-227">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="67fd4-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="67fd4-228">MPNID</span></span></td>
<td><p><span data-ttu-id="67fd4-229">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="67fd4-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="67fd4-230">4390934</span><span class="sxs-lookup"><span data-stu-id="67fd4-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="67fd4-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="67fd4-232">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="67fd4-233">请参阅[由合作伙伴列出明细](#itemizebypartner)。</span><span class="sxs-lookup"><span data-stu-id="67fd4-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="67fd4-234">4390934</span><span class="sxs-lookup"><span data-stu-id="67fd4-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="67fd4-235">DomainName</span></span></td>
<td><p><span data-ttu-id="67fd4-236">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="67fd4-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="67fd4-237">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="67fd4-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="67fd4-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="67fd4-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="67fd4-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="67fd4-240">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-240">Subscription nickname.</span></span> <span data-ttu-id="67fd4-241">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="67fd4-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="67fd4-242">联机项目</span><span class="sxs-lookup"><span data-stu-id="67fd4-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="67fd4-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="67fd4-244">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="67fd4-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="67fd4-245">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="67fd4-246">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="67fd4-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="67fd4-247">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="67fd4-247">Usage-based file fields</span></span>


<span data-ttu-id="67fd4-248">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="67fd4-249">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="67fd4-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="67fd4-250">列</span><span class="sxs-lookup"><span data-stu-id="67fd4-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="67fd4-251">说明</span><span class="sxs-lookup"><span data-stu-id="67fd4-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="67fd4-252">示例值</span><span class="sxs-lookup"><span data-stu-id="67fd4-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="67fd4-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="67fd4-254">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="67fd4-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="67fd4-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="67fd4-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="67fd4-257">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="67fd4-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="67fd4-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="67fd4-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="67fd4-260">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="67fd4-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="67fd4-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="67fd4-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="67fd4-263">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="67fd4-264">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="67fd4-265">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="67fd4-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="67fd4-266">MPNID</span></span></td>
<td><p><span data-ttu-id="67fd4-267">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="67fd4-268">4390934</span><span class="sxs-lookup"><span data-stu-id="67fd4-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="67fd4-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="67fd4-270">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="67fd4-271">请参阅[由合作伙伴列出明细](#itemizebypartner)。</span><span class="sxs-lookup"><span data-stu-id="67fd4-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="67fd4-272">4390934</span><span class="sxs-lookup"><span data-stu-id="67fd4-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="67fd4-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="67fd4-274">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="67fd4-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="67fd4-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="67fd4-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="67fd4-277">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="67fd4-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="67fd4-278">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="67fd4-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="67fd4-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="67fd4-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="67fd4-281">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="67fd4-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="67fd4-282">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="67fd4-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="67fd4-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="67fd4-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="67fd4-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="67fd4-285">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="67fd4-286">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="67fd4-287">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="67fd4-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="67fd4-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="67fd4-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="67fd4-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="67fd4-290">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="67fd4-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="67fd4-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="67fd4-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="67fd4-293">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="67fd4-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="67fd4-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="67fd4-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="67fd4-295">OrderID</span></span></td>
<td><p><span data-ttu-id="67fd4-296">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="67fd4-297">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="67fd4-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="67fd4-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="67fd4-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="67fd4-300">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="67fd4-301">虚拟机</span><span class="sxs-lookup"><span data-stu-id="67fd4-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="67fd4-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="67fd4-303">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="67fd4-304">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="67fd4-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="67fd4-305">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="67fd4-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="67fd4-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="67fd4-307">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="67fd4-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="67fd4-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-309">资源名称</span><span class="sxs-lookup"><span data-stu-id="67fd4-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="67fd4-310">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="67fd4-311">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="67fd4-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="67fd4-312">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="67fd4-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-313">区域</span><span class="sxs-lookup"><span data-stu-id="67fd4-313">Region</span></span></td>
<td><p><span data-ttu-id="67fd4-314">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="67fd4-314">The region the usage applies to.</span></span> <span data-ttu-id="67fd4-315">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="67fd4-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="67fd4-316">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="67fd4-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-317">SKU</span><span class="sxs-lookup"><span data-stu-id="67fd4-317">SKU</span></span></td>
<td><p><span data-ttu-id="67fd4-318">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="67fd4-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="67fd4-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="67fd4-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="67fd4-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="67fd4-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="67fd4-321">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="67fd4-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="67fd4-322">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="67fd4-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="67fd4-323">1</span><span class="sxs-lookup"><span data-stu-id="67fd4-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="67fd4-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="67fd4-325">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="67fd4-326">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="67fd4-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="67fd4-327">11</span><span class="sxs-lookup"><span data-stu-id="67fd4-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="67fd4-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="67fd4-329">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="67fd4-329">Units included as part of the offer.</span></span> <span data-ttu-id="67fd4-330">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="67fd4-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="67fd4-331">0</span><span class="sxs-lookup"><span data-stu-id="67fd4-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="67fd4-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="67fd4-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="67fd4-333">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="67fd4-334">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="67fd4-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="67fd4-335">11</span><span class="sxs-lookup"><span data-stu-id="67fd4-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="67fd4-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="67fd4-337">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="67fd4-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="67fd4-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="67fd4-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="67fd4-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="67fd4-340">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="67fd4-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="67fd4-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="67fd4-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="67fd4-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="67fd4-343">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="67fd4-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="67fd4-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="67fd4-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="67fd4-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="67fd4-346">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="67fd4-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="67fd4-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-348">货币</span><span class="sxs-lookup"><span data-stu-id="67fd4-348">Currency</span></span></td>
<td><p><span data-ttu-id="67fd4-349">货币类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-349">Currency type.</span></span> <span data-ttu-id="67fd4-350">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="67fd4-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="67fd4-351">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="67fd4-352">EUR</span><span class="sxs-lookup"><span data-stu-id="67fd4-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="67fd4-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="67fd4-354">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="67fd4-354">Pretax price per unit.</span></span> <span data-ttu-id="67fd4-355">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="67fd4-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="67fd4-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="67fd4-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="67fd4-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="67fd4-358">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="67fd4-358">Post tax price per unit.</span></span> <span data-ttu-id="67fd4-359">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="67fd4-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="67fd4-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="67fd4-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="67fd4-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="67fd4-362">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-362">The type of charge or adjustment.</span></span> <span data-ttu-id="67fd4-363">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="67fd4-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="67fd4-364">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="67fd4-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="67fd4-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="67fd4-366">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="67fd4-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="67fd4-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="67fd4-369">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="67fd4-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="67fd4-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="67fd4-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="67fd4-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="67fd4-372">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="67fd4-373">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="67fd4-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="67fd4-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="67fd4-375">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="67fd4-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="67fd4-376">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="67fd4-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="67fd4-377">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="67fd4-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="67fd4-378">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="67fd4-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="67fd4-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="67fd4-380">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="67fd4-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="67fd4-381">外部</span><span class="sxs-lookup"><span data-stu-id="67fd4-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-382">项目</span><span class="sxs-lookup"><span data-stu-id="67fd4-382">Project</span></span></td>
<td><p><span data-ttu-id="67fd4-383">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="67fd4-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="67fd4-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="67fd4-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="67fd4-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="67fd4-386">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="67fd4-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="67fd4-387">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="67fd4-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="67fd4-388">如果你有已预配服务总线连接的 25 个包，并且在那一天利用了 1 个，则这一天的每日使用情况声明将指示“25 连接/ 30 天 – 已使用：1.000000”。</span><span class="sxs-lookup"><span data-stu-id="67fd4-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="67fd4-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="67fd4-390">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="67fd4-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="67fd4-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="67fd4-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="67fd4-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="67fd4-392">DomainName</span></span></td>
<td><p><span data-ttu-id="67fd4-393">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="67fd4-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="67fd4-394">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="67fd4-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="67fd4-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="67fd4-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="67fd4-396">单位</span><span class="sxs-lookup"><span data-stu-id="67fd4-396">Unit</span></span></td>
<td><p><span data-ttu-id="67fd4-397">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="67fd4-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="67fd4-398">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="67fd4-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="67fd4-399">一次性购买文件字段</span><span class="sxs-lookup"><span data-stu-id="67fd4-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="67fd4-400">字段</span><span class="sxs-lookup"><span data-stu-id="67fd4-400">Field</span></span>** |**<span data-ttu-id="67fd4-401">定义</span><span class="sxs-lookup"><span data-stu-id="67fd4-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="67fd4-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="67fd4-402">PartnerId</span></span> |<span data-ttu-id="67fd4-403">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="67fd4-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="67fd4-404">CustomerId</span></span> |<span data-ttu-id="67fd4-405">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="67fd4-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="67fd4-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="67fd4-406">CustomerName</span></span> |<span data-ttu-id="67fd4-407">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="67fd4-408">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="67fd4-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="67fd4-409">CustomerDomainName</span></span> |<span data-ttu-id="67fd4-410">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="67fd4-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="67fd4-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="67fd4-411">CustomerCountry</span></span> |<span data-ttu-id="67fd4-412">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="67fd4-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="67fd4-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="67fd4-413">InvoiceNumber</span></span> |<span data-ttu-id="67fd4-414">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="67fd4-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="67fd4-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="67fd4-415">MpnId</span></span> |<span data-ttu-id="67fd4-416">云解决方案提供商合作伙伴（直接或间接）的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="67fd4-417">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="67fd4-417">Reseller MPN ID</span></span> |<span data-ttu-id="67fd4-418">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="67fd4-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="67fd4-419">预订记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="67fd4-420">这对应于针对合作伙伴中心中的特定预订所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="67fd4-421">如果云解决方案提供商合作伙伴将预订直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="67fd4-422">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="67fd4-423">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="67fd4-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="67fd4-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="67fd4-424">OrderId</span></span> |<span data-ttu-id="67fd4-425">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67fd4-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="67fd4-426">当联系支持人员而不用于对帐时，可能对识别 Azure 预订非常有用。</span><span class="sxs-lookup"><span data-stu-id="67fd4-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="67fd4-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="67fd4-427">OrderDate</span></span> |<span data-ttu-id="67fd4-428">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="67fd4-428">The date the order was placed.</span></span> |
|<span data-ttu-id="67fd4-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="67fd4-429">ProductId</span></span> |<span data-ttu-id="67fd4-430">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-430">The ID for the product.</span></span> |
|<span data-ttu-id="67fd4-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="67fd4-431">SkuId</span></span>  |<span data-ttu-id="67fd4-432">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="67fd4-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="67fd4-433">AvailabilityId</span></span> |<span data-ttu-id="67fd4-434">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="67fd4-434">The ID for a particular Availability.</span></span> <span data-ttu-id="67fd4-435">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="67fd4-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="67fd4-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="67fd4-436">SkuName</span></span>  |<span data-ttu-id="67fd4-437">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="67fd4-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="67fd4-438">ProductName</span></span> |<span data-ttu-id="67fd4-439">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="67fd4-439">The name of the product.</span></span> |
|<span data-ttu-id="67fd4-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="67fd4-440">ChargeType</span></span> |<span data-ttu-id="67fd4-441">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="67fd4-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="67fd4-442">UnitPrice</span></span> |<span data-ttu-id="67fd4-443">所订购的每个产品的价格。</span><span class="sxs-lookup"><span data-stu-id="67fd4-443">Price per product ordered.</span></span> |
|<span data-ttu-id="67fd4-444">数量</span><span class="sxs-lookup"><span data-stu-id="67fd4-444">Quantity</span></span> |<span data-ttu-id="67fd4-445">所订购产品的数量。</span><span class="sxs-lookup"><span data-stu-id="67fd4-445">Number of products ordered.</span></span> |
|<span data-ttu-id="67fd4-446">小计</span><span class="sxs-lookup"><span data-stu-id="67fd4-446">Subtotal</span></span> |<span data-ttu-id="67fd4-447">税前总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-447">Total before tax.</span></span> <span data-ttu-id="67fd4-448">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="67fd4-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="67fd4-449">TaxTotal</span></span> |<span data-ttu-id="67fd4-450">所有适用税款的总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="67fd4-451">总计</span><span class="sxs-lookup"><span data-stu-id="67fd4-451">Total</span></span> |<span data-ttu-id="67fd4-452">此订单的总额。</span><span class="sxs-lookup"><span data-stu-id="67fd4-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="67fd4-453">货币</span><span class="sxs-lookup"><span data-stu-id="67fd4-453">Currency</span></span> |<span data-ttu-id="67fd4-454">货币类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-454">Currency type.</span></span> <span data-ttu-id="67fd4-455">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="67fd4-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="67fd4-456">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="67fd4-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="67fd4-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="67fd4-457">DiscountDetails</span></span> |<span data-ttu-id="67fd4-458">任何相关折扣的详细列表。</span><span class="sxs-lookup"><span data-stu-id="67fd4-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="67fd4-459">映射发票与对帐文件之间的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="67fd4-460">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="67fd4-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="67fd4-461">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="67fd4-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="67fd4-462">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="67fd4-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="67fd4-463">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="67fd4-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="67fd4-464">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="67fd4-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="67fd4-465">发票费用描述</span><span class="sxs-lookup"><span data-stu-id="67fd4-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="67fd4-466">对帐文件费用描述（ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="67fd4-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="67fd4-467">此费用是什么？</span><span class="sxs-lookup"><span data-stu-id="67fd4-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="67fd4-468">如何将这些 ChargeTypes 映射到发票？</span><span class="sxs-lookup"><span data-stu-id="67fd4-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="67fd4-469">定期费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-469">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="67fd4-470">激活费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-471">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="67fd4-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="67fd4-472">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-473">取消费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-474">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-475">周期费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-476">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-477">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="67fd4-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-478">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-479">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-480">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="67fd4-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-481">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-482">购买后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-482">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-483">购买费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-484">订阅的初始费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-484">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-485">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-486">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-487">续订费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-488">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="67fd4-489">其他产品和服务</span><span class="sxs-lookup"><span data-stu-id="67fd4-489">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="67fd4-490">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-491">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-492">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-492">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="67fd4-493">使用费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-493">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="67fd4-494">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-494">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-495">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-495">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="67fd4-496">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-496">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-497">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-497">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-498">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-498">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="67fd4-499">积分&amp;调整</span><span class="sxs-lookup"><span data-stu-id="67fd4-499">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="67fd4-500">偏移行项</span><span class="sxs-lookup"><span data-stu-id="67fd4-500">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-501">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="67fd4-501">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-502">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-502">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="67fd4-503">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-503">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="67fd4-504">其他折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-504">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="67fd4-505">（基于使用情况）</span><span class="sxs-lookup"><span data-stu-id="67fd4-505">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="67fd4-506">激活折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-506">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-507">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-507">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="67fd4-508">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-508">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-509">周期折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-509">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-510">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-510">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="67fd4-511">续订折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-511">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-512">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-512">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="67fd4-513">取消折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-513">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-514">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="67fd4-514">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="67fd4-515">其他折扣</span><span class="sxs-lookup"><span data-stu-id="67fd4-515">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="67fd4-516">（基于许可证）</span><span class="sxs-lookup"><span data-stu-id="67fd4-516">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="67fd4-517">可能应用于多种费用类型</span><span class="sxs-lookup"><span data-stu-id="67fd4-517">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="67fd4-518">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-518">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="67fd4-519"><strong>税款</strong>&nbsp;或&nbsp;<strong> VAT</strong></span><span class="sxs-lookup"><span data-stu-id="67fd4-519"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="67fd4-520">可能应用于多种费用类型</span><span class="sxs-lookup"><span data-stu-id="67fd4-520">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="67fd4-521">例外：“偏移行项”已经包括税款。</span><span class="sxs-lookup"><span data-stu-id="67fd4-521">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="67fd4-522">请参阅上面的“积分&amp;调整”。</span><span class="sxs-lookup"><span data-stu-id="67fd4-522">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="67fd4-523">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="67fd4-523">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="67fd4-524">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-524">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="67fd4-525">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="67fd4-525">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
