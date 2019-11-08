---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要详细了解计费周期中的每个费用，请从合作伙伴中心下载协调文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753859"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="ed166-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="ed166-103">Use the reconciliation files</span></span>

<span data-ttu-id="ed166-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="ed166-104">**Applies to**</span></span>

-  <span data-ttu-id="ed166-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="ed166-105">Partner Center</span></span>
-  <span data-ttu-id="ed166-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="ed166-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="ed166-107">**适当的角色**</span><span class="sxs-lookup"><span data-stu-id="ed166-107">**Appropriate roles**</span></span>

- <span data-ttu-id="ed166-108">帐单管理员</span><span class="sxs-lookup"><span data-stu-id="ed166-108">Billing admin</span></span>
- <span data-ttu-id="ed166-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ed166-109">Global admin</span></span>

<span data-ttu-id="ed166-110">若要详细了解计费周期中的每个费用，请从合作伙伴中心下载协调文件。</span><span class="sxs-lookup"><span data-stu-id="ed166-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="ed166-111">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="ed166-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="ed166-112">格式化问题</span><span class="sxs-lookup"><span data-stu-id="ed166-112">Formatting issues</span></span>

<span data-ttu-id="ed166-113">有时，侦测文件可能会出现格式问题。</span><span class="sxs-lookup"><span data-stu-id="ed166-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="ed166-114">（例如，如果不使用 EN-US 区域设置，则可能会发生这种情况。）请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="ed166-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="ed166-115">在 Excel 中打开 .csv 文件，然后选择第一列。</span><span class="sxs-lookup"><span data-stu-id="ed166-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="ed166-116">在功能区上，选择 "<strong>数据</strong>"，然后选择 "<strong>文本到列</strong>"。</span><span class="sxs-lookup"><span data-stu-id="ed166-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="ed166-117">在 "将文本转换为列" 向导中，选择 "<strong>分隔文件类型</strong>"，然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="ed166-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ed166-118">在分隔符字段中，选择 "<strong>逗号</strong>"。</span><span class="sxs-lookup"><span data-stu-id="ed166-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="ed166-119">如果已选择<strong>"选项卡</strong>"，则可以保留它。</span><span class="sxs-lookup"><span data-stu-id="ed166-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="ed166-120">选择<strong>下一步</strong> 。</span><span class="sxs-lookup"><span data-stu-id="ed166-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="ed166-121">在 "列数据格式" 字段中，选择<strong>Date： MDY</strong>，然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="ed166-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ed166-122">在 "列数据格式" 字段中，为 "所有数量" 列选择 "<strong>文本</strong>"，然后选择 "<strong>完成</strong>"。</span><span class="sxs-lookup"><span data-stu-id="ed166-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="ed166-123">下载大型侦测文件</span><span class="sxs-lookup"><span data-stu-id="ed166-123">Downloading a large recon file</span></span>

<span data-ttu-id="ed166-124">侦测文件可能会变得非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="ed166-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="ed166-125">有关用于帮助下载大型侦测文件的 PowerShell 脚本，请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="ed166-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="ed166-126">按合作伙伴列举</span><span class="sxs-lookup"><span data-stu-id="ed166-126">Itemize by partner</span></span>


<span data-ttu-id="ed166-127">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="ed166-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ed166-128">MPN ID</span><span class="sxs-lookup"><span data-stu-id="ed166-128">MPN ID</span></span></th>
<th><span data-ttu-id="ed166-129">描述</span><span class="sxs-lookup"><span data-stu-id="ed166-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ed166-130">MPN ID</span><span class="sxs-lookup"><span data-stu-id="ed166-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="ed166-131">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-132">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="ed166-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="ed166-133">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="ed166-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="ed166-134">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ed166-135">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="ed166-136">eTo 查看或更新经销商，从合作伙伴中心菜单中选择 "<strong>客户</strong>"，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="ed166-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="ed166-137">在“客户”菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="ed166-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="ed166-138">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="ed166-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="ed166-139">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="ed166-140">如果 CSP 合作伙伴的分销商没有 MPN ID，则此值将改为设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="ed166-141">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="ed166-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="ed166-142">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="ed166-142">License-based file fields</span></span>


