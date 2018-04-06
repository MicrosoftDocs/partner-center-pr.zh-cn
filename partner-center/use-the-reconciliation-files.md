---
title: 使用对帐文件 | 合作伙伴中心
description: 有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 51716e8abedf83237050cb51bc76e54a954cd28b
ms.sourcegitcommit: ec00affdfc79c1346cf8df482ce39dae98e20772
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2018
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="37d78-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="37d78-103">Use the reconciliation files</span></span>

**<span data-ttu-id="37d78-104">适用于</span><span class="sxs-lookup"><span data-stu-id="37d78-104">Applies to</span></span>**

-  <span data-ttu-id="37d78-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="37d78-105">Partner Center</span></span>
-  <span data-ttu-id="37d78-106">美国政府 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="37d78-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="37d78-107">德国 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="37d78-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="37d78-108">有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。</span><span class="sxs-lookup"><span data-stu-id="37d78-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="37d78-109">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="37d78-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="37d78-110">由合作伙伴列出明细</span><span class="sxs-lookup"><span data-stu-id="37d78-110">Itemize by partner</span></span>


<span data-ttu-id="37d78-111">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="37d78-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="37d78-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="37d78-112">MPN ID</span></span></th>
<th><span data-ttu-id="37d78-113">描述</span><span class="sxs-lookup"><span data-stu-id="37d78-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="37d78-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="37d78-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="37d78-115">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-116">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="37d78-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="37d78-117">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="37d78-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="37d78-118">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="37d78-119">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="37d78-120">若要查看或更新经销商，请在“合作伙伴中心”菜单中，选择“客户”<strong></strong>，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="37d78-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="37d78-121">在“客户”菜单中，选择“订阅”<strong></strong>，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="37d78-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="37d78-122">选择“更新”<strong></strong>以更改“经销商 (MPN ID)”<strong></strong>。</span><span class="sxs-lookup"><span data-stu-id="37d78-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="37d78-123">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="37d78-124">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="37d78-125">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="37d78-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="37d78-126">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="37d78-126">License-based file fields</span></span>


