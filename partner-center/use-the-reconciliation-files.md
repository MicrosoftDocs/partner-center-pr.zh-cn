---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
description: 在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 275d3eee5613d52f0ac7b8c78f7a7ddd74f56c9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2019
ms.locfileid: "59430196"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="f420a-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="f420a-103">Use the reconciliation files</span></span>

**<span data-ttu-id="f420a-104">适用对象</span><span class="sxs-lookup"><span data-stu-id="f420a-104">Applies to</span></span>**

-  <span data-ttu-id="f420a-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="f420a-105">Partner Center</span></span>
-  <span data-ttu-id="f420a-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="f420a-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="f420a-107">在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。</span><span class="sxs-lookup"><span data-stu-id="f420a-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="f420a-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="f420a-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="f420a-109">格式设置问题</span><span class="sxs-lookup"><span data-stu-id="f420a-109">Formatting issues</span></span>

<span data-ttu-id="f420a-110">偶尔侦测文件可能会遇到格式问题。</span><span class="sxs-lookup"><span data-stu-id="f420a-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="f420a-111">（这可能发生，例如，如果不使用 EN-US 区域设置。）请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="f420a-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="f420a-112">在 Excel 中打开.csv 文件，并选择第一列。</span><span class="sxs-lookup"><span data-stu-id="f420a-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="f420a-113">在功能区中，选择<strong>数据</strong>，然后选择<strong>分列</strong>。</span><span class="sxs-lookup"><span data-stu-id="f420a-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="f420a-114">在转换文本分列向导，选择<strong>分隔的文件类型</strong>，然后选择<strong>下一步</strong>。</span><span class="sxs-lookup"><span data-stu-id="f420a-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="f420a-115">在分隔符字段中，选择<strong>逗号</strong>。</span><span class="sxs-lookup"><span data-stu-id="f420a-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="f420a-116">如果<strong>选项卡</strong>是尚未选中，你可以将其保留。</span><span class="sxs-lookup"><span data-stu-id="f420a-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="f420a-117">选择“<strong>下一步</strong>”。</span><span class="sxs-lookup"><span data-stu-id="f420a-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="f420a-118">在列数据格式字段中，选择<strong>日期：MDY</strong>，然后选择<strong>下一步</strong>。</span><span class="sxs-lookup"><span data-stu-id="f420a-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="f420a-119">在列数据格式字段中，选择<strong>文本</strong>的列，并选择所有金额<strong>完成</strong>。</span><span class="sxs-lookup"><span data-stu-id="f420a-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="f420a-120">由合作伙伴详细列举</span><span class="sxs-lookup"><span data-stu-id="f420a-120">Itemize by partner</span></span>


<span data-ttu-id="f420a-121">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="f420a-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f420a-122">MPN ID</span><span class="sxs-lookup"><span data-stu-id="f420a-122">MPN ID</span></span></th>
<th><span data-ttu-id="f420a-123">描述</span><span class="sxs-lookup"><span data-stu-id="f420a-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f420a-124">MPN ID</span><span class="sxs-lookup"><span data-stu-id="f420a-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="f420a-125">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-126">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="f420a-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="f420a-127">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="f420a-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="f420a-128">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f420a-129">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="f420a-130">干支查看或更新的分销商，在合作伙伴中心菜单中，选择<strong>客户</strong>，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="f420a-131">在客户菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="f420a-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="f420a-132">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="f420a-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="f420a-133">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="f420a-134">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="f420a-135">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="f420a-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="f420a-136">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="f420a-136">License-based file fields</span></span>


