---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 07/08/2019
description: 若要详细了解计费周期中的每个费用，请从合作伙伴中心下载协调文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: cbc982fa5bf6848cb77a2de2dcdaa7660c422888
ms.sourcegitcommit: 30f946b3c5c2c30a5ee3276037385ea97e644781
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/03/2019
ms.locfileid: "71931579"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="e45a3-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="e45a3-103">Use the reconciliation files</span></span>

<span data-ttu-id="e45a3-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="e45a3-104">**Applies to**</span></span>

-  <span data-ttu-id="e45a3-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="e45a3-105">Partner Center</span></span>
-  <span data-ttu-id="e45a3-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="e45a3-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="e45a3-107">若要详细了解计费周期中的每个费用，请从合作伙伴中心下载协调文件。</span><span class="sxs-lookup"><span data-stu-id="e45a3-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="e45a3-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="e45a3-109">格式化问题</span><span class="sxs-lookup"><span data-stu-id="e45a3-109">Formatting issues</span></span>

<span data-ttu-id="e45a3-110">有时，侦测文件可能会出现格式问题。</span><span class="sxs-lookup"><span data-stu-id="e45a3-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="e45a3-111">（例如，如果不使用 EN-US 区域设置，则可能会发生这种情况。）请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="e45a3-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="e45a3-112">在 Excel 中打开 .csv 文件，然后选择第一列。</span><span class="sxs-lookup"><span data-stu-id="e45a3-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="e45a3-113">在功能区上，选择 "<strong>数据</strong>"，然后选择 "<strong>文本到列</strong>"。</span><span class="sxs-lookup"><span data-stu-id="e45a3-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="e45a3-114">在 "将文本转换为列" 向导中，选择 "<strong>分隔文件类型</strong>"，然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="e45a3-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="e45a3-115">在分隔符字段中，选择 "<strong>逗号</strong>"。</span><span class="sxs-lookup"><span data-stu-id="e45a3-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="e45a3-116">如果已选择<strong>"选项卡</strong>"，则可以保留它。</span><span class="sxs-lookup"><span data-stu-id="e45a3-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="e45a3-117">选择<strong>下一步</strong> 。</span><span class="sxs-lookup"><span data-stu-id="e45a3-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="e45a3-118">在 "列数据格式" 字段中，选择<strong>Date： MDY</strong>，然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="e45a3-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="e45a3-119">在 "列数据格式" 字段中，为 "所有数量" 列选择 "<strong>文本</strong>"，然后选择 "<strong>完成</strong>"。</span><span class="sxs-lookup"><span data-stu-id="e45a3-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="e45a3-120">下载大型侦测文件</span><span class="sxs-lookup"><span data-stu-id="e45a3-120">Downloading a large recon file</span></span>

<span data-ttu-id="e45a3-121">侦测文件可能会变得非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="e45a3-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="e45a3-122">有关用于帮助下载大型侦测文件的 PowerShell 脚本，请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="e45a3-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="e45a3-123">按合作伙伴列举</span><span class="sxs-lookup"><span data-stu-id="e45a3-123">Itemize by partner</span></span>


<span data-ttu-id="e45a3-124">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="e45a3-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e45a3-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="e45a3-125">MPN ID</span></span></th>
<th><span data-ttu-id="e45a3-126">描述</span><span class="sxs-lookup"><span data-stu-id="e45a3-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e45a3-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="e45a3-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="e45a3-128">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-129">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="e45a3-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="e45a3-130">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="e45a3-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="e45a3-131">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e45a3-132">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="e45a3-133">eTo 查看或更新经销商，从合作伙伴中心菜单中选择 "<strong>客户</strong>"，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="e45a3-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="e45a3-134">在“客户”菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="e45a3-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="e45a3-135">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="e45a3-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="e45a3-136">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="e45a3-137">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="e45a3-138">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="e45a3-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="e45a3-139">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="e45a3-139">License-based file fields</span></span>