<span data-ttu-id="37d78-127">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="37d78-128">列</span><span class="sxs-lookup"><span data-stu-id="37d78-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="37d78-129">描述</span><span class="sxs-lookup"><span data-stu-id="37d78-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="37d78-130">示例值</span><span class="sxs-lookup"><span data-stu-id="37d78-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="37d78-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="37d78-132">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="37d78-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="37d78-133">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="37d78-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="37d78-134">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="37d78-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="37d78-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="37d78-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="37d78-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="37d78-137">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="37d78-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="37d78-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="37d78-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="37d78-139">OrderID</span></span></td>
<td><p><span data-ttu-id="37d78-140">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37d78-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="37d78-141">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="37d78-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="37d78-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="37d78-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="37d78-144">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37d78-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="37d78-145">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="37d78-146">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="37d78-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="37d78-147">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="37d78-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="37d78-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="37d78-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="37d78-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="37d78-150">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37d78-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="37d78-151">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="37d78-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="37d78-152">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="37d78-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="37d78-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="37d78-154">OfferID</span></span></td>
<td><p><span data-ttu-id="37d78-155">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-155">Unique offer ID.</span></span> <span data-ttu-id="37d78-156">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="37d78-157"><b>注意</b>：此值与价目表中的产品/服务 ID 不匹配。</span><span class="sxs-lookup"><span data-stu-id="37d78-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="37d78-158">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="37d78-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="37d78-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="37d78-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="37d78-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="37d78-161">唯一的持久型产品/服务 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="37d78-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="37d78-162"><b>注意</b>：此值与价目表中的产品/服务 ID 匹配。</span><span class="sxs-lookup"><span data-stu-id="37d78-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="37d78-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="37d78-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="37d78-164">OfferName</span></span></td>
<td><p><span data-ttu-id="37d78-165">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="37d78-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="37d78-166">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="37d78-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="37d78-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="37d78-168">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="37d78-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="37d78-169">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="37d78-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="37d78-170">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="37d78-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="37d78-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="37d78-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="37d78-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="37d78-173">订阅结束日期：12 个月 + 开始日期之后的 x 天（以便与合作伙伴帐单日期一致）或从续订日期算起的 12 个月。</span><span class="sxs-lookup"><span data-stu-id="37d78-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="37d78-174">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="37d78-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="37d78-175">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="37d78-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="37d78-176">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="37d78-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="37d78-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="37d78-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="37d78-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="37d78-179">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="37d78-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="37d78-180">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="37d78-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="37d78-181">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="37d78-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="37d78-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="37d78-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="37d78-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="37d78-184">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="37d78-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="37d78-185">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="37d78-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="37d78-186">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="37d78-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="37d78-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="37d78-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="37d78-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="37d78-189">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="37d78-189">The type of charge or adjustment.</span></span> <span data-ttu-id="37d78-190">请参阅<a href="#charge_types">映射发票与对帐文件之间的费用</a></span><span class="sxs-lookup"><span data-stu-id="37d78-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="37d78-191">请参阅<a href="#charge_types">映射发票与对帐文件之间的费用</a></span><span class="sxs-lookup"><span data-stu-id="37d78-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="37d78-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="37d78-193">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="37d78-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="37d78-194">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="37d78-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="37d78-195">6.82</span><span class="sxs-lookup"><span data-stu-id="37d78-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-196">数量</span><span class="sxs-lookup"><span data-stu-id="37d78-196">Quantity</span></span></td>
<td><p><span data-ttu-id="37d78-197">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="37d78-197">Number of seats.</span></span> <span data-ttu-id="37d78-198">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="37d78-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="37d78-199">2</span><span class="sxs-lookup"><span data-stu-id="37d78-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-200">金额</span><span class="sxs-lookup"><span data-stu-id="37d78-200">Amount</span></span></td>
<td><p><span data-ttu-id="37d78-201">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="37d78-201">Total of price for quantity.</span></span> <span data-ttu-id="37d78-202">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="37d78-203">13.32</span><span class="sxs-lookup"><span data-stu-id="37d78-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="37d78-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="37d78-205">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="37d78-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="37d78-206">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="37d78-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="37d78-207">2.32</span><span class="sxs-lookup"><span data-stu-id="37d78-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-208">小计</span><span class="sxs-lookup"><span data-stu-id="37d78-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="37d78-209">税前总额。</span><span class="sxs-lookup"><span data-stu-id="37d78-209">Total before tax.</span></span> <span data-ttu-id="37d78-210">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="37d78-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="37d78-211">11</span><span class="sxs-lookup"><span data-stu-id="37d78-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-212">税务</span><span class="sxs-lookup"><span data-stu-id="37d78-212">Tax</span></span></td>
<td><p><span data-ttu-id="37d78-213">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="37d78-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="37d78-214">0</span><span class="sxs-lookup"><span data-stu-id="37d78-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="37d78-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="37d78-216">税后总额。</span><span class="sxs-lookup"><span data-stu-id="37d78-216">Total after tax.</span></span> <span data-ttu-id="37d78-217">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="37d78-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="37d78-218">11</span><span class="sxs-lookup"><span data-stu-id="37d78-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-219">货币</span><span class="sxs-lookup"><span data-stu-id="37d78-219">Currency</span></span></td>
<td><p><span data-ttu-id="37d78-220">货币类型。</span><span class="sxs-lookup"><span data-stu-id="37d78-220">Currency type.</span></span> <span data-ttu-id="37d78-221">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="37d78-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="37d78-222">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="37d78-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="37d78-223">EUR</span><span class="sxs-lookup"><span data-stu-id="37d78-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="37d78-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="37d78-225">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="37d78-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="37d78-226">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="37d78-227">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="37d78-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="37d78-228">MPNID</span></span></td>
<td><p><span data-ttu-id="37d78-229">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="37d78-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="37d78-230">4390934</span><span class="sxs-lookup"><span data-stu-id="37d78-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="37d78-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="37d78-232">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="37d78-233">请参阅[由合作伙伴列出明细](#itemizebypartner)。</span><span class="sxs-lookup"><span data-stu-id="37d78-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="37d78-234">4390934</span><span class="sxs-lookup"><span data-stu-id="37d78-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="37d78-235">DomainName</span></span></td>
<td><p><span data-ttu-id="37d78-236">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="37d78-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="37d78-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="37d78-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="37d78-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="37d78-239">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="37d78-239">Subscription nickname.</span></span> <span data-ttu-id="37d78-240">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="37d78-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="37d78-241">联机项目</span><span class="sxs-lookup"><span data-stu-id="37d78-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="37d78-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="37d78-243">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="37d78-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="37d78-244">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="37d78-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="37d78-245">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="37d78-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="37d78-246">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="37d78-246">Usage-based file fields</span></span>


