---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
description: 在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 5ce9b7cd9ead08b7709c68a0e967d64e9f2a32bd
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57585130"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="cccb7-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="cccb7-103">Use the reconciliation files</span></span>

<span data-ttu-id="cccb7-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="cccb7-104">**Applies to**</span></span>

-  <span data-ttu-id="cccb7-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="cccb7-105">Partner Center</span></span>
-  <span data-ttu-id="cccb7-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="cccb7-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="cccb7-107">在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。</span><span class="sxs-lookup"><span data-stu-id="cccb7-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="cccb7-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="cccb7-109">由合作伙伴详细列举</span><span class="sxs-lookup"><span data-stu-id="cccb7-109">Itemize by partner</span></span>


<span data-ttu-id="cccb7-110">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="cccb7-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cccb7-111">MPN ID</span><span class="sxs-lookup"><span data-stu-id="cccb7-111">MPN ID</span></span></th>
<th><span data-ttu-id="cccb7-112">描述</span><span class="sxs-lookup"><span data-stu-id="cccb7-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cccb7-113">MPN ID</span><span class="sxs-lookup"><span data-stu-id="cccb7-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="cccb7-114">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-115">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="cccb7-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="cccb7-116">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="cccb7-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="cccb7-117">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cccb7-118">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="cccb7-119">干支查看或更新的分销商，在合作伙伴中心菜单中，选择<strong>客户</strong>，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="cccb7-120">在客户菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="cccb7-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="cccb7-121">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="cccb7-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="cccb7-122">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="cccb7-123">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="cccb7-124">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="cccb7-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="cccb7-125">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="cccb7-125">License-based file fields</span></span>