<span data-ttu-id="f420a-137">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="f420a-138">列</span><span class="sxs-lookup"><span data-stu-id="f420a-138">Column</span></span></strong></td>
<td><strong><span data-ttu-id="f420a-139">描述</span><span class="sxs-lookup"><span data-stu-id="f420a-139">Description</span></span></strong></td>
<td><strong><span data-ttu-id="f420a-140">示例值</span><span class="sxs-lookup"><span data-stu-id="f420a-140">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f420a-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="f420a-142">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="f420a-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f420a-143">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="f420a-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f420a-144">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="f420a-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="f420a-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="f420a-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f420a-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="f420a-147">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f420a-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="f420a-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="f420a-149">OrderID</span></span></td>
<td><p><span data-ttu-id="f420a-150">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f420a-151">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f420a-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f420a-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f420a-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f420a-154">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f420a-155">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f420a-156">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="f420a-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="f420a-157">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="f420a-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="f420a-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f420a-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="f420a-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="f420a-160">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="f420a-161">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="f420a-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="f420a-162">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f420a-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="f420a-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="f420a-164">OfferID</span></span></td>
<td><p><span data-ttu-id="f420a-165">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-165">Unique offer ID.</span></span> <span data-ttu-id="f420a-166">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="f420a-167"><b>注意</b>：此值不匹配价格列表中的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="f420a-168">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="f420a-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="f420a-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="f420a-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="f420a-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="f420a-171">唯一的持久型产品 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="f420a-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="f420a-172"><b>注意</b>：此值与从价格列表产品/服务 ID 相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="f420a-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="f420a-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="f420a-174">OfferName</span></span></td>
<td><p><span data-ttu-id="f420a-175">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="f420a-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="f420a-176">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="f420a-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="f420a-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="f420a-178">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="f420a-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="f420a-179">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="f420a-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="f420a-180">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="f420a-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f420a-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f420a-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="f420a-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="f420a-183">订阅结束日期：12 个月 + x 天之后开始日期 （符合合作伙伴计费日期） 或 12 个月续订日期。</span><span class="sxs-lookup"><span data-stu-id="f420a-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="f420a-184">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="f420a-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="f420a-185">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="f420a-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="f420a-186">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="f420a-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f420a-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f420a-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f420a-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f420a-189">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="f420a-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="f420a-190">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="f420a-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f420a-191">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="f420a-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f420a-192">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f420a-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f420a-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f420a-194">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="f420a-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="f420a-195">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="f420a-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f420a-196">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="f420a-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f420a-197">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="f420a-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f420a-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="f420a-199">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-199">The type of charge or adjustment.</span></span> <span data-ttu-id="f420a-200">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="f420a-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f420a-201">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="f420a-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="f420a-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="f420a-203">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="f420a-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f420a-204">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f420a-205">6.82</span><span class="sxs-lookup"><span data-stu-id="f420a-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-206">数量</span><span class="sxs-lookup"><span data-stu-id="f420a-206">Quantity</span></span></td>
<td><p><span data-ttu-id="f420a-207">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="f420a-207">Number of seats.</span></span> <span data-ttu-id="f420a-208">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f420a-209">2</span><span class="sxs-lookup"><span data-stu-id="f420a-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-210">金额</span><span class="sxs-lookup"><span data-stu-id="f420a-210">Amount</span></span></td>
<td><p><span data-ttu-id="f420a-211">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="f420a-211">Total of price for quantity.</span></span> <span data-ttu-id="f420a-212">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="f420a-213">13.32</span><span class="sxs-lookup"><span data-stu-id="f420a-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="f420a-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="f420a-215">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="f420a-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="f420a-216">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="f420a-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="f420a-217">2.32</span><span class="sxs-lookup"><span data-stu-id="f420a-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-218">小计</span><span class="sxs-lookup"><span data-stu-id="f420a-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="f420a-219">税前总额。</span><span class="sxs-lookup"><span data-stu-id="f420a-219">Total before tax.</span></span> <span data-ttu-id="f420a-220">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="f420a-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="f420a-221">11</span><span class="sxs-lookup"><span data-stu-id="f420a-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-222">税</span><span class="sxs-lookup"><span data-stu-id="f420a-222">Tax</span></span></td>
<td><p><span data-ttu-id="f420a-223">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="f420a-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f420a-224">0</span><span class="sxs-lookup"><span data-stu-id="f420a-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="f420a-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="f420a-226">税后总额。</span><span class="sxs-lookup"><span data-stu-id="f420a-226">Total after tax.</span></span> <span data-ttu-id="f420a-227">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="f420a-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="f420a-228">11</span><span class="sxs-lookup"><span data-stu-id="f420a-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-229">货币</span><span class="sxs-lookup"><span data-stu-id="f420a-229">Currency</span></span></td>
<td><p><span data-ttu-id="f420a-230">货币类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-230">Currency type.</span></span> <span data-ttu-id="f420a-231">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="f420a-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="f420a-232">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f420a-233">EUR</span><span class="sxs-lookup"><span data-stu-id="f420a-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f420a-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="f420a-235">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="f420a-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f420a-236">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f420a-237">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="f420a-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="f420a-238">MPNID</span></span></td>
<td><p><span data-ttu-id="f420a-239">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="f420a-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="f420a-240">4390934</span><span class="sxs-lookup"><span data-stu-id="f420a-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f420a-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f420a-242">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f420a-243">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="f420a-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f420a-244">4390934</span><span class="sxs-lookup"><span data-stu-id="f420a-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="f420a-245">DomainName</span></span></td>
<td><p><span data-ttu-id="f420a-246">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f420a-247">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="f420a-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f420a-248">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="f420a-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f420a-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f420a-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f420a-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f420a-251">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="f420a-251">Subscription nickname.</span></span> <span data-ttu-id="f420a-252">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="f420a-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="f420a-253">联机项目</span><span class="sxs-lookup"><span data-stu-id="f420a-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f420a-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f420a-255">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="f420a-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f420a-256">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="f420a-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="f420a-257">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="f420a-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="f420a-258">基于使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="f420a-258">Usage-based file fields</span></span>


