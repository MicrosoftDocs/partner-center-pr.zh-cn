---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
description: 在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 2d5792ad8f1a01c94336b208c825b10a269ae054
ms.sourcegitcommit: 47a91bb6d961630f154fde738075b73ff84a829e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2019
ms.locfileid: "67193423"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="bb47c-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="bb47c-103">Use the reconciliation files</span></span>

<span data-ttu-id="bb47c-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="bb47c-104">**Applies to**</span></span>

-  <span data-ttu-id="bb47c-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="bb47c-105">Partner Center</span></span>
-  <span data-ttu-id="bb47c-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="bb47c-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="bb47c-107">在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。</span><span class="sxs-lookup"><span data-stu-id="bb47c-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="bb47c-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="bb47c-109">格式设置问题</span><span class="sxs-lookup"><span data-stu-id="bb47c-109">Formatting issues</span></span>

<span data-ttu-id="bb47c-110">偶尔侦测文件可能会遇到格式问题。</span><span class="sxs-lookup"><span data-stu-id="bb47c-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="bb47c-111">（这可能发生，例如，如果不使用 EN-US 区域设置。）请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="bb47c-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="bb47c-112">在 Excel 中打开.csv 文件，并选择第一列。</span><span class="sxs-lookup"><span data-stu-id="bb47c-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="bb47c-113">在功能区中，选择<strong>数据</strong>，然后选择<strong>分列</strong>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="bb47c-114">在转换文本分列向导，选择<strong>分隔的文件类型</strong>，然后选择<strong>下一步</strong>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="bb47c-115">在分隔符字段中，选择<strong>逗号</strong>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="bb47c-116">如果<strong>选项卡</strong>是尚未选中，你可以将其保留。</span><span class="sxs-lookup"><span data-stu-id="bb47c-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="bb47c-117">选择“<strong>下一步</strong>”。</span><span class="sxs-lookup"><span data-stu-id="bb47c-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="bb47c-118">在列数据格式字段中，选择<strong>日期：MDY</strong>，然后选择<strong>下一步</strong>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="bb47c-119">在列数据格式字段中，选择<strong>文本</strong>的列，并选择所有金额<strong>完成</strong>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="bb47c-120">下载较大的侦测文件</span><span class="sxs-lookup"><span data-stu-id="bb47c-120">Downloading a large recon file</span></span>

<span data-ttu-id="bb47c-121">侦测文件可以变得很大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="bb47c-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="bb47c-122">若要帮助下载大型侦测文件的 PowerShell 脚本，请参阅[获取发票行项](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="bb47c-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="bb47c-123">由合作伙伴详细列举</span><span class="sxs-lookup"><span data-stu-id="bb47c-123">Itemize by partner</span></span>


<span data-ttu-id="bb47c-124">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="bb47c-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="bb47c-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="bb47c-125">MPN ID</span></span></th>
<th><span data-ttu-id="bb47c-126">描述</span><span class="sxs-lookup"><span data-stu-id="bb47c-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="bb47c-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="bb47c-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="bb47c-128">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-129">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="bb47c-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="bb47c-130">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="bb47c-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="bb47c-131">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="bb47c-132">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="bb47c-133">干支查看或更新的分销商，在合作伙伴中心菜单中，选择<strong>客户</strong>，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="bb47c-134">在客户菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="bb47c-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="bb47c-135">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="bb47c-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="bb47c-136">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="bb47c-137">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="bb47c-138">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="bb47c-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="bb47c-139">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="bb47c-139">License-based file fields</span></span>


