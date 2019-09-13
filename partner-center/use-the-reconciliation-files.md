---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 07/08/2019
description: 若要详细了解计费周期中的每个费用, 请从合作伙伴中心下载协调文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8fae84790aa84b3c5a006d65a632668a33ac24a7
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820564"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="58de6-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="58de6-103">Use the reconciliation files</span></span>

<span data-ttu-id="58de6-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="58de6-104">**Applies to**</span></span>

-  <span data-ttu-id="58de6-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="58de6-105">Partner Center</span></span>
-  <span data-ttu-id="58de6-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="58de6-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="58de6-107">若要详细了解计费周期中的每个费用, 请从合作伙伴中心下载协调文件。</span><span class="sxs-lookup"><span data-stu-id="58de6-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="58de6-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="58de6-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="58de6-109">格式化问题</span><span class="sxs-lookup"><span data-stu-id="58de6-109">Formatting issues</span></span>

<span data-ttu-id="58de6-110">有时, 侦测文件可能会出现格式问题。</span><span class="sxs-lookup"><span data-stu-id="58de6-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="58de6-111">(例如, 如果不使用 EN-US 区域设置, 则可能会发生这种情况。)请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="58de6-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="58de6-112">在 Excel 中打开 .csv 文件, 然后选择第一列。</span><span class="sxs-lookup"><span data-stu-id="58de6-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="58de6-113">在功能区上, 选择 "<strong>数据</strong>", 然后选择 "<strong>文本到列</strong>"。</span><span class="sxs-lookup"><span data-stu-id="58de6-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="58de6-114">在 "将文本转换为列" 向导中, 选择 "<strong>分隔文件类型</strong>", 然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="58de6-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="58de6-115">在分隔符字段中, 选择 "<strong>逗号</strong>"。</span><span class="sxs-lookup"><span data-stu-id="58de6-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="58de6-116">如果已选择<strong>"选项卡</strong>", 则可以保留它。</span><span class="sxs-lookup"><span data-stu-id="58de6-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="58de6-117">选择“<strong>下一步</strong>”。</span><span class="sxs-lookup"><span data-stu-id="58de6-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="58de6-118">在 "列数据格式" 字段中<strong>, 选择 Date:MDY</strong>, 然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="58de6-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="58de6-119">在 "列数据格式" 字段中, 为 "所有数量" 列选择 "<strong>文本</strong>", 然后选择 "<strong>完成</strong>"。</span><span class="sxs-lookup"><span data-stu-id="58de6-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="58de6-120">下载大型侦测文件</span><span class="sxs-lookup"><span data-stu-id="58de6-120">Downloading a large recon file</span></span>

<span data-ttu-id="58de6-121">侦测文件可能会变得非常大, 有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="58de6-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="58de6-122">有关用于帮助下载大型侦测文件的 PowerShell 脚本, 请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="58de6-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="58de6-123">按合作伙伴列举</span><span class="sxs-lookup"><span data-stu-id="58de6-123">Itemize by partner</span></span>


<span data-ttu-id="58de6-124">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="58de6-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="58de6-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="58de6-125">MPN ID</span></span></th>
<th><span data-ttu-id="58de6-126">描述</span><span class="sxs-lookup"><span data-stu-id="58de6-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="58de6-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="58de6-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="58de6-128">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-129">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="58de6-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="58de6-130">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="58de6-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="58de6-131">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58de6-132">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="58de6-133">eTo 查看或更新经销商, 从合作伙伴中心菜单中选择 "<strong>客户</strong>", 然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="58de6-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="58de6-134">在客户菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="58de6-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="58de6-135">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="58de6-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="58de6-136">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="58de6-137">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="58de6-138">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="58de6-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="58de6-139">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="58de6-139">License-based file fields</span></span>


