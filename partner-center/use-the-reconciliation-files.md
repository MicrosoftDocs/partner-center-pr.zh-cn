---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 07/08/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要详细了解计费周期中的每个费用，请从合作伙伴中心下载协调文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 7b27e99e5c0dc55fad3b06cc22316e8282dbe35c
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653977"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="5d90d-103">使用对帐文件</span><span class="sxs-lookup"><span data-stu-id="5d90d-103">Use the reconciliation files</span></span>

<span data-ttu-id="5d90d-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="5d90d-104">**Applies to**</span></span>

-  <span data-ttu-id="5d90d-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="5d90d-105">Partner Center</span></span>
-  <span data-ttu-id="5d90d-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="5d90d-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="5d90d-107">若要详细了解计费周期中的每个费用，请从合作伙伴中心下载协调文件。</span><span class="sxs-lookup"><span data-stu-id="5d90d-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="5d90d-108">详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="5d90d-109">格式化问题</span><span class="sxs-lookup"><span data-stu-id="5d90d-109">Formatting issues</span></span>

<span data-ttu-id="5d90d-110">有时，侦测文件可能会出现格式问题。</span><span class="sxs-lookup"><span data-stu-id="5d90d-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="5d90d-111">（例如，如果不使用 EN-US 区域设置，则可能会发生这种情况。）请按照以下步骤来解决这些问题。</span><span class="sxs-lookup"><span data-stu-id="5d90d-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="5d90d-112">在 Excel 中打开 .csv 文件，然后选择第一列。</span><span class="sxs-lookup"><span data-stu-id="5d90d-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="5d90d-113">在功能区上，选择 "<strong>数据</strong>"，然后选择 "<strong>文本到列</strong>"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="5d90d-114">在 "将文本转换为列" 向导中，选择 "<strong>分隔文件类型</strong>"，然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="5d90d-115">在分隔符字段中，选择 "<strong>逗号</strong>"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="5d90d-116">如果已选择<strong>"选项卡</strong>"，则可以保留它。</span><span class="sxs-lookup"><span data-stu-id="5d90d-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="5d90d-117">选择<strong>下一步</strong> 。</span><span class="sxs-lookup"><span data-stu-id="5d90d-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="5d90d-118">在 "列数据格式" 字段中，选择<strong>Date： MDY</strong>，然后选择 "<strong>下一步</strong>"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="5d90d-119">在 "列数据格式" 字段中，为 "所有数量" 列选择 "<strong>文本</strong>"，然后选择 "<strong>完成</strong>"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="5d90d-120">下载大型侦测文件</span><span class="sxs-lookup"><span data-stu-id="5d90d-120">Downloading a large recon file</span></span>

<span data-ttu-id="5d90d-121">侦测文件可能会变得非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="5d90d-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="5d90d-122">有关用于帮助下载大型侦测文件的 PowerShell 脚本，请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="5d90d-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="5d90d-123">按合作伙伴列举</span><span class="sxs-lookup"><span data-stu-id="5d90d-123">Itemize by partner</span></span>


<span data-ttu-id="5d90d-124">间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。</span><span class="sxs-lookup"><span data-stu-id="5d90d-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="5d90d-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="5d90d-125">MPN ID</span></span></th>
<th><span data-ttu-id="5d90d-126">描述</span><span class="sxs-lookup"><span data-stu-id="5d90d-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="5d90d-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="5d90d-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="5d90d-128">CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-129">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="5d90d-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="5d90d-130">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="5d90d-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="5d90d-131">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5d90d-132">这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="5d90d-133">eTo 查看或更新经销商，从合作伙伴中心菜单中选择 "<strong>客户</strong>"，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="5d90d-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="5d90d-134">在“客户”菜单中，选择“订阅”，然后从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="5d90d-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="5d90d-135">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="5d90d-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="5d90d-136">如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="5d90d-137">如果 CSP 合作伙伴的分销商没有 MPN ID，则此值将改为设置为合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="5d90d-138">如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</span><span class="sxs-lookup"><span data-stu-id="5d90d-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="5d90d-139">基于许可证的文件字段</span><span class="sxs-lookup"><span data-stu-id="5d90d-139">License-based file fields</span></span>