<span data-ttu-id="cccb7-126">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cccb7-127"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="cccb7-128"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="cccb7-129"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="cccb7-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="cccb7-131">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="cccb7-132">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="cccb7-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="cccb7-133">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="cccb7-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="cccb7-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="cccb7-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="cccb7-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="cccb7-136">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="cccb7-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="cccb7-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="cccb7-138">OrderID</span></span></td>
<td><p><span data-ttu-id="cccb7-139">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="cccb7-140">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="cccb7-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="cccb7-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="cccb7-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="cccb7-143">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cccb7-144">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="cccb7-145">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="cccb7-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="cccb7-146">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="cccb7-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="cccb7-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="cccb7-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="cccb7-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="cccb7-149">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="cccb7-150">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="cccb7-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="cccb7-151">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="cccb7-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="cccb7-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="cccb7-153">OfferID</span></span></td>
<td><p><span data-ttu-id="cccb7-154">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-154">Unique offer ID.</span></span> <span data-ttu-id="cccb7-155">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="cccb7-156"><b>注意</b>：此值不匹配价格列表中的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="cccb7-157">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="cccb7-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="cccb7-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="cccb7-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="cccb7-160">唯一的持久型产品 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="cccb7-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="cccb7-161"><b>注意</b>：此值与从价格列表产品/服务 ID 相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="cccb7-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="cccb7-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="cccb7-163">OfferName</span></span></td>
<td><p><span data-ttu-id="cccb7-164">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="cccb7-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="cccb7-165">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="cccb7-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="cccb7-167">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="cccb7-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="cccb7-168">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="cccb7-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="cccb7-169">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="cccb7-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cccb7-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cccb7-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="cccb7-172">订阅结束日期：12 个月 + x 天之后开始日期 （符合合作伙伴计费日期） 或 12 个月续订日期。</span><span class="sxs-lookup"><span data-stu-id="cccb7-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="cccb7-173">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="cccb7-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="cccb7-174">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="cccb7-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="cccb7-175">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="cccb7-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cccb7-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cccb7-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cccb7-178">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="cccb7-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="cccb7-179">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="cccb7-180">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="cccb7-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cccb7-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cccb7-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cccb7-183">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="cccb7-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="cccb7-184">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="cccb7-185">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="cccb7-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="cccb7-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="cccb7-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="cccb7-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="cccb7-188">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-188">The type of charge or adjustment.</span></span> <span data-ttu-id="cccb7-189">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="cccb7-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="cccb7-190">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="cccb7-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="cccb7-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="cccb7-192">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="cccb7-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cccb7-193">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="cccb7-194">6.82</span><span class="sxs-lookup"><span data-stu-id="cccb7-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-195">数量</span><span class="sxs-lookup"><span data-stu-id="cccb7-195">Quantity</span></span></td>
<td><p><span data-ttu-id="cccb7-196">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="cccb7-196">Number of seats.</span></span> <span data-ttu-id="cccb7-197">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="cccb7-198">2</span><span class="sxs-lookup"><span data-stu-id="cccb7-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-199">金额</span><span class="sxs-lookup"><span data-stu-id="cccb7-199">Amount</span></span></td>
<td><p><span data-ttu-id="cccb7-200">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="cccb7-200">Total of price for quantity.</span></span> <span data-ttu-id="cccb7-201">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="cccb7-202">13.32</span><span class="sxs-lookup"><span data-stu-id="cccb7-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="cccb7-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="cccb7-204">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="cccb7-205">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="cccb7-206">2.32</span><span class="sxs-lookup"><span data-stu-id="cccb7-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-207">小计</span><span class="sxs-lookup"><span data-stu-id="cccb7-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="cccb7-208">税前总额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-208">Total before tax.</span></span> <span data-ttu-id="cccb7-209">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="cccb7-210">11</span><span class="sxs-lookup"><span data-stu-id="cccb7-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-211">税</span><span class="sxs-lookup"><span data-stu-id="cccb7-211">Tax</span></span></td>
<td><p><span data-ttu-id="cccb7-212">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="cccb7-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="cccb7-213">0</span><span class="sxs-lookup"><span data-stu-id="cccb7-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="cccb7-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="cccb7-215">税后总额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-215">Total after tax.</span></span> <span data-ttu-id="cccb7-216">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="cccb7-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="cccb7-217">11</span><span class="sxs-lookup"><span data-stu-id="cccb7-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-218">货币</span><span class="sxs-lookup"><span data-stu-id="cccb7-218">Currency</span></span></td>
<td><p><span data-ttu-id="cccb7-219">货币类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-219">Currency type.</span></span> <span data-ttu-id="cccb7-220">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="cccb7-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="cccb7-221">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="cccb7-222">EUR</span><span class="sxs-lookup"><span data-stu-id="cccb7-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="cccb7-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="cccb7-224">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="cccb7-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="cccb7-225">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="cccb7-226">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="cccb7-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="cccb7-227">MPNID</span></span></td>
<td><p><span data-ttu-id="cccb7-228">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="cccb7-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="cccb7-229">4390934</span><span class="sxs-lookup"><span data-stu-id="cccb7-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="cccb7-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="cccb7-231">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cccb7-232">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="cccb7-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="cccb7-233">4390934</span><span class="sxs-lookup"><span data-stu-id="cccb7-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="cccb7-234">DomainName</span></span></td>
<td><p><span data-ttu-id="cccb7-235">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="cccb7-236">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="cccb7-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="cccb7-237">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="cccb7-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="cccb7-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cccb7-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="cccb7-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="cccb7-240">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-240">Subscription nickname.</span></span> <span data-ttu-id="cccb7-241">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="cccb7-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="cccb7-242">联机项目</span><span class="sxs-lookup"><span data-stu-id="cccb7-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="cccb7-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="cccb7-244">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="cccb7-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="cccb7-245">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="cccb7-246">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="cccb7-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="cccb7-247">基于使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="cccb7-247">Usage-based file fields</span></span>