<span data-ttu-id="ed166-143">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ed166-144"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ed166-145"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ed166-146"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ed166-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="ed166-148">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="ed166-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ed166-149">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="ed166-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ed166-150">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="ed166-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="ed166-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="ed166-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ed166-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="ed166-153">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="ed166-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ed166-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="ed166-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="ed166-155">OrderID</span></span></td>
<td><p><span data-ttu-id="ed166-156">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ed166-157">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ed166-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ed166-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ed166-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ed166-160">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ed166-161">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ed166-162">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="ed166-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="ed166-163">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="ed166-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="ed166-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ed166-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="ed166-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="ed166-166">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="ed166-167">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="ed166-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="ed166-168">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ed166-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="ed166-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="ed166-170">OfferID</span></span></td>
<td><p><span data-ttu-id="ed166-171">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-171">Unique offer ID.</span></span> <span data-ttu-id="ed166-172">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="ed166-173"><b>注意</b>：此值与价目表中的产品/服务 ID 不匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="ed166-174">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="ed166-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="ed166-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="ed166-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="ed166-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="ed166-177">唯一的持久型产品/服务 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="ed166-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="ed166-178"><b>注意</b>：此值与价目表中的产品/服务 ID 匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="ed166-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="ed166-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="ed166-180">OfferName</span></span></td>
<td><p><span data-ttu-id="ed166-181">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="ed166-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="ed166-182">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="ed166-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="ed166-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="ed166-184">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="ed166-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="ed166-185">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="ed166-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="ed166-186">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="ed166-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ed166-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ed166-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="ed166-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="ed166-189">订阅结束日期：12 个月 + 开始日期之后的 x 天（以便与合作伙伴帐单日期一致）或从续订日期算起的 12 个月。</span><span class="sxs-lookup"><span data-stu-id="ed166-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="ed166-190">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="ed166-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="ed166-191">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="ed166-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="ed166-192">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="ed166-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ed166-193">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ed166-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ed166-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ed166-195">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="ed166-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="ed166-196">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="ed166-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ed166-197">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="ed166-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ed166-198">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ed166-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ed166-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ed166-200">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="ed166-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="ed166-201">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="ed166-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ed166-202">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="ed166-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ed166-203">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="ed166-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ed166-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="ed166-205">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-205">The type of charge or adjustment.</span></span> <span data-ttu-id="ed166-206">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="ed166-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ed166-207">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="ed166-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ed166-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="ed166-209">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ed166-210">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ed166-211">6.82</span><span class="sxs-lookup"><span data-stu-id="ed166-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-212">数量</span><span class="sxs-lookup"><span data-stu-id="ed166-212">Quantity</span></span></td>
<td><p><span data-ttu-id="ed166-213">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="ed166-213">Number of seats.</span></span> <span data-ttu-id="ed166-214">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ed166-215">2</span><span class="sxs-lookup"><span data-stu-id="ed166-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-216">金额</span><span class="sxs-lookup"><span data-stu-id="ed166-216">Amount</span></span></td>
<td><p><span data-ttu-id="ed166-217">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="ed166-217">Total of price for quantity.</span></span> <span data-ttu-id="ed166-218">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="ed166-219">13.32</span><span class="sxs-lookup"><span data-stu-id="ed166-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="ed166-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="ed166-221">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="ed166-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="ed166-222">资格或地图随附的产品许可证或适用于激励的新订阅还将在此列中包含折扣金额。</span><span class="sxs-lookup"><span data-stu-id="ed166-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="ed166-223">2.32</span><span class="sxs-lookup"><span data-stu-id="ed166-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-224">小计</span><span class="sxs-lookup"><span data-stu-id="ed166-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="ed166-225">税前总额。</span><span class="sxs-lookup"><span data-stu-id="ed166-225">Total before tax.</span></span> <span data-ttu-id="ed166-226">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="ed166-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="ed166-227">11</span><span class="sxs-lookup"><span data-stu-id="ed166-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-228">税</span><span class="sxs-lookup"><span data-stu-id="ed166-228">Tax</span></span></td>
<td><p><span data-ttu-id="ed166-229">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="ed166-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ed166-230">0</span><span class="sxs-lookup"><span data-stu-id="ed166-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="ed166-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="ed166-232">税后总额。</span><span class="sxs-lookup"><span data-stu-id="ed166-232">Total after tax.</span></span> <span data-ttu-id="ed166-233">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="ed166-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="ed166-234">11</span><span class="sxs-lookup"><span data-stu-id="ed166-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-235">货币</span><span class="sxs-lookup"><span data-stu-id="ed166-235">Currency</span></span></td>
<td><p><span data-ttu-id="ed166-236">货币类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-236">Currency type.</span></span> <span data-ttu-id="ed166-237">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="ed166-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="ed166-238">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ed166-239">EUR</span><span class="sxs-lookup"><span data-stu-id="ed166-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ed166-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="ed166-241">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ed166-242">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ed166-243">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="ed166-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="ed166-244">MPNID</span></span></td>
<td><p><span data-ttu-id="ed166-245">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="ed166-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="ed166-246">4390934</span><span class="sxs-lookup"><span data-stu-id="ed166-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ed166-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ed166-248">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ed166-249">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="ed166-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ed166-250">4390934</span><span class="sxs-lookup"><span data-stu-id="ed166-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="ed166-251">DomainName</span></span></td>
<td><p><span data-ttu-id="ed166-252">客户&#39;的域名，用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="ed166-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ed166-253">这不应用于唯一地标识客户，因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="ed166-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ed166-254">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="ed166-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ed166-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ed166-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ed166-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ed166-257">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="ed166-257">Subscription nickname.</span></span> <span data-ttu-id="ed166-258">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="ed166-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="ed166-259">联机项目</span><span class="sxs-lookup"><span data-stu-id="ed166-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ed166-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ed166-261">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="ed166-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ed166-262">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="ed166-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="ed166-263">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="ed166-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="ed166-264">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="ed166-264">Usage-based file fields</span></span>