<span data-ttu-id="5d90d-140">若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="5d90d-141"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="5d90d-142"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="5d90d-143"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="5d90d-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="5d90d-145">特定计费单位的唯一标识符（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="5d90d-146">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="5d90d-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="5d90d-147">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="5d90d-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="5d90d-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="5d90d-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="5d90d-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="5d90d-150">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="5d90d-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="5d90d-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="5d90d-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="5d90d-152">OrderID</span></span></td>
<td><p><span data-ttu-id="5d90d-153">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="5d90d-154">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="5d90d-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="5d90d-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="5d90d-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="5d90d-157">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="5d90d-158">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="5d90d-159">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="5d90d-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="5d90d-160">请参阅 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="5d90d-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="5d90d-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="5d90d-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="5d90d-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="5d90d-163">订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="5d90d-164">客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</span><span class="sxs-lookup"><span data-stu-id="5d90d-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="5d90d-165">此字段将映射到合作伙伴管理员控制台中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="5d90d-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="5d90d-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="5d90d-167">OfferID</span></span></td>
<td><p><span data-ttu-id="5d90d-168">唯一的产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-168">Unique offer ID.</span></span> <span data-ttu-id="5d90d-169">根据价目表的标准产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="5d90d-170"><b>注意</b>：此值与价目表中的产品/服务 ID 不匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="5d90d-171">请参阅下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="5d90d-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="5d90d-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="5d90d-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="5d90d-174">唯一的持久型产品/服务 ID，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="5d90d-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="5d90d-175"><b>注意</b>：此值与价目表中的产品/服务 ID 匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="5d90d-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="5d90d-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="5d90d-177">OfferName</span></span></td>
<td><p><span data-ttu-id="5d90d-178">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="5d90d-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="5d90d-179">Microsoft Office 365（计划 E3）</span><span class="sxs-lookup"><span data-stu-id="5d90d-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="5d90d-181">订阅开始日期，设置为提交订单后的第二天。</span><span class="sxs-lookup"><span data-stu-id="5d90d-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="5d90d-182">通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</span><span class="sxs-lookup"><span data-stu-id="5d90d-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="5d90d-183">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="5d90d-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5d90d-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="5d90d-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="5d90d-186">订阅结束日期：12 个月 + 开始日期之后的 x 天（以便与合作伙伴帐单日期一致）或从续订日期算起的 12 个月。</span><span class="sxs-lookup"><span data-stu-id="5d90d-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="5d90d-187">续订时，价格将更新为当前价目表。</span><span class="sxs-lookup"><span data-stu-id="5d90d-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="5d90d-188">自动续订之前可能需要与客户进行通信。</span><span class="sxs-lookup"><span data-stu-id="5d90d-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="5d90d-189">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="5d90d-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5d90d-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="5d90d-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="5d90d-192">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="5d90d-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="5d90d-193">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="5d90d-194">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="5d90d-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5d90d-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="5d90d-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="5d90d-197">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="5d90d-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="5d90d-198">当客户更改座位数量时，此数字用于计算每日（按比例）费用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="5d90d-199">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="5d90d-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="5d90d-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="5d90d-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="5d90d-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="5d90d-202">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-202">The type of charge or adjustment.</span></span> <span data-ttu-id="5d90d-203">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="5d90d-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="5d90d-204">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="5d90d-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="5d90d-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="5d90d-206">购买时公布在价目表中的每一席位的价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="5d90d-207">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="5d90d-208">6.82</span><span class="sxs-lookup"><span data-stu-id="5d90d-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-209">数量</span><span class="sxs-lookup"><span data-stu-id="5d90d-209">Quantity</span></span></td>
<td><p><span data-ttu-id="5d90d-210">席位的数量。</span><span class="sxs-lookup"><span data-stu-id="5d90d-210">Number of seats.</span></span> <span data-ttu-id="5d90d-211">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="5d90d-212">2</span><span class="sxs-lookup"><span data-stu-id="5d90d-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-213">金额</span><span class="sxs-lookup"><span data-stu-id="5d90d-213">Amount</span></span></td>
<td><p><span data-ttu-id="5d90d-214">数量的总价。</span><span class="sxs-lookup"><span data-stu-id="5d90d-214">Total of price for quantity.</span></span> <span data-ttu-id="5d90d-215">在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="5d90d-216">13.32</span><span class="sxs-lookup"><span data-stu-id="5d90d-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="5d90d-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="5d90d-218">适用于这些费用的折扣金额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="5d90d-219">资格或地图随附的产品许可证或适用于激励的新订阅还将在此列中包含折扣金额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="5d90d-220">2.32</span><span class="sxs-lookup"><span data-stu-id="5d90d-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-221">小计</span><span class="sxs-lookup"><span data-stu-id="5d90d-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="5d90d-222">税前总额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-222">Total before tax.</span></span> <span data-ttu-id="5d90d-223">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="5d90d-224">11</span><span class="sxs-lookup"><span data-stu-id="5d90d-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-225">税</span><span class="sxs-lookup"><span data-stu-id="5d90d-225">Tax</span></span></td>
<td><p><span data-ttu-id="5d90d-226">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="5d90d-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="5d90d-227">0</span><span class="sxs-lookup"><span data-stu-id="5d90d-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="5d90d-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="5d90d-229">税后总额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-229">Total after tax.</span></span> <span data-ttu-id="5d90d-230">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="5d90d-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="5d90d-231">11</span><span class="sxs-lookup"><span data-stu-id="5d90d-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-232">货币</span><span class="sxs-lookup"><span data-stu-id="5d90d-232">Currency</span></span></td>
<td><p><span data-ttu-id="5d90d-233">货币类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-233">Currency type.</span></span> <span data-ttu-id="5d90d-234">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="5d90d-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="5d90d-235">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="5d90d-236">EUR</span><span class="sxs-lookup"><span data-stu-id="5d90d-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="5d90d-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="5d90d-238">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="5d90d-239">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="5d90d-240">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="5d90d-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="5d90d-241">MPNID</span></span></td>
<td><p><span data-ttu-id="5d90d-242">云解决方案提供商合作伙伴的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="5d90d-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="5d90d-243">4390934</span><span class="sxs-lookup"><span data-stu-id="5d90d-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="5d90d-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="5d90d-245">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5d90d-246">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="5d90d-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="5d90d-247">4390934</span><span class="sxs-lookup"><span data-stu-id="5d90d-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="5d90d-248">DomainName</span></span></td>
<td><p><span data-ttu-id="5d90d-249">客户&#39;的域名，用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="5d90d-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="5d90d-250">这不应用于唯一地标识客户，因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="5d90d-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="5d90d-251">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="5d90d-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="5d90d-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5d90d-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="5d90d-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="5d90d-254">订阅昵称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-254">Subscription nickname.</span></span> <span data-ttu-id="5d90d-255">如果未指定昵称，合作伙伴中心将使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="5d90d-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="5d90d-256">联机项目</span><span class="sxs-lookup"><span data-stu-id="5d90d-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="5d90d-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="5d90d-258">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="5d90d-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="5d90d-259">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="5d90d-260">不带项目客户端的高级联机项目</span><span class="sxs-lookup"><span data-stu-id="5d90d-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="5d90d-261">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="5d90d-261">Usage-based file fields</span></span>


