---
title: 使用对帐文件（由世纪互联运营的合作伙伴中心）
ms.topic: article
ms.date: 10/29/2018
description: 有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584980"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="e02ef-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="e02ef-103">Use the reconciliation files</span></span>

<span data-ttu-id="e02ef-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="e02ef-104">**Applies to**</span></span>

-   <span data-ttu-id="e02ef-105">由世纪互联运营的合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="e02ef-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="e02ef-106">有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。</span><span class="sxs-lookup"><span data-stu-id="e02ef-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="e02ef-107">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="e02ef-108">由合作伙伴详细列举</span><span class="sxs-lookup"><span data-stu-id="e02ef-108">Itemize by partner</span></span>


<span data-ttu-id="e02ef-109">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="e02ef-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e02ef-110">MPN ID</span><span class="sxs-lookup"><span data-stu-id="e02ef-110">MPN ID</span></span></th>
<th><span data-ttu-id="e02ef-111">描述</span><span class="sxs-lookup"><span data-stu-id="e02ef-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e02ef-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="e02ef-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="e02ef-113">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-114">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="e02ef-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="e02ef-115">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="e02ef-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="e02ef-116">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e02ef-117">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="e02ef-118">若要查看或更新经销商，请在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="e02ef-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="e02ef-119">在客户菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="e02ef-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="e02ef-120">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="e02ef-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="e02ef-121">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="e02ef-122">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="e02ef-123">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="e02ef-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="e02ef-124">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="e02ef-124">License-based file fields</span></span>