<span data-ttu-id="cccb7-248">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="cccb7-249">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="cccb7-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cccb7-250"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="cccb7-251"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="cccb7-252"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="cccb7-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="cccb7-254">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="cccb7-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="cccb7-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="cccb7-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="cccb7-257">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="cccb7-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="cccb7-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="cccb7-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="cccb7-260">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="cccb7-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="cccb7-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="cccb7-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="cccb7-263">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="cccb7-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="cccb7-264">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="cccb7-265">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="cccb7-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="cccb7-266">MPNID</span></span></td>
<td><p><span data-ttu-id="cccb7-267">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="cccb7-268">4390934</span><span class="sxs-lookup"><span data-stu-id="cccb7-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="cccb7-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="cccb7-270">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cccb7-271">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="cccb7-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="cccb7-272">4390934</span><span class="sxs-lookup"><span data-stu-id="cccb7-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="cccb7-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="cccb7-274">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="cccb7-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="cccb7-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="cccb7-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cccb7-277">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="cccb7-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="cccb7-278">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="cccb7-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cccb7-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="cccb7-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cccb7-281">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="cccb7-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="cccb7-282">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="cccb7-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="cccb7-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="cccb7-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="cccb7-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="cccb7-285">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cccb7-286">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="cccb7-287">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="cccb7-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="cccb7-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="cccb7-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="cccb7-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="cccb7-290">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="cccb7-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cccb7-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="cccb7-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="cccb7-293">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="cccb7-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="cccb7-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cccb7-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="cccb7-295">OrderID</span></span></td>
<td><p><span data-ttu-id="cccb7-296">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="cccb7-297">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="cccb7-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="cccb7-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="cccb7-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="cccb7-300">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="cccb7-301">虚拟机</span><span class="sxs-lookup"><span data-stu-id="cccb7-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="cccb7-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="cccb7-303">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="cccb7-304">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="cccb7-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="cccb7-305">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="cccb7-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="cccb7-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="cccb7-307">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="cccb7-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="cccb7-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-309">资源名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="cccb7-310">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="cccb7-311">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="cccb7-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="cccb7-312">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="cccb7-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-313">Region</span><span class="sxs-lookup"><span data-stu-id="cccb7-313">Region</span></span></td>
<td><p><span data-ttu-id="cccb7-314">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="cccb7-314">The region the usage applies to.</span></span> <span data-ttu-id="cccb7-315">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="cccb7-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="cccb7-316">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="cccb7-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-317">SKU</span><span class="sxs-lookup"><span data-stu-id="cccb7-317">SKU</span></span></td>
<td><p><span data-ttu-id="cccb7-318">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cccb7-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="cccb7-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="cccb7-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="cccb7-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="cccb7-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="cccb7-321">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="cccb7-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="cccb7-322">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="cccb7-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="cccb7-323">1</span><span class="sxs-lookup"><span data-stu-id="cccb7-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="cccb7-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="cccb7-325">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="cccb7-326">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="cccb7-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="cccb7-327">11</span><span class="sxs-lookup"><span data-stu-id="cccb7-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="cccb7-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="cccb7-329">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="cccb7-329">Units included as part of the offer.</span></span> <span data-ttu-id="cccb7-330">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="cccb7-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="cccb7-331">0</span><span class="sxs-lookup"><span data-stu-id="cccb7-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="cccb7-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="cccb7-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="cccb7-333">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="cccb7-334">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="cccb7-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="cccb7-335">11</span><span class="sxs-lookup"><span data-stu-id="cccb7-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="cccb7-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="cccb7-337">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="cccb7-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="cccb7-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="cccb7-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="cccb7-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="cccb7-340">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="cccb7-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cccb7-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="cccb7-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="cccb7-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="cccb7-343">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="cccb7-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="cccb7-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="cccb7-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="cccb7-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="cccb7-346">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="cccb7-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="cccb7-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-348">货币</span><span class="sxs-lookup"><span data-stu-id="cccb7-348">Currency</span></span></td>
<td><p><span data-ttu-id="cccb7-349">货币类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-349">Currency type.</span></span> <span data-ttu-id="cccb7-350">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="cccb7-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="cccb7-351">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="cccb7-352">EUR</span><span class="sxs-lookup"><span data-stu-id="cccb7-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="cccb7-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="cccb7-354">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="cccb7-354">Pretax price per unit.</span></span> <span data-ttu-id="cccb7-355">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="cccb7-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cccb7-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="cccb7-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="cccb7-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="cccb7-358">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="cccb7-358">Post tax price per unit.</span></span> <span data-ttu-id="cccb7-359">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="cccb7-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cccb7-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="cccb7-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="cccb7-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="cccb7-362">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-362">The type of charge or adjustment.</span></span> <span data-ttu-id="cccb7-363">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="cccb7-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="cccb7-364">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="cccb7-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="cccb7-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="cccb7-366">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="cccb7-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="cccb7-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="cccb7-369">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="cccb7-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="cccb7-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="cccb7-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="cccb7-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="cccb7-372">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="cccb7-373">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="cccb7-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="cccb7-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="cccb7-375">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="cccb7-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="cccb7-376">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="cccb7-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="cccb7-377">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="cccb7-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="cccb7-378">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="cccb7-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="cccb7-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="cccb7-380">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="cccb7-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="cccb7-381">外部</span><span class="sxs-lookup"><span data-stu-id="cccb7-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-382">项目</span><span class="sxs-lookup"><span data-stu-id="cccb7-382">Project</span></span></td>
<td><p><span data-ttu-id="cccb7-383">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="cccb7-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="cccb7-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="cccb7-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="cccb7-386">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="cccb7-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="cccb7-387">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="cccb7-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="cccb7-388">如果必须预配的服务总线连接的 25 包，并且你必须在那一天中使用了 1，这一天您每日使用情况语句将指示"25 连接 / 30 天 – 使用：1.000000”.</span><span class="sxs-lookup"><span data-stu-id="cccb7-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="cccb7-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="cccb7-390">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="cccb7-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="cccb7-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cccb7-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="cccb7-392">DomainName</span></span></td>
<td><p><span data-ttu-id="cccb7-393">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="cccb7-394">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="cccb7-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="cccb7-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cccb7-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="cccb7-396">单位</span><span class="sxs-lookup"><span data-stu-id="cccb7-396">Unit</span></span></td>
<td><p><span data-ttu-id="cccb7-397">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="cccb7-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="cccb7-398">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="cccb7-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="cccb7-399">一次性和重复性文件字段</span><span class="sxs-lookup"><span data-stu-id="cccb7-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cccb7-400">列</span><span class="sxs-lookup"><span data-stu-id="cccb7-400">Column</span></span></th>
<th><span data-ttu-id="cccb7-401">描述</span><span class="sxs-lookup"><span data-stu-id="cccb7-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="cccb7-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="cccb7-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="cccb7-403">唯一的 GUID 格式中的特定计费实体的 Microsoft Azure Active Directory 租户标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="cccb7-404">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="cccb7-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="cccb7-405">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="cccb7-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-406">客户 Id</span><span class="sxs-lookup"><span data-stu-id="cccb7-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="cccb7-407">Microsoft Azure Active Directory 租户中唯一 ID，用于标识客户的 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="cccb7-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-408">客户名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="cccb7-409">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="cccb7-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="cccb7-411">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="cccb7-412">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="cccb7-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="cccb7-413">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="cccb7-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-414">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="cccb7-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="cccb7-415">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="cccb7-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-416">发票编号</span><span class="sxs-lookup"><span data-stu-id="cccb7-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="cccb7-417">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="cccb7-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="cccb7-418">MpnId</span></span></td>
<td><p><span data-ttu-id="cccb7-419">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-420">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="cccb7-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="cccb7-421">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-422">订单编码</span><span class="sxs-lookup"><span data-stu-id="cccb7-422">Order ID</span></span></td>
<td><p><span data-ttu-id="cccb7-423">Microsoft 商务平台中的订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="cccb7-424">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-425">订单日期</span><span class="sxs-lookup"><span data-stu-id="cccb7-425">Order date</span></span></td>
<td><p><span data-ttu-id="cccb7-426">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="cccb7-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="cccb7-427">ProductId</span></span></td>
<td><p><span data-ttu-id="cccb7-428">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="cccb7-429">SkuId</span></span></td>
<td><p><span data-ttu-id="cccb7-430">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="cccb7-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="cccb7-432">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-432">The ID for a particular Availability.</span></span> <span data-ttu-id="cccb7-433">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="cccb7-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-434">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="cccb7-435">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-436">产品名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-436">Product name</span></span></td>
<td><p><span data-ttu-id="cccb7-437">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="cccb7-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="cccb7-439">该产品的发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="cccb7-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="cccb7-441">此发布服务器的的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-442">订阅说明</span><span class="sxs-lookup"><span data-stu-id="cccb7-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="cccb7-443">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-444">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="cccb7-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="cccb7-445">Microsoft 商务平台中的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="cccb7-446">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="cccb7-447">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="cccb7-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cccb7-449">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="cccb7-449">Start day of the charges.</span></span> <span data-ttu-id="cccb7-450">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="cccb7-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cccb7-452">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="cccb7-452">End day of the charges.</span></span> <span data-ttu-id="cccb7-453">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="cccb7-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-454">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="cccb7-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="cccb7-455">期限长度和购买的计费周期。</span><span class="sxs-lookup"><span data-stu-id="cccb7-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="cccb7-456">例如，"1 年，每月一次。"</span><span class="sxs-lookup"><span data-stu-id="cccb7-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-457">费用类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="cccb7-458">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-459">单价</span><span class="sxs-lookup"><span data-stu-id="cccb7-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="cccb7-460">因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="cccb7-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cccb7-461">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-462">有效的单位价格</span><span class="sxs-lookup"><span data-stu-id="cccb7-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="cccb7-463">单位价格后已进行调整。</span><span class="sxs-lookup"><span data-stu-id="cccb7-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-464">数量</span><span class="sxs-lookup"><span data-stu-id="cccb7-464">Quantity</span></span></td>
<td><p><span data-ttu-id="cccb7-465">单位数。</span><span class="sxs-lookup"><span data-stu-id="cccb7-465">Number of units.</span></span> <span data-ttu-id="cccb7-466">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-467">单位类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-467">Unit type</span></span></td>
<td><p><span data-ttu-id="cccb7-468">正在购买一个单位的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="cccb7-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="cccb7-470">所有适用的折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="cccb7-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-471">子汇总</span><span class="sxs-lookup"><span data-stu-id="cccb7-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="cccb7-472">税前总额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-472">Total before tax.</span></span> <span data-ttu-id="cccb7-473">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-474">税务总计</span><span class="sxs-lookup"><span data-stu-id="cccb7-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="cccb7-475">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="cccb7-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-476">总计</span><span class="sxs-lookup"><span data-stu-id="cccb7-476">Total</span></span></td>
<td><p><span data-ttu-id="cccb7-477">税后总额。</span><span class="sxs-lookup"><span data-stu-id="cccb7-477">Total after tax.</span></span> <span data-ttu-id="cccb7-478">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="cccb7-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-479">货币</span><span class="sxs-lookup"><span data-stu-id="cccb7-479">Currency</span></span></td>
<td><p><span data-ttu-id="cccb7-480">货币类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-480">Currency type.</span></span> <span data-ttu-id="cccb7-481">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="cccb7-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="cccb7-482">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="cccb7-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="cccb7-484">备用标识符关联到一个 id。</span><span class="sxs-lookup"><span data-stu-id="cccb7-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="cccb7-485">评定的每日使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="cccb7-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cccb7-486">列</span><span class="sxs-lookup"><span data-stu-id="cccb7-486">Column</span></span></th>
<th><span data-ttu-id="cccb7-487">描述</span><span class="sxs-lookup"><span data-stu-id="cccb7-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="cccb7-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="cccb7-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="cccb7-489">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="cccb7-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="cccb7-491">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="cccb7-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="cccb7-493">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="cccb7-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="cccb7-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="cccb7-495">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="cccb7-496">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="cccb7-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="cccb7-498">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="cccb7-498">The customer’s domain name.</span></span> <span data-ttu-id="cccb7-499">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-500">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="cccb7-500">Customer country</span></span></td>
<td><p><span data-ttu-id="cccb7-501">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="cccb7-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="cccb7-502">MPNID</span></span></td>
<td><p><span data-ttu-id="cccb7-503">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-504">分销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="cccb7-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="cccb7-505">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cccb7-506">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="cccb7-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="cccb7-508">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="cccb7-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="cccb7-509">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="cccb7-510">ProductId</span></span></td>
<td><p><span data-ttu-id="cccb7-511">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="cccb7-512">SkuId</span></span></td>
<td><p><span data-ttu-id="cccb7-513">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="cccb7-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="cccb7-515">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-515">The ID for a particular Availability.</span></span> <span data-ttu-id="cccb7-516">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="cccb7-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-517">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="cccb7-518">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="cccb7-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="cccb7-520">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="cccb7-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="cccb7-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="cccb7-522">GUID 格式中的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="cccb7-523">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="cccb7-524">订阅说明</span><span class="sxs-lookup"><span data-stu-id="cccb7-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="cccb7-525">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="cccb7-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="cccb7-526">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-527">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="cccb7-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="cccb7-528">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cccb7-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cccb7-529">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="cccb7-530">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="cccb7-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cccb7-532">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="cccb7-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="cccb7-533">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="cccb7-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cccb7-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cccb7-535">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="cccb7-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="cccb7-536">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="cccb7-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-537">使用日期</span><span class="sxs-lookup"><span data-stu-id="cccb7-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="cccb7-538">服务使用情况的日期。</span><span class="sxs-lookup"><span data-stu-id="cccb7-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-539">计量类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="cccb7-540">测定仪的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-541">计量类别</span><span class="sxs-lookup"><span data-stu-id="cccb7-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="cccb7-542">用于使用情况的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="cccb7-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-543">计量 Id</span><span class="sxs-lookup"><span data-stu-id="cccb7-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="cccb7-544">正在使用的计量 ID。</span><span class="sxs-lookup"><span data-stu-id="cccb7-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-545">计量子类别</span><span class="sxs-lookup"><span data-stu-id="cccb7-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="cccb7-546">可以会影响费率的 Azure 服务的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-547">测定仪名称</span><span class="sxs-lookup"><span data-stu-id="cccb7-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="cccb7-548">已使用的测定仪的度量单位。</span><span class="sxs-lookup"><span data-stu-id="cccb7-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-549">计量区域</span><span class="sxs-lookup"><span data-stu-id="cccb7-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="cccb7-550">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-551">单位</span><span class="sxs-lookup"><span data-stu-id="cccb7-551">Unit</span></span></td>
<td><p><span data-ttu-id="cccb7-552">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="cccb7-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-553">已使用的数量</span><span class="sxs-lookup"><span data-stu-id="cccb7-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="cccb7-554">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="cccb7-555">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="cccb7-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-556">资源位置</span><span class="sxs-lookup"><span data-stu-id="cccb7-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="cccb7-557">测定仪正在其中运行数据中心。</span><span class="sxs-lookup"><span data-stu-id="cccb7-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-558">使用的服务</span><span class="sxs-lookup"><span data-stu-id="cccb7-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="cccb7-559">使用 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="cccb7-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-560">资源组</span><span class="sxs-lookup"><span data-stu-id="cccb7-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="cccb7-561">资源组部署的测定仪正在其中运行。</span><span class="sxs-lookup"><span data-stu-id="cccb7-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-562">资源 URI</span><span class="sxs-lookup"><span data-stu-id="cccb7-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="cccb7-563">正在使用的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="cccb7-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-564">费用类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-564">Charge type</span></span></td>
<td><p><span data-ttu-id="cccb7-565">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-565">The type of charge or adjustment.</span></span> <span data-ttu-id="cccb7-566">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-567">单价</span><span class="sxs-lookup"><span data-stu-id="cccb7-567">Unit price</span></span></td>
<td><p><span data-ttu-id="cccb7-568">每个许可证，因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="cccb7-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cccb7-569">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-570">数量</span><span class="sxs-lookup"><span data-stu-id="cccb7-570">Quantity</span></span></td>
<td><p><span data-ttu-id="cccb7-571">许可证的数量。</span><span class="sxs-lookup"><span data-stu-id="cccb7-571">Number of licenses.</span></span> <span data-ttu-id="cccb7-572">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="cccb7-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-573">单位类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-573">Unit type</span></span></td>
<td><p><span data-ttu-id="cccb7-574">测定仪的计价中的单元的类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="cccb7-575">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-576">计费 pre 税</span><span class="sxs-lookup"><span data-stu-id="cccb7-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="cccb7-577">税前的总量。</span><span class="sxs-lookup"><span data-stu-id="cccb7-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-578">计费货币</span><span class="sxs-lookup"><span data-stu-id="cccb7-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="cccb7-579">客户所在的地理区域中的币种</span><span class="sxs-lookup"><span data-stu-id="cccb7-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-580">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="cccb7-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="cccb7-581">定价之前添加的税款。</span><span class="sxs-lookup"><span data-stu-id="cccb7-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-582">定价货币</span><span class="sxs-lookup"><span data-stu-id="cccb7-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="cccb7-583">在价目表中货币。</span><span class="sxs-lookup"><span data-stu-id="cccb7-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-584">服务信息 1</span><span class="sxs-lookup"><span data-stu-id="cccb7-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="cccb7-585">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="cccb7-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-586">服务信息 2</span><span class="sxs-lookup"><span data-stu-id="cccb7-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="cccb7-587">旧字段，用于捕获可选的服务特定元数据的说明。</span><span class="sxs-lookup"><span data-stu-id="cccb7-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cccb7-588">标记</span><span class="sxs-lookup"><span data-stu-id="cccb7-588">Tags</span></span></td>
<td><p><span data-ttu-id="cccb7-589">分配给测定仪按顺序对计费记录进行分组的标记。</span><span class="sxs-lookup"><span data-stu-id="cccb7-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="cccb7-590">例如，可以使用标记按使用测定仪的部门分配费用。</span><span class="sxs-lookup"><span data-stu-id="cccb7-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cccb7-591">其他信息</span><span class="sxs-lookup"><span data-stu-id="cccb7-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="cccb7-592">其他列中未涉及的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="cccb7-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="cccb7-593">发票和对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="cccb7-594">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="cccb7-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="cccb7-595">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="cccb7-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="cccb7-596">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="cccb7-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="cccb7-597">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="cccb7-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="cccb7-598">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="cccb7-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="cccb7-599"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-600"><strong>对帐文件费用说明 （ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-601"><strong>什么是此费用？</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-602"><strong>如何将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="cccb7-603"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-604">激活费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-605">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="cccb7-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="cccb7-606">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-607">取消费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-608">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-609">周期费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-610">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-611">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="cccb7-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-612">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-613">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-614">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="cccb7-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-615">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-616">订阅时使用年出单费用类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-617">购买费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-618">使用每月费用时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="cccb7-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-619">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-620">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="cccb7-621">续订费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-622">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-623">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-624">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="cccb7-625"><strong>使用费</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-626">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-627">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="cccb7-628">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-629">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-630">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-631"><strong>信用额度</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-632">偏移行项</span><span class="sxs-lookup"><span data-stu-id="cccb7-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-633">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="cccb7-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-634">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="cccb7-635">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="cccb7-636"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-637">激活折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-638">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="cccb7-639">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-640">周期折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-641">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-642">续订折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-643">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-644">取消折扣</span><span class="sxs-lookup"><span data-stu-id="cccb7-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-645">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="cccb7-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="cccb7-646"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-647"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="cccb7-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="cccb7-648">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cccb7-649"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="cccb7-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-650"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="cccb7-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="cccb7-651"><em>异常：&quot;行项的偏移量&quot;已包含的税款。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="cccb7-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-652">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="cccb7-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="cccb7-653">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="cccb7-654">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="cccb7-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