<span data-ttu-id="bb47c-140">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="bb47c-141"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="bb47c-142"><strong>说明</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="bb47c-143"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="bb47c-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="bb47c-145">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="bb47c-146">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="bb47c-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="bb47c-147">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="bb47c-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="bb47c-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="bb47c-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="bb47c-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="bb47c-150">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="bb47c-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="bb47c-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="bb47c-152">OrderID</span></span></td>
<td><p><span data-ttu-id="bb47c-153">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="bb47c-154">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="bb47c-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="bb47c-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="bb47c-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="bb47c-157">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="bb47c-158">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="bb47c-159">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="bb47c-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="bb47c-160">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="bb47c-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="bb47c-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="bb47c-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="bb47c-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="bb47c-163">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="bb47c-164">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="bb47c-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="bb47c-165">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="bb47c-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="bb47c-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="bb47c-167">OfferID</span></span></td>
<td><p><span data-ttu-id="bb47c-168">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-168">Unique offer ID.</span></span> <span data-ttu-id="bb47c-169">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="bb47c-170"><b>注意</b>：此值不匹配价格列表中的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="bb47c-171">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="bb47c-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="bb47c-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="bb47c-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="bb47c-174">唯一的持久型产品 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="bb47c-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="bb47c-175"><b>注意</b>：此值与从价格列表产品/服务 ID 相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="bb47c-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="bb47c-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="bb47c-177">OfferName</span></span></td>
<td><p><span data-ttu-id="bb47c-178">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="bb47c-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="bb47c-179">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="bb47c-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="bb47c-181">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="bb47c-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="bb47c-182">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="bb47c-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="bb47c-183">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="bb47c-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="bb47c-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="bb47c-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="bb47c-186">订阅结束日期：12 个月 + x 天之后开始日期 （符合合作伙伴计费日期） 或 12 个月续订日期。</span><span class="sxs-lookup"><span data-stu-id="bb47c-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="bb47c-187">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="bb47c-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="bb47c-188">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="bb47c-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="bb47c-189">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="bb47c-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="bb47c-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="bb47c-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="bb47c-192">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="bb47c-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="bb47c-193">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="bb47c-194">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="bb47c-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="bb47c-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="bb47c-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="bb47c-197">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="bb47c-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="bb47c-198">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="bb47c-199">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="bb47c-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="bb47c-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="bb47c-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="bb47c-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="bb47c-202">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-202">The type of charge or adjustment.</span></span> <span data-ttu-id="bb47c-203">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="bb47c-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="bb47c-204">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="bb47c-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="bb47c-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="bb47c-206">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="bb47c-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="bb47c-207">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="bb47c-208">6.82</span><span class="sxs-lookup"><span data-stu-id="bb47c-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-209">数量</span><span class="sxs-lookup"><span data-stu-id="bb47c-209">Quantity</span></span></td>
<td><p><span data-ttu-id="bb47c-210">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="bb47c-210">Number of seats.</span></span> <span data-ttu-id="bb47c-211">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="bb47c-212">2</span><span class="sxs-lookup"><span data-stu-id="bb47c-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-213">金额</span><span class="sxs-lookup"><span data-stu-id="bb47c-213">Amount</span></span></td>
<td><p><span data-ttu-id="bb47c-214">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="bb47c-214">Total of price for quantity.</span></span> <span data-ttu-id="bb47c-215">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="bb47c-216">13.32</span><span class="sxs-lookup"><span data-stu-id="bb47c-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="bb47c-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="bb47c-218">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="bb47c-219">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="bb47c-220">2.32</span><span class="sxs-lookup"><span data-stu-id="bb47c-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-221">小计</span><span class="sxs-lookup"><span data-stu-id="bb47c-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="bb47c-222">税前总额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-222">Total before tax.</span></span> <span data-ttu-id="bb47c-223">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="bb47c-224">11</span><span class="sxs-lookup"><span data-stu-id="bb47c-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-225">税</span><span class="sxs-lookup"><span data-stu-id="bb47c-225">Tax</span></span></td>
<td><p><span data-ttu-id="bb47c-226">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="bb47c-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="bb47c-227">0</span><span class="sxs-lookup"><span data-stu-id="bb47c-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="bb47c-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="bb47c-229">税后总额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-229">Total after tax.</span></span> <span data-ttu-id="bb47c-230">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="bb47c-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="bb47c-231">11</span><span class="sxs-lookup"><span data-stu-id="bb47c-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-232">货币</span><span class="sxs-lookup"><span data-stu-id="bb47c-232">Currency</span></span></td>
<td><p><span data-ttu-id="bb47c-233">货币类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-233">Currency type.</span></span> <span data-ttu-id="bb47c-234">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="bb47c-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="bb47c-235">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="bb47c-236">EUR</span><span class="sxs-lookup"><span data-stu-id="bb47c-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="bb47c-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="bb47c-238">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="bb47c-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="bb47c-239">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="bb47c-240">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="bb47c-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="bb47c-241">MPNID</span></span></td>
<td><p><span data-ttu-id="bb47c-242">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="bb47c-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="bb47c-243">4390934</span><span class="sxs-lookup"><span data-stu-id="bb47c-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="bb47c-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="bb47c-245">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="bb47c-246">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="bb47c-247">4390934</span><span class="sxs-lookup"><span data-stu-id="bb47c-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="bb47c-248">DomainName</span></span></td>
<td><p><span data-ttu-id="bb47c-249">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="bb47c-250">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="bb47c-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="bb47c-251">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="bb47c-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="bb47c-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="bb47c-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="bb47c-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="bb47c-254">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-254">Subscription nickname.</span></span> <span data-ttu-id="bb47c-255">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="bb47c-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="bb47c-256">联机项目</span><span class="sxs-lookup"><span data-stu-id="bb47c-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="bb47c-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="bb47c-258">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="bb47c-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="bb47c-259">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="bb47c-260">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="bb47c-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="bb47c-261">基于使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="bb47c-261">Usage-based file fields</span></span>