<span data-ttu-id="5d90d-262">若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="5d90d-263">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="5d90d-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="5d90d-264"><strong>该列</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="5d90d-265"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="5d90d-266"><strong>示例值</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="5d90d-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="5d90d-268">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="5d90d-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="5d90d-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="5d90d-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="5d90d-271">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="5d90d-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="5d90d-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="5d90d-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="5d90d-274">合作伙伴帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="5d90d-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="5d90d-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="5d90d-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="5d90d-277">合作伙伴&#39;中心报告的客户组织名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="5d90d-278">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="5d90d-279">测试客户 A</span><span class="sxs-lookup"><span data-stu-id="5d90d-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="5d90d-280">MPNID</span></span></td>
<td><p><span data-ttu-id="5d90d-281">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="5d90d-282">4390934</span><span class="sxs-lookup"><span data-stu-id="5d90d-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="5d90d-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="5d90d-284">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5d90d-285">请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</span><span class="sxs-lookup"><span data-stu-id="5d90d-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="5d90d-286">4390934</span><span class="sxs-lookup"><span data-stu-id="5d90d-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="5d90d-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="5d90d-288">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="5d90d-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="5d90d-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="5d90d-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="5d90d-291">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="5d90d-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="5d90d-292">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="5d90d-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5d90d-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="5d90d-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="5d90d-295">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="5d90d-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="5d90d-296">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="5d90d-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="5d90d-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="5d90d-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="5d90d-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="5d90d-299">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="5d90d-300">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="5d90d-301">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="5d90d-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="5d90d-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="5d90d-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="5d90d-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="5d90d-304">服务产品的昵称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="5d90d-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="5d90d-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="5d90d-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="5d90d-307">服务产品的业务线</span><span class="sxs-lookup"><span data-stu-id="5d90d-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="5d90d-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="5d90d-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="5d90d-309">OrderID</span></span></td>
<td><p><span data-ttu-id="5d90d-310">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="5d90d-311">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="5d90d-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="5d90d-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="5d90d-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="5d90d-314">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="5d90d-315">虚拟机</span><span class="sxs-lookup"><span data-stu-id="5d90d-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="5d90d-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="5d90d-317">Windows Azure 服务的特定类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="5d90d-318">Service Bus-个人或包</span><span class="sxs-lookup"><span data-stu-id="5d90d-318">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="5d90d-319">SQL Azure 数据库-企业版或 Web 版</span><span class="sxs-lookup"><span data-stu-id="5d90d-319">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="5d90d-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="5d90d-321">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="5d90d-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="5d90d-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-323">资源名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="5d90d-324">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="5d90d-325">数据传输入 (GB)</span><span class="sxs-lookup"><span data-stu-id="5d90d-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="5d90d-326">数据传输出 (GB)</span><span class="sxs-lookup"><span data-stu-id="5d90d-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-327">Region</span><span class="sxs-lookup"><span data-stu-id="5d90d-327">Region</span></span></td>
<td><p><span data-ttu-id="5d90d-328">使用情况适用的区域。</span><span class="sxs-lookup"><span data-stu-id="5d90d-328">The region the usage applies to.</span></span> <span data-ttu-id="5d90d-329">主要用于分配数据传输的速率，速率因地区而异。</span><span class="sxs-lookup"><span data-stu-id="5d90d-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="5d90d-330">亚太、欧洲、拉丁美洲、北美</span><span class="sxs-lookup"><span data-stu-id="5d90d-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-331">SKU</span><span class="sxs-lookup"><span data-stu-id="5d90d-331">SKU</span></span></td>
<td><p><span data-ttu-id="5d90d-332">产品/服务的 MSFT 唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5d90d-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="5d90d-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="5d90d-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="5d90d-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="5d90d-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="5d90d-335">用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。</span><span class="sxs-lookup"><span data-stu-id="5d90d-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="5d90d-336">对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</span><span class="sxs-lookup"><span data-stu-id="5d90d-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="5d90d-337">1</span><span class="sxs-lookup"><span data-stu-id="5d90d-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="5d90d-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="5d90d-339">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="5d90d-340">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="5d90d-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="5d90d-341">11</span><span class="sxs-lookup"><span data-stu-id="5d90d-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="5d90d-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="5d90d-343">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="5d90d-343">Units included as part of the offer.</span></span> <span data-ttu-id="5d90d-344">通常不显示在云解决方案提供商中。</span><span class="sxs-lookup"><span data-stu-id="5d90d-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="5d90d-345">0</span><span class="sxs-lookup"><span data-stu-id="5d90d-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5d90d-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="5d90d-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="5d90d-347">不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="5d90d-348">等于 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="5d90d-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="5d90d-349">11</span><span class="sxs-lookup"><span data-stu-id="5d90d-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="5d90d-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="5d90d-351">订阅开始日期的有效产品/服务价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="5d90d-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="5d90d-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="5d90d-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="5d90d-354">ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="5d90d-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="5d90d-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="5d90d-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="5d90d-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="5d90d-357">根据你的市场&#39;税率规则和特定情况收费。</span><span class="sxs-lookup"><span data-stu-id="5d90d-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="5d90d-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="5d90d-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="5d90d-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="5d90d-360">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="5d90d-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="5d90d-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-362">货币</span><span class="sxs-lookup"><span data-stu-id="5d90d-362">Currency</span></span></td>
<td><p><span data-ttu-id="5d90d-363">货币类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-363">Currency type.</span></span> <span data-ttu-id="5d90d-364">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="5d90d-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="5d90d-365">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="5d90d-366">EUR</span><span class="sxs-lookup"><span data-stu-id="5d90d-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="5d90d-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="5d90d-368">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-368">Pretax price per unit.</span></span> <span data-ttu-id="5d90d-369">等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="5d90d-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="5d90d-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="5d90d-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="5d90d-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="5d90d-372">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-372">Post tax price per unit.</span></span> <span data-ttu-id="5d90d-373">等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</span><span class="sxs-lookup"><span data-stu-id="5d90d-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="5d90d-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="5d90d-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="5d90d-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="5d90d-376">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-376">The type of charge or adjustment.</span></span> <span data-ttu-id="5d90d-377">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="5d90d-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="5d90d-378">请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</span><span class="sxs-lookup"><span data-stu-id="5d90d-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="5d90d-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="5d90d-380">MSFT 帐单平台中的唯一帐户 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="5d90d-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="5d90d-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="5d90d-383">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="5d90d-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="5d90d-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="5d90d-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="5d90d-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="5d90d-386">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="5d90d-387">东亚、东南亚、北欧、西欧、美国中北部、美国中南部</span><span class="sxs-lookup"><span data-stu-id="5d90d-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="5d90d-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="5d90d-389">此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="5d90d-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="5d90d-390">例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。</span><span class="sxs-lookup"><span data-stu-id="5d90d-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="5d90d-391">此 MeteredService 列将指示使用情况适用的特定服务。</span><span class="sxs-lookup"><span data-stu-id="5d90d-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="5d90d-392">访问控制、CDN、计算、数据库、服务总线、存储</span><span class="sxs-lookup"><span data-stu-id="5d90d-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="5d90d-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="5d90d-394">进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</span><span class="sxs-lookup"><span data-stu-id="5d90d-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="5d90d-395">外部</span><span class="sxs-lookup"><span data-stu-id="5d90d-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-396">项目</span><span class="sxs-lookup"><span data-stu-id="5d90d-396">Project</span></span></td>
<td><p><span data-ttu-id="5d90d-397">客户定义的用于其服务实例的名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="5d90d-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="5d90d-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="5d90d-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="5d90d-400">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="5d90d-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="5d90d-401">例如：如果你在30天的时间月内单独预配了连接，服务信息1将读取 "1.000000 连接/30 天"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="5d90d-402">如果预配了 25 pack 连接，并且在该天内使用了1，则该日期的每日使用声明将指示 "25 个连接/30 天-使用时间： 1.000000"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="5d90d-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="5d90d-404">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="5d90d-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="5d90d-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="5d90d-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5d90d-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="5d90d-406">DomainName</span></span></td>
<td><p><span data-ttu-id="5d90d-407">客户&#39;的域名，用于帮助确定客户身份。</span><span class="sxs-lookup"><span data-stu-id="5d90d-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="5d90d-408">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="5d90d-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="5d90d-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5d90d-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="5d90d-410">单位</span><span class="sxs-lookup"><span data-stu-id="5d90d-410">Unit</span></span></td>
<td><p><span data-ttu-id="5d90d-411">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="5d90d-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="5d90d-412">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="5d90d-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="5d90d-413">一次性和定期文件字段</span><span class="sxs-lookup"><span data-stu-id="5d90d-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="5d90d-414">列</span><span class="sxs-lookup"><span data-stu-id="5d90d-414">Column</span></span></th>
<th><span data-ttu-id="5d90d-415">描述</span><span class="sxs-lookup"><span data-stu-id="5d90d-415">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="5d90d-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="5d90d-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="5d90d-417">特定计费实体的唯一 Microsoft Azure Active Directory 租户标识符，采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="5d90d-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="5d90d-418">对帐不需要，但可能是有用的信息。</span><span class="sxs-lookup"><span data-stu-id="5d90d-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="5d90d-419">在所有行中均相同。</span><span class="sxs-lookup"><span data-stu-id="5d90d-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-420">客户 Id</span><span class="sxs-lookup"><span data-stu-id="5d90d-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="5d90d-421">用于标识客户的唯一 Microsoft Azure Active Directory 租户 ID，采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="5d90d-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-422">客户名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="5d90d-423">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="5d90d-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="5d90d-425">客户的域名，用于帮助识别客户。</span><span class="sxs-lookup"><span data-stu-id="5d90d-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="5d90d-426">这不应用于唯一地标识客户，因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。</span><span class="sxs-lookup"><span data-stu-id="5d90d-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="5d90d-427">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="5d90d-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-428">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="5d90d-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="5d90d-429">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="5d90d-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-430">发票编号</span><span class="sxs-lookup"><span data-stu-id="5d90d-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="5d90d-431">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="5d90d-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="5d90d-432">MpnId</span></span></td>
<td><p><span data-ttu-id="5d90d-433">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-434">经销商 MpnId</span><span class="sxs-lookup"><span data-stu-id="5d90d-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="5d90d-435">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-436">订单编码</span><span class="sxs-lookup"><span data-stu-id="5d90d-436">Order ID</span></span></td>
<td><p><span data-ttu-id="5d90d-437">Microsoft commerce 平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="5d90d-438">当联系支持人员而不用于对帐时，可能对识别订单非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-439">订单日期</span><span class="sxs-lookup"><span data-stu-id="5d90d-439">Order date</span></span></td>
<td><p><span data-ttu-id="5d90d-440">下达订单的日期。</span><span class="sxs-lookup"><span data-stu-id="5d90d-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="5d90d-441">ProductId</span></span></td>
<td><p><span data-ttu-id="5d90d-442">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="5d90d-443">SkuId</span></span></td>
<td><p><span data-ttu-id="5d90d-444">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="5d90d-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="5d90d-446">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-446">The ID for a particular Availability.</span></span> <span data-ttu-id="5d90d-447">"可用性" 指的是特定 SKU 是否可用于给定国家/地区、货币、行业段等。</span><span class="sxs-lookup"><span data-stu-id="5d90d-447">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-448">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="5d90d-449">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-450">产品名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-450">Product name</span></span></td>
<td><p><span data-ttu-id="5d90d-451">产品的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="5d90d-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="5d90d-453">产品发布者的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-453">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="5d90d-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="5d90d-455">此发布服务器的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-456">订阅说明</span><span class="sxs-lookup"><span data-stu-id="5d90d-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="5d90d-457">订阅的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-458">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="5d90d-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="5d90d-459">Microsoft commerce 平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="5d90d-460">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="5d90d-461">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="5d90d-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="5d90d-463">费用的开始日。</span><span class="sxs-lookup"><span data-stu-id="5d90d-463">Start day of the charges.</span></span> <span data-ttu-id="5d90d-464">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="5d90d-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="5d90d-466">费用的结束日。</span><span class="sxs-lookup"><span data-stu-id="5d90d-466">End day of the charges.</span></span> <span data-ttu-id="5d90d-467">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="5d90d-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-468">术语和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="5d90d-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="5d90d-469">采购的术语长度和计费周期。</span><span class="sxs-lookup"><span data-stu-id="5d90d-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="5d90d-470">例如，"1 年，每月"。</span><span class="sxs-lookup"><span data-stu-id="5d90d-470">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-471">费用类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="5d90d-472">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-473">单价</span><span class="sxs-lookup"><span data-stu-id="5d90d-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="5d90d-474">购买时在 pricelist 中发布的价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="5d90d-475">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-476">有效单价</span><span class="sxs-lookup"><span data-stu-id="5d90d-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="5d90d-477">进行调整后的单位价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-478">数量</span><span class="sxs-lookup"><span data-stu-id="5d90d-478">Quantity</span></span></td>
<td><p><span data-ttu-id="5d90d-479">单位数。</span><span class="sxs-lookup"><span data-stu-id="5d90d-479">Number of units.</span></span> <span data-ttu-id="5d90d-480">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-481">单位类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-481">Unit type</span></span></td>
<td><p><span data-ttu-id="5d90d-482">要购买的单位类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="5d90d-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="5d90d-484">适用于任何适用折扣的说明。</span><span class="sxs-lookup"><span data-stu-id="5d90d-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-485">Sub Total</span><span class="sxs-lookup"><span data-stu-id="5d90d-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="5d90d-486">税前总额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-486">Total before tax.</span></span> <span data-ttu-id="5d90d-487">如果有折扣，请检查你的小计是否匹配你的预期总额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-488">税金总计</span><span class="sxs-lookup"><span data-stu-id="5d90d-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="5d90d-489">税务金额费用，基于你的市场税务规则和特定情况。</span><span class="sxs-lookup"><span data-stu-id="5d90d-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-490">总计</span><span class="sxs-lookup"><span data-stu-id="5d90d-490">Total</span></span></td>
<td><p><span data-ttu-id="5d90d-491">税后总额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-491">Total after tax.</span></span> <span data-ttu-id="5d90d-492">检查你是否在发票中计入了税务。</span><span class="sxs-lookup"><span data-stu-id="5d90d-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-493">货币</span><span class="sxs-lookup"><span data-stu-id="5d90d-493">Currency</span></span></td>
<td><p><span data-ttu-id="5d90d-494">货币类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-494">Currency type.</span></span> <span data-ttu-id="5d90d-495">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="5d90d-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="5d90d-496">检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="5d90d-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="5d90d-498">订单 ID 的备用标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-499">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="5d90d-499">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="5d90d-500">启用每月计费时显示每月。</span><span class="sxs-lookup"><span data-stu-id="5d90d-500">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="5d90d-501">否则为空白。</span><span class="sxs-lookup"><span data-stu-id="5d90d-501">Otherwise blank.</span></span> </p></td>
</tr>