<span data-ttu-id="37d78-247">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="37d78-248">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="37d78-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="37d78-249">列</span><span class="sxs-lookup"><span data-stu-id="37d78-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="37d78-250">说明</span><span class="sxs-lookup"><span data-stu-id="37d78-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="37d78-251">示例值</span><span class="sxs-lookup"><span data-stu-id="37d78-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="37d78-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="37d78-253">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="37d78-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="37d78-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="37d78-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="37d78-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="37d78-256">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="37d78-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="37d78-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="37d78-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="37d78-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="37d78-259">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="37d78-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="37d78-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="37d78-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="37d78-262">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="37d78-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="37d78-263">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="37d78-264">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="37d78-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="37d78-265">MPNID</span></span></td>
<td><p><span data-ttu-id="37d78-266">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="37d78-267">4390934</span><span class="sxs-lookup"><span data-stu-id="37d78-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="37d78-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="37d78-269">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="37d78-270">请参阅[由合作伙伴列出明细](#itemizebypartner)。</span><span class="sxs-lookup"><span data-stu-id="37d78-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="37d78-271">4390934</span><span class="sxs-lookup"><span data-stu-id="37d78-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="37d78-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="37d78-273">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="37d78-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="37d78-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="37d78-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="37d78-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="37d78-276">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="37d78-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="37d78-277">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="37d78-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="37d78-278">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="37d78-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="37d78-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="37d78-280">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="37d78-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="37d78-281">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="37d78-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="37d78-282">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="37d78-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="37d78-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="37d78-284">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37d78-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="37d78-285">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="37d78-286">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="37d78-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="37d78-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="37d78-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="37d78-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="37d78-289">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="37d78-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="37d78-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="37d78-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="37d78-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="37d78-292">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="37d78-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="37d78-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="37d78-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="37d78-294">OrderID</span></span></td>
<td><p><span data-ttu-id="37d78-295">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37d78-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="37d78-296">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="37d78-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="37d78-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="37d78-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="37d78-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="37d78-299">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="37d78-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="37d78-300">虚拟机</span><span class="sxs-lookup"><span data-stu-id="37d78-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="37d78-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="37d78-302">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="37d78-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="37d78-303">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="37d78-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="37d78-304">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="37d78-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="37d78-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="37d78-306">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37d78-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="37d78-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="37d78-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-308">资源名称</span><span class="sxs-lookup"><span data-stu-id="37d78-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="37d78-309">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="37d78-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="37d78-310">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="37d78-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="37d78-311">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="37d78-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-312">区域</span><span class="sxs-lookup"><span data-stu-id="37d78-312">Region</span></span></td>
<td><p><span data-ttu-id="37d78-313">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="37d78-313">The region the usage applies to.</span></span> <span data-ttu-id="37d78-314">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="37d78-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="37d78-315">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="37d78-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-316">SKU</span><span class="sxs-lookup"><span data-stu-id="37d78-316">SKU</span></span></td>
<td><p><span data-ttu-id="37d78-317">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="37d78-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="37d78-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="37d78-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="37d78-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="37d78-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="37d78-320">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="37d78-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="37d78-321">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="37d78-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="37d78-322">1</span><span class="sxs-lookup"><span data-stu-id="37d78-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="37d78-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="37d78-324">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="37d78-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="37d78-325">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="37d78-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="37d78-326">11</span><span class="sxs-lookup"><span data-stu-id="37d78-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="37d78-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="37d78-328">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="37d78-328">Units included as part of the offer.</span></span> <span data-ttu-id="37d78-329">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="37d78-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="37d78-330">0</span><span class="sxs-lookup"><span data-stu-id="37d78-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="37d78-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="37d78-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="37d78-332">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="37d78-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="37d78-333">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="37d78-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="37d78-334">11</span><span class="sxs-lookup"><span data-stu-id="37d78-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="37d78-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="37d78-336">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="37d78-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="37d78-337">$0.0808</span><span class="sxs-lookup"><span data-stu-id="37d78-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="37d78-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="37d78-339">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="37d78-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="37d78-340">$0.085</span><span class="sxs-lookup"><span data-stu-id="37d78-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="37d78-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="37d78-342">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="37d78-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="37d78-343">$0.08</span><span class="sxs-lookup"><span data-stu-id="37d78-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="37d78-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="37d78-345">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="37d78-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="37d78-346">$0.93</span><span class="sxs-lookup"><span data-stu-id="37d78-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-347">货币</span><span class="sxs-lookup"><span data-stu-id="37d78-347">Currency</span></span></td>
<td><p><span data-ttu-id="37d78-348">货币类型。</span><span class="sxs-lookup"><span data-stu-id="37d78-348">Currency type.</span></span> <span data-ttu-id="37d78-349">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="37d78-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="37d78-350">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="37d78-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="37d78-351">EUR</span><span class="sxs-lookup"><span data-stu-id="37d78-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="37d78-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="37d78-353">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="37d78-353">Pretax price per unit.</span></span> <span data-ttu-id="37d78-354">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="37d78-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="37d78-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="37d78-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="37d78-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="37d78-357">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="37d78-357">Post tax price per unit.</span></span> <span data-ttu-id="37d78-358">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="37d78-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="37d78-359">$0.08</span><span class="sxs-lookup"><span data-stu-id="37d78-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="37d78-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="37d78-361">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="37d78-361">The type of charge or adjustment.</span></span> <span data-ttu-id="37d78-362">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="37d78-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="37d78-363">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="37d78-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="37d78-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="37d78-365">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="37d78-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="37d78-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="37d78-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="37d78-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="37d78-368">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="37d78-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="37d78-369">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="37d78-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="37d78-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="37d78-371">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="37d78-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="37d78-372">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="37d78-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="37d78-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="37d78-374">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="37d78-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="37d78-375">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="37d78-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="37d78-376">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="37d78-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="37d78-377">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="37d78-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="37d78-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="37d78-379">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="37d78-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="37d78-380">外部</span><span class="sxs-lookup"><span data-stu-id="37d78-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-381">项目</span><span class="sxs-lookup"><span data-stu-id="37d78-381">Project</span></span></td>
<td><p><span data-ttu-id="37d78-382">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="37d78-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="37d78-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="37d78-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="37d78-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="37d78-385">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="37d78-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="37d78-386">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="37d78-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="37d78-387">如果你有已预配服务总线连接的 25 个包，并且在那一天利用了 1 个，则这一天的每日使用情况声明将指示“25 连接/ 30 天 – 已使用：1.000000”。</span><span class="sxs-lookup"><span data-stu-id="37d78-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="37d78-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="37d78-389">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="37d78-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="37d78-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="37d78-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="37d78-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="37d78-391">DomainName</span></span></td>
<td><p><span data-ttu-id="37d78-392">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="37d78-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="37d78-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="37d78-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="37d78-394">单位</span><span class="sxs-lookup"><span data-stu-id="37d78-394">Unit</span></span></td>
<td><p><span data-ttu-id="37d78-395">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="37d78-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="37d78-396">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="37d78-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="37d78-397">映射发票与对帐文件之间的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-397">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="37d78-398">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="37d78-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="37d78-399">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="37d78-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="37d78-400">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="37d78-400">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="37d78-401">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="37d78-401">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="37d78-402">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="37d78-402">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="37d78-403">发票费用描述</span><span class="sxs-lookup"><span data-stu-id="37d78-403">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="37d78-404">对帐文件费用描述（ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="37d78-404">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="37d78-405">此费用是什么？</span><span class="sxs-lookup"><span data-stu-id="37d78-405">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="37d78-406">如何将这些 ChargeTypes 映射到发票？</span><span class="sxs-lookup"><span data-stu-id="37d78-406">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="37d78-407">定期费用</span><span class="sxs-lookup"><span data-stu-id="37d78-407">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="37d78-408">激活费用</span><span class="sxs-lookup"><span data-stu-id="37d78-408">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-409">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="37d78-409">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="37d78-410">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-410">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-411">取消费用</span><span class="sxs-lookup"><span data-stu-id="37d78-411">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-412">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-412">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-413">周期费用</span><span class="sxs-lookup"><span data-stu-id="37d78-413">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-414">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="37d78-414">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-415">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="37d78-415">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-416">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-416">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-417">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-417">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-418">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="37d78-418">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-419">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-419">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-420">购买后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-420">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-421">购买费用</span><span class="sxs-lookup"><span data-stu-id="37d78-421">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-422">订阅的初始费用</span><span class="sxs-lookup"><span data-stu-id="37d78-422">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-423">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-423">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-424">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-424">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-425">续订费用</span><span class="sxs-lookup"><span data-stu-id="37d78-425">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-426">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="37d78-426">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="37d78-427">其他产品和服务</span><span class="sxs-lookup"><span data-stu-id="37d78-427">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="37d78-428">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-428">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-429">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-429">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-430">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-430">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="37d78-431">使用费用</span><span class="sxs-lookup"><span data-stu-id="37d78-431">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="37d78-432">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="37d78-432">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-433">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="37d78-433">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="37d78-434">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-434">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-435">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="37d78-435">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-436">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="37d78-436">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="37d78-437">积分&amp;调整</span><span class="sxs-lookup"><span data-stu-id="37d78-437">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="37d78-438">偏移行项</span><span class="sxs-lookup"><span data-stu-id="37d78-438">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-439">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="37d78-439">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-440">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-440">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="37d78-441">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-441">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="37d78-442">其他折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-442">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="37d78-443">（基于使用情况）</span><span class="sxs-lookup"><span data-stu-id="37d78-443">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="37d78-444">激活折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-444">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-445">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-445">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="37d78-446">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-446">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-447">周期折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-447">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-448">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-448">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="37d78-449">续订折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-449">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-450">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-450">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="37d78-451">取消折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-451">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-452">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="37d78-452">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="37d78-453">其他折扣</span><span class="sxs-lookup"><span data-stu-id="37d78-453">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="37d78-454">（基于许可证）</span><span class="sxs-lookup"><span data-stu-id="37d78-454">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="37d78-455">可能应用于多种费用类型</span><span class="sxs-lookup"><span data-stu-id="37d78-455">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="37d78-456">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-456">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="37d78-457"><strong>税款</strong>&nbsp;或&nbsp;<strong> VAT</strong></span><span class="sxs-lookup"><span data-stu-id="37d78-457"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="37d78-458">可能应用于多种费用类型</span><span class="sxs-lookup"><span data-stu-id="37d78-458">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="37d78-459">例外：“偏移行项”已经包括税款。</span><span class="sxs-lookup"><span data-stu-id="37d78-459">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="37d78-460">请参阅上面的“积分&amp;调整”。</span><span class="sxs-lookup"><span data-stu-id="37d78-460">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="37d78-461">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="37d78-461">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="37d78-462">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-462">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="37d78-463">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="37d78-463">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