<span data-ttu-id="bb47c-262">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="bb47c-263">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="bb47c-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="bb47c-264"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="bb47c-265"><strong>说明</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="bb47c-266"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="bb47c-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="bb47c-268">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="bb47c-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="bb47c-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="bb47c-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="bb47c-271">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="bb47c-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="bb47c-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="bb47c-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="bb47c-274">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="bb47c-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="bb47c-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="bb47c-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="bb47c-277">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="bb47c-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="bb47c-278">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="bb47c-279">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="bb47c-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="bb47c-280">MPNID</span></span></td>
<td><p><span data-ttu-id="bb47c-281">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="bb47c-282">4390934</span><span class="sxs-lookup"><span data-stu-id="bb47c-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="bb47c-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="bb47c-284">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="bb47c-285">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="bb47c-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="bb47c-286">4390934</span><span class="sxs-lookup"><span data-stu-id="bb47c-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="bb47c-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="bb47c-288">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="bb47c-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="bb47c-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="bb47c-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="bb47c-291">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="bb47c-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="bb47c-292">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="bb47c-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="bb47c-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="bb47c-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="bb47c-295">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="bb47c-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="bb47c-296">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="bb47c-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="bb47c-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="bb47c-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="bb47c-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="bb47c-299">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="bb47c-300">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="bb47c-301">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="bb47c-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="bb47c-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="bb47c-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="bb47c-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="bb47c-304">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="bb47c-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="bb47c-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="bb47c-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="bb47c-307">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="bb47c-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="bb47c-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="bb47c-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="bb47c-309">OrderID</span></span></td>
<td><p><span data-ttu-id="bb47c-310">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="bb47c-311">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="bb47c-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="bb47c-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="bb47c-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="bb47c-314">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="bb47c-315">虚拟机</span><span class="sxs-lookup"><span data-stu-id="bb47c-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="bb47c-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="bb47c-317">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="bb47c-318">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="bb47c-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="bb47c-319">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="bb47c-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="bb47c-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="bb47c-321">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="bb47c-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="bb47c-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-323">资源名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="bb47c-324">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="bb47c-325">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="bb47c-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="bb47c-326">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="bb47c-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-327">Region</span><span class="sxs-lookup"><span data-stu-id="bb47c-327">Region</span></span></td>
<td><p><span data-ttu-id="bb47c-328">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="bb47c-328">The region the usage applies to.</span></span> <span data-ttu-id="bb47c-329">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="bb47c-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="bb47c-330">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="bb47c-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-331">SKU</span><span class="sxs-lookup"><span data-stu-id="bb47c-331">SKU</span></span></td>
<td><p><span data-ttu-id="bb47c-332">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bb47c-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="bb47c-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="bb47c-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="bb47c-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="bb47c-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="bb47c-335">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="bb47c-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="bb47c-336">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="bb47c-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="bb47c-337">1</span><span class="sxs-lookup"><span data-stu-id="bb47c-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="bb47c-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="bb47c-339">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="bb47c-340">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="bb47c-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="bb47c-341">11</span><span class="sxs-lookup"><span data-stu-id="bb47c-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="bb47c-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="bb47c-343">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="bb47c-343">Units included as part of the offer.</span></span> <span data-ttu-id="bb47c-344">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="bb47c-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="bb47c-345">0</span><span class="sxs-lookup"><span data-stu-id="bb47c-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="bb47c-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="bb47c-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="bb47c-347">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="bb47c-348">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="bb47c-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="bb47c-349">11</span><span class="sxs-lookup"><span data-stu-id="bb47c-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="bb47c-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="bb47c-351">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="bb47c-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="bb47c-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="bb47c-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="bb47c-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="bb47c-354">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="bb47c-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="bb47c-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="bb47c-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="bb47c-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="bb47c-357">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="bb47c-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="bb47c-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="bb47c-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="bb47c-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="bb47c-360">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="bb47c-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="bb47c-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-362">货币</span><span class="sxs-lookup"><span data-stu-id="bb47c-362">Currency</span></span></td>
<td><p><span data-ttu-id="bb47c-363">货币类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-363">Currency type.</span></span> <span data-ttu-id="bb47c-364">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="bb47c-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="bb47c-365">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="bb47c-366">EUR</span><span class="sxs-lookup"><span data-stu-id="bb47c-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="bb47c-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="bb47c-368">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="bb47c-368">Pretax price per unit.</span></span> <span data-ttu-id="bb47c-369">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="bb47c-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="bb47c-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="bb47c-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="bb47c-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="bb47c-372">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="bb47c-372">Post tax price per unit.</span></span> <span data-ttu-id="bb47c-373">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="bb47c-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="bb47c-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="bb47c-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="bb47c-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="bb47c-376">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-376">The type of charge or adjustment.</span></span> <span data-ttu-id="bb47c-377">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="bb47c-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="bb47c-378">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="bb47c-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="bb47c-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="bb47c-380">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="bb47c-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="bb47c-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="bb47c-383">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="bb47c-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="bb47c-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="bb47c-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="bb47c-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="bb47c-386">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="bb47c-387">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="bb47c-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="bb47c-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="bb47c-389">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="bb47c-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="bb47c-390">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="bb47c-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="bb47c-391">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="bb47c-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="bb47c-392">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="bb47c-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="bb47c-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="bb47c-394">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="bb47c-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="bb47c-395">外部</span><span class="sxs-lookup"><span data-stu-id="bb47c-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-396">项目</span><span class="sxs-lookup"><span data-stu-id="bb47c-396">Project</span></span></td>
<td><p><span data-ttu-id="bb47c-397">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="bb47c-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="bb47c-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="bb47c-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="bb47c-400">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="bb47c-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="bb47c-401">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="bb47c-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="bb47c-402">如果必须预配的服务总线连接的 25 包，并且你必须在那一天中使用了 1，这一天您每日使用情况语句将指示"25 连接 / 30 天 – 使用：1.000000”.</span><span class="sxs-lookup"><span data-stu-id="bb47c-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="bb47c-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="bb47c-404">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="bb47c-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="bb47c-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="bb47c-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="bb47c-406">DomainName</span></span></td>
<td><p><span data-ttu-id="bb47c-407">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="bb47c-408">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="bb47c-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="bb47c-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="bb47c-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="bb47c-410">单位</span><span class="sxs-lookup"><span data-stu-id="bb47c-410">Unit</span></span></td>
<td><p><span data-ttu-id="bb47c-411">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="bb47c-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="bb47c-412">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="bb47c-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="bb47c-413">一次性和重复性文件字段</span><span class="sxs-lookup"><span data-stu-id="bb47c-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="bb47c-414">列</span><span class="sxs-lookup"><span data-stu-id="bb47c-414">Column</span></span></th>
<th><span data-ttu-id="bb47c-415">描述</span><span class="sxs-lookup"><span data-stu-id="bb47c-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="bb47c-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="bb47c-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="bb47c-417">唯一的 GUID 格式中的特定计费实体的 Microsoft Azure Active Directory 租户标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="bb47c-418">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="bb47c-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="bb47c-419">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="bb47c-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-420">客户 Id</span><span class="sxs-lookup"><span data-stu-id="bb47c-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="bb47c-421">Microsoft Azure Active Directory 租户中唯一 ID，用于标识客户的 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="bb47c-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-422">客户名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="bb47c-423">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="bb47c-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="bb47c-425">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="bb47c-426">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="bb47c-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="bb47c-427">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="bb47c-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-428">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="bb47c-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="bb47c-429">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="bb47c-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-430">发票编号</span><span class="sxs-lookup"><span data-stu-id="bb47c-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="bb47c-431">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="bb47c-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="bb47c-432">MpnId</span></span></td>
<td><p><span data-ttu-id="bb47c-433">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="bb47c-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="bb47c-435">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-436">订单编码</span><span class="sxs-lookup"><span data-stu-id="bb47c-436">Order ID</span></span></td>
<td><p><span data-ttu-id="bb47c-437">Microsoft 商务平台中的订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="bb47c-438">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-439">订单日期</span><span class="sxs-lookup"><span data-stu-id="bb47c-439">Order date</span></span></td>
<td><p><span data-ttu-id="bb47c-440">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="bb47c-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="bb47c-441">ProductId</span></span></td>
<td><p><span data-ttu-id="bb47c-442">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="bb47c-443">SkuId</span></span></td>
<td><p><span data-ttu-id="bb47c-444">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="bb47c-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="bb47c-446">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-446">The ID for a particular Availability.</span></span> <span data-ttu-id="bb47c-447">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="bb47c-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-448">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="bb47c-449">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-450">产品名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-450">Product name</span></span></td>
<td><p><span data-ttu-id="bb47c-451">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="bb47c-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="bb47c-453">该产品的发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="bb47c-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="bb47c-455">此发布服务器的的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-456">订阅说明</span><span class="sxs-lookup"><span data-stu-id="bb47c-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="bb47c-457">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-458">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="bb47c-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="bb47c-459">Microsoft 商务平台中的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="bb47c-460">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="bb47c-461">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="bb47c-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="bb47c-463">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="bb47c-463">Start day of the charges.</span></span> <span data-ttu-id="bb47c-464">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="bb47c-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="bb47c-466">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="bb47c-466">End day of the charges.</span></span> <span data-ttu-id="bb47c-467">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="bb47c-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-468">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="bb47c-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="bb47c-469">期限长度和购买的计费周期。</span><span class="sxs-lookup"><span data-stu-id="bb47c-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="bb47c-470">例如，"1 年，每月一次。"</span><span class="sxs-lookup"><span data-stu-id="bb47c-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-471">费用类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="bb47c-472">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-473">单价</span><span class="sxs-lookup"><span data-stu-id="bb47c-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="bb47c-474">因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="bb47c-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="bb47c-475">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-476">有效的单位价格</span><span class="sxs-lookup"><span data-stu-id="bb47c-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="bb47c-477">单位价格后已进行调整。</span><span class="sxs-lookup"><span data-stu-id="bb47c-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-478">数量</span><span class="sxs-lookup"><span data-stu-id="bb47c-478">Quantity</span></span></td>
<td><p><span data-ttu-id="bb47c-479">单位数。</span><span class="sxs-lookup"><span data-stu-id="bb47c-479">Number of units.</span></span> <span data-ttu-id="bb47c-480">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-481">单位类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-481">Unit type</span></span></td>
<td><p><span data-ttu-id="bb47c-482">正在购买一个单位的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="bb47c-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="bb47c-484">所有适用的折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="bb47c-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-485">子汇总</span><span class="sxs-lookup"><span data-stu-id="bb47c-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="bb47c-486">税前总额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-486">Total before tax.</span></span> <span data-ttu-id="bb47c-487">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-488">税务总计</span><span class="sxs-lookup"><span data-stu-id="bb47c-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="bb47c-489">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="bb47c-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-490">总计</span><span class="sxs-lookup"><span data-stu-id="bb47c-490">Total</span></span></td>
<td><p><span data-ttu-id="bb47c-491">税后总额。</span><span class="sxs-lookup"><span data-stu-id="bb47c-491">Total after tax.</span></span> <span data-ttu-id="bb47c-492">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="bb47c-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-493">货币</span><span class="sxs-lookup"><span data-stu-id="bb47c-493">Currency</span></span></td>
<td><p><span data-ttu-id="bb47c-494">货币类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-494">Currency type.</span></span> <span data-ttu-id="bb47c-495">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="bb47c-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="bb47c-496">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="bb47c-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="bb47c-498">备用标识符关联到一个订单 id。</span><span class="sxs-lookup"><span data-stu-id="bb47c-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="bb47c-499">评定的每日使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="bb47c-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="bb47c-500">列</span><span class="sxs-lookup"><span data-stu-id="bb47c-500">Column</span></span></th>
<th><span data-ttu-id="bb47c-501">描述</span><span class="sxs-lookup"><span data-stu-id="bb47c-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="bb47c-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="bb47c-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="bb47c-503">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="bb47c-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="bb47c-505">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="bb47c-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="bb47c-507">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="bb47c-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="bb47c-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="bb47c-509">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="bb47c-510">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="bb47c-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="bb47c-512">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="bb47c-512">The customer’s domain name.</span></span> <span data-ttu-id="bb47c-513">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-514">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="bb47c-514">Customer country</span></span></td>
<td><p><span data-ttu-id="bb47c-515">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="bb47c-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="bb47c-516">MPNID</span></span></td>
<td><p><span data-ttu-id="bb47c-517">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-518">分销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="bb47c-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="bb47c-519">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="bb47c-520">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="bb47c-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="bb47c-522">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="bb47c-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="bb47c-523">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="bb47c-524">ProductId</span></span></td>
<td><p><span data-ttu-id="bb47c-525">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="bb47c-526">SkuId</span></span></td>
<td><p><span data-ttu-id="bb47c-527">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="bb47c-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="bb47c-529">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-529">The ID for a particular Availability.</span></span> <span data-ttu-id="bb47c-530">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="bb47c-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-531">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="bb47c-532">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="bb47c-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="bb47c-534">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="bb47c-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="bb47c-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="bb47c-536">GUID 格式中的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="bb47c-537">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="bb47c-538">订阅说明</span><span class="sxs-lookup"><span data-stu-id="bb47c-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="bb47c-539">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="bb47c-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="bb47c-540">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-541">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="bb47c-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="bb47c-542">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb47c-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="bb47c-543">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="bb47c-544">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="bb47c-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="bb47c-546">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="bb47c-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="bb47c-547">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="bb47c-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="bb47c-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="bb47c-549">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="bb47c-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="bb47c-550">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="bb47c-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-551">使用日期</span><span class="sxs-lookup"><span data-stu-id="bb47c-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="bb47c-552">服务使用情况的日期。</span><span class="sxs-lookup"><span data-stu-id="bb47c-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-553">计量类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="bb47c-554">测定仪的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-555">计量类别</span><span class="sxs-lookup"><span data-stu-id="bb47c-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="bb47c-556">用于使用情况的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="bb47c-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-557">计量 Id</span><span class="sxs-lookup"><span data-stu-id="bb47c-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="bb47c-558">正在使用的计量 ID。</span><span class="sxs-lookup"><span data-stu-id="bb47c-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-559">计量子类别</span><span class="sxs-lookup"><span data-stu-id="bb47c-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="bb47c-560">可以会影响费率的 Azure 服务的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-561">测定仪名称</span><span class="sxs-lookup"><span data-stu-id="bb47c-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="bb47c-562">已使用的测定仪的度量单位。</span><span class="sxs-lookup"><span data-stu-id="bb47c-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-563">计量区域</span><span class="sxs-lookup"><span data-stu-id="bb47c-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="bb47c-564">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-565">单位</span><span class="sxs-lookup"><span data-stu-id="bb47c-565">Unit</span></span></td>
<td><p><span data-ttu-id="bb47c-566">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="bb47c-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-567">已使用的数量</span><span class="sxs-lookup"><span data-stu-id="bb47c-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="bb47c-568">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="bb47c-569">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="bb47c-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-570">资源位置</span><span class="sxs-lookup"><span data-stu-id="bb47c-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="bb47c-571">测定仪正在其中运行数据中心。</span><span class="sxs-lookup"><span data-stu-id="bb47c-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-572">使用的服务</span><span class="sxs-lookup"><span data-stu-id="bb47c-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="bb47c-573">使用 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="bb47c-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-574">资源组</span><span class="sxs-lookup"><span data-stu-id="bb47c-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="bb47c-575">资源组部署的测定仪正在其中运行。</span><span class="sxs-lookup"><span data-stu-id="bb47c-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-576">资源 URI</span><span class="sxs-lookup"><span data-stu-id="bb47c-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="bb47c-577">正在使用的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="bb47c-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-578">费用类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-578">Charge type</span></span></td>
<td><p><span data-ttu-id="bb47c-579">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-579">The type of charge or adjustment.</span></span> <span data-ttu-id="bb47c-580">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-581">单价</span><span class="sxs-lookup"><span data-stu-id="bb47c-581">Unit price</span></span></td>
<td><p><span data-ttu-id="bb47c-582">每个许可证，因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="bb47c-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="bb47c-583">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-584">数量</span><span class="sxs-lookup"><span data-stu-id="bb47c-584">Quantity</span></span></td>
<td><p><span data-ttu-id="bb47c-585">许可证的数量。</span><span class="sxs-lookup"><span data-stu-id="bb47c-585">Number of licenses.</span></span> <span data-ttu-id="bb47c-586">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="bb47c-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-587">单位类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-587">Unit type</span></span></td>
<td><p><span data-ttu-id="bb47c-588">测定仪的计价中的单元的类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="bb47c-589">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-590">计费 pre 税</span><span class="sxs-lookup"><span data-stu-id="bb47c-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="bb47c-591">税前的总量。</span><span class="sxs-lookup"><span data-stu-id="bb47c-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-592">计费货币</span><span class="sxs-lookup"><span data-stu-id="bb47c-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="bb47c-593">客户所在的地理区域中的币种</span><span class="sxs-lookup"><span data-stu-id="bb47c-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-594">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="bb47c-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="bb47c-595">定价之前添加的税款。</span><span class="sxs-lookup"><span data-stu-id="bb47c-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-596">定价货币</span><span class="sxs-lookup"><span data-stu-id="bb47c-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="bb47c-597">在价目表中货币。</span><span class="sxs-lookup"><span data-stu-id="bb47c-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-598">服务信息 1</span><span class="sxs-lookup"><span data-stu-id="bb47c-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="bb47c-599">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="bb47c-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-600">服务信息 2</span><span class="sxs-lookup"><span data-stu-id="bb47c-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="bb47c-601">旧字段，用于捕获可选的服务特定元数据的说明。</span><span class="sxs-lookup"><span data-stu-id="bb47c-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="bb47c-602">Tags</span><span class="sxs-lookup"><span data-stu-id="bb47c-602">Tags</span></span></td>
<td><p><span data-ttu-id="bb47c-603">分配给测定仪按顺序对计费记录进行分组的标记。</span><span class="sxs-lookup"><span data-stu-id="bb47c-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="bb47c-604">例如，可以使用标记按使用测定仪的部门分配费用。</span><span class="sxs-lookup"><span data-stu-id="bb47c-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="bb47c-605">其他信息</span><span class="sxs-lookup"><span data-stu-id="bb47c-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="bb47c-606">其他列中未涉及的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="bb47c-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="bb47c-607">发票和对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="bb47c-608">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="bb47c-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="bb47c-609">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="bb47c-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="bb47c-610">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="bb47c-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="bb47c-611">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="bb47c-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="bb47c-612">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="bb47c-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="bb47c-613"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-614"><strong>对帐文件费用说明 （ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-615"><strong>什么是此费用？</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-616"><strong>如何将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="bb47c-617"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-618">激活费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-619">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="bb47c-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="bb47c-620">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-621">取消费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-622">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-623">周期费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-624">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-625">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="bb47c-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-626">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-627">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-628">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="bb47c-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-629">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-630">订阅时使用年出单费用类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-631">购买费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-632">使用每月费用时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="bb47c-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-633">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-634">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="bb47c-635">续订费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-636">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-637">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-638">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>


<tr>
<td rowspan="2">
<p><span data-ttu-id="bb47c-639"><strong>使用费</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-639"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-640">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-640">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-641">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-641">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="bb47c-642">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-642">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-643">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-643">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-644">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-644">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="bb47c-645"><strong>信用额度</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-645"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-646">偏移行项</span><span class="sxs-lookup"><span data-stu-id="bb47c-646">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-647">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="bb47c-647">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-648">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-648">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="bb47c-649">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-649">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="bb47c-650"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-650"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-651">激活折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-651">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-652">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-652">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="bb47c-653">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-654">周期折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-654">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-655">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-655">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-656">续订折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-656">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-657">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-657">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-658">取消折扣</span><span class="sxs-lookup"><span data-stu-id="bb47c-658">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-659">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="bb47c-659">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="bb47c-660"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-660"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-661"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="bb47c-661"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="bb47c-662">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-662">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="bb47c-663"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="bb47c-663"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-664"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="bb47c-664"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="bb47c-665"><em>异常：&quot;行项的偏移量&quot;已包含的税款。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="bb47c-665"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-666">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="bb47c-666">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="bb47c-667">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-667">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="bb47c-668">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="bb47c-668">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