<span data-ttu-id="58de6-140">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="58de6-141"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="58de6-142"><strong>说明</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="58de6-143"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="58de6-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="58de6-145">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="58de6-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="58de6-146">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="58de6-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="58de6-147">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="58de6-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="58de6-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="58de6-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="58de6-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="58de6-150">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="58de6-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="58de6-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="58de6-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="58de6-152">OrderID</span></span></td>
<td><p><span data-ttu-id="58de6-153">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="58de6-154">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="58de6-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="58de6-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="58de6-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="58de6-157">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="58de6-158">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="58de6-159">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="58de6-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="58de6-160">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="58de6-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="58de6-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="58de6-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="58de6-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="58de6-163">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="58de6-164">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="58de6-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="58de6-165">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="58de6-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="58de6-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="58de6-167">OfferID</span></span></td>
<td><p><span data-ttu-id="58de6-168">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-168">Unique offer ID.</span></span> <span data-ttu-id="58de6-169">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="58de6-170"><b>注意</b>：此值与价目表中的产品 ID 不匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="58de6-171">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="58de6-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="58de6-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="58de6-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="58de6-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="58de6-174">唯一的持久型产品 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="58de6-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="58de6-175"><b>注意</b>：此值与价目表中的产品 ID 匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="58de6-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="58de6-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="58de6-177">OfferName</span></span></td>
<td><p><span data-ttu-id="58de6-178">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="58de6-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="58de6-179">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="58de6-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="58de6-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="58de6-181">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="58de6-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="58de6-182">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="58de6-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="58de6-183">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="58de6-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58de6-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="58de6-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="58de6-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="58de6-186">订阅结束日期:12个月 + 开始日期之后的 x 天 (与合作伙伴计费日期相同) 或从续订日期起的12个月。</span><span class="sxs-lookup"><span data-stu-id="58de6-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="58de6-187">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="58de6-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="58de6-188">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="58de6-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="58de6-189">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="58de6-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58de6-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="58de6-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="58de6-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="58de6-192">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="58de6-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="58de6-193">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="58de6-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="58de6-194">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="58de6-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58de6-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="58de6-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="58de6-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="58de6-197">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="58de6-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="58de6-198">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="58de6-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="58de6-199">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="58de6-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="58de6-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="58de6-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="58de6-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="58de6-202">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-202">The type of charge or adjustment.</span></span> <span data-ttu-id="58de6-203">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="58de6-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="58de6-204">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="58de6-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="58de6-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="58de6-206">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="58de6-207">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="58de6-208">6.82</span><span class="sxs-lookup"><span data-stu-id="58de6-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-209">数量</span><span class="sxs-lookup"><span data-stu-id="58de6-209">Quantity</span></span></td>
<td><p><span data-ttu-id="58de6-210">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="58de6-210">Number of seats.</span></span> <span data-ttu-id="58de6-211">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="58de6-212">2</span><span class="sxs-lookup"><span data-stu-id="58de6-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-213">金额</span><span class="sxs-lookup"><span data-stu-id="58de6-213">Amount</span></span></td>
<td><p><span data-ttu-id="58de6-214">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="58de6-214">Total of price for quantity.</span></span> <span data-ttu-id="58de6-215">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="58de6-216">13.32</span><span class="sxs-lookup"><span data-stu-id="58de6-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="58de6-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="58de6-218">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="58de6-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="58de6-219">资格或地图随附的产品许可证或适用于激励的新订阅还将在此列中包含折扣金额。</span><span class="sxs-lookup"><span data-stu-id="58de6-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="58de6-220">2.32</span><span class="sxs-lookup"><span data-stu-id="58de6-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-221">小计</span><span class="sxs-lookup"><span data-stu-id="58de6-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="58de6-222">税前总额。</span><span class="sxs-lookup"><span data-stu-id="58de6-222">Total before tax.</span></span> <span data-ttu-id="58de6-223">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="58de6-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="58de6-224">11</span><span class="sxs-lookup"><span data-stu-id="58de6-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-225">税</span><span class="sxs-lookup"><span data-stu-id="58de6-225">Tax</span></span></td>
<td><p><span data-ttu-id="58de6-226">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="58de6-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="58de6-227">0</span><span class="sxs-lookup"><span data-stu-id="58de6-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="58de6-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="58de6-229">税后总额。</span><span class="sxs-lookup"><span data-stu-id="58de6-229">Total after tax.</span></span> <span data-ttu-id="58de6-230">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="58de6-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="58de6-231">11</span><span class="sxs-lookup"><span data-stu-id="58de6-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-232">Currency</span><span class="sxs-lookup"><span data-stu-id="58de6-232">Currency</span></span></td>
<td><p><span data-ttu-id="58de6-233">货币类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-233">Currency type.</span></span> <span data-ttu-id="58de6-234">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="58de6-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="58de6-235">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="58de6-236">EUR</span><span class="sxs-lookup"><span data-stu-id="58de6-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="58de6-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="58de6-238">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="58de6-239">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="58de6-240">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="58de6-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="58de6-241">MPNID</span></span></td>
<td><p><span data-ttu-id="58de6-242">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="58de6-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="58de6-243">4390934</span><span class="sxs-lookup"><span data-stu-id="58de6-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="58de6-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="58de6-245">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58de6-246">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="58de6-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="58de6-247">4390934</span><span class="sxs-lookup"><span data-stu-id="58de6-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="58de6-248">DomainName</span></span></td>
<td><p><span data-ttu-id="58de6-249">客户&#39;的域名, 用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="58de6-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="58de6-250">这不应用于唯一地标识客户, 因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="58de6-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="58de6-251">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="58de6-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="58de6-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="58de6-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="58de6-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="58de6-254">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="58de6-254">Subscription nickname.</span></span> <span data-ttu-id="58de6-255">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="58de6-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="58de6-256">联机项目</span><span class="sxs-lookup"><span data-stu-id="58de6-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="58de6-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="58de6-258">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="58de6-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="58de6-259">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="58de6-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="58de6-260">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="58de6-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="58de6-261">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="58de6-261">Usage-based file fields</span></span>


