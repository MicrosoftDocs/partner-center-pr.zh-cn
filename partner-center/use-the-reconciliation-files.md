---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 07/08/2019
description: 在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 83be47cd9963d7e5f14b6c670cd57a8ab1d54011
ms.sourcegitcommit: 66afdaa662cfad217e29ba1f9e3a9ffd4349112f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2019
ms.locfileid: "67694929"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="3f656-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="3f656-103">Use the reconciliation files</span></span>

<span data-ttu-id="3f656-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="3f656-104">**Applies to**</span></span>

-  <span data-ttu-id="3f656-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="3f656-105">Partner Center</span></span>
-  <span data-ttu-id="3f656-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="3f656-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="3f656-107">在计费周期中每个收费的详细的明细项目视图，从合作伙伴中心下载的对帐文件。</span><span class="sxs-lookup"><span data-stu-id="3f656-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="3f656-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="3f656-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="3f656-109">格式设置问题</span><span class="sxs-lookup"><span data-stu-id="3f656-109">Formatting issues</span></span>

<span data-ttu-id="3f656-110">偶尔侦测文件可能会遇到格式问题。</span><span class="sxs-lookup"><span data-stu-id="3f656-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="3f656-111">（这可能发生，例如，如果不使用 EN-US 区域设置。）请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="3f656-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="3f656-112">在 Excel 中打开.csv 文件，并选择第一列。</span><span class="sxs-lookup"><span data-stu-id="3f656-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="3f656-113">在功能区中，选择<strong>数据</strong>，然后选择<strong>分列</strong>。</span><span class="sxs-lookup"><span data-stu-id="3f656-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="3f656-114">在转换文本分列向导，选择<strong>分隔的文件类型</strong>，然后选择<strong>下一步</strong>。</span><span class="sxs-lookup"><span data-stu-id="3f656-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="3f656-115">在分隔符字段中，选择<strong>逗号</strong>。</span><span class="sxs-lookup"><span data-stu-id="3f656-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="3f656-116">如果<strong>选项卡</strong>是尚未选中，你可以将其保留。</span><span class="sxs-lookup"><span data-stu-id="3f656-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="3f656-117">选择“<strong>下一步</strong>”。</span><span class="sxs-lookup"><span data-stu-id="3f656-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="3f656-118">在列数据格式字段中，选择<strong>日期：MDY</strong>，然后选择<strong>下一步</strong>。</span><span class="sxs-lookup"><span data-stu-id="3f656-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="3f656-119">在列数据格式字段中，选择<strong>文本</strong>的列，并选择所有金额<strong>完成</strong>。</span><span class="sxs-lookup"><span data-stu-id="3f656-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="3f656-120">下载较大的侦测文件</span><span class="sxs-lookup"><span data-stu-id="3f656-120">Downloading a large recon file</span></span>

<span data-ttu-id="3f656-121">侦测文件可以变得很大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="3f656-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="3f656-122">若要帮助下载大型侦测文件的 PowerShell 脚本，请参阅[获取发票行项](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="3f656-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="3f656-123">由合作伙伴详细列举</span><span class="sxs-lookup"><span data-stu-id="3f656-123">Itemize by partner</span></span>


<span data-ttu-id="3f656-124">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="3f656-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="3f656-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f656-125">MPN ID</span></span></th>
<th><span data-ttu-id="3f656-126">描述</span><span class="sxs-lookup"><span data-stu-id="3f656-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="3f656-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f656-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="3f656-128">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-129">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f656-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="3f656-130">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="3f656-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="3f656-131">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="3f656-132">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="3f656-133">干支查看或更新的分销商，在合作伙伴中心菜单中，选择<strong>客户</strong>，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="3f656-134">在客户菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="3f656-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="3f656-135">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="3f656-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="3f656-136">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="3f656-137">如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="3f656-138">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="3f656-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="3f656-139">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="3f656-139">License-based file fields</span></span>


