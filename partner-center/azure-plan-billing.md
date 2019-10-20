---
title: Azure 计划 - 计费 | 合作伙伴中心
ms.topic: article
ms.date: 10/04/2019
description: 描述发票和对帐文件结构
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171304"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="a2ab9-103">CSP 中的新商务体验 - Azure 计费</span><span class="sxs-lookup"><span data-stu-id="a2ab9-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="a2ab9-104">Azure 计划中的计费是一个简化的计费体验，它使用一致的单一计费日期和基于日历月份的计费周期。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="a2ab9-105">有关计费平台的信息，请阅读[合作伙伴中心新式商务操作指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="a2ab9-106">计费概要</span><span class="sxs-lookup"><span data-stu-id="a2ab9-106">Summary of billing essentials</span></span>

- <span data-ttu-id="a2ab9-107">**发票日期**：发票和对帐文件将在 8 号（UTC 午夜）在合作伙伴中心仪表板/API 中提供。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="a2ab9-108">**发票计费周期**：发票计费周期与日历月份相一致，例如 10/1 - 10/31、11/1 - 11/30。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="a2ab9-109">**费用服务周期**：费用与日历月份相一致。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="a2ab9-110">例如，如果计费合作伙伴在 10/15 通过 Azure 计划添加了 Azure 服务，而客户在 10/15 开始使用 Azure 服务，则计费合作伙伴将在 11/8 收到客户在服务周期 10/15 - 10/31 的使用费发票/对帐文件。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="a2ab9-111">在 12/8 生成的下个月发票包含服务周期 11/1 - 11/31 的所有费用。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="a2ab9-112">**发票付款期限**：净 60 天。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="a2ab9-113">**发票货币**：继续按客户所在国家/地区的指定货币对合作伙伴计费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="a2ab9-114">例如，如果计费合作伙伴位于爱尔兰，而客户位于英国、挪威和德国，则计费合作伙伴将收到英镑、挪威克朗和欧元货币的发票/对帐文件。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="a2ab9-115">**合作伙伴奖励**：从发票月份结束时间起的 45 天付费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="a2ab9-116">访问发票和对帐文件</span><span class="sxs-lookup"><span data-stu-id="a2ab9-116">Access your invoices and recon files</span></span>

<span data-ttu-id="a2ab9-117">当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="a2ab9-118">**访问发票和对帐文件**</span><span class="sxs-lookup"><span data-stu-id="a2ab9-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="a2ab9-119">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="a2ab9-120">在“合作伙伴中心”菜单中，选择“计费”。 </span><span class="sxs-lookup"><span data-stu-id="a2ab9-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="a2ab9-121">选择“基于日历”对应的选项卡，以及所需的货币。 </span><span class="sxs-lookup"><span data-stu-id="a2ab9-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![计费](images/azure/billing1.png)

4. <span data-ttu-id="a2ab9-123">选择“发票和对帐文件”。 </span><span class="sxs-lookup"><span data-stu-id="a2ab9-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="a2ab9-124">若要查看历史发票和对帐文件，请展开下面的“计费历史记录”行。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="a2ab9-125">阅读发票</span><span class="sxs-lookup"><span data-stu-id="a2ab9-125">Read the invoice</span></span>

1. <span data-ttu-id="a2ab9-126">提供发票的日期不会晚于每个月的 8 号。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="a2ab9-127">合作伙伴可在 60 天内汇款。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="a2ab9-128">计费周期涵盖给定的日历月份，例如 10/1 - 10/31。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="a2ab9-129">费用是净调整额（金额是“合作伙伴赚取的托管服务返点”的净额）。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="a2ab9-130">查看发票对帐文件和每日分类的使用情况文件，以了解更多计费详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![发票](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="a2ab9-132">阅读对帐文件</span><span class="sxs-lookup"><span data-stu-id="a2ab9-132">Read the recon file</span></span>

1. <span data-ttu-id="a2ab9-133">在对帐文件中，每个 Azure 订阅计量项目最多可以占用两个计费行。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="a2ab9-134">如果该计量项目符合任何类型的折扣或返点（例如，第 1 层折扣，或合作伙伴赚取的托管服务返点）条件，则对帐文件只包含一个计费行。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="a2ab9-135">**PriceAdjusmentDescription** 列引用折扣或赚取的返点；有效单价是零售价减去合作伙伴赚取的返点或其他任何折扣。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="a2ab9-136">如果该计量项目在整个日历月份内都不符合合作伙伴赚取的托管服务返点条件，则对帐文件只包含一个计费行，有效单价是零售价（即单价）。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="a2ab9-137">如果该计量项目在当月的某些日期符合**合作伙伴赚取的托管服务返点**条件，则对帐文件将包含两个计费行。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="a2ab9-138">其中一行表示该计量项目符合条件的天数，另一行表示该计量项目不符合条件的天数。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="a2ab9-139">阅读每日使用情况文件</span><span class="sxs-lookup"><span data-stu-id="a2ab9-139">Read the daily usage file</span></span>

- <span data-ttu-id="a2ab9-140">Azure 计划中的订阅计量项目将会分类，并每日累积。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="a2ab9-141">**合作伙伴赚取的托管服务返点**按日确定和应用。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="a2ab9-142">对于月份中发生了消耗的每个日期，每个订阅计量项目都有对应的一行。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="a2ab9-143">在以下示例中：</span><span class="sxs-lookup"><span data-stu-id="a2ab9-143">In the example below:</span></span>

  - <span data-ttu-id="a2ab9-144">计量项目在 7/1 – 7/3 符合**合作伙伴赚取的托管服务返点**条件（请注意，有效单价为零售价减去合作伙伴获取的返点）。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="a2ab9-145">计量项目在 7/4 – 7/7 不符合**合作伙伴赚取的托管服务返点**条件（请注意，有效单价为零售价）。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="a2ab9-146">计量项目在 7/8 – 7/31 符合**合作伙伴赚取的托管服务返点**条件（请注意，有效单价为零售价减去合作伙伴获取的返点）。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![对帐 2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="a2ab9-148">采用客户货币的发票</span><span class="sxs-lookup"><span data-stu-id="a2ab9-148">Invoice in customer currency</span></span> 

<span data-ttu-id="a2ab9-149">通过 Azure 计划销售的 Azure 服务按美元定价，并按客户所在国家/地区指定的货币计费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="a2ab9-150">如果计费货币不是美元，则发票的最后一页上会显示使用的外汇汇率。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="a2ab9-151">外汇汇率每月确定，并应用于随后的发票。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="a2ab9-152">有关国家/地区货币的完整列表，请查看[新商务套餐在各个国家/地区的上市情况和客户货币矩阵](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V)。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="a2ab9-153">Microsoft 将使用 [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) 来确定外汇汇率，以此确定定价货币与发票货币之间的兑换率。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="a2ab9-154">外汇汇率将在月份最后一日的前一天刷新，然后将会应用。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="a2ab9-155">**示例**：服务周期 8 月 1 日 – 8 月 31 日的使用费将按 8 月 1 日发布的外汇汇率计费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="a2ab9-156">这些费用将显示在 9 月份的发票上，该发票的最后一页将注明外汇汇率。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="a2ab9-157">无论计费货币是什么，合作伙伴租户用户仍会看到有关所有客户和所有订单的特定于角色的相关信息。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="a2ab9-158">此外，用户还可以看到所有货币的所有发票。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="a2ab9-159">Azure 预订</span><span class="sxs-lookup"><span data-stu-id="a2ab9-159">Azure reservations</span></span> 

<span data-ttu-id="a2ab9-160">如果通过 Azure 计划购买 [Azure 预留项](https://docs.microsoft.com/partner-center/azure-reservations)，最初只能在合作伙伴中心选择一次性计费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="a2ab9-161">Azure 门户提供每月计费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="a2ab9-162">将来，合作伙伴中心也会提供每月计费。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="a2ab9-163">Azure 成本管理</span><span class="sxs-lookup"><span data-stu-id="a2ab9-163">Azure cost management</span></span> 

<span data-ttu-id="a2ab9-164">Azure 成本管理工具可帮助组织可视化、管理和优化 Microsoft Azure 的成本。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="a2ab9-165">此功能将在 Azure 门户中提供。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="a2ab9-166">合作伙伴可以借助以下功能获得永不中断的低延迟解决方案：</span><span class="sxs-lookup"><span data-stu-id="a2ab9-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="a2ab9-167">更丰富的分析和预算警报</span><span class="sxs-lookup"><span data-stu-id="a2ab9-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="a2ab9-168">API 和 Power BI 连接器</span><span class="sxs-lookup"><span data-stu-id="a2ab9-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="a2ab9-169">多客户视图</span><span class="sxs-lookup"><span data-stu-id="a2ab9-169">Multi-customer view</span></span> 
- <span data-ttu-id="a2ab9-170">免费管理 Azure 成本</span><span class="sxs-lookup"><span data-stu-id="a2ab9-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="a2ab9-171">角色/用户扩展</span><span class="sxs-lookup"><span data-stu-id="a2ab9-171">Expansion of roles/users</span></span> 

<span data-ttu-id="a2ab9-172">有关此功能（已在 2019 年 2 月根据企业协议推出）的详细信息，请参阅 [Azure 成本管理](https://azure.microsoft.com/services/cost-management)。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="a2ab9-173">此功能仅适用于购买的 Azure 服务，是 Azure CSP 新商务体验的一部分。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="a2ab9-174">Azure 支出</span><span class="sxs-lookup"><span data-stu-id="a2ab9-174">Azure spending</span></span> 

<span data-ttu-id="a2ab9-175">Azure 支出工具将在合作伙伴中心提供，是 CSP 新商务体验的一部分。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="a2ab9-176">应用后，此功能可让合作伙伴查看：</span><span class="sxs-lookup"><span data-stu-id="a2ab9-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="a2ab9-177">针对客户的总预算</span><span class="sxs-lookup"><span data-stu-id="a2ab9-177">Total budget on a customer</span></span> 
- <span data-ttu-id="a2ab9-178">现有 Azure 计划的总估算支出</span><span class="sxs-lookup"><span data-stu-id="a2ab9-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="a2ab9-179">每个计费周期的客户用量百分比</span><span class="sxs-lookup"><span data-stu-id="a2ab9-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="a2ab9-180">由于通过 Azure 计划销售的 Azure 服务的计费模型是付后使用，因此，为了避免帐单超过预期，合作伙伴可以应用每月预算并跟踪用量百分比。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="a2ab9-181">一次可对一个或多个客户应用预算。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure 支出](images/azure/azurespend.png)

<span data-ttu-id="a2ab9-183">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="a2ab9-183">**For more information**</span></span>

-  <span data-ttu-id="a2ab9-184">通过合作伙伴中心仪表板提供的价目表中提供了合作伙伴赚取的返点 (PEC) 的计算方式。</span><span class="sxs-lookup"><span data-stu-id="a2ab9-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="a2ab9-185">购买 Azure 计划</span><span class="sxs-lookup"><span data-stu-id="a2ab9-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="a2ab9-186">CSP 新商务体验的价目表</span><span class="sxs-lookup"><span data-stu-id="a2ab9-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