<span data-ttu-id="e45a3-140">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e45a3-141"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="e45a3-142"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="e45a3-143"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e45a3-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="e45a3-145">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e45a3-146">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="e45a3-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e45a3-147">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="e45a3-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="e45a3-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="e45a3-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e45a3-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="e45a3-150">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="e45a3-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e45a3-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="e45a3-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="e45a3-152">OrderID</span></span></td>
<td><p><span data-ttu-id="e45a3-153">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e45a3-154">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e45a3-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e45a3-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e45a3-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e45a3-157">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e45a3-158">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e45a3-159">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="e45a3-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="e45a3-160">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="e45a3-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="e45a3-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e45a3-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="e45a3-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="e45a3-163">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="e45a3-164">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="e45a3-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="e45a3-165">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e45a3-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="e45a3-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="e45a3-167">OfferID</span></span></td>
<td><p><span data-ttu-id="e45a3-168">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-168">Unique offer ID.</span></span> <span data-ttu-id="e45a3-169">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="e45a3-170"><b>注意</b>：此值与价目表中的产品/服务 ID 不匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="e45a3-171">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="e45a3-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="e45a3-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="e45a3-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="e45a3-174">唯一的持久型产品/服务 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e45a3-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="e45a3-175"><b>注意</b>：此值与价目表中的产品/服务 ID 匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="e45a3-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="e45a3-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="e45a3-177">OfferName</span></span></td>
<td><p><span data-ttu-id="e45a3-178">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e45a3-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="e45a3-179">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="e45a3-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="e45a3-181">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="e45a3-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="e45a3-182">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="e45a3-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="e45a3-183">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e45a3-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e45a3-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e45a3-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="e45a3-186">订阅结束日期：12 个月 + 开始日期之后的 x 天（以便与合作伙伴帐单日期一致）或从续订日期算起的 12 个月。</span><span class="sxs-lookup"><span data-stu-id="e45a3-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="e45a3-187">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="e45a3-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="e45a3-188">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="e45a3-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="e45a3-189">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e45a3-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e45a3-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e45a3-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e45a3-192">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="e45a3-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="e45a3-193">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e45a3-194">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e45a3-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e45a3-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e45a3-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e45a3-197">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="e45a3-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="e45a3-198">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e45a3-199">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="e45a3-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e45a3-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="e45a3-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e45a3-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="e45a3-202">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-202">The type of charge or adjustment.</span></span> <span data-ttu-id="e45a3-203">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e45a3-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e45a3-204">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e45a3-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e45a3-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="e45a3-206">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e45a3-207">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e45a3-208">6.82</span><span class="sxs-lookup"><span data-stu-id="e45a3-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-209">数量</span><span class="sxs-lookup"><span data-stu-id="e45a3-209">Quantity</span></span></td>
<td><p><span data-ttu-id="e45a3-210">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="e45a3-210">Number of seats.</span></span> <span data-ttu-id="e45a3-211">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e45a3-212">2</span><span class="sxs-lookup"><span data-stu-id="e45a3-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-213">金额</span><span class="sxs-lookup"><span data-stu-id="e45a3-213">Amount</span></span></td>
<td><p><span data-ttu-id="e45a3-214">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="e45a3-214">Total of price for quantity.</span></span> <span data-ttu-id="e45a3-215">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="e45a3-216">13.32</span><span class="sxs-lookup"><span data-stu-id="e45a3-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="e45a3-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="e45a3-218">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="e45a3-219">资格或地图随附的产品许可证或适用于激励的新订阅还将在此列中包含折扣金额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="e45a3-220">2.32</span><span class="sxs-lookup"><span data-stu-id="e45a3-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-221">小计</span><span class="sxs-lookup"><span data-stu-id="e45a3-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="e45a3-222">税前总额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-222">Total before tax.</span></span> <span data-ttu-id="e45a3-223">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="e45a3-224">11</span><span class="sxs-lookup"><span data-stu-id="e45a3-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-225">税</span><span class="sxs-lookup"><span data-stu-id="e45a3-225">Tax</span></span></td>
<td><p><span data-ttu-id="e45a3-226">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="e45a3-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e45a3-227">0</span><span class="sxs-lookup"><span data-stu-id="e45a3-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="e45a3-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="e45a3-229">税后总额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-229">Total after tax.</span></span> <span data-ttu-id="e45a3-230">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="e45a3-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="e45a3-231">11</span><span class="sxs-lookup"><span data-stu-id="e45a3-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-232">货币</span><span class="sxs-lookup"><span data-stu-id="e45a3-232">Currency</span></span></td>
<td><p><span data-ttu-id="e45a3-233">货币类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-233">Currency type.</span></span> <span data-ttu-id="e45a3-234">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="e45a3-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="e45a3-235">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e45a3-236">EUR</span><span class="sxs-lookup"><span data-stu-id="e45a3-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e45a3-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="e45a3-238">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="e45a3-239">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e45a3-240">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="e45a3-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="e45a3-241">MPNID</span></span></td>
<td><p><span data-ttu-id="e45a3-242">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="e45a3-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="e45a3-243">4390934</span><span class="sxs-lookup"><span data-stu-id="e45a3-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e45a3-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e45a3-245">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e45a3-246">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="e45a3-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="e45a3-247">4390934</span><span class="sxs-lookup"><span data-stu-id="e45a3-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="e45a3-248">DomainName</span></span></td>
<td><p><span data-ttu-id="e45a3-249">客户&#39;的域名，用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="e45a3-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="e45a3-250">这不应用于唯一地标识客户，因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="e45a3-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="e45a3-251">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="e45a3-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e45a3-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e45a3-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e45a3-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e45a3-254">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-254">Subscription nickname.</span></span> <span data-ttu-id="e45a3-255">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="e45a3-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="e45a3-256">联机项目</span><span class="sxs-lookup"><span data-stu-id="e45a3-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e45a3-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e45a3-258">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e45a3-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e45a3-259">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="e45a3-260">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="e45a3-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="e45a3-261">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="e45a3-261">Usage-based file fields</span></span>