<span data-ttu-id="3f656-140">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="3f656-141"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="3f656-142"><strong>说明</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="3f656-143"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="3f656-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="3f656-145">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="3f656-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="3f656-146">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="3f656-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="3f656-147">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="3f656-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="3f656-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="3f656-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="3f656-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="3f656-150">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="3f656-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="3f656-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="3f656-152">OrderID</span></span></td>
<td><p><span data-ttu-id="3f656-153">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="3f656-154">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="3f656-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="3f656-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="3f656-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="3f656-157">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="3f656-158">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="3f656-159">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="3f656-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="3f656-160">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="3f656-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="3f656-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="3f656-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="3f656-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="3f656-163">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="3f656-164">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="3f656-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="3f656-165">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="3f656-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="3f656-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="3f656-167">OfferID</span></span></td>
<td><p><span data-ttu-id="3f656-168">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-168">Unique offer ID.</span></span> <span data-ttu-id="3f656-169">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="3f656-170"><b>注意</b>：此值不匹配价格列表中的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="3f656-171">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="3f656-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="3f656-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="3f656-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="3f656-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="3f656-174">唯一的持久型产品 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="3f656-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="3f656-175"><b>注意</b>：此值与从价格列表产品/服务 ID 相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="3f656-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="3f656-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="3f656-177">OfferName</span></span></td>
<td><p><span data-ttu-id="3f656-178">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="3f656-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="3f656-179">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="3f656-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="3f656-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="3f656-181">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="3f656-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="3f656-182">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="3f656-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="3f656-183">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="3f656-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="3f656-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="3f656-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="3f656-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="3f656-186">订阅结束日期：12 个月 + x 天之后开始日期 （符合合作伙伴计费日期） 或 12 个月续订日期。</span><span class="sxs-lookup"><span data-stu-id="3f656-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="3f656-187">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="3f656-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="3f656-188">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="3f656-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="3f656-189">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="3f656-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="3f656-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="3f656-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="3f656-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="3f656-192">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="3f656-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="3f656-193">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="3f656-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="3f656-194">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="3f656-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="3f656-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="3f656-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="3f656-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="3f656-197">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="3f656-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="3f656-198">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="3f656-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="3f656-199">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="3f656-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="3f656-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="3f656-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="3f656-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="3f656-202">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-202">The type of charge or adjustment.</span></span> <span data-ttu-id="3f656-203">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="3f656-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="3f656-204">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="3f656-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="3f656-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="3f656-206">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="3f656-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="3f656-207">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="3f656-208">6.82</span><span class="sxs-lookup"><span data-stu-id="3f656-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-209">数量</span><span class="sxs-lookup"><span data-stu-id="3f656-209">Quantity</span></span></td>
<td><p><span data-ttu-id="3f656-210">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="3f656-210">Number of seats.</span></span> <span data-ttu-id="3f656-211">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="3f656-212">2</span><span class="sxs-lookup"><span data-stu-id="3f656-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-213">金额</span><span class="sxs-lookup"><span data-stu-id="3f656-213">Amount</span></span></td>
<td><p><span data-ttu-id="3f656-214">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="3f656-214">Total of price for quantity.</span></span> <span data-ttu-id="3f656-215">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="3f656-216">13.32</span><span class="sxs-lookup"><span data-stu-id="3f656-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="3f656-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="3f656-218">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="3f656-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="3f656-219">IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="3f656-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="3f656-220">2.32</span><span class="sxs-lookup"><span data-stu-id="3f656-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-221">小计</span><span class="sxs-lookup"><span data-stu-id="3f656-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="3f656-222">税前总额。</span><span class="sxs-lookup"><span data-stu-id="3f656-222">Total before tax.</span></span> <span data-ttu-id="3f656-223">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="3f656-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="3f656-224">11</span><span class="sxs-lookup"><span data-stu-id="3f656-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-225">税</span><span class="sxs-lookup"><span data-stu-id="3f656-225">Tax</span></span></td>
<td><p><span data-ttu-id="3f656-226">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="3f656-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="3f656-227">0</span><span class="sxs-lookup"><span data-stu-id="3f656-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="3f656-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="3f656-229">税后总额。</span><span class="sxs-lookup"><span data-stu-id="3f656-229">Total after tax.</span></span> <span data-ttu-id="3f656-230">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="3f656-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="3f656-231">11</span><span class="sxs-lookup"><span data-stu-id="3f656-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-232">货币</span><span class="sxs-lookup"><span data-stu-id="3f656-232">Currency</span></span></td>
<td><p><span data-ttu-id="3f656-233">货币类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-233">Currency type.</span></span> <span data-ttu-id="3f656-234">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="3f656-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="3f656-235">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="3f656-236">EUR</span><span class="sxs-lookup"><span data-stu-id="3f656-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="3f656-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="3f656-238">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="3f656-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="3f656-239">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="3f656-240">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="3f656-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="3f656-241">MPNID</span></span></td>
<td><p><span data-ttu-id="3f656-242">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f656-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="3f656-243">4390934</span><span class="sxs-lookup"><span data-stu-id="3f656-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="3f656-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="3f656-245">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="3f656-246">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="3f656-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="3f656-247">4390934</span><span class="sxs-lookup"><span data-stu-id="3f656-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="3f656-248">DomainName</span></span></td>
<td><p><span data-ttu-id="3f656-249">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="3f656-250">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="3f656-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="3f656-251">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="3f656-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="3f656-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="3f656-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="3f656-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="3f656-254">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="3f656-254">Subscription nickname.</span></span> <span data-ttu-id="3f656-255">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="3f656-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="3f656-256">联机项目</span><span class="sxs-lookup"><span data-stu-id="3f656-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="3f656-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="3f656-258">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="3f656-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="3f656-259">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="3f656-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="3f656-260">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="3f656-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="3f656-261">基于使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="3f656-261">Usage-based file fields</span></span>