<span data-ttu-id="f420a-259">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="f420a-260">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="f420a-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="f420a-261">列</span><span class="sxs-lookup"><span data-stu-id="f420a-261">Column</span></span></strong></td>
<td><strong><span data-ttu-id="f420a-262">描述</span><span class="sxs-lookup"><span data-stu-id="f420a-262">Description</span></span></strong></td>
<td><strong><span data-ttu-id="f420a-263">示例值</span><span class="sxs-lookup"><span data-stu-id="f420a-263">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f420a-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="f420a-265">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="f420a-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="f420a-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f420a-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f420a-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="f420a-268">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="f420a-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="f420a-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="f420a-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="f420a-271">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="f420a-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="f420a-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f420a-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="f420a-274">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="f420a-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f420a-275">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f420a-276">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="f420a-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="f420a-277">MPNID</span></span></td>
<td><p><span data-ttu-id="f420a-278">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="f420a-279">4390934</span><span class="sxs-lookup"><span data-stu-id="f420a-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f420a-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f420a-281">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f420a-282">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="f420a-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f420a-283">4390934</span><span class="sxs-lookup"><span data-stu-id="f420a-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f420a-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f420a-285">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="f420a-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="f420a-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="f420a-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f420a-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f420a-288">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="f420a-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f420a-289">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="f420a-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f420a-290">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f420a-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f420a-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f420a-292">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="f420a-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f420a-293">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="f420a-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f420a-294">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="f420a-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f420a-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f420a-296">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f420a-297">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f420a-298">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="f420a-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f420a-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f420a-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f420a-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f420a-301">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="f420a-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="f420a-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f420a-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f420a-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f420a-304">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="f420a-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="f420a-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f420a-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="f420a-306">OrderID</span></span></td>
<td><p><span data-ttu-id="f420a-307">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f420a-308">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f420a-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f420a-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="f420a-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="f420a-311">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="f420a-312">虚拟机</span><span class="sxs-lookup"><span data-stu-id="f420a-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="f420a-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="f420a-314">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f420a-315">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="f420a-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="f420a-316">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="f420a-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="f420a-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="f420a-318">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="f420a-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f420a-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-320">资源名称</span><span class="sxs-lookup"><span data-stu-id="f420a-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="f420a-321">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f420a-322">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="f420a-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="f420a-323">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="f420a-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-324">Region</span><span class="sxs-lookup"><span data-stu-id="f420a-324">Region</span></span></td>
<td><p><span data-ttu-id="f420a-325">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="f420a-325">The region the usage applies to.</span></span> <span data-ttu-id="f420a-326">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="f420a-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="f420a-327">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="f420a-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-328">SKU</span><span class="sxs-lookup"><span data-stu-id="f420a-328">SKU</span></span></td>
<td><p><span data-ttu-id="f420a-329">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f420a-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="f420a-330">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="f420a-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="f420a-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="f420a-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="f420a-332">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="f420a-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="f420a-333">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="f420a-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="f420a-334">1</span><span class="sxs-lookup"><span data-stu-id="f420a-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="f420a-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="f420a-336">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="f420a-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="f420a-337">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="f420a-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="f420a-338">11</span><span class="sxs-lookup"><span data-stu-id="f420a-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="f420a-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="f420a-340">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="f420a-340">Units included as part of the offer.</span></span> <span data-ttu-id="f420a-341">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="f420a-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="f420a-342">0</span><span class="sxs-lookup"><span data-stu-id="f420a-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f420a-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="f420a-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="f420a-344">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="f420a-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="f420a-345">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="f420a-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="f420a-346">11</span><span class="sxs-lookup"><span data-stu-id="f420a-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="f420a-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="f420a-348">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="f420a-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="f420a-349">$0.0808</span><span class="sxs-lookup"><span data-stu-id="f420a-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="f420a-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="f420a-351">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="f420a-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f420a-352">$0.085</span><span class="sxs-lookup"><span data-stu-id="f420a-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="f420a-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="f420a-354">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="f420a-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f420a-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="f420a-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="f420a-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="f420a-357">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="f420a-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="f420a-358">$0.93</span><span class="sxs-lookup"><span data-stu-id="f420a-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-359">货币</span><span class="sxs-lookup"><span data-stu-id="f420a-359">Currency</span></span></td>
<td><p><span data-ttu-id="f420a-360">货币类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-360">Currency type.</span></span> <span data-ttu-id="f420a-361">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="f420a-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="f420a-362">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f420a-363">EUR</span><span class="sxs-lookup"><span data-stu-id="f420a-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f420a-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f420a-365">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="f420a-365">Pretax price per unit.</span></span> <span data-ttu-id="f420a-366">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="f420a-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f420a-367">$0.08</span><span class="sxs-lookup"><span data-stu-id="f420a-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f420a-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f420a-369">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="f420a-369">Post tax price per unit.</span></span> <span data-ttu-id="f420a-370">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="f420a-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f420a-371">$0.08</span><span class="sxs-lookup"><span data-stu-id="f420a-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f420a-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="f420a-373">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-373">The type of charge or adjustment.</span></span> <span data-ttu-id="f420a-374">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="f420a-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f420a-375">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="f420a-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="f420a-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="f420a-377">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="f420a-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="f420a-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="f420a-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="f420a-380">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="f420a-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="f420a-381">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f420a-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="f420a-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="f420a-383">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="f420a-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="f420a-384">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="f420a-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="f420a-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="f420a-386">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="f420a-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="f420a-387">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="f420a-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="f420a-388">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="f420a-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="f420a-389">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="f420a-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="f420a-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="f420a-391">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="f420a-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="f420a-392">外部</span><span class="sxs-lookup"><span data-stu-id="f420a-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-393">项目</span><span class="sxs-lookup"><span data-stu-id="f420a-393">Project</span></span></td>
<td><p><span data-ttu-id="f420a-394">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="f420a-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="f420a-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f420a-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="f420a-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="f420a-397">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="f420a-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="f420a-398">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="f420a-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="f420a-399">如果必须预配的服务总线连接的 25 包，并且你必须在那一天中使用了 1，这一天您每日使用情况语句将指示"25 连接 / 30 天 – 使用：1.000000”.</span><span class="sxs-lookup"><span data-stu-id="f420a-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f420a-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="f420a-401">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f420a-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f420a-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f420a-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="f420a-403">DomainName</span></span></td>
<td><p><span data-ttu-id="f420a-404">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f420a-405">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="f420a-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f420a-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f420a-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="f420a-407">单位</span><span class="sxs-lookup"><span data-stu-id="f420a-407">Unit</span></span></td>
<td><p><span data-ttu-id="f420a-408">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="f420a-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="f420a-409">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="f420a-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="f420a-410">一次性和重复性文件字段</span><span class="sxs-lookup"><span data-stu-id="f420a-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f420a-411">列</span><span class="sxs-lookup"><span data-stu-id="f420a-411">Column</span></span></th>
<th><span data-ttu-id="f420a-412">描述</span><span class="sxs-lookup"><span data-stu-id="f420a-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="f420a-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f420a-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="f420a-414">唯一的 GUID 格式中的特定计费实体的 Microsoft Azure Active Directory 租户标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f420a-415">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="f420a-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f420a-416">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="f420a-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-417">客户 Id</span><span class="sxs-lookup"><span data-stu-id="f420a-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="f420a-418">Microsoft Azure Active Directory 租户中唯一 ID，用于标识客户的 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="f420a-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-419">客户名称</span><span class="sxs-lookup"><span data-stu-id="f420a-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="f420a-420">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f420a-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f420a-422">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="f420a-423">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="f420a-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f420a-424">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="f420a-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-425">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="f420a-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="f420a-426">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="f420a-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-427">发票编号</span><span class="sxs-lookup"><span data-stu-id="f420a-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="f420a-428">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="f420a-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="f420a-429">MpnId</span></span></td>
<td><p><span data-ttu-id="f420a-430">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="f420a-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="f420a-432">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-433">订单编码</span><span class="sxs-lookup"><span data-stu-id="f420a-433">Order ID</span></span></td>
<td><p><span data-ttu-id="f420a-434">Microsoft 商务平台中的订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="f420a-435">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-436">订单日期</span><span class="sxs-lookup"><span data-stu-id="f420a-436">Order date</span></span></td>
<td><p><span data-ttu-id="f420a-437">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="f420a-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="f420a-438">ProductId</span></span></td>
<td><p><span data-ttu-id="f420a-439">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="f420a-440">SkuId</span></span></td>
<td><p><span data-ttu-id="f420a-441">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f420a-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f420a-443">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-443">The ID for a particular Availability.</span></span> <span data-ttu-id="f420a-444">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="f420a-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-445">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="f420a-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="f420a-446">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-447">产品名称</span><span class="sxs-lookup"><span data-stu-id="f420a-447">Product name</span></span></td>
<td><p><span data-ttu-id="f420a-448">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f420a-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="f420a-450">该产品的发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f420a-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="f420a-452">此发布服务器的的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-453">订阅说明</span><span class="sxs-lookup"><span data-stu-id="f420a-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f420a-454">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-455">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="f420a-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f420a-456">Microsoft 商务平台中的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="f420a-457">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f420a-458">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="f420a-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f420a-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f420a-460">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="f420a-460">Start day of the charges.</span></span> <span data-ttu-id="f420a-461">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="f420a-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f420a-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f420a-463">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="f420a-463">End day of the charges.</span></span> <span data-ttu-id="f420a-464">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="f420a-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-465">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="f420a-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="f420a-466">期限长度和购买的计费周期。</span><span class="sxs-lookup"><span data-stu-id="f420a-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="f420a-467">例如，"1 年，每月一次。"</span><span class="sxs-lookup"><span data-stu-id="f420a-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-468">费用类型</span><span class="sxs-lookup"><span data-stu-id="f420a-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="f420a-469">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-470">单价</span><span class="sxs-lookup"><span data-stu-id="f420a-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="f420a-471">因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="f420a-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f420a-472">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-473">有效的单位价格</span><span class="sxs-lookup"><span data-stu-id="f420a-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="f420a-474">单位价格后已进行调整。</span><span class="sxs-lookup"><span data-stu-id="f420a-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-475">数量</span><span class="sxs-lookup"><span data-stu-id="f420a-475">Quantity</span></span></td>
<td><p><span data-ttu-id="f420a-476">单位数。</span><span class="sxs-lookup"><span data-stu-id="f420a-476">Number of units.</span></span> <span data-ttu-id="f420a-477">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-478">单位类型</span><span class="sxs-lookup"><span data-stu-id="f420a-478">Unit type</span></span></td>
<td><p><span data-ttu-id="f420a-479">正在购买一个单位的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="f420a-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="f420a-481">所有适用的折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="f420a-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-482">子汇总</span><span class="sxs-lookup"><span data-stu-id="f420a-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="f420a-483">税前总额。</span><span class="sxs-lookup"><span data-stu-id="f420a-483">Total before tax.</span></span> <span data-ttu-id="f420a-484">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="f420a-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-485">税务总计</span><span class="sxs-lookup"><span data-stu-id="f420a-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="f420a-486">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="f420a-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-487">总计</span><span class="sxs-lookup"><span data-stu-id="f420a-487">Total</span></span></td>
<td><p><span data-ttu-id="f420a-488">税后总额。</span><span class="sxs-lookup"><span data-stu-id="f420a-488">Total after tax.</span></span> <span data-ttu-id="f420a-489">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="f420a-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-490">货币</span><span class="sxs-lookup"><span data-stu-id="f420a-490">Currency</span></span></td>
<td><p><span data-ttu-id="f420a-491">货币类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-491">Currency type.</span></span> <span data-ttu-id="f420a-492">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="f420a-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="f420a-493">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="f420a-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="f420a-495">备用标识符关联到一个订单 id。</span><span class="sxs-lookup"><span data-stu-id="f420a-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="f420a-496">评定的每日使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="f420a-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f420a-497">列</span><span class="sxs-lookup"><span data-stu-id="f420a-497">Column</span></span></th>
<th><span data-ttu-id="f420a-498">描述</span><span class="sxs-lookup"><span data-stu-id="f420a-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="f420a-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f420a-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="f420a-500">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="f420a-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f420a-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="f420a-502">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="f420a-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="f420a-504">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="f420a-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="f420a-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="f420a-506">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="f420a-507">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f420a-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f420a-509">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="f420a-509">The customer’s domain name.</span></span> <span data-ttu-id="f420a-510">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="f420a-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-511">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="f420a-511">Customer country</span></span></td>
<td><p><span data-ttu-id="f420a-512">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="f420a-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="f420a-513">MPNID</span></span></td>
<td><p><span data-ttu-id="f420a-514">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-515">分销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="f420a-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="f420a-516">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f420a-517">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="f420a-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f420a-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f420a-519">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="f420a-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="f420a-520">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="f420a-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="f420a-521">ProductId</span></span></td>
<td><p><span data-ttu-id="f420a-522">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="f420a-523">SkuId</span></span></td>
<td><p><span data-ttu-id="f420a-524">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f420a-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f420a-526">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-526">The ID for a particular Availability.</span></span> <span data-ttu-id="f420a-527">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="f420a-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-528">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="f420a-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="f420a-529">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f420a-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="f420a-531">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="f420a-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f420a-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="f420a-533">GUID 格式中的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="f420a-534">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="f420a-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="f420a-535">订阅说明</span><span class="sxs-lookup"><span data-stu-id="f420a-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f420a-536">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="f420a-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f420a-537">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="f420a-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-538">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="f420a-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f420a-539">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f420a-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f420a-540">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="f420a-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f420a-541">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="f420a-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f420a-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f420a-543">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="f420a-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f420a-544">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="f420a-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f420a-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f420a-546">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="f420a-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f420a-547">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="f420a-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-548">使用日期</span><span class="sxs-lookup"><span data-stu-id="f420a-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="f420a-549">服务使用情况的日期。</span><span class="sxs-lookup"><span data-stu-id="f420a-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-550">计量类型</span><span class="sxs-lookup"><span data-stu-id="f420a-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="f420a-551">测定仪的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-552">计量类别</span><span class="sxs-lookup"><span data-stu-id="f420a-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="f420a-553">用于使用情况的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="f420a-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-554">计量 Id</span><span class="sxs-lookup"><span data-stu-id="f420a-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="f420a-555">正在使用的计量 ID。</span><span class="sxs-lookup"><span data-stu-id="f420a-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-556">计量子类别</span><span class="sxs-lookup"><span data-stu-id="f420a-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="f420a-557">可以会影响费率的 Azure 服务的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-558">测定仪名称</span><span class="sxs-lookup"><span data-stu-id="f420a-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="f420a-559">已使用的测定仪的度量单位。</span><span class="sxs-lookup"><span data-stu-id="f420a-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-560">计量区域</span><span class="sxs-lookup"><span data-stu-id="f420a-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="f420a-561">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="f420a-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-562">单位</span><span class="sxs-lookup"><span data-stu-id="f420a-562">Unit</span></span></td>
<td><p><span data-ttu-id="f420a-563">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="f420a-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-564">已使用的数量</span><span class="sxs-lookup"><span data-stu-id="f420a-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="f420a-565">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="f420a-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="f420a-566">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="f420a-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-567">资源位置</span><span class="sxs-lookup"><span data-stu-id="f420a-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="f420a-568">测定仪正在其中运行数据中心。</span><span class="sxs-lookup"><span data-stu-id="f420a-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-569">使用的服务</span><span class="sxs-lookup"><span data-stu-id="f420a-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="f420a-570">使用 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="f420a-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-571">资源组</span><span class="sxs-lookup"><span data-stu-id="f420a-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="f420a-572">资源组部署的测定仪正在其中运行。</span><span class="sxs-lookup"><span data-stu-id="f420a-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-573">资源 URI</span><span class="sxs-lookup"><span data-stu-id="f420a-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="f420a-574">正在使用的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="f420a-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-575">费用类型</span><span class="sxs-lookup"><span data-stu-id="f420a-575">Charge type</span></span></td>
<td><p><span data-ttu-id="f420a-576">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-576">The type of charge or adjustment.</span></span> <span data-ttu-id="f420a-577">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="f420a-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-578">单价</span><span class="sxs-lookup"><span data-stu-id="f420a-578">Unit price</span></span></td>
<td><p><span data-ttu-id="f420a-579">每个许可证，因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="f420a-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f420a-580">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-581">数量</span><span class="sxs-lookup"><span data-stu-id="f420a-581">Quantity</span></span></td>
<td><p><span data-ttu-id="f420a-582">许可证的数量。</span><span class="sxs-lookup"><span data-stu-id="f420a-582">Number of licenses.</span></span> <span data-ttu-id="f420a-583">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="f420a-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-584">单位类型</span><span class="sxs-lookup"><span data-stu-id="f420a-584">Unit type</span></span></td>
<td><p><span data-ttu-id="f420a-585">测定仪的计价中的单元的类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="f420a-586">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="f420a-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-587">计费 pre 税</span><span class="sxs-lookup"><span data-stu-id="f420a-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="f420a-588">税前的总量。</span><span class="sxs-lookup"><span data-stu-id="f420a-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-589">计费货币</span><span class="sxs-lookup"><span data-stu-id="f420a-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="f420a-590">客户所在的地理区域中的币种</span><span class="sxs-lookup"><span data-stu-id="f420a-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-591">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="f420a-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="f420a-592">定价之前添加的税款。</span><span class="sxs-lookup"><span data-stu-id="f420a-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-593">定价货币</span><span class="sxs-lookup"><span data-stu-id="f420a-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="f420a-594">在价目表中货币。</span><span class="sxs-lookup"><span data-stu-id="f420a-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-595">服务信息 1</span><span class="sxs-lookup"><span data-stu-id="f420a-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="f420a-596">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="f420a-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-597">服务信息 2</span><span class="sxs-lookup"><span data-stu-id="f420a-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="f420a-598">旧字段，用于捕获可选的服务特定元数据的说明。</span><span class="sxs-lookup"><span data-stu-id="f420a-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f420a-599">Tags</span><span class="sxs-lookup"><span data-stu-id="f420a-599">Tags</span></span></td>
<td><p><span data-ttu-id="f420a-600">分配给测定仪按顺序对计费记录进行分组的标记。</span><span class="sxs-lookup"><span data-stu-id="f420a-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="f420a-601">例如，可以使用标记按使用测定仪的部门分配费用。</span><span class="sxs-lookup"><span data-stu-id="f420a-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f420a-602">其他信息</span><span class="sxs-lookup"><span data-stu-id="f420a-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="f420a-603">其他列中未涉及的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="f420a-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="f420a-604">发票和对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="f420a-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="f420a-605">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="f420a-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="f420a-606">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="f420a-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="f420a-607">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="f420a-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="f420a-608">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="f420a-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="f420a-609">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="f420a-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="f420a-610">发票费用描述</span><span class="sxs-lookup"><span data-stu-id="f420a-610">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="f420a-611">对帐文件费用描述（ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="f420a-611">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="f420a-612">此费用是什么？</span><span class="sxs-lookup"><span data-stu-id="f420a-612">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="f420a-613">如何将这些 ChargeTypes 映射到发票？</span><span class="sxs-lookup"><span data-stu-id="f420a-613">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="f420a-614">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-614">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="f420a-615">激活费用</span><span class="sxs-lookup"><span data-stu-id="f420a-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-616">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="f420a-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="f420a-617">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-618">取消费用</span><span class="sxs-lookup"><span data-stu-id="f420a-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-619">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-620">周期费用</span><span class="sxs-lookup"><span data-stu-id="f420a-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-621">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="f420a-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-622">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="f420a-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-623">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-624">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-625">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="f420a-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-626">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-627">订阅时使用年出单费用类型</span><span class="sxs-lookup"><span data-stu-id="f420a-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-628">购买费用</span><span class="sxs-lookup"><span data-stu-id="f420a-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-629">使用每月费用时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="f420a-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-630">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-631">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="f420a-632">续订费用</span><span class="sxs-lookup"><span data-stu-id="f420a-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-633">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="f420a-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-634">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-635">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="f420a-636">使用费用</span><span class="sxs-lookup"><span data-stu-id="f420a-636">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="f420a-637">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="f420a-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-638">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="f420a-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="f420a-639">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-640">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="f420a-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-641">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="f420a-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="f420a-642">退款额</span><span class="sxs-lookup"><span data-stu-id="f420a-642">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="f420a-643">偏移行项</span><span class="sxs-lookup"><span data-stu-id="f420a-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-644">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="f420a-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-645">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="f420a-646">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="f420a-647">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-647">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="f420a-648">激活折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-649">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="f420a-650">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-651">周期折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-652">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-653">续订折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-654">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-655">取消折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-656">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="f420a-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="f420a-657">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="f420a-657">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="f420a-658">可能应用于多种费用类型</span><span class="sxs-lookup"><span data-stu-id="f420a-658">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="f420a-659">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f420a-660"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="f420a-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="f420a-661">可能应用于多种费用类型</span><span class="sxs-lookup"><span data-stu-id="f420a-661">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="f420a-662">例外：&quot;行项的偏移量&quot;已包含的税款。</span><span class="sxs-lookup"><span data-stu-id="f420a-662">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="f420a-663">请参阅上述“退款额”。</span><span class="sxs-lookup"><span data-stu-id="f420a-663">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="f420a-664">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="f420a-664">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="f420a-665">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-665">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="f420a-666">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="f420a-666">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