<span data-ttu-id="e45a3-262">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="e45a3-263">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="e45a3-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e45a3-264"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="e45a3-265"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="e45a3-266"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="e45a3-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="e45a3-268">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="e45a3-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e45a3-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e45a3-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="e45a3-271">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="e45a3-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="e45a3-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="e45a3-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="e45a3-274">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="e45a3-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="e45a3-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e45a3-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="e45a3-277">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="e45a3-278">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e45a3-279">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="e45a3-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="e45a3-280">MPNID</span></span></td>
<td><p><span data-ttu-id="e45a3-281">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="e45a3-282">4390934</span><span class="sxs-lookup"><span data-stu-id="e45a3-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e45a3-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e45a3-284">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e45a3-285">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="e45a3-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="e45a3-286">4390934</span><span class="sxs-lookup"><span data-stu-id="e45a3-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e45a3-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e45a3-288">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="e45a3-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="e45a3-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="e45a3-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e45a3-291">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="e45a3-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e45a3-292">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e45a3-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e45a3-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e45a3-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e45a3-295">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="e45a3-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e45a3-296">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="e45a3-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e45a3-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="e45a3-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e45a3-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e45a3-299">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e45a3-300">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e45a3-301">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="e45a3-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e45a3-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e45a3-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e45a3-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e45a3-304">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="e45a3-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e45a3-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e45a3-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e45a3-307">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="e45a3-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="e45a3-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e45a3-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="e45a3-309">OrderID</span></span></td>
<td><p><span data-ttu-id="e45a3-310">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e45a3-311">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e45a3-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e45a3-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="e45a3-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="e45a3-314">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="e45a3-315">虚拟机</span><span class="sxs-lookup"><span data-stu-id="e45a3-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="e45a3-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="e45a3-317">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e45a3-318">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="e45a3-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="e45a3-319">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="e45a3-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="e45a3-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="e45a3-321">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="e45a3-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e45a3-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-323">资源名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="e45a3-324">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e45a3-325">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="e45a3-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="e45a3-326">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="e45a3-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-327">Region</span><span class="sxs-lookup"><span data-stu-id="e45a3-327">Region</span></span></td>
<td><p><span data-ttu-id="e45a3-328">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="e45a3-328">The region the usage applies to.</span></span> <span data-ttu-id="e45a3-329">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="e45a3-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="e45a3-330">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="e45a3-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-331">SKU</span><span class="sxs-lookup"><span data-stu-id="e45a3-331">SKU</span></span></td>
<td><p><span data-ttu-id="e45a3-332">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e45a3-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="e45a3-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="e45a3-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="e45a3-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="e45a3-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="e45a3-335">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="e45a3-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="e45a3-336">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="e45a3-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="e45a3-337">1</span><span class="sxs-lookup"><span data-stu-id="e45a3-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="e45a3-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="e45a3-339">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="e45a3-340">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="e45a3-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="e45a3-341">11</span><span class="sxs-lookup"><span data-stu-id="e45a3-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="e45a3-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="e45a3-343">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="e45a3-343">Units included as part of the offer.</span></span> <span data-ttu-id="e45a3-344">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="e45a3-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="e45a3-345">0</span><span class="sxs-lookup"><span data-stu-id="e45a3-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="e45a3-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="e45a3-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="e45a3-347">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="e45a3-348">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="e45a3-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="e45a3-349">11</span><span class="sxs-lookup"><span data-stu-id="e45a3-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="e45a3-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="e45a3-351">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="e45a3-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="e45a3-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="e45a3-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="e45a3-354">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="e45a3-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e45a3-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="e45a3-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="e45a3-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="e45a3-357">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="e45a3-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e45a3-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="e45a3-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="e45a3-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="e45a3-360">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="e45a3-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="e45a3-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-362">货币</span><span class="sxs-lookup"><span data-stu-id="e45a3-362">Currency</span></span></td>
<td><p><span data-ttu-id="e45a3-363">货币类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-363">Currency type.</span></span> <span data-ttu-id="e45a3-364">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="e45a3-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="e45a3-365">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e45a3-366">EUR</span><span class="sxs-lookup"><span data-stu-id="e45a3-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e45a3-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e45a3-368">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-368">Pretax price per unit.</span></span> <span data-ttu-id="e45a3-369">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="e45a3-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e45a3-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="e45a3-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e45a3-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e45a3-372">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-372">Post tax price per unit.</span></span> <span data-ttu-id="e45a3-373">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="e45a3-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e45a3-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="e45a3-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e45a3-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="e45a3-376">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-376">The type of charge or adjustment.</span></span> <span data-ttu-id="e45a3-377">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e45a3-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e45a3-378">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="e45a3-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="e45a3-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="e45a3-380">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="e45a3-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="e45a3-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="e45a3-383">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="e45a3-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="e45a3-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e45a3-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="e45a3-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="e45a3-386">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="e45a3-387">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="e45a3-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="e45a3-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="e45a3-389">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="e45a3-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="e45a3-390">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="e45a3-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="e45a3-391">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="e45a3-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="e45a3-392">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="e45a3-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="e45a3-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="e45a3-394">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="e45a3-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="e45a3-395">外部</span><span class="sxs-lookup"><span data-stu-id="e45a3-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-396">项目</span><span class="sxs-lookup"><span data-stu-id="e45a3-396">Project</span></span></td>
<td><p><span data-ttu-id="e45a3-397">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="e45a3-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e45a3-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="e45a3-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="e45a3-400">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="e45a3-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="e45a3-401">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="e45a3-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="e45a3-402">如果你有已预配服务总线连接的 25 个包，并且在那一天利用了 1 个，则这一天的每日使用情况声明将指示“25 连接/ 30 天 – 已使用：1.000000”。</span><span class="sxs-lookup"><span data-stu-id="e45a3-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e45a3-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="e45a3-404">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="e45a3-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e45a3-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e45a3-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e45a3-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="e45a3-406">DomainName</span></span></td>
<td><p><span data-ttu-id="e45a3-407">客户&#39;的域名，用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="e45a3-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="e45a3-408">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="e45a3-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e45a3-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e45a3-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="e45a3-410">单位</span><span class="sxs-lookup"><span data-stu-id="e45a3-410">Unit</span></span></td>
<td><p><span data-ttu-id="e45a3-411">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="e45a3-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="e45a3-412">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="e45a3-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="e45a3-413">一次性和定期文件字段</span><span class="sxs-lookup"><span data-stu-id="e45a3-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e45a3-414">列</span><span class="sxs-lookup"><span data-stu-id="e45a3-414">Column</span></span></th>
<th><span data-ttu-id="e45a3-415">描述</span><span class="sxs-lookup"><span data-stu-id="e45a3-415">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="e45a3-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e45a3-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="e45a3-417">特定计费实体的唯一 Microsoft Azure Active Directory 租户标识符，采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="e45a3-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e45a3-418">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="e45a3-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e45a3-419">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="e45a3-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-420">客户 Id</span><span class="sxs-lookup"><span data-stu-id="e45a3-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="e45a3-421">用于标识客户的唯一 Microsoft Azure Active Directory 租户 ID，采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="e45a3-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-422">客户名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="e45a3-423">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="e45a3-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="e45a3-425">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="e45a3-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="e45a3-426">这不应用于唯一地标识客户，因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="e45a3-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="e45a3-427">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="e45a3-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-428">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="e45a3-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="e45a3-429">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="e45a3-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-430">发票编号</span><span class="sxs-lookup"><span data-stu-id="e45a3-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="e45a3-431">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="e45a3-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="e45a3-432">MpnId</span></span></td>
<td><p><span data-ttu-id="e45a3-433">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-434">经销商 MpnId</span><span class="sxs-lookup"><span data-stu-id="e45a3-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="e45a3-435">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-436">订单编码</span><span class="sxs-lookup"><span data-stu-id="e45a3-436">Order ID</span></span></td>
<td><p><span data-ttu-id="e45a3-437">Microsoft commerce 平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="e45a3-438">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-439">订单日期</span><span class="sxs-lookup"><span data-stu-id="e45a3-439">Order date</span></span></td>
<td><p><span data-ttu-id="e45a3-440">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="e45a3-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="e45a3-441">ProductId</span></span></td>
<td><p><span data-ttu-id="e45a3-442">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="e45a3-443">SkuId</span></span></td>
<td><p><span data-ttu-id="e45a3-444">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="e45a3-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="e45a3-446">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-446">The ID for a particular Availability.</span></span> <span data-ttu-id="e45a3-447">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="e45a3-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-448">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="e45a3-449">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-450">产品名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-450">Product name</span></span></td>
<td><p><span data-ttu-id="e45a3-451">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="e45a3-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="e45a3-453">产品发布者的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="e45a3-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="e45a3-455">此发布服务器的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-456">订阅说明</span><span class="sxs-lookup"><span data-stu-id="e45a3-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="e45a3-457">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-458">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="e45a3-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="e45a3-459">Microsoft commerce 平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="e45a3-460">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="e45a3-461">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="e45a3-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e45a3-463">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="e45a3-463">Start day of the charges.</span></span> <span data-ttu-id="e45a3-464">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e45a3-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e45a3-466">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="e45a3-466">End day of the charges.</span></span> <span data-ttu-id="e45a3-467">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="e45a3-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-468">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="e45a3-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="e45a3-469">采购的术语长度和计费周期。</span><span class="sxs-lookup"><span data-stu-id="e45a3-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="e45a3-470">例如，"1 年，每月"。</span><span class="sxs-lookup"><span data-stu-id="e45a3-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-471">费用类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="e45a3-472">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-473">单价</span><span class="sxs-lookup"><span data-stu-id="e45a3-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="e45a3-474">购买时在 pricelist 中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e45a3-475">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-476">有效单价</span><span class="sxs-lookup"><span data-stu-id="e45a3-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="e45a3-477">进行调整后的单位价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-478">数量</span><span class="sxs-lookup"><span data-stu-id="e45a3-478">Quantity</span></span></td>
<td><p><span data-ttu-id="e45a3-479">单位数。</span><span class="sxs-lookup"><span data-stu-id="e45a3-479">Number of units.</span></span> <span data-ttu-id="e45a3-480">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-481">单位类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-481">Unit type</span></span></td>
<td><p><span data-ttu-id="e45a3-482">要购买的单位类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="e45a3-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="e45a3-484">适用于任何适用折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="e45a3-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-485">Sub Total</span><span class="sxs-lookup"><span data-stu-id="e45a3-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="e45a3-486">税前总额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-486">Total before tax.</span></span> <span data-ttu-id="e45a3-487">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-488">税金总计</span><span class="sxs-lookup"><span data-stu-id="e45a3-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="e45a3-489">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="e45a3-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-490">总计</span><span class="sxs-lookup"><span data-stu-id="e45a3-490">Total</span></span></td>
<td><p><span data-ttu-id="e45a3-491">税后总额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-491">Total after tax.</span></span> <span data-ttu-id="e45a3-492">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="e45a3-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-493">货币</span><span class="sxs-lookup"><span data-stu-id="e45a3-493">Currency</span></span></td>
<td><p><span data-ttu-id="e45a3-494">货币类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-494">Currency type.</span></span> <span data-ttu-id="e45a3-495">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="e45a3-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="e45a3-496">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="e45a3-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="e45a3-498">订单 ID 的备用标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-499">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="e45a3-499">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="e45a3-500">启用每月计费时显示每月。</span><span class="sxs-lookup"><span data-stu-id="e45a3-500">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="e45a3-501">否则为空白。</span><span class="sxs-lookup"><span data-stu-id="e45a3-501">Otherwise blank.</span></span> </p></td>
</tr>