<span data-ttu-id="3f656-262">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="3f656-263">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="3f656-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="3f656-264"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="3f656-265"><strong>说明</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="3f656-266"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="3f656-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="3f656-268">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="3f656-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="3f656-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="3f656-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="3f656-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="3f656-271">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="3f656-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="3f656-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="3f656-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="3f656-274">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="3f656-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="3f656-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="3f656-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="3f656-277">客户&#39;s 组织名称在合作伙伴中心的报告。</span><span class="sxs-lookup"><span data-stu-id="3f656-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="3f656-278">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="3f656-279">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="3f656-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="3f656-280">MPNID</span></span></td>
<td><p><span data-ttu-id="3f656-281">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="3f656-282">4390934</span><span class="sxs-lookup"><span data-stu-id="3f656-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="3f656-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="3f656-284">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="3f656-285">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="3f656-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="3f656-286">4390934</span><span class="sxs-lookup"><span data-stu-id="3f656-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="3f656-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="3f656-288">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="3f656-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="3f656-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="3f656-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="3f656-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="3f656-291">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="3f656-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="3f656-292">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="3f656-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="3f656-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="3f656-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="3f656-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="3f656-295">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="3f656-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="3f656-296">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="3f656-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="3f656-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="3f656-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="3f656-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="3f656-299">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="3f656-300">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="3f656-301">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="3f656-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="3f656-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="3f656-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="3f656-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="3f656-304">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="3f656-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="3f656-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="3f656-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="3f656-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="3f656-307">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="3f656-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="3f656-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="3f656-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="3f656-309">OrderID</span></span></td>
<td><p><span data-ttu-id="3f656-310">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="3f656-311">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="3f656-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="3f656-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="3f656-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="3f656-314">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="3f656-315">虚拟机</span><span class="sxs-lookup"><span data-stu-id="3f656-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="3f656-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="3f656-317">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="3f656-318">服务总线 – 个人或包</span><span class="sxs-lookup"><span data-stu-id="3f656-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="3f656-319">SQL Azure 数据库 – 商用版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="3f656-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="3f656-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="3f656-321">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="3f656-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="3f656-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-323">资源名称</span><span class="sxs-lookup"><span data-stu-id="3f656-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="3f656-324">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="3f656-325">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="3f656-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="3f656-326">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="3f656-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-327">Region</span><span class="sxs-lookup"><span data-stu-id="3f656-327">Region</span></span></td>
<td><p><span data-ttu-id="3f656-328">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="3f656-328">The region the usage applies to.</span></span> <span data-ttu-id="3f656-329">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="3f656-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="3f656-330">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="3f656-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-331">SKU</span><span class="sxs-lookup"><span data-stu-id="3f656-331">SKU</span></span></td>
<td><p><span data-ttu-id="3f656-332">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3f656-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="3f656-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="3f656-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="3f656-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="3f656-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="3f656-335">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="3f656-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="3f656-336">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="3f656-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="3f656-337">1</span><span class="sxs-lookup"><span data-stu-id="3f656-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="3f656-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="3f656-339">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="3f656-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="3f656-340">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="3f656-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="3f656-341">11</span><span class="sxs-lookup"><span data-stu-id="3f656-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="3f656-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="3f656-343">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="3f656-343">Units included as part of the offer.</span></span> <span data-ttu-id="3f656-344">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="3f656-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="3f656-345">0</span><span class="sxs-lookup"><span data-stu-id="3f656-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="3f656-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="3f656-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="3f656-347">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="3f656-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="3f656-348">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="3f656-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="3f656-349">11</span><span class="sxs-lookup"><span data-stu-id="3f656-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="3f656-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="3f656-351">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="3f656-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="3f656-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="3f656-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="3f656-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="3f656-354">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="3f656-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="3f656-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="3f656-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="3f656-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="3f656-357">税务量的费用，根据您的市场&#39;s 税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="3f656-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="3f656-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="3f656-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="3f656-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="3f656-360">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="3f656-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="3f656-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="3f656-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-362">货币</span><span class="sxs-lookup"><span data-stu-id="3f656-362">Currency</span></span></td>
<td><p><span data-ttu-id="3f656-363">货币类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-363">Currency type.</span></span> <span data-ttu-id="3f656-364">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="3f656-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="3f656-365">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="3f656-366">EUR</span><span class="sxs-lookup"><span data-stu-id="3f656-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="3f656-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="3f656-368">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="3f656-368">Pretax price per unit.</span></span> <span data-ttu-id="3f656-369">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="3f656-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="3f656-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="3f656-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="3f656-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="3f656-372">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="3f656-372">Post tax price per unit.</span></span> <span data-ttu-id="3f656-373">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="3f656-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="3f656-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="3f656-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="3f656-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="3f656-376">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-376">The type of charge or adjustment.</span></span> <span data-ttu-id="3f656-377">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="3f656-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="3f656-378">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="3f656-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="3f656-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="3f656-380">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="3f656-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="3f656-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="3f656-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="3f656-383">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="3f656-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="3f656-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="3f656-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="3f656-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="3f656-386">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="3f656-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="3f656-387">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="3f656-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="3f656-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="3f656-389">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="3f656-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="3f656-390">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="3f656-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="3f656-391">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="3f656-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="3f656-392">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="3f656-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="3f656-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="3f656-394">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="3f656-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="3f656-395">外部</span><span class="sxs-lookup"><span data-stu-id="3f656-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-396">项目</span><span class="sxs-lookup"><span data-stu-id="3f656-396">Project</span></span></td>
<td><p><span data-ttu-id="3f656-397">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="3f656-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="3f656-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="3f656-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="3f656-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="3f656-400">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="3f656-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="3f656-401">例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。</span><span class="sxs-lookup"><span data-stu-id="3f656-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="3f656-402">如果必须预配的服务总线连接的 25 包，并且你必须在那一天中使用了 1，这一天您每日使用情况语句将指示"25 连接 / 30 天 – 使用：1.000000”.</span><span class="sxs-lookup"><span data-stu-id="3f656-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="3f656-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="3f656-404">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="3f656-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="3f656-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="3f656-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="3f656-406">DomainName</span></span></td>
<td><p><span data-ttu-id="3f656-407">客户&#39;s 域名，用于帮助标识客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="3f656-408">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="3f656-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="3f656-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="3f656-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="3f656-410">单位</span><span class="sxs-lookup"><span data-stu-id="3f656-410">Unit</span></span></td>
<td><p><span data-ttu-id="3f656-411">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="3f656-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="3f656-412">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="3f656-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="3f656-413">一次性和重复性文件字段</span><span class="sxs-lookup"><span data-stu-id="3f656-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="3f656-414">列</span><span class="sxs-lookup"><span data-stu-id="3f656-414">Column</span></span></th>
<th><span data-ttu-id="3f656-415">描述</span><span class="sxs-lookup"><span data-stu-id="3f656-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="3f656-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="3f656-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="3f656-417">唯一的 GUID 格式中的特定计费实体的 Microsoft Azure Active Directory 租户标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="3f656-418">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="3f656-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="3f656-419">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="3f656-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-420">客户 Id</span><span class="sxs-lookup"><span data-stu-id="3f656-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="3f656-421">Microsoft Azure Active Directory 租户中唯一 ID，用于标识客户的 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="3f656-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-422">客户名称</span><span class="sxs-lookup"><span data-stu-id="3f656-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="3f656-423">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="3f656-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="3f656-425">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="3f656-426">这不应该用于唯一地标识客户，为客户/合作伙伴可以更新通过 O365 门户的虚构/默认域。</span><span class="sxs-lookup"><span data-stu-id="3f656-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="3f656-427">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="3f656-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-428">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="3f656-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="3f656-429">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3f656-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-430">发票编号</span><span class="sxs-lookup"><span data-stu-id="3f656-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="3f656-431">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="3f656-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="3f656-432">MpnId</span></span></td>
<td><p><span data-ttu-id="3f656-433">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="3f656-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="3f656-435">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-436">订单编码</span><span class="sxs-lookup"><span data-stu-id="3f656-436">Order ID</span></span></td>
<td><p><span data-ttu-id="3f656-437">Microsoft 商务平台中的订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="3f656-438">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-439">订单日期</span><span class="sxs-lookup"><span data-stu-id="3f656-439">Order date</span></span></td>
<td><p><span data-ttu-id="3f656-440">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="3f656-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="3f656-441">ProductId</span></span></td>
<td><p><span data-ttu-id="3f656-442">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="3f656-443">SkuId</span></span></td>
<td><p><span data-ttu-id="3f656-444">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="3f656-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="3f656-446">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-446">The ID for a particular Availability.</span></span> <span data-ttu-id="3f656-447">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="3f656-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-448">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="3f656-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="3f656-449">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-450">产品名称</span><span class="sxs-lookup"><span data-stu-id="3f656-450">Product name</span></span></td>
<td><p><span data-ttu-id="3f656-451">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="3f656-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="3f656-453">该产品的发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="3f656-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="3f656-455">此发布服务器的的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-456">订阅说明</span><span class="sxs-lookup"><span data-stu-id="3f656-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="3f656-457">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-458">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="3f656-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="3f656-459">Microsoft 商务平台中的订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="3f656-460">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="3f656-461">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="3f656-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="3f656-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="3f656-463">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="3f656-463">Start day of the charges.</span></span> <span data-ttu-id="3f656-464">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="3f656-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="3f656-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="3f656-466">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="3f656-466">End day of the charges.</span></span> <span data-ttu-id="3f656-467">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="3f656-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-468">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="3f656-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="3f656-469">期限长度和购买的计费周期。</span><span class="sxs-lookup"><span data-stu-id="3f656-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="3f656-470">例如，"1 年，每月一次。"</span><span class="sxs-lookup"><span data-stu-id="3f656-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-471">费用类型</span><span class="sxs-lookup"><span data-stu-id="3f656-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="3f656-472">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-473">单价</span><span class="sxs-lookup"><span data-stu-id="3f656-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="3f656-474">因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="3f656-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="3f656-475">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-476">有效的单位价格</span><span class="sxs-lookup"><span data-stu-id="3f656-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="3f656-477">单位价格后已进行调整。</span><span class="sxs-lookup"><span data-stu-id="3f656-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-478">数量</span><span class="sxs-lookup"><span data-stu-id="3f656-478">Quantity</span></span></td>
<td><p><span data-ttu-id="3f656-479">单位数。</span><span class="sxs-lookup"><span data-stu-id="3f656-479">Number of units.</span></span> <span data-ttu-id="3f656-480">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-481">单位类型</span><span class="sxs-lookup"><span data-stu-id="3f656-481">Unit type</span></span></td>
<td><p><span data-ttu-id="3f656-482">正在购买一个单位的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="3f656-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="3f656-484">所有适用的折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="3f656-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-485">子汇总</span><span class="sxs-lookup"><span data-stu-id="3f656-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="3f656-486">税前总额。</span><span class="sxs-lookup"><span data-stu-id="3f656-486">Total before tax.</span></span> <span data-ttu-id="3f656-487">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="3f656-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-488">税务总计</span><span class="sxs-lookup"><span data-stu-id="3f656-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="3f656-489">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="3f656-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-490">总计</span><span class="sxs-lookup"><span data-stu-id="3f656-490">Total</span></span></td>
<td><p><span data-ttu-id="3f656-491">税后总额。</span><span class="sxs-lookup"><span data-stu-id="3f656-491">Total after tax.</span></span> <span data-ttu-id="3f656-492">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="3f656-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-493">货币</span><span class="sxs-lookup"><span data-stu-id="3f656-493">Currency</span></span></td>
<td><p><span data-ttu-id="3f656-494">货币类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-494">Currency type.</span></span> <span data-ttu-id="3f656-495">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="3f656-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="3f656-496">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="3f656-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="3f656-498">备用标识符关联到一个订单 id。</span><span class="sxs-lookup"><span data-stu-id="3f656-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="3f656-499">评定的每日使用情况文件字段</span><span class="sxs-lookup"><span data-stu-id="3f656-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="3f656-500">列</span><span class="sxs-lookup"><span data-stu-id="3f656-500">Column</span></span></th>
<th><span data-ttu-id="3f656-501">描述</span><span class="sxs-lookup"><span data-stu-id="3f656-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="3f656-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="3f656-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="3f656-503">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="3f656-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="3f656-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="3f656-505">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="3f656-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="3f656-507">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="3f656-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="3f656-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="3f656-509">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="3f656-510">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="3f656-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="3f656-512">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="3f656-512">The customer’s domain name.</span></span> <span data-ttu-id="3f656-513">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="3f656-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-514">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="3f656-514">Customer country</span></span></td>
<td><p><span data-ttu-id="3f656-515">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3f656-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="3f656-516">MPNID</span></span></td>
<td><p><span data-ttu-id="3f656-517">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-518">分销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="3f656-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="3f656-519">订阅的记录经销商的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="3f656-520">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="3f656-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="3f656-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="3f656-522">显示执行交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="3f656-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="3f656-523">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="3f656-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="3f656-524">ProductId</span></span></td>
<td><p><span data-ttu-id="3f656-525">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="3f656-526">SkuId</span></span></td>
<td><p><span data-ttu-id="3f656-527">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="3f656-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="3f656-529">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-529">The ID for a particular Availability.</span></span> <span data-ttu-id="3f656-530">“可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</span><span class="sxs-lookup"><span data-stu-id="3f656-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-531">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="3f656-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="3f656-532">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="3f656-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="3f656-534">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="3f656-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="3f656-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="3f656-536">GUID 格式中的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="3f656-537">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="3f656-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="3f656-538">订阅说明</span><span class="sxs-lookup"><span data-stu-id="3f656-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="3f656-539">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="3f656-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="3f656-540">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="3f656-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-541">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="3f656-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="3f656-542">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f656-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="3f656-543">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="3f656-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="3f656-544">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="3f656-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="3f656-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="3f656-546">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="3f656-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="3f656-547">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="3f656-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="3f656-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="3f656-549">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="3f656-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="3f656-550">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="3f656-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-551">使用日期</span><span class="sxs-lookup"><span data-stu-id="3f656-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="3f656-552">服务使用情况的日期。</span><span class="sxs-lookup"><span data-stu-id="3f656-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-553">计量类型</span><span class="sxs-lookup"><span data-stu-id="3f656-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="3f656-554">测定仪的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-555">计量类别</span><span class="sxs-lookup"><span data-stu-id="3f656-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="3f656-556">用于使用情况的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="3f656-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-557">计量 Id</span><span class="sxs-lookup"><span data-stu-id="3f656-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="3f656-558">正在使用的计量 ID。</span><span class="sxs-lookup"><span data-stu-id="3f656-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-559">计量子类别</span><span class="sxs-lookup"><span data-stu-id="3f656-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="3f656-560">可以会影响费率的 Azure 服务的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-561">测定仪名称</span><span class="sxs-lookup"><span data-stu-id="3f656-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="3f656-562">已使用的测定仪的度量单位。</span><span class="sxs-lookup"><span data-stu-id="3f656-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-563">计量区域</span><span class="sxs-lookup"><span data-stu-id="3f656-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="3f656-564">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="3f656-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-565">单位</span><span class="sxs-lookup"><span data-stu-id="3f656-565">Unit</span></span></td>
<td><p><span data-ttu-id="3f656-566">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="3f656-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-567">已使用的数量</span><span class="sxs-lookup"><span data-stu-id="3f656-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="3f656-568">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="3f656-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="3f656-569">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="3f656-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-570">资源位置</span><span class="sxs-lookup"><span data-stu-id="3f656-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="3f656-571">测定仪正在其中运行数据中心。</span><span class="sxs-lookup"><span data-stu-id="3f656-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-572">使用的服务</span><span class="sxs-lookup"><span data-stu-id="3f656-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="3f656-573">使用 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="3f656-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="3f656-574">资源 URI</span><span class="sxs-lookup"><span data-stu-id="3f656-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="3f656-575">正在使用的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="3f656-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-576">费用类型</span><span class="sxs-lookup"><span data-stu-id="3f656-576">Charge type</span></span></td>
<td><p><span data-ttu-id="3f656-577">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-577">The type of charge or adjustment.</span></span> <span data-ttu-id="3f656-578">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="3f656-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-579">单价</span><span class="sxs-lookup"><span data-stu-id="3f656-579">Unit price</span></span></td>
<td><p><span data-ttu-id="3f656-580">每个许可证，因为在购买时在价目表中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="3f656-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="3f656-581">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-582">数量</span><span class="sxs-lookup"><span data-stu-id="3f656-582">Quantity</span></span></td>
<td><p><span data-ttu-id="3f656-583">许可证的数量。</span><span class="sxs-lookup"><span data-stu-id="3f656-583">Number of licenses.</span></span> <span data-ttu-id="3f656-584">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="3f656-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-585">单位类型</span><span class="sxs-lookup"><span data-stu-id="3f656-585">Unit type</span></span></td>
<td><p><span data-ttu-id="3f656-586">测定仪的计价中的单元的类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="3f656-587">当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="3f656-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-588">计费 pre 税</span><span class="sxs-lookup"><span data-stu-id="3f656-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="3f656-589">税前的总量。</span><span class="sxs-lookup"><span data-stu-id="3f656-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-590">计费货币</span><span class="sxs-lookup"><span data-stu-id="3f656-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="3f656-591">客户所在的地理区域中的币种</span><span class="sxs-lookup"><span data-stu-id="3f656-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-592">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="3f656-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="3f656-593">定价之前添加的税款。</span><span class="sxs-lookup"><span data-stu-id="3f656-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-594">定价货币</span><span class="sxs-lookup"><span data-stu-id="3f656-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="3f656-595">在价目表中货币。</span><span class="sxs-lookup"><span data-stu-id="3f656-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="3f656-596">服务信息 1</span><span class="sxs-lookup"><span data-stu-id="3f656-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="3f656-597">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="3f656-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-598">服务信息 2</span><span class="sxs-lookup"><span data-stu-id="3f656-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="3f656-599">旧字段，用于捕获可选的服务特定元数据的说明。</span><span class="sxs-lookup"><span data-stu-id="3f656-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="3f656-600">其他信息</span><span class="sxs-lookup"><span data-stu-id="3f656-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="3f656-601">其他列中未涉及的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="3f656-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="3f656-602">发票和对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="3f656-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="3f656-603">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="3f656-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="3f656-604">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="3f656-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="3f656-605">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="3f656-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="3f656-606">对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="3f656-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="3f656-607">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="3f656-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="3f656-608"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-609"><strong>对帐文件费用说明 （ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-610"><strong>什么是此费用？</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-611"><strong>如何将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="3f656-612"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-613">激活费用</span><span class="sxs-lookup"><span data-stu-id="3f656-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-614">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="3f656-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="3f656-615">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-616">取消费用</span><span class="sxs-lookup"><span data-stu-id="3f656-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-617">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-618">周期费用</span><span class="sxs-lookup"><span data-stu-id="3f656-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-619">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="3f656-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-620">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="3f656-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-621">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-622">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-623">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="3f656-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-624">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-625">订阅时使用年出单费用类型</span><span class="sxs-lookup"><span data-stu-id="3f656-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-626">购买费用</span><span class="sxs-lookup"><span data-stu-id="3f656-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-627">使用每月费用时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="3f656-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-628">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-629">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="3f656-630">续订费用</span><span class="sxs-lookup"><span data-stu-id="3f656-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-631">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="3f656-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-632">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-633">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="3f656-634"><strong>一次性费用</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="3f656-635">新增</span><span class="sxs-lookup"><span data-stu-id="3f656-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-636">创建新的购买时使用</span><span class="sxs-lookup"><span data-stu-id="3f656-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="3f656-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-638">增加后使用退款原始购买和新数量</span><span class="sxs-lookup"><span data-stu-id="3f656-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="3f656-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-640">后降低使用退款原始购买和新数量</span><span class="sxs-lookup"><span data-stu-id="3f656-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-641">Cancel</span><span class="sxs-lookup"><span data-stu-id="3f656-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-642">当取消订阅时，使用</span><span class="sxs-lookup"><span data-stu-id="3f656-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-643">转换</span><span class="sxs-lookup"><span data-stu-id="3f656-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-644">当升级许可证，但席位数保持不变时使用</span><span class="sxs-lookup"><span data-stu-id="3f656-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="3f656-645"><strong>使用费</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-646">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="3f656-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-647">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="3f656-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="3f656-648">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-649">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="3f656-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-650">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="3f656-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="3f656-651"><strong>信用额度</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-652">偏移行项</span><span class="sxs-lookup"><span data-stu-id="3f656-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-653">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="3f656-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-654">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="3f656-655">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="3f656-656"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-657">激活折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-658">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="3f656-659">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-660">周期折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-661">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-662">续订折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-663">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-664">取消折扣</span><span class="sxs-lookup"><span data-stu-id="3f656-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-665">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="3f656-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="3f656-666"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-667"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="3f656-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="3f656-668">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="3f656-669"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="3f656-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-670"><em>可能会应用于多个费用类型</em></span><span class="sxs-lookup"><span data-stu-id="3f656-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="3f656-671"><em>异常：&quot;行项的偏移量&quot;已包含的税款。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="3f656-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-672">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="3f656-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="3f656-673">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="3f656-674">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="3f656-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