<span data-ttu-id="ed166-265">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="ed166-266">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="ed166-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ed166-267"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ed166-268"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ed166-269"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="ed166-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="ed166-271">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="ed166-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="ed166-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ed166-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ed166-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="ed166-274">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="ed166-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="ed166-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="ed166-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="ed166-277">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="ed166-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="ed166-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ed166-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="ed166-280">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ed166-281">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ed166-282">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="ed166-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="ed166-283">MPNID</span></span></td>
<td><p><span data-ttu-id="ed166-284">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="ed166-285">4390934</span><span class="sxs-lookup"><span data-stu-id="ed166-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ed166-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ed166-287">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ed166-288">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="ed166-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ed166-289">4390934</span><span class="sxs-lookup"><span data-stu-id="ed166-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ed166-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ed166-291">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="ed166-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="ed166-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="ed166-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ed166-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ed166-294">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="ed166-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ed166-295">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="ed166-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ed166-296">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ed166-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ed166-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ed166-298">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="ed166-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ed166-299">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="ed166-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ed166-300">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="ed166-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ed166-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ed166-302">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ed166-303">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ed166-304">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="ed166-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ed166-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ed166-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ed166-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ed166-307">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="ed166-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="ed166-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ed166-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ed166-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ed166-310">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="ed166-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="ed166-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ed166-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="ed166-312">OrderID</span></span></td>
<td><p><span data-ttu-id="ed166-313">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ed166-314">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ed166-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ed166-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="ed166-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="ed166-317">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="ed166-318">虚拟机</span><span class="sxs-lookup"><span data-stu-id="ed166-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="ed166-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="ed166-320">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ed166-321">Service Bus-个人或包</span><span class="sxs-lookup"><span data-stu-id="ed166-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="ed166-322">SQL Azure 数据库-企业版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="ed166-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="ed166-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="ed166-324">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="ed166-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ed166-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-326">资源名称</span><span class="sxs-lookup"><span data-stu-id="ed166-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="ed166-327">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ed166-328">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="ed166-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="ed166-329">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="ed166-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-330">Region</span><span class="sxs-lookup"><span data-stu-id="ed166-330">Region</span></span></td>
<td><p><span data-ttu-id="ed166-331">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="ed166-331">The region the usage applies to.</span></span> <span data-ttu-id="ed166-332">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="ed166-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="ed166-333">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="ed166-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-334">SKU</span><span class="sxs-lookup"><span data-stu-id="ed166-334">SKU</span></span></td>
<td><p><span data-ttu-id="ed166-335">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="ed166-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="ed166-336">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="ed166-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="ed166-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="ed166-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="ed166-338">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="ed166-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="ed166-339">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="ed166-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="ed166-340">1</span><span class="sxs-lookup"><span data-stu-id="ed166-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="ed166-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="ed166-342">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="ed166-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="ed166-343">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="ed166-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="ed166-344">11</span><span class="sxs-lookup"><span data-stu-id="ed166-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="ed166-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="ed166-346">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="ed166-346">Units included as part of the offer.</span></span> <span data-ttu-id="ed166-347">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="ed166-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="ed166-348">0</span><span class="sxs-lookup"><span data-stu-id="ed166-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="ed166-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="ed166-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="ed166-350">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="ed166-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="ed166-351">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="ed166-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="ed166-352">11</span><span class="sxs-lookup"><span data-stu-id="ed166-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="ed166-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="ed166-354">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="ed166-355">$0.0808</span><span class="sxs-lookup"><span data-stu-id="ed166-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="ed166-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="ed166-357">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="ed166-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ed166-358">$0.085</span><span class="sxs-lookup"><span data-stu-id="ed166-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="ed166-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="ed166-360">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="ed166-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ed166-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="ed166-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="ed166-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="ed166-363">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="ed166-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="ed166-364">$0.93</span><span class="sxs-lookup"><span data-stu-id="ed166-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-365">货币</span><span class="sxs-lookup"><span data-stu-id="ed166-365">Currency</span></span></td>
<td><p><span data-ttu-id="ed166-366">货币类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-366">Currency type.</span></span> <span data-ttu-id="ed166-367">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="ed166-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="ed166-368">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ed166-369">EUR</span><span class="sxs-lookup"><span data-stu-id="ed166-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ed166-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ed166-371">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-371">Pretax price per unit.</span></span> <span data-ttu-id="ed166-372">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="ed166-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ed166-373">$0.08</span><span class="sxs-lookup"><span data-stu-id="ed166-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ed166-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ed166-375">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-375">Post tax price per unit.</span></span> <span data-ttu-id="ed166-376">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="ed166-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ed166-377">$0.08</span><span class="sxs-lookup"><span data-stu-id="ed166-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ed166-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="ed166-379">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-379">The type of charge or adjustment.</span></span> <span data-ttu-id="ed166-380">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="ed166-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ed166-381">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="ed166-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="ed166-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="ed166-383">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="ed166-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="ed166-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="ed166-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="ed166-386">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="ed166-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="ed166-387">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ed166-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="ed166-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="ed166-389">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="ed166-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="ed166-390">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="ed166-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="ed166-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="ed166-392">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="ed166-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="ed166-393">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="ed166-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="ed166-394">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="ed166-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="ed166-395">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="ed166-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="ed166-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="ed166-397">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="ed166-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="ed166-398">外部</span><span class="sxs-lookup"><span data-stu-id="ed166-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-399">项目</span><span class="sxs-lookup"><span data-stu-id="ed166-399">Project</span></span></td>
<td><p><span data-ttu-id="ed166-400">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="ed166-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="ed166-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ed166-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="ed166-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="ed166-403">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="ed166-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="ed166-404">例如：如果你在30天的时间月内单独预配了连接，服务信息1将读取 "1.000000 连接/30 天"。</span><span class="sxs-lookup"><span data-stu-id="ed166-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="ed166-405">如果预配了 25 pack 连接，并且在该天内使用了1，则该日期的每日使用声明将指示 "25 个连接/30 天-使用时间： 1.000000"。</span><span class="sxs-lookup"><span data-stu-id="ed166-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ed166-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="ed166-407">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="ed166-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ed166-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ed166-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="ed166-409">DomainName</span></span></td>
<td><p><span data-ttu-id="ed166-410">客户&#39;的域名，用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="ed166-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ed166-411">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="ed166-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ed166-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ed166-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-413">单位</span><span class="sxs-lookup"><span data-stu-id="ed166-413">Unit</span></span></td>
<td><p><span data-ttu-id="ed166-414">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="ed166-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="ed166-415">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="ed166-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="ed166-416">一次性和定期文件字段</span><span class="sxs-lookup"><span data-stu-id="ed166-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ed166-417">列</span><span class="sxs-lookup"><span data-stu-id="ed166-417">Column</span></span></th>
<th><span data-ttu-id="ed166-418">描述</span><span class="sxs-lookup"><span data-stu-id="ed166-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="ed166-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ed166-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="ed166-420">特定计费实体的唯一 Microsoft Azure Active Directory 租户标识符，采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="ed166-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ed166-421">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="ed166-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ed166-422">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="ed166-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-423">客户 Id</span><span class="sxs-lookup"><span data-stu-id="ed166-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="ed166-424">用于标识客户的唯一 Microsoft Azure Active Directory 租户 ID，采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="ed166-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-425">客户名称</span><span class="sxs-lookup"><span data-stu-id="ed166-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="ed166-426">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ed166-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ed166-428">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="ed166-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="ed166-429">这不应用于唯一地标识客户，因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="ed166-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ed166-430">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="ed166-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-431">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="ed166-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="ed166-432">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="ed166-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-433">发票编号</span><span class="sxs-lookup"><span data-stu-id="ed166-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="ed166-434">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="ed166-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="ed166-435">MpnId</span></span></td>
<td><p><span data-ttu-id="ed166-436">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-437">经销商 MpnId</span><span class="sxs-lookup"><span data-stu-id="ed166-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="ed166-438">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-439">订单编码</span><span class="sxs-lookup"><span data-stu-id="ed166-439">Order ID</span></span></td>
<td><p><span data-ttu-id="ed166-440">Microsoft commerce 平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="ed166-441">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-442">订单日期</span><span class="sxs-lookup"><span data-stu-id="ed166-442">Order date</span></span></td>
<td><p><span data-ttu-id="ed166-443">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="ed166-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="ed166-444">ProductId</span></span></td>
<td><p><span data-ttu-id="ed166-445">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="ed166-446">SkuId</span></span></td>
<td><p><span data-ttu-id="ed166-447">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ed166-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ed166-449">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-449">The ID for a particular Availability.</span></span> <span data-ttu-id="ed166-450">"可用性" 指的是特定 SKU 是否可用于给定国家/地区、货币、行业段等。</span><span class="sxs-lookup"><span data-stu-id="ed166-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-451">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="ed166-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="ed166-452">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-453">产品名称</span><span class="sxs-lookup"><span data-stu-id="ed166-453">Product name</span></span></td>
<td><p><span data-ttu-id="ed166-454">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ed166-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="ed166-456">产品发布者的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ed166-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="ed166-458">此发布服务器的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-459">订阅说明</span><span class="sxs-lookup"><span data-stu-id="ed166-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ed166-460">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-461">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="ed166-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ed166-462">Microsoft commerce 平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="ed166-463">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ed166-464">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="ed166-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ed166-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ed166-466">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="ed166-466">Start day of the charges.</span></span> <span data-ttu-id="ed166-467">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="ed166-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ed166-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ed166-469">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="ed166-469">End day of the charges.</span></span> <span data-ttu-id="ed166-470">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="ed166-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-471">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="ed166-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="ed166-472">采购的术语长度和计费周期。</span><span class="sxs-lookup"><span data-stu-id="ed166-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="ed166-473">例如，"1 年，每月"。</span><span class="sxs-lookup"><span data-stu-id="ed166-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-474">费用类型</span><span class="sxs-lookup"><span data-stu-id="ed166-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="ed166-475">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-476">单价</span><span class="sxs-lookup"><span data-stu-id="ed166-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="ed166-477">购买时在 pricelist 中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ed166-478">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-479">有效单价</span><span class="sxs-lookup"><span data-stu-id="ed166-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="ed166-480">进行调整后的单位价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-481">数量</span><span class="sxs-lookup"><span data-stu-id="ed166-481">Quantity</span></span></td>
<td><p><span data-ttu-id="ed166-482">单位数。</span><span class="sxs-lookup"><span data-stu-id="ed166-482">Number of units.</span></span> <span data-ttu-id="ed166-483">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-484">单位类型</span><span class="sxs-lookup"><span data-stu-id="ed166-484">Unit type</span></span></td>
<td><p><span data-ttu-id="ed166-485">要购买的单位类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="ed166-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="ed166-487">适用于任何适用折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="ed166-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-488">Sub Total</span><span class="sxs-lookup"><span data-stu-id="ed166-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="ed166-489">税前总额。</span><span class="sxs-lookup"><span data-stu-id="ed166-489">Total before tax.</span></span> <span data-ttu-id="ed166-490">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="ed166-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-491">税金总计</span><span class="sxs-lookup"><span data-stu-id="ed166-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="ed166-492">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="ed166-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-493">总计</span><span class="sxs-lookup"><span data-stu-id="ed166-493">Total</span></span></td>
<td><p><span data-ttu-id="ed166-494">税后总额。</span><span class="sxs-lookup"><span data-stu-id="ed166-494">Total after tax.</span></span> <span data-ttu-id="ed166-495">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="ed166-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-496">货币</span><span class="sxs-lookup"><span data-stu-id="ed166-496">Currency</span></span></td>
<td><p><span data-ttu-id="ed166-497">货币类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-497">Currency type.</span></span> <span data-ttu-id="ed166-498">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="ed166-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="ed166-499">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="ed166-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="ed166-501">订单 ID 的备用标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="ed166-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="ed166-503">启用每月计费时显示每月。</span><span class="sxs-lookup"><span data-stu-id="ed166-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="ed166-504">否则为空白。</span><span class="sxs-lookup"><span data-stu-id="ed166-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="ed166-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="ed166-506">表示购买或消耗的总单位数。</span><span class="sxs-lookup"><span data-stu-id="ed166-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-507">pricingCurrency</span><span class="sxs-lookup"><span data-stu-id="ed166-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="ed166-508">列出资源或产品/服务的价格</span><span class="sxs-lookup"><span data-stu-id="ed166-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="ed166-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="ed166-510">定价货币应用于（客户）计费货币的汇率</span><span class="sxs-lookup"><span data-stu-id="ed166-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="ed166-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="ed166-512">确定向计费货币汇率的日期。</span><span class="sxs-lookup"><span data-stu-id="ed166-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="ed166-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="ed166-514">消耗行项的计量说明</span><span class="sxs-lookup"><span data-stu-id="ed166-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="ed166-515">每日分级使用文件字段</span><span class="sxs-lookup"><span data-stu-id="ed166-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ed166-516">列</span><span class="sxs-lookup"><span data-stu-id="ed166-516">Column</span></span></th>
<th><span data-ttu-id="ed166-517">描述</span><span class="sxs-lookup"><span data-stu-id="ed166-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="ed166-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ed166-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="ed166-519">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="ed166-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ed166-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="ed166-521">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="ed166-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="ed166-523">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="ed166-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="ed166-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="ed166-525">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ed166-526">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ed166-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ed166-528">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="ed166-528">The customer's domain name.</span></span> <span data-ttu-id="ed166-529">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="ed166-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-530">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="ed166-530">Customer country</span></span></td>
<td><p><span data-ttu-id="ed166-531">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="ed166-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="ed166-532">MPNID</span></span></td>
<td><p><span data-ttu-id="ed166-533">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-534">经销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="ed166-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="ed166-535">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ed166-536">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="ed166-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ed166-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ed166-538">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="ed166-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="ed166-539">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="ed166-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="ed166-540">ProductId</span></span></td>
<td><p><span data-ttu-id="ed166-541">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="ed166-542">SkuId</span></span></td>
<td><p><span data-ttu-id="ed166-543">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ed166-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ed166-545">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-545">The ID for a particular Availability.</span></span> <span data-ttu-id="ed166-546">"可用性" 指的是特定 SKU 是否可用于给定国家/地区、货币、行业段等。</span><span class="sxs-lookup"><span data-stu-id="ed166-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-547">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="ed166-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="ed166-548">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ed166-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="ed166-550">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ed166-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="ed166-552">GUID 格式的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="ed166-553">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="ed166-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-554">订阅说明</span><span class="sxs-lookup"><span data-stu-id="ed166-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ed166-555">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="ed166-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ed166-556">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="ed166-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-557">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="ed166-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ed166-558">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed166-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ed166-559">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed166-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ed166-560">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="ed166-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ed166-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ed166-562">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="ed166-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ed166-563">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="ed166-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ed166-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ed166-565">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="ed166-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ed166-566">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="ed166-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-567">使用日期</span><span class="sxs-lookup"><span data-stu-id="ed166-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="ed166-568">服务使用日期。</span><span class="sxs-lookup"><span data-stu-id="ed166-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-569">计量类型</span><span class="sxs-lookup"><span data-stu-id="ed166-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="ed166-570">计量器的类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-571">计量类别</span><span class="sxs-lookup"><span data-stu-id="ed166-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="ed166-572">使用的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="ed166-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-573">计量 Id</span><span class="sxs-lookup"><span data-stu-id="ed166-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="ed166-574">正在使用的计量的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed166-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-575">计量子类别</span><span class="sxs-lookup"><span data-stu-id="ed166-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="ed166-576">可能影响速度的 Azure 服务类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-577">计量名称</span><span class="sxs-lookup"><span data-stu-id="ed166-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="ed166-578">所使用的计量的度量单位。</span><span class="sxs-lookup"><span data-stu-id="ed166-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-579">计量区域</span><span class="sxs-lookup"><span data-stu-id="ed166-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="ed166-580">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="ed166-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-581">单位</span><span class="sxs-lookup"><span data-stu-id="ed166-581">Unit</span></span></td>
<td><p><span data-ttu-id="ed166-582">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="ed166-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-583">已消耗数量</span><span class="sxs-lookup"><span data-stu-id="ed166-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="ed166-584">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="ed166-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="ed166-585">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="ed166-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-586">资源位置</span><span class="sxs-lookup"><span data-stu-id="ed166-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="ed166-587">计量器正在其中运行的数据中心。</span><span class="sxs-lookup"><span data-stu-id="ed166-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-588">已使用服务</span><span class="sxs-lookup"><span data-stu-id="ed166-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="ed166-589">你使用的 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="ed166-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="ed166-590">资源 URI</span><span class="sxs-lookup"><span data-stu-id="ed166-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="ed166-591">所使用资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="ed166-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-592">费用类型</span><span class="sxs-lookup"><span data-stu-id="ed166-592">Charge type</span></span></td>
<td><p><span data-ttu-id="ed166-593">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-593">The type of charge or adjustment.</span></span> <span data-ttu-id="ed166-594">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="ed166-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-595">单价</span><span class="sxs-lookup"><span data-stu-id="ed166-595">Unit price</span></span></td>
<td><p><span data-ttu-id="ed166-596">购买时在 pricelist 中发布的每个许可证的价格。</span><span class="sxs-lookup"><span data-stu-id="ed166-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ed166-597">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-598">数量</span><span class="sxs-lookup"><span data-stu-id="ed166-598">Quantity</span></span></td>
<td><p><span data-ttu-id="ed166-599">许可证数量。</span><span class="sxs-lookup"><span data-stu-id="ed166-599">Number of licenses.</span></span> <span data-ttu-id="ed166-600">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="ed166-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-601">单位类型</span><span class="sxs-lookup"><span data-stu-id="ed166-601">Unit type</span></span></td>
<td><p><span data-ttu-id="ed166-602">计量计量器的单位类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="ed166-603">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="ed166-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-604">帐单税前税</span><span class="sxs-lookup"><span data-stu-id="ed166-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="ed166-605">税前的总金额。</span><span class="sxs-lookup"><span data-stu-id="ed166-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-606">计费货币</span><span class="sxs-lookup"><span data-stu-id="ed166-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="ed166-607">客户的地理区域中的货币</span><span class="sxs-lookup"><span data-stu-id="ed166-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-608">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="ed166-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="ed166-609">添加税款之前的定价。</span><span class="sxs-lookup"><span data-stu-id="ed166-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-610">定价货币</span><span class="sxs-lookup"><span data-stu-id="ed166-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="ed166-611">Pricelist 中的货币。</span><span class="sxs-lookup"><span data-stu-id="ed166-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-612">服务信息1</span><span class="sxs-lookup"><span data-stu-id="ed166-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="ed166-613">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="ed166-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ed166-614">服务信息2</span><span class="sxs-lookup"><span data-stu-id="ed166-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="ed166-615">捕获可选的服务特定元数据的旧字段。</span><span class="sxs-lookup"><span data-stu-id="ed166-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ed166-616">附加信息</span><span class="sxs-lookup"><span data-stu-id="ed166-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="ed166-617">其他列中未涵盖的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="ed166-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="ed166-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="ed166-619">按单位收费的实际值（包括折扣、挣贷款等）。</span><span class="sxs-lookup"><span data-stu-id="ed166-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="ed166-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="ed166-621">定价货币应用于（客户）计费货币的汇率。</span><span class="sxs-lookup"><span data-stu-id="ed166-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="ed166-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="ed166-623">确定定价货币与计费货币汇率的日期。</span><span class="sxs-lookup"><span data-stu-id="ed166-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ed166-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="ed166-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="ed166-625">表示 Azure subscriptionID。</span><span class="sxs-lookup"><span data-stu-id="ed166-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ed166-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="ed166-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="ed166-627">表示 Azure 订阅的名称。</span><span class="sxs-lookup"><span data-stu-id="ed166-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="ed166-628">发票与对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="ed166-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="ed166-629">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="ed166-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="ed166-630">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="ed166-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="ed166-631">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="ed166-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="ed166-632">按 "调整" 形式出现在发票上的一个信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="ed166-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="ed166-633">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="ed166-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="ed166-634"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-635"><strong>对帐文件费用说明（ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-636"><strong>此费用是什么？</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-637"><strong>如何实现将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="ed166-638"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-639">激活费用</span><span class="sxs-lookup"><span data-stu-id="ed166-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-640">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="ed166-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="ed166-641">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-642">取消费用</span><span class="sxs-lookup"><span data-stu-id="ed166-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-643">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-644">周期费用</span><span class="sxs-lookup"><span data-stu-id="ed166-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-645">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="ed166-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-646">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="ed166-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-647">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-648">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-649">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="ed166-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-650">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-651">使用年度计费时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="ed166-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-652">购买费用</span><span class="sxs-lookup"><span data-stu-id="ed166-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-653">使用月度帐单时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="ed166-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-654">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-655">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="ed166-656">续订费用</span><span class="sxs-lookup"><span data-stu-id="ed166-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-657">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="ed166-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-658">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-659">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="ed166-660"><strong>一次性费用</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="ed166-661">新</span><span class="sxs-lookup"><span data-stu-id="ed166-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-662">创建新购买时使用</span><span class="sxs-lookup"><span data-stu-id="ed166-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="ed166-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-664">用于原始购买的退款和增加后的新数量</span><span class="sxs-lookup"><span data-stu-id="ed166-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="ed166-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-666">用于原始购买的退款和减少后的新数量</span><span class="sxs-lookup"><span data-stu-id="ed166-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-667">“取消”</span><span class="sxs-lookup"><span data-stu-id="ed166-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-668">取消订阅时使用</span><span class="sxs-lookup"><span data-stu-id="ed166-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-669">转换</span><span class="sxs-lookup"><span data-stu-id="ed166-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-670">升级许可证时使用，但座位数保持不变</span><span class="sxs-lookup"><span data-stu-id="ed166-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="ed166-671"><strong>使用费用</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-672">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="ed166-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-673">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="ed166-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="ed166-674">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-675">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="ed166-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-676">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="ed166-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="ed166-677"><strong>制作</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-678">偏移行项</span><span class="sxs-lookup"><span data-stu-id="ed166-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-679">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="ed166-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-680">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="ed166-681">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="ed166-682"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-683">激活折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-684">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="ed166-685">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-686">周期折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-687">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-688">续订折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-689">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-690">取消折扣</span><span class="sxs-lookup"><span data-stu-id="ed166-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-691">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="ed166-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="ed166-692"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-693"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="ed166-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="ed166-694">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ed166-695"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="ed166-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-696"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="ed166-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="ed166-697"><em>异常：行项 &quot;Offset &quot; 已包含税金。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="ed166-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-698">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="ed166-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="ed166-699">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="ed166-700">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="ed166-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