</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="e45a3-502">每日分级使用文件字段</span><span class="sxs-lookup"><span data-stu-id="e45a3-502">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e45a3-503">列</span><span class="sxs-lookup"><span data-stu-id="e45a3-503">Column</span></span></th>
<th><span data-ttu-id="e45a3-504">描述</span><span class="sxs-lookup"><span data-stu-id="e45a3-504">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="e45a3-505">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e45a3-505">PartnerId</span></span></td>
<td><p><span data-ttu-id="e45a3-506">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-506">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-507">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e45a3-507">PartnerName</span></span></td>
<td><p><span data-ttu-id="e45a3-508">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-508">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-509">CustomerId</span><span class="sxs-lookup"><span data-stu-id="e45a3-509">CustomerId</span></span></td>
<td><p><span data-ttu-id="e45a3-510">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="e45a3-510">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-511">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="e45a3-511">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="e45a3-512">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-512">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e45a3-513">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-513">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-514">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="e45a3-514">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="e45a3-515">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="e45a3-515">The customer’s domain name.</span></span> <span data-ttu-id="e45a3-516">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-516">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-517">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="e45a3-517">Customer country</span></span></td>
<td><p><span data-ttu-id="e45a3-518">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="e45a3-518">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-519">MPNID</span><span class="sxs-lookup"><span data-stu-id="e45a3-519">MPNID</span></span></td>
<td><p><span data-ttu-id="e45a3-520">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-520">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-521">经销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="e45a3-521">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="e45a3-522">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-522">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e45a3-523">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-524">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e45a3-524">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e45a3-525">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="e45a3-525">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="e45a3-526">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-526">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-527">ProductId</span><span class="sxs-lookup"><span data-stu-id="e45a3-527">ProductId</span></span></td>
<td><p><span data-ttu-id="e45a3-528">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-528">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-529">SkuId</span><span class="sxs-lookup"><span data-stu-id="e45a3-529">SkuId</span></span></td>
<td><p><span data-ttu-id="e45a3-530">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-530">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-531">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="e45a3-531">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="e45a3-532">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-532">The ID for a particular Availability.</span></span> <span data-ttu-id="e45a3-533">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="e45a3-533">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-534">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-534">SKU Name</span></span></td>
<td><p><span data-ttu-id="e45a3-535">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-535">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-536">PublisherName</span><span class="sxs-lookup"><span data-stu-id="e45a3-536">PublisherName</span></span></td>
<td><p><span data-ttu-id="e45a3-537">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="e45a3-537">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-538">PublisherID</span><span class="sxs-lookup"><span data-stu-id="e45a3-538">PublisherID</span></span></td>
<td><p><span data-ttu-id="e45a3-539">GUID 格式的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-539">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="e45a3-540">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-540">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="e45a3-541">订阅说明</span><span class="sxs-lookup"><span data-stu-id="e45a3-541">Subscription Description</span></span></td>
<td><p><span data-ttu-id="e45a3-542">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="e45a3-542">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e45a3-543">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-543">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-544">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="e45a3-544">Subscription ID</span></span></td>
<td><p><span data-ttu-id="e45a3-545">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e45a3-545">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e45a3-546">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-546">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="e45a3-547">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="e45a3-547">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-548">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-548">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e45a3-549">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="e45a3-549">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="e45a3-550">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="e45a3-550">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-551">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e45a3-551">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e45a3-552">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="e45a3-552">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="e45a3-553">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="e45a3-553">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-554">使用日期</span><span class="sxs-lookup"><span data-stu-id="e45a3-554">Usage Date</span></span></td>
<td><p><span data-ttu-id="e45a3-555">服务使用日期。</span><span class="sxs-lookup"><span data-stu-id="e45a3-555">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-556">计量类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-556">Meter Type</span></span></td>
<td><p><span data-ttu-id="e45a3-557">计量器的类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-557">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-558">计量类别</span><span class="sxs-lookup"><span data-stu-id="e45a3-558">Meter Category</span></span></td>
<td><p><span data-ttu-id="e45a3-559">使用的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="e45a3-559">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-560">计量 Id</span><span class="sxs-lookup"><span data-stu-id="e45a3-560">Meter Id</span></span></td>
<td><p><span data-ttu-id="e45a3-561">正在使用的计量的 ID。</span><span class="sxs-lookup"><span data-stu-id="e45a3-561">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-562">计量子类别</span><span class="sxs-lookup"><span data-stu-id="e45a3-562">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="e45a3-563">可能影响速度的 Azure 服务类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-563">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-564">计量名称</span><span class="sxs-lookup"><span data-stu-id="e45a3-564">Meter Name</span></span></td>
<td><p><span data-ttu-id="e45a3-565">所使用的计量的度量单位。</span><span class="sxs-lookup"><span data-stu-id="e45a3-565">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-566">计量区域</span><span class="sxs-lookup"><span data-stu-id="e45a3-566">Meter Region</span></span></td>
<td><p><span data-ttu-id="e45a3-567">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-567">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-568">单位</span><span class="sxs-lookup"><span data-stu-id="e45a3-568">Unit</span></span></td>
<td><p><span data-ttu-id="e45a3-569">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="e45a3-569">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-570">已消耗数量</span><span class="sxs-lookup"><span data-stu-id="e45a3-570">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="e45a3-571">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-571">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="e45a3-572">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="e45a3-572">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-573">资源位置</span><span class="sxs-lookup"><span data-stu-id="e45a3-573">Resource Location</span></span></td>
<td><p><span data-ttu-id="e45a3-574">计量器正在其中运行的数据中心。</span><span class="sxs-lookup"><span data-stu-id="e45a3-574">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-575">已使用服务</span><span class="sxs-lookup"><span data-stu-id="e45a3-575">Consumed Service</span></span></td>
<td><p><span data-ttu-id="e45a3-576">你使用的 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="e45a3-576">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="e45a3-577">资源 URI</span><span class="sxs-lookup"><span data-stu-id="e45a3-577">Resource URI</span></span></td>
<td><p><span data-ttu-id="e45a3-578">所使用资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="e45a3-578">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-579">费用类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-579">Charge type</span></span></td>
<td><p><span data-ttu-id="e45a3-580">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-580">The type of charge or adjustment.</span></span> <span data-ttu-id="e45a3-581">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-581">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-582">单价</span><span class="sxs-lookup"><span data-stu-id="e45a3-582">Unit price</span></span></td>
<td><p><span data-ttu-id="e45a3-583">购买时在 pricelist 中发布的每个许可证的价格。</span><span class="sxs-lookup"><span data-stu-id="e45a3-583">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e45a3-584">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-585">数量</span><span class="sxs-lookup"><span data-stu-id="e45a3-585">Quantity</span></span></td>
<td><p><span data-ttu-id="e45a3-586">许可证数量。</span><span class="sxs-lookup"><span data-stu-id="e45a3-586">Number of licenses.</span></span> <span data-ttu-id="e45a3-587">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="e45a3-587">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-588">单位类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-588">Unit type</span></span></td>
<td><p><span data-ttu-id="e45a3-589">计量计量器的单位类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-589">The type of unit the meter is charged in.</span></span> <span data-ttu-id="e45a3-590">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="e45a3-590">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-591">帐单税前税</span><span class="sxs-lookup"><span data-stu-id="e45a3-591">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="e45a3-592">税前的总金额。</span><span class="sxs-lookup"><span data-stu-id="e45a3-592">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-593">计费货币</span><span class="sxs-lookup"><span data-stu-id="e45a3-593">Billing currency</span></span></td>
<td><p><span data-ttu-id="e45a3-594">客户的地理区域中的货币</span><span class="sxs-lookup"><span data-stu-id="e45a3-594">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-595">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="e45a3-595">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="e45a3-596">添加税款之前的定价。</span><span class="sxs-lookup"><span data-stu-id="e45a3-596">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-597">定价货币</span><span class="sxs-lookup"><span data-stu-id="e45a3-597">Pricing currency</span></span></td>
<td><p><span data-ttu-id="e45a3-598">Pricelist 中的货币。</span><span class="sxs-lookup"><span data-stu-id="e45a3-598">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e45a3-599">服务信息1</span><span class="sxs-lookup"><span data-stu-id="e45a3-599">Service Info 1</span></span></td>
<td><p><span data-ttu-id="e45a3-600">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="e45a3-600">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-601">服务信息2</span><span class="sxs-lookup"><span data-stu-id="e45a3-601">Service Info 2</span></span></td>
<td><p><span data-ttu-id="e45a3-602">捕获可选的服务特定元数据的旧字段。</span><span class="sxs-lookup"><span data-stu-id="e45a3-602">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e45a3-603">附加信息</span><span class="sxs-lookup"><span data-stu-id="e45a3-603">Additional Info</span></span></td>
<td><p><span data-ttu-id="e45a3-604">其他列中未涵盖的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="e45a3-604">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="e45a3-605">发票与对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-605">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="e45a3-606">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="e45a3-606">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="e45a3-607">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="e45a3-607">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="e45a3-608">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="e45a3-608">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="e45a3-609">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="e45a3-609">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="e45a3-610">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="e45a3-610">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="e45a3-611"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-611"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-612"><strong>对帐文件费用说明（ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-612"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-613"><strong>此费用是什么？</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-613"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-614"><strong>如何实现将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-614"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="e45a3-615"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-615"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-616">激活费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-616">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-617">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="e45a3-617">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="e45a3-618">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-618">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-619">取消费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-619">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-620">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-620">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-621">周期费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-621">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-622">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-622">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-623">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="e45a3-623">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-624">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-624">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-625">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-625">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-626">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="e45a3-626">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-627">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-627">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-628">使用年度计费时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-628">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-629">购买费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-629">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-630">使用月度帐单时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="e45a3-630">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-631">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-631">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-632">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-632">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="e45a3-633">续订费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-633">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-634">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-634">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-635">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-635">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-636">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-636">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="e45a3-637"><strong>一次性费用</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-637"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="e45a3-638">新</span><span class="sxs-lookup"><span data-stu-id="e45a3-638">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-639">创建新购买时使用</span><span class="sxs-lookup"><span data-stu-id="e45a3-639">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-640">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e45a3-640">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-641">用于原始购买的退款和增加后的新数量</span><span class="sxs-lookup"><span data-stu-id="e45a3-641">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-642">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e45a3-642">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-643">用于原始购买的退款和减少后的新数量</span><span class="sxs-lookup"><span data-stu-id="e45a3-643">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-644">“取消”</span><span class="sxs-lookup"><span data-stu-id="e45a3-644">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-645">取消订阅时使用</span><span class="sxs-lookup"><span data-stu-id="e45a3-645">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-646">转换</span><span class="sxs-lookup"><span data-stu-id="e45a3-646">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-647">升级许可证时使用，但座位数保持不变</span><span class="sxs-lookup"><span data-stu-id="e45a3-647">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="e45a3-648"><strong>使用费用</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-648"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-649">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-649">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-650">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-650">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="e45a3-651">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-651">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-652">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-652">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-653">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-653">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="e45a3-654"><strong>制作</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-654"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-655">偏移行项</span><span class="sxs-lookup"><span data-stu-id="e45a3-655">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-656">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="e45a3-656">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-657">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-657">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="e45a3-658">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-658">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="e45a3-659"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-659"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-660">激活折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-660">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-661">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-661">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="e45a3-662">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-662">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-663">周期折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-663">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-664">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-664">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-665">续订折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-665">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-666">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-666">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-667">取消折扣</span><span class="sxs-lookup"><span data-stu-id="e45a3-667">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-668">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="e45a3-668">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="e45a3-669"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-669"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-670"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="e45a3-670"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="e45a3-671">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-671">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e45a3-672"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="e45a3-672"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-673"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="e45a3-673"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="e45a3-674"><em>异常：行项 &quot;Offset &quot; 已包含税金。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="e45a3-674"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-675">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="e45a3-675">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="e45a3-676">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-676">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="e45a3-677">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="e45a3-677">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