<span data-ttu-id="e02ef-125">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e02ef-126"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="e02ef-127"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="e02ef-128"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e02ef-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="e02ef-130">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e02ef-131">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="e02ef-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e02ef-132">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="e02ef-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="e02ef-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="e02ef-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e02ef-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="e02ef-135">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="e02ef-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e02ef-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="e02ef-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="e02ef-137">OrderID</span></span></td>
<td><p><span data-ttu-id="e02ef-138">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e02ef-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e02ef-139">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e02ef-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e02ef-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e02ef-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e02ef-142">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e02ef-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e02ef-143">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e02ef-144">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="e02ef-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="e02ef-145">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="e02ef-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="e02ef-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e02ef-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="e02ef-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="e02ef-148">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e02ef-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="e02ef-149">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="e02ef-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="e02ef-150">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e02ef-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="e02ef-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="e02ef-152">OfferID</span></span></td>
<td><p><span data-ttu-id="e02ef-153">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-153">Unique offer ID.</span></span> <span data-ttu-id="e02ef-154">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="e02ef-155"><b>注意</b>：此值不匹配价格列表中的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="e02ef-156">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="e02ef-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="e02ef-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="e02ef-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="e02ef-159">唯一的持久型产品 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e02ef-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="e02ef-160"><b>注意</b>：此值与从价格列表产品/服务 ID 相匹配。</span><span class="sxs-lookup"><span data-stu-id="e02ef-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="e02ef-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="e02ef-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="e02ef-162">OfferName</span></span></td>
<td><p><span data-ttu-id="e02ef-163">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e02ef-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="e02ef-164">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="e02ef-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="e02ef-166">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="e02ef-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="e02ef-167">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="e02ef-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="e02ef-168">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e02ef-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e02ef-169">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e02ef-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="e02ef-171">订阅结束日期：12 个月 + x 天之后开始日期 （符合合作伙伴计费日期） 或 12 个月续订日期。</span><span class="sxs-lookup"><span data-stu-id="e02ef-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="e02ef-172">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="e02ef-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="e02ef-173">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="e02ef-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="e02ef-174">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e02ef-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e02ef-175">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e02ef-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e02ef-177">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="e02ef-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="e02ef-178">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e02ef-179">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e02ef-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e02ef-180">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e02ef-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e02ef-182">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="e02ef-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="e02ef-183">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e02ef-184">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="e02ef-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e02ef-185">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="e02ef-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e02ef-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="e02ef-187">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="e02ef-187">The type of charge or adjustment.</span></span> <span data-ttu-id="e02ef-188">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e02ef-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e02ef-189">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e02ef-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e02ef-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="e02ef-191">每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="e02ef-191">Price per seat.</span></span> <span data-ttu-id="e02ef-192">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e02ef-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e02ef-193">6.82</span><span class="sxs-lookup"><span data-stu-id="e02ef-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-194">数量</span><span class="sxs-lookup"><span data-stu-id="e02ef-194">Quantity</span></span></td>
<td><p><span data-ttu-id="e02ef-195">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="e02ef-195">Number of seats.</span></span> <span data-ttu-id="e02ef-196">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e02ef-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e02ef-197">2</span><span class="sxs-lookup"><span data-stu-id="e02ef-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-198">金额</span><span class="sxs-lookup"><span data-stu-id="e02ef-198">Amount</span></span></td>
<td><p><span data-ttu-id="e02ef-199">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="e02ef-199">Total of price for quantity.</span></span> <span data-ttu-id="e02ef-200">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="e02ef-201">13.32</span><span class="sxs-lookup"><span data-stu-id="e02ef-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="e02ef-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="e02ef-203">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="e02ef-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="e02ef-204">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="e02ef-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="e02ef-205">2.32</span><span class="sxs-lookup"><span data-stu-id="e02ef-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-206">小计</span><span class="sxs-lookup"><span data-stu-id="e02ef-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="e02ef-207">税前总额。</span><span class="sxs-lookup"><span data-stu-id="e02ef-207">Total before tax.</span></span> <span data-ttu-id="e02ef-208">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="e02ef-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="e02ef-209">11</span><span class="sxs-lookup"><span data-stu-id="e02ef-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-210">税</span><span class="sxs-lookup"><span data-stu-id="e02ef-210">Tax</span></span></td>
<td><p><span data-ttu-id="e02ef-211">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="e02ef-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e02ef-212">0</span><span class="sxs-lookup"><span data-stu-id="e02ef-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="e02ef-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="e02ef-214">税后总额。</span><span class="sxs-lookup"><span data-stu-id="e02ef-214">Total after tax.</span></span> <span data-ttu-id="e02ef-215">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="e02ef-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="e02ef-216">11</span><span class="sxs-lookup"><span data-stu-id="e02ef-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-217">货币</span><span class="sxs-lookup"><span data-stu-id="e02ef-217">Currency</span></span></td>
<td><p><span data-ttu-id="e02ef-218">货币类型。</span><span class="sxs-lookup"><span data-stu-id="e02ef-218">Currency type.</span></span> <span data-ttu-id="e02ef-219">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="e02ef-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="e02ef-220">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="e02ef-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e02ef-221">元</span><span class="sxs-lookup"><span data-stu-id="e02ef-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e02ef-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="e02ef-223">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e02ef-224">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e02ef-225">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="e02ef-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="e02ef-226">MPNID</span></span></td>
<td><p><span data-ttu-id="e02ef-227">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="e02ef-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="e02ef-228">4390934</span><span class="sxs-lookup"><span data-stu-id="e02ef-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e02ef-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e02ef-230">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e02ef-231">请参阅[由合作伙伴列出明细](#itemizebypartner)。</span><span class="sxs-lookup"><span data-stu-id="e02ef-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="e02ef-232">4390934</span><span class="sxs-lookup"><span data-stu-id="e02ef-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="e02ef-233">DomainName</span></span></td>
<td><p><span data-ttu-id="e02ef-234">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="e02ef-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="e02ef-235">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e02ef-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e02ef-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e02ef-237">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-237">Subscription nickname.</span></span> <span data-ttu-id="e02ef-238">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="e02ef-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="e02ef-239">联机项目</span><span class="sxs-lookup"><span data-stu-id="e02ef-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e02ef-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e02ef-241">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e02ef-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e02ef-242">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="e02ef-243">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="e02ef-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="e02ef-244">基于使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="e02ef-244">Usage-based file fields</span></span>


<span data-ttu-id="e02ef-245">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="e02ef-246">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="e02ef-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e02ef-247"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="e02ef-248"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="e02ef-249"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="e02ef-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="e02ef-251">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="e02ef-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e02ef-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e02ef-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="e02ef-254">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="e02ef-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="e02ef-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="e02ef-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="e02ef-257">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="e02ef-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="e02ef-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e02ef-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="e02ef-260">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e02ef-261">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e02ef-262">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="e02ef-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="e02ef-263">MPNID</span></span></td>
<td><p><span data-ttu-id="e02ef-264">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="e02ef-265">4390934</span><span class="sxs-lookup"><span data-stu-id="e02ef-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e02ef-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e02ef-267">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e02ef-268">请参阅[由合作伙伴列出明细](#itemizebypartner)。</span><span class="sxs-lookup"><span data-stu-id="e02ef-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="e02ef-269">4390934</span><span class="sxs-lookup"><span data-stu-id="e02ef-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e02ef-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e02ef-271">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="e02ef-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="e02ef-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="e02ef-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e02ef-274">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="e02ef-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e02ef-275">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e02ef-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e02ef-276">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e02ef-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e02ef-278">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="e02ef-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e02ef-279">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="e02ef-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e02ef-280">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="e02ef-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e02ef-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e02ef-282">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e02ef-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e02ef-283">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e02ef-284">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="e02ef-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e02ef-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e02ef-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e02ef-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e02ef-287">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="e02ef-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e02ef-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e02ef-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e02ef-290">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="e02ef-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="e02ef-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e02ef-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="e02ef-292">OrderID</span></span></td>
<td><p><span data-ttu-id="e02ef-293">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e02ef-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e02ef-294">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e02ef-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e02ef-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="e02ef-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="e02ef-297">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="e02ef-298">虚拟机</span><span class="sxs-lookup"><span data-stu-id="e02ef-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="e02ef-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="e02ef-300">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="e02ef-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e02ef-301">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="e02ef-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="e02ef-302">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="e02ef-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="e02ef-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="e02ef-304">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e02ef-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="e02ef-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e02ef-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-306">资源名称</span><span class="sxs-lookup"><span data-stu-id="e02ef-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="e02ef-307">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="e02ef-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e02ef-308">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="e02ef-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="e02ef-309">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="e02ef-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-310">Region</span><span class="sxs-lookup"><span data-stu-id="e02ef-310">Region</span></span></td>
<td><p><span data-ttu-id="e02ef-311">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="e02ef-311">The region the usage applies to.</span></span> <span data-ttu-id="e02ef-312">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="e02ef-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="e02ef-313">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="e02ef-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-314">SKU</span><span class="sxs-lookup"><span data-stu-id="e02ef-314">SKU</span></span></td>
<td><p><span data-ttu-id="e02ef-315">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e02ef-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="e02ef-316">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="e02ef-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="e02ef-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="e02ef-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="e02ef-318">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="e02ef-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="e02ef-319">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="e02ef-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="e02ef-320">1</span><span class="sxs-lookup"><span data-stu-id="e02ef-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="e02ef-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="e02ef-322">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="e02ef-323">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="e02ef-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="e02ef-324">11</span><span class="sxs-lookup"><span data-stu-id="e02ef-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="e02ef-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="e02ef-326">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="e02ef-326">Units included as part of the offer.</span></span> <span data-ttu-id="e02ef-327">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="e02ef-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="e02ef-328">0</span><span class="sxs-lookup"><span data-stu-id="e02ef-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="e02ef-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="e02ef-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="e02ef-330">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="e02ef-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="e02ef-331">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="e02ef-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="e02ef-332">11</span><span class="sxs-lookup"><span data-stu-id="e02ef-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="e02ef-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="e02ef-334">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="e02ef-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="e02ef-335">$0.0808</span><span class="sxs-lookup"><span data-stu-id="e02ef-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="e02ef-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="e02ef-337">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="e02ef-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e02ef-338">$0.085</span><span class="sxs-lookup"><span data-stu-id="e02ef-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="e02ef-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="e02ef-340">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="e02ef-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e02ef-341">$0.08</span><span class="sxs-lookup"><span data-stu-id="e02ef-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="e02ef-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="e02ef-343">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="e02ef-344">$0.93</span><span class="sxs-lookup"><span data-stu-id="e02ef-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-345">货币</span><span class="sxs-lookup"><span data-stu-id="e02ef-345">Currency</span></span></td>
<td><p><span data-ttu-id="e02ef-346">货币类型。</span><span class="sxs-lookup"><span data-stu-id="e02ef-346">Currency type.</span></span> <span data-ttu-id="e02ef-347">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="e02ef-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="e02ef-348">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="e02ef-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e02ef-349">元</span><span class="sxs-lookup"><span data-stu-id="e02ef-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e02ef-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e02ef-351">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="e02ef-351">Pretax price per unit.</span></span> <span data-ttu-id="e02ef-352">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="e02ef-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e02ef-353">$0.08</span><span class="sxs-lookup"><span data-stu-id="e02ef-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e02ef-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e02ef-355">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="e02ef-355">Post tax price per unit.</span></span> <span data-ttu-id="e02ef-356">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="e02ef-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e02ef-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="e02ef-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e02ef-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="e02ef-359">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="e02ef-359">The type of charge or adjustment.</span></span> <span data-ttu-id="e02ef-360">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e02ef-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e02ef-361">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e02ef-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="e02ef-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="e02ef-363">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="e02ef-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="e02ef-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="e02ef-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="e02ef-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="e02ef-366">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="e02ef-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="e02ef-367">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e02ef-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="e02ef-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="e02ef-369">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="e02ef-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="e02ef-370">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="e02ef-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="e02ef-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="e02ef-372">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="e02ef-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="e02ef-373">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="e02ef-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="e02ef-374">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="e02ef-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="e02ef-375">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="e02ef-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="e02ef-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="e02ef-377">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="e02ef-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="e02ef-378">外部</span><span class="sxs-lookup"><span data-stu-id="e02ef-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-379">项目</span><span class="sxs-lookup"><span data-stu-id="e02ef-379">Project</span></span></td>
<td><p><span data-ttu-id="e02ef-380">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="e02ef-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="e02ef-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e02ef-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="e02ef-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="e02ef-383">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="e02ef-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="e02ef-384">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="e02ef-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="e02ef-385">如果必须预配的服务总线连接的 25 包，并且你必须在那一天中使用了 1，这一天您每日使用情况语句将指示"25 连接 / 30 天 – 使用：1.000000”.</span><span class="sxs-lookup"><span data-stu-id="e02ef-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e02ef-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e02ef-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="e02ef-387">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="e02ef-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e02ef-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e02ef-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e02ef-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="e02ef-389">DomainName</span></span></td>
<td><p><span data-ttu-id="e02ef-390">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="e02ef-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="e02ef-391">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e02ef-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="e02ef-392">发票和对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="e02ef-393">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="e02ef-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="e02ef-394">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="e02ef-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="e02ef-395">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="e02ef-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="e02ef-396"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-397"><strong>对帐文件费用说明 （ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-398"><strong>什么是此费用？</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-399"><strong>如何将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="e02ef-400"><strong>周期性费用</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-401">取消实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="e02ef-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-402">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="e02ef-403">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-404">周期费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-405">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-406">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="e02ef-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-407">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-408">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-409">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="e02ef-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-410">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-411">购买后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-412">购买费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-413">订阅的初始费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-414">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-415">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-416">续订费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-417">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-418"><strong>其他产品和服务</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-419">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-420">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-421">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="e02ef-422"><strong>使用费</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-423">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-424">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="e02ef-425">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-426">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-427">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-428"><strong>信用额度&amp;调整</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-429">偏移行项</span><span class="sxs-lookup"><span data-stu-id="e02ef-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-430">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="e02ef-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-431">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="e02ef-432">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="e02ef-433"><strong>其他折扣</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="e02ef-434">
<em>(usage-based)</em></span><span class="sxs-lookup"><span data-stu-id="e02ef-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-435">激活折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-436">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="e02ef-437">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-438">周期折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-439">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="e02ef-440">续订折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-441">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="e02ef-442">取消折扣</span><span class="sxs-lookup"><span data-stu-id="e02ef-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-443">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="e02ef-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-444"><strong>其他折扣</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="e02ef-445">
<em>（基于许可证的）</em></span><span class="sxs-lookup"><span data-stu-id="e02ef-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-446"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="e02ef-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="e02ef-447">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e02ef-448"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="e02ef-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-449"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="e02ef-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="e02ef-450"><em>异常："偏移量行项"已包含的税款。请参阅信用额度&amp;调整、 更高版本。</em></span><span class="sxs-lookup"><span data-stu-id="e02ef-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-451">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="e02ef-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="e02ef-452">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="e02ef-453">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e02ef-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