</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="5d90d-502">每日分级使用文件字段</span><span class="sxs-lookup"><span data-stu-id="5d90d-502">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="5d90d-503">列</span><span class="sxs-lookup"><span data-stu-id="5d90d-503">Column</span></span></th>
<th><span data-ttu-id="5d90d-504">描述</span><span class="sxs-lookup"><span data-stu-id="5d90d-504">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="5d90d-505">PartnerId</span><span class="sxs-lookup"><span data-stu-id="5d90d-505">PartnerId</span></span></td>
<td><p><span data-ttu-id="5d90d-506">合作伙伴 ID（采用 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-506">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-507">PartnerName</span><span class="sxs-lookup"><span data-stu-id="5d90d-507">PartnerName</span></span></td>
<td><p><span data-ttu-id="5d90d-508">合作伙伴名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-508">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-509">CustomerId</span><span class="sxs-lookup"><span data-stu-id="5d90d-509">CustomerId</span></span></td>
<td><p><span data-ttu-id="5d90d-510">唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</span><span class="sxs-lookup"><span data-stu-id="5d90d-510">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-511">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="5d90d-511">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="5d90d-512">在合作伙伴中心中报告的客户的组织名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-512">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="5d90d-513">这在使用系统信息对发票进行对帐时非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-513">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-514">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="5d90d-514">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="5d90d-515">客户的域名。</span><span class="sxs-lookup"><span data-stu-id="5d90d-515">The customer's domain name.</span></span> <span data-ttu-id="5d90d-516">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-516">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-517">客户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="5d90d-517">Customer country</span></span></td>
<td><p><span data-ttu-id="5d90d-518">客户所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="5d90d-518">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-519">MPNID</span><span class="sxs-lookup"><span data-stu-id="5d90d-519">MPNID</span></span></td>
<td><p><span data-ttu-id="5d90d-520">云解决方案提供商合作伙伴的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-520">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-521">经销商 MPNID</span><span class="sxs-lookup"><span data-stu-id="5d90d-521">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="5d90d-522">订阅记录的经销商 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-522">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5d90d-523">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-524">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="5d90d-524">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="5d90d-525">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="5d90d-525">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="5d90d-526">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-526">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-527">ProductId</span><span class="sxs-lookup"><span data-stu-id="5d90d-527">ProductId</span></span></td>
<td><p><span data-ttu-id="5d90d-528">产品的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-528">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-529">SkuId</span><span class="sxs-lookup"><span data-stu-id="5d90d-529">SkuId</span></span></td>
<td><p><span data-ttu-id="5d90d-530">特定 SKU 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-530">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-531">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="5d90d-531">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="5d90d-532">特定可用性的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-532">The ID for a particular Availability.</span></span> <span data-ttu-id="5d90d-533">"可用性" 指的是特定 SKU 是否可用于给定国家/地区、货币、行业段等。</span><span class="sxs-lookup"><span data-stu-id="5d90d-533">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-534">SKU 名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-534">SKU Name</span></span></td>
<td><p><span data-ttu-id="5d90d-535">特定 SKU 的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-535">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-536">PublisherName</span><span class="sxs-lookup"><span data-stu-id="5d90d-536">PublisherName</span></span></td>
<td><p><span data-ttu-id="5d90d-537">发布服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="5d90d-537">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-538">PublisherID</span><span class="sxs-lookup"><span data-stu-id="5d90d-538">PublisherID</span></span></td>
<td><p><span data-ttu-id="5d90d-539">GUID 格式的发布服务器的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-539">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="5d90d-540">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-540">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-541">订阅说明</span><span class="sxs-lookup"><span data-stu-id="5d90d-541">Subscription Description</span></span></td>
<td><p><span data-ttu-id="5d90d-542">客户购买的服务产品的名称，如价目表中所定义。</span><span class="sxs-lookup"><span data-stu-id="5d90d-542">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="5d90d-543">（与产品/服务名称字段相同）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-543">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-544">订阅 ID</span><span class="sxs-lookup"><span data-stu-id="5d90d-544">Subscription ID</span></span></td>
<td><p><span data-ttu-id="5d90d-545">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d90d-545">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="5d90d-546">当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-546">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="5d90d-547">这与合作伙伴管理员控制台中的订阅 ID 不相同。</span><span class="sxs-lookup"><span data-stu-id="5d90d-547">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-548">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-548">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="5d90d-549">计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="5d90d-549">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="5d90d-550">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="5d90d-550">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-551">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="5d90d-551">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="5d90d-552">计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</span><span class="sxs-lookup"><span data-stu-id="5d90d-552">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="5d90d-553">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="5d90d-553">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-554">使用日期</span><span class="sxs-lookup"><span data-stu-id="5d90d-554">Usage Date</span></span></td>
<td><p><span data-ttu-id="5d90d-555">服务使用日期。</span><span class="sxs-lookup"><span data-stu-id="5d90d-555">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-556">计量类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-556">Meter Type</span></span></td>
<td><p><span data-ttu-id="5d90d-557">计量器的类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-557">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-558">计量类别</span><span class="sxs-lookup"><span data-stu-id="5d90d-558">Meter Category</span></span></td>
<td><p><span data-ttu-id="5d90d-559">使用的顶级服务。</span><span class="sxs-lookup"><span data-stu-id="5d90d-559">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-560">计量 Id</span><span class="sxs-lookup"><span data-stu-id="5d90d-560">Meter Id</span></span></td>
<td><p><span data-ttu-id="5d90d-561">正在使用的计量的 ID。</span><span class="sxs-lookup"><span data-stu-id="5d90d-561">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-562">计量子类别</span><span class="sxs-lookup"><span data-stu-id="5d90d-562">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="5d90d-563">可能影响速度的 Azure 服务类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-563">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-564">计量名称</span><span class="sxs-lookup"><span data-stu-id="5d90d-564">Meter Name</span></span></td>
<td><p><span data-ttu-id="5d90d-565">所使用的计量的度量单位。</span><span class="sxs-lookup"><span data-stu-id="5d90d-565">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-566">计量区域</span><span class="sxs-lookup"><span data-stu-id="5d90d-566">Meter Region</span></span></td>
<td><p><span data-ttu-id="5d90d-567">此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-567">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-568">单位</span><span class="sxs-lookup"><span data-stu-id="5d90d-568">Unit</span></span></td>
<td><p><span data-ttu-id="5d90d-569">资源名称的单位。</span><span class="sxs-lookup"><span data-stu-id="5d90d-569">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-570">已消耗数量</span><span class="sxs-lookup"><span data-stu-id="5d90d-570">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="5d90d-571">报告期间的服务消耗量（小时，GB 等）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-571">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="5d90d-572">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="5d90d-572">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-573">资源位置</span><span class="sxs-lookup"><span data-stu-id="5d90d-573">Resource Location</span></span></td>
<td><p><span data-ttu-id="5d90d-574">计量器正在其中运行的数据中心。</span><span class="sxs-lookup"><span data-stu-id="5d90d-574">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-575">已使用服务</span><span class="sxs-lookup"><span data-stu-id="5d90d-575">Consumed Service</span></span></td>
<td><p><span data-ttu-id="5d90d-576">你使用的 Azure 平台服务。</span><span class="sxs-lookup"><span data-stu-id="5d90d-576">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="5d90d-577">资源 URI</span><span class="sxs-lookup"><span data-stu-id="5d90d-577">Resource URI</span></span></td>
<td><p><span data-ttu-id="5d90d-578">所使用资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="5d90d-578">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-579">费用类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-579">Charge type</span></span></td>
<td><p><span data-ttu-id="5d90d-580">费用或调整的类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-580">The type of charge or adjustment.</span></span> <span data-ttu-id="5d90d-581">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-581">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-582">单价</span><span class="sxs-lookup"><span data-stu-id="5d90d-582">Unit price</span></span></td>
<td><p><span data-ttu-id="5d90d-583">购买时在 pricelist 中发布的每个许可证的价格。</span><span class="sxs-lookup"><span data-stu-id="5d90d-583">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="5d90d-584">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-585">数量</span><span class="sxs-lookup"><span data-stu-id="5d90d-585">Quantity</span></span></td>
<td><p><span data-ttu-id="5d90d-586">许可证数量。</span><span class="sxs-lookup"><span data-stu-id="5d90d-586">Number of licenses.</span></span> <span data-ttu-id="5d90d-587">确保这与在对帐期间你的计费系统中存储的信息相匹配。</span><span class="sxs-lookup"><span data-stu-id="5d90d-587">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-588">单位类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-588">Unit type</span></span></td>
<td><p><span data-ttu-id="5d90d-589">计量计量器的单位类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-589">The type of unit the meter is charged in.</span></span> <span data-ttu-id="5d90d-590">对当前活动不可用。</span><span class="sxs-lookup"><span data-stu-id="5d90d-590">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-591">帐单税前税</span><span class="sxs-lookup"><span data-stu-id="5d90d-591">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="5d90d-592">税前的总金额。</span><span class="sxs-lookup"><span data-stu-id="5d90d-592">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-593">计费货币</span><span class="sxs-lookup"><span data-stu-id="5d90d-593">Billing currency</span></span></td>
<td><p><span data-ttu-id="5d90d-594">客户的地理区域中的货币</span><span class="sxs-lookup"><span data-stu-id="5d90d-594">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-595">定价 pretax 总计</span><span class="sxs-lookup"><span data-stu-id="5d90d-595">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="5d90d-596">添加税款之前的定价。</span><span class="sxs-lookup"><span data-stu-id="5d90d-596">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-597">定价货币</span><span class="sxs-lookup"><span data-stu-id="5d90d-597">Pricing currency</span></span></td>
<td><p><span data-ttu-id="5d90d-598">Pricelist 中的货币。</span><span class="sxs-lookup"><span data-stu-id="5d90d-598">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="5d90d-599">服务信息1</span><span class="sxs-lookup"><span data-stu-id="5d90d-599">Service Info 1</span></span></td>
<td><p><span data-ttu-id="5d90d-600">已预配并且已在指定日利用的服务总线连接数。</span><span class="sxs-lookup"><span data-stu-id="5d90d-600">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-601">服务信息2</span><span class="sxs-lookup"><span data-stu-id="5d90d-601">Service Info 2</span></span></td>
<td><p><span data-ttu-id="5d90d-602">捕获可选的服务特定元数据的旧字段。</span><span class="sxs-lookup"><span data-stu-id="5d90d-602">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="5d90d-603">附加信息</span><span class="sxs-lookup"><span data-stu-id="5d90d-603">Additional Info</span></span></td>
<td><p><span data-ttu-id="5d90d-604">其他列中未涵盖的任何其他信息。</span><span class="sxs-lookup"><span data-stu-id="5d90d-604">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="5d90d-605">发票与对帐文件之间的映射费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-605">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="5d90d-606">发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="5d90d-606">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="5d90d-607">若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。</span><span class="sxs-lookup"><span data-stu-id="5d90d-607">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="5d90d-608">基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。</span><span class="sxs-lookup"><span data-stu-id="5d90d-608">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="5d90d-609">按 "调整" 形式出现在发票上的一个信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="5d90d-609">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="5d90d-610">下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="5d90d-610">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="5d90d-611"><strong>发票费用说明</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-611"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-612"><strong>对帐文件费用说明（ChargeType 列）</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-612"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-613"><strong>此费用是什么？</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-613"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-614"><strong>如何实现将这些 ChargeTypes 映射到发票？</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-614"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="5d90d-615"><strong>基于许可证的费用</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-615"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-616">激活费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-616">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-617">客户购买后使用订阅时向其收取的金额</span><span class="sxs-lookup"><span data-stu-id="5d90d-617">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="5d90d-618">从基于许可证的文件，对 <strong>Amount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-618">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-619">取消费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-619">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-620">相关席位发生变化时，退款给客户的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-620">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-621">周期费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-621">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-622">订阅的定期费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-622">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-623">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="5d90d-623">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-624">相关席位发生变化时，客户评估的按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-624">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-625">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-625">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-626">取消后服务的未使用部分按比例计算的退款</span><span class="sxs-lookup"><span data-stu-id="5d90d-626">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-627">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-627">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-628">使用年度计费时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-628">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-629">购买费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-629">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-630">使用月度帐单时的订阅费用类型</span><span class="sxs-lookup"><span data-stu-id="5d90d-630">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-631">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-631">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-632">订阅续订后按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-632">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="5d90d-633">续订费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-633">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-634">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-634">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-635">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-635">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-636">从激活到计费周期结束时间段内按比例计算的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-636">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="5d90d-637"><strong>一次性费用</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-637"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="5d90d-638">新</span><span class="sxs-lookup"><span data-stu-id="5d90d-638">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-639">创建新购买时使用</span><span class="sxs-lookup"><span data-stu-id="5d90d-639">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-640">addQuantity</span><span class="sxs-lookup"><span data-stu-id="5d90d-640">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-641">用于原始购买的退款和增加后的新数量</span><span class="sxs-lookup"><span data-stu-id="5d90d-641">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-642">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="5d90d-642">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-643">用于原始购买的退款和减少后的新数量</span><span class="sxs-lookup"><span data-stu-id="5d90d-643">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-644">“取消”</span><span class="sxs-lookup"><span data-stu-id="5d90d-644">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-645">取消订阅时使用</span><span class="sxs-lookup"><span data-stu-id="5d90d-645">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-646">转换</span><span class="sxs-lookup"><span data-stu-id="5d90d-646">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-647">升级许可证时使用，但座位数保持不变</span><span class="sxs-lookup"><span data-stu-id="5d90d-647">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="5d90d-648"><strong>使用费用</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-648"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-649">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-649">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-650">评估当前计费周期内取消未付款使用量的使用费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-650">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="5d90d-651">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-651">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-652">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-652">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-653">访问当前计费周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-653">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="5d90d-654"><strong>制作</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-654"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-655">偏移行项</span><span class="sxs-lookup"><span data-stu-id="5d90d-655">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-656">部分或全部退款到行项，包括税款</span><span class="sxs-lookup"><span data-stu-id="5d90d-656">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-657">从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-657">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="5d90d-658">从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-658">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="5d90d-659"><strong>基于使用情况的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-659"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-660">激活折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-660">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-661">激活订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-661">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="5d90d-662">从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-662">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-663">周期折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-663">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-664">对定期费用应用的折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-664">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-665">续订折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-665">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-666">续订订阅时应用的折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-666">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-667">取消折扣</span><span class="sxs-lookup"><span data-stu-id="5d90d-667">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-668">取消折扣时应用的费用</span><span class="sxs-lookup"><span data-stu-id="5d90d-668">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="5d90d-669"><strong>基于许可证的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-669"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-670"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="5d90d-670"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="5d90d-671">从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-671">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5d90d-672"><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="5d90d-672"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-673"><em>可应用于多种费用类型</em></span><span class="sxs-lookup"><span data-stu-id="5d90d-673"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="5d90d-674"><em>异常：行项 &quot;Offset &quot; 已包含税金。请参阅上面的信用额度。</em></span><span class="sxs-lookup"><span data-stu-id="5d90d-674"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-675">税款或增值税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="5d90d-675">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="5d90d-676">从基于许可证的文件，对 <strong>Tax</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-676">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="5d90d-677">从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</span><span class="sxs-lookup"><span data-stu-id="5d90d-677">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