<span data-ttu-id="58de6-262">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="58de6-263">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="58de6-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="58de6-264"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="58de6-265"><strong>说明</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="58de6-266"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="58de6-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="58de6-268">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="58de6-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="58de6-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="58de6-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="58de6-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="58de6-271">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="58de6-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="58de6-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="58de6-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="58de6-274">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="58de6-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="58de6-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="58de6-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="58de6-277">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="58de6-278">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="58de6-279">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="58de6-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="58de6-280">MPNID</span></span></td>
<td><p><span data-ttu-id="58de6-281">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="58de6-282">4390934</span><span class="sxs-lookup"><span data-stu-id="58de6-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="58de6-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="58de6-284">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58de6-285">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="58de6-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="58de6-286">4390934</span><span class="sxs-lookup"><span data-stu-id="58de6-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="58de6-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="58de6-288">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="58de6-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="58de6-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="58de6-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="58de6-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="58de6-291">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="58de6-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="58de6-292">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="58de6-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58de6-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="58de6-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="58de6-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="58de6-295">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="58de6-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="58de6-296">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="58de6-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="58de6-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="58de6-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="58de6-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="58de6-299">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="58de6-300">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="58de6-301">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="58de6-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="58de6-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="58de6-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="58de6-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="58de6-304">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="58de6-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="58de6-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="58de6-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="58de6-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="58de6-307">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="58de6-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="58de6-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="58de6-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="58de6-309">OrderID</span></span></td>
<td><p><span data-ttu-id="58de6-310">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="58de6-311">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="58de6-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="58de6-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="58de6-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="58de6-314">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="58de6-315">虚拟机</span><span class="sxs-lookup"><span data-stu-id="58de6-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="58de6-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="58de6-317">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="58de6-318">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="58de6-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="58de6-319">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="58de6-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="58de6-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="58de6-321">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="58de6-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="58de6-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-323">资源名称</span><span class="sxs-lookup"><span data-stu-id="58de6-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="58de6-324">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="58de6-325">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="58de6-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="58de6-326">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="58de6-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-327">Region</span><span class="sxs-lookup"><span data-stu-id="58de6-327">Region</span></span></td>
<td><p><span data-ttu-id="58de6-328">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="58de6-328">The region the usage applies to.</span></span> <span data-ttu-id="58de6-329">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="58de6-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="58de6-330">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="58de6-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-331">SKU</span><span class="sxs-lookup"><span data-stu-id="58de6-331">SKU</span></span></td>
<td><p><span data-ttu-id="58de6-332">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="58de6-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="58de6-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="58de6-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="58de6-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="58de6-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="58de6-335">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="58de6-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="58de6-336">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="58de6-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="58de6-337">1</span><span class="sxs-lookup"><span data-stu-id="58de6-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="58de6-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="58de6-339">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="58de6-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="58de6-340">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="58de6-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="58de6-341">11</span><span class="sxs-lookup"><span data-stu-id="58de6-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="58de6-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="58de6-343">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="58de6-343">Units included as part of the offer.</span></span> <span data-ttu-id="58de6-344">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="58de6-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="58de6-345">0</span><span class="sxs-lookup"><span data-stu-id="58de6-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="58de6-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="58de6-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="58de6-347">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="58de6-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="58de6-348">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="58de6-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="58de6-349">11</span><span class="sxs-lookup"><span data-stu-id="58de6-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="58de6-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="58de6-351">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="58de6-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="58de6-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="58de6-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="58de6-354">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="58de6-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="58de6-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="58de6-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="58de6-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="58de6-357">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="58de6-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="58de6-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="58de6-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="58de6-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="58de6-360">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="58de6-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="58de6-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="58de6-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-362">Currency</span><span class="sxs-lookup"><span data-stu-id="58de6-362">Currency</span></span></td>
<td><p><span data-ttu-id="58de6-363">货币类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-363">Currency type.</span></span> <span data-ttu-id="58de6-364">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="58de6-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="58de6-365">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="58de6-366">EUR</span><span class="sxs-lookup"><span data-stu-id="58de6-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="58de6-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="58de6-368">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-368">Pretax price per unit.</span></span> <span data-ttu-id="58de6-369">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="58de6-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="58de6-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="58de6-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="58de6-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="58de6-372">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-372">Post tax price per unit.</span></span> <span data-ttu-id="58de6-373">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="58de6-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="58de6-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="58de6-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="58de6-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="58de6-376">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-376">The type of charge or adjustment.</span></span> <span data-ttu-id="58de6-377">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="58de6-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="58de6-378">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="58de6-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="58de6-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="58de6-380">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="58de6-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="58de6-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="58de6-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="58de6-383">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="58de6-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="58de6-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="58de6-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="58de6-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="58de6-386">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="58de6-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="58de6-387">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="58de6-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="58de6-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="58de6-389">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="58de6-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="58de6-390">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="58de6-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="58de6-391">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="58de6-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="58de6-392">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="58de6-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="58de6-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="58de6-394">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="58de6-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="58de6-395">外部</span><span class="sxs-lookup"><span data-stu-id="58de6-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-396">项目</span><span class="sxs-lookup"><span data-stu-id="58de6-396">Project</span></span></td>
<td><p><span data-ttu-id="58de6-397">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="58de6-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="58de6-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="58de6-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="58de6-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="58de6-400">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="58de6-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="58de6-401">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="58de6-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="58de6-402">如果你预配了25个 2: 1/2 pack 连接, 并且在该天内使用了 1, 则该天的每日使用声明将显示 "25 个连接/30 天-使用:1.000000 "。</span><span class="sxs-lookup"><span data-stu-id="58de6-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="58de6-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="58de6-404">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="58de6-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="58de6-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="58de6-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58de6-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="58de6-406">DomainName</span></span></td>
<td><p><span data-ttu-id="58de6-407">客户&#39;的域名, 用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="58de6-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="58de6-408">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="58de6-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="58de6-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="58de6-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="58de6-410">单位</span><span class="sxs-lookup"><span data-stu-id="58de6-410">Unit</span></span></td>
<td><p><span data-ttu-id="58de6-411">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="58de6-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="58de6-412">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="58de6-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="58de6-413">一次性和定期文件字段</span><span class="sxs-lookup"><span data-stu-id="58de6-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="58de6-414">列</span><span class="sxs-lookup"><span data-stu-id="58de6-414">Column</span></span></th>
<th><span data-ttu-id="58de6-415">描述</span><span class="sxs-lookup"><span data-stu-id="58de6-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="58de6-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="58de6-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="58de6-417">特定计费实体的唯一 Microsoft Azure Active Directory 租户标识符, 采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="58de6-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="58de6-418">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="58de6-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="58de6-419">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="58de6-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-420">客户 Id</span><span class="sxs-lookup"><span data-stu-id="58de6-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="58de6-421">用于标识客户的唯一 Microsoft Azure Active Directory 租户 ID, 采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="58de6-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-422">客户名称</span><span class="sxs-lookup"><span data-stu-id="58de6-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="58de6-423">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="58de6-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="58de6-425">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="58de6-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="58de6-426">这不应用于唯一地标识客户, 因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="58de6-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="58de6-427">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="58de6-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-428">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="58de6-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="58de6-429">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="58de6-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-430">发票编号</span><span class="sxs-lookup"><span data-stu-id="58de6-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="58de6-431">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="58de6-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="58de6-432">MpnId</span></span></td>
<td><p><span data-ttu-id="58de6-433">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-434">经销商 MpnId</span><span class="sxs-lookup"><span data-stu-id="58de6-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="58de6-435">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-436">订单编码</span><span class="sxs-lookup"><span data-stu-id="58de6-436">Order ID</span></span></td>
<td><p><span data-ttu-id="58de6-437">Microsoft commerce 平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="58de6-438">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-439">订单日期</span><span class="sxs-lookup"><span data-stu-id="58de6-439">Order date</span></span></td>
<td><p><span data-ttu-id="58de6-440">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="58de6-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="58de6-441">ProductId</span></span></td>
<td><p><span data-ttu-id="58de6-442">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="58de6-443">SkuId</span></span></td>
<td><p><span data-ttu-id="58de6-444">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="58de6-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="58de6-446">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-446">The ID for a particular Availability.</span></span> <span data-ttu-id="58de6-447">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="58de6-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-448">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="58de6-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="58de6-449">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-450">产品名称</span><span class="sxs-lookup"><span data-stu-id="58de6-450">Product name</span></span></td>
<td><p><span data-ttu-id="58de6-451">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="58de6-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="58de6-453">产品发布者的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="58de6-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="58de6-455">此发布服务器的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-456">订阅说明</span><span class="sxs-lookup"><span data-stu-id="58de6-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="58de6-457">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-458">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="58de6-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="58de6-459">Microsoft commerce 平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="58de6-460">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="58de6-461">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="58de6-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="58de6-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="58de6-463">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="58de6-463">Start day of the charges.</span></span> <span data-ttu-id="58de6-464">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="58de6-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="58de6-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="58de6-466">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="58de6-466">End day of the charges.</span></span> <span data-ttu-id="58de6-467">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="58de6-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-468">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="58de6-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="58de6-469">采购的术语长度和计费周期。</span><span class="sxs-lookup"><span data-stu-id="58de6-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="58de6-470">例如, "1 年, 每月"。</span><span class="sxs-lookup"><span data-stu-id="58de6-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-471">费用类型</span><span class="sxs-lookup"><span data-stu-id="58de6-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="58de6-472">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-473">单价</span><span class="sxs-lookup"><span data-stu-id="58de6-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="58de6-474">购买时在 pricelist 中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="58de6-475">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-476">有效单价</span><span class="sxs-lookup"><span data-stu-id="58de6-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="58de6-477">进行调整后的单位价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-478">数量</span><span class="sxs-lookup"><span data-stu-id="58de6-478">Quantity</span></span></td>
<td><p><span data-ttu-id="58de6-479">单位数。</span><span class="sxs-lookup"><span data-stu-id="58de6-479">Number of units.</span></span> <span data-ttu-id="58de6-480">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-481">单位类型</span><span class="sxs-lookup"><span data-stu-id="58de6-481">Unit type</span></span></td>
<td><p><span data-ttu-id="58de6-482">要购买的单位类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="58de6-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="58de6-484">适用于任何适用折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="58de6-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-485">Sub Total</span><span class="sxs-lookup"><span data-stu-id="58de6-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="58de6-486">税前总额。</span><span class="sxs-lookup"><span data-stu-id="58de6-486">Total before tax.</span></span> <span data-ttu-id="58de6-487">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="58de6-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-488">税金总计</span><span class="sxs-lookup"><span data-stu-id="58de6-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="58de6-489">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="58de6-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-490">总计</span><span class="sxs-lookup"><span data-stu-id="58de6-490">Total</span></span></td>
<td><p><span data-ttu-id="58de6-491">税后总额。</span><span class="sxs-lookup"><span data-stu-id="58de6-491">Total after tax.</span></span> <span data-ttu-id="58de6-492">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="58de6-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-493">Currency</span><span class="sxs-lookup"><span data-stu-id="58de6-493">Currency</span></span></td>
<td><p><span data-ttu-id="58de6-494">货币类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-494">Currency type.</span></span> <span data-ttu-id="58de6-495">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="58de6-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="58de6-496">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="58de6-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="58de6-498">订单 ID 的备用标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="58de6-499">每日分级使用文件字段</span><span class="sxs-lookup"><span data-stu-id="58de6-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="58de6-500">列</span><span class="sxs-lookup"><span data-stu-id="58de6-500">Column</span></span></th>
<th><span data-ttu-id="58de6-501">描述</span><span class="sxs-lookup"><span data-stu-id="58de6-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="58de6-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="58de6-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="58de6-503">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="58de6-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="58de6-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="58de6-505">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="58de6-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="58de6-507">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="58de6-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="58de6-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="58de6-509">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="58de6-510">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="58de6-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="58de6-512">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="58de6-512">The customer’s domain name.</span></span> <span data-ttu-id="58de6-513">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="58de6-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-514">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="58de6-514">Customer country</span></span></td>
<td><p><span data-ttu-id="58de6-515">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="58de6-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="58de6-516">MPNID</span></span></td>
<td><p><span data-ttu-id="58de6-517">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-518">经销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="58de6-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="58de6-519">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58de6-520">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="58de6-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="58de6-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="58de6-522">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="58de6-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="58de6-523">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="58de6-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="58de6-524">ProductId</span></span></td>
<td><p><span data-ttu-id="58de6-525">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="58de6-526">SkuId</span></span></td>
<td><p><span data-ttu-id="58de6-527">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="58de6-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="58de6-529">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-529">The ID for a particular Availability.</span></span> <span data-ttu-id="58de6-530">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="58de6-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-531">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="58de6-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="58de6-532">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="58de6-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="58de6-534">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="58de6-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="58de6-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="58de6-536">GUID 格式的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="58de6-537">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="58de6-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="58de6-538">订阅说明</span><span class="sxs-lookup"><span data-stu-id="58de6-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="58de6-539">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="58de6-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="58de6-540">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="58de6-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-541">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="58de6-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="58de6-542">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58de6-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="58de6-543">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="58de6-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="58de6-544">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="58de6-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="58de6-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="58de6-546">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="58de6-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="58de6-547">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="58de6-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="58de6-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="58de6-549">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="58de6-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="58de6-550">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="58de6-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-551">使用日期</span><span class="sxs-lookup"><span data-stu-id="58de6-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="58de6-552">服务使用日期。</span><span class="sxs-lookup"><span data-stu-id="58de6-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-553">计量类型</span><span class="sxs-lookup"><span data-stu-id="58de6-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="58de6-554">计量器的类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-555">计量类别</span><span class="sxs-lookup"><span data-stu-id="58de6-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="58de6-556">使用的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="58de6-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-557">计量 Id</span><span class="sxs-lookup"><span data-stu-id="58de6-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="58de6-558">正在使用的计量的 ID。</span><span class="sxs-lookup"><span data-stu-id="58de6-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-559">计量子类别</span><span class="sxs-lookup"><span data-stu-id="58de6-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="58de6-560">可能影响速度的 Azure 服务类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-561">计量名称</span><span class="sxs-lookup"><span data-stu-id="58de6-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="58de6-562">所使用的计量的度量单位。</span><span class="sxs-lookup"><span data-stu-id="58de6-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-563">计量区域</span><span class="sxs-lookup"><span data-stu-id="58de6-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="58de6-564">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="58de6-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-565">单位</span><span class="sxs-lookup"><span data-stu-id="58de6-565">Unit</span></span></td>
<td><p><span data-ttu-id="58de6-566">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="58de6-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-567">已消耗数量</span><span class="sxs-lookup"><span data-stu-id="58de6-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="58de6-568">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="58de6-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="58de6-569">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="58de6-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-570">资源位置</span><span class="sxs-lookup"><span data-stu-id="58de6-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="58de6-571">计量器正在其中运行的数据中心。</span><span class="sxs-lookup"><span data-stu-id="58de6-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-572">已使用服务</span><span class="sxs-lookup"><span data-stu-id="58de6-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="58de6-573">你使用的 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="58de6-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="58de6-574">资源 URI</span><span class="sxs-lookup"><span data-stu-id="58de6-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="58de6-575">所使用资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="58de6-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-576">费用类型</span><span class="sxs-lookup"><span data-stu-id="58de6-576">Charge type</span></span></td>
<td><p><span data-ttu-id="58de6-577">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-577">The type of charge or adjustment.</span></span> <span data-ttu-id="58de6-578">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="58de6-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-579">单价</span><span class="sxs-lookup"><span data-stu-id="58de6-579">Unit price</span></span></td>
<td><p><span data-ttu-id="58de6-580">购买时在 pricelist 中发布的每个许可证的价格。</span><span class="sxs-lookup"><span data-stu-id="58de6-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="58de6-581">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-582">数量</span><span class="sxs-lookup"><span data-stu-id="58de6-582">Quantity</span></span></td>
<td><p><span data-ttu-id="58de6-583">许可证数量。</span><span class="sxs-lookup"><span data-stu-id="58de6-583">Number of licenses.</span></span> <span data-ttu-id="58de6-584">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="58de6-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-585">单位类型</span><span class="sxs-lookup"><span data-stu-id="58de6-585">Unit type</span></span></td>
<td><p><span data-ttu-id="58de6-586">计量计量器的单位类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="58de6-587">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="58de6-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-588">帐单税前税</span><span class="sxs-lookup"><span data-stu-id="58de6-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="58de6-589">税前的总金额。</span><span class="sxs-lookup"><span data-stu-id="58de6-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-590">计费货币</span><span class="sxs-lookup"><span data-stu-id="58de6-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="58de6-591">客户的地理区域中的货币</span><span class="sxs-lookup"><span data-stu-id="58de6-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-592">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="58de6-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="58de6-593">添加税款之前的定价。</span><span class="sxs-lookup"><span data-stu-id="58de6-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-594">定价货币</span><span class="sxs-lookup"><span data-stu-id="58de6-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="58de6-595">Pricelist 中的货币。</span><span class="sxs-lookup"><span data-stu-id="58de6-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="58de6-596">服务信息1</span><span class="sxs-lookup"><span data-stu-id="58de6-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="58de6-597">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="58de6-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-598">服务信息2</span><span class="sxs-lookup"><span data-stu-id="58de6-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="58de6-599">捕获可选的服务特定元数据的旧字段。</span><span class="sxs-lookup"><span data-stu-id="58de6-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="58de6-600">附加信息</span><span class="sxs-lookup"><span data-stu-id="58de6-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="58de6-601">其他列中未涵盖的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="58de6-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="58de6-602">发票与对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="58de6-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="58de6-603">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="58de6-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="58de6-604">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="58de6-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="58de6-605">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="58de6-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="58de6-606">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="58de6-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="58de6-607">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="58de6-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="58de6-608"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-609"><strong>对帐文件费用说明 (ChargeType 列)</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-610"><strong>此费用是什么？</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-611"><strong>如何实现将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="58de6-612"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-613">激活费用</span><span class="sxs-lookup"><span data-stu-id="58de6-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-614">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="58de6-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="58de6-615">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-616">取消费用</span><span class="sxs-lookup"><span data-stu-id="58de6-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-617">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-618">周期费用</span><span class="sxs-lookup"><span data-stu-id="58de6-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-619">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="58de6-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-620">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="58de6-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-621">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-622">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-623">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="58de6-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-624">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-625">使用年度计费时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="58de6-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-626">购买费用</span><span class="sxs-lookup"><span data-stu-id="58de6-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-627">使用月度帐单时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="58de6-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-628">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-629">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="58de6-630">续订费用</span><span class="sxs-lookup"><span data-stu-id="58de6-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-631">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="58de6-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-632">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-633">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="58de6-634"><strong>一次性费用</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="58de6-635">新增</span><span class="sxs-lookup"><span data-stu-id="58de6-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-636">创建新购买时使用</span><span class="sxs-lookup"><span data-stu-id="58de6-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="58de6-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-638">用于原始购买的退款和增加后的新数量</span><span class="sxs-lookup"><span data-stu-id="58de6-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="58de6-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-640">用于原始购买的退款和减少后的新数量</span><span class="sxs-lookup"><span data-stu-id="58de6-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-641">Cancel</span><span class="sxs-lookup"><span data-stu-id="58de6-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-642">取消订阅时使用</span><span class="sxs-lookup"><span data-stu-id="58de6-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-643">转换</span><span class="sxs-lookup"><span data-stu-id="58de6-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-644">升级许可证时使用, 但座位数保持不变</span><span class="sxs-lookup"><span data-stu-id="58de6-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="58de6-645"><strong>使用费用</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-646">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="58de6-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-647">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="58de6-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="58de6-648">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-649">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="58de6-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-650">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="58de6-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="58de6-651"><strong>制作</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-652">偏移行项</span><span class="sxs-lookup"><span data-stu-id="58de6-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-653">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="58de6-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-654">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="58de6-655">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="58de6-656"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-657">激活折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-658">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="58de6-659">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-660">周期折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-661">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-662">续订折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-663">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-664">取消折扣</span><span class="sxs-lookup"><span data-stu-id="58de6-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-665">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="58de6-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="58de6-666"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-667"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="58de6-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="58de6-668">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58de6-669"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="58de6-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-670"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="58de6-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="58de6-671"><em>异常：&quot;偏移行项&quot;已包含税金。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="58de6-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-672">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="58de6-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="58de6-673">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="58de6-674">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="58de6-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
