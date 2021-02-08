---
title: Azure 计划计费 - 发票和对帐文件
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何访问和理解与 Azure 计划计费相关的发票和对帐文件结构。
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924987"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="e06fa-103">CSP 中的新商务体验 - Azure 计费</span><span class="sxs-lookup"><span data-stu-id="e06fa-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="e06fa-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="e06fa-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e06fa-105">管理员代理</span><span class="sxs-lookup"><span data-stu-id="e06fa-105">Admin agent</span></span>
- <span data-ttu-id="e06fa-106">计费管理员</span><span class="sxs-lookup"><span data-stu-id="e06fa-106">Billing admin</span></span>
- <span data-ttu-id="e06fa-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e06fa-107">Global admin</span></span>

<span data-ttu-id="e06fa-108">本文介绍了如何访问和理解与 Azure 计划计费相关的发票和对帐文件结构。</span><span class="sxs-lookup"><span data-stu-id="e06fa-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="e06fa-109">Azure 计划中的计费是一个简化的计费体验，它使用一致的单一计费日期和基于日历月份的计费周期。</span><span class="sxs-lookup"><span data-stu-id="e06fa-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="e06fa-110">计费概要</span><span class="sxs-lookup"><span data-stu-id="e06fa-110">Summary of billing essentials</span></span>

- <span data-ttu-id="e06fa-111">**发票日期**：发票和对帐文件将在 8 号（UTC 午夜）在合作伙伴中心仪表板/API 中提供。</span><span class="sxs-lookup"><span data-stu-id="e06fa-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="e06fa-112">**发票计费周期**：发票计费周期与日历月份相一致，例如 10/1 - 10/31、11/1 - 11/30。</span><span class="sxs-lookup"><span data-stu-id="e06fa-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="e06fa-113">**费用服务周期**：费用与日历月份相一致。</span><span class="sxs-lookup"><span data-stu-id="e06fa-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="e06fa-114">例如，如果计费合作伙伴在 10/15 通过 Azure 计划添加了 Azure 服务，而客户在 10/15 开始使用 Azure 服务，则计费合作伙伴将在 11/8 收到客户在服务周期 10/15 - 10/31 的使用费发票/对帐文件。</span><span class="sxs-lookup"><span data-stu-id="e06fa-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="e06fa-115">在 12/8 生成的下个月发票包含服务周期 11/1 - 11/31 的所有费用。</span><span class="sxs-lookup"><span data-stu-id="e06fa-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="e06fa-116">**发票付款期限**：净 60 天。</span><span class="sxs-lookup"><span data-stu-id="e06fa-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="e06fa-117">**发票货币**：从 2021 年 1 月 28 日开始，对于欧盟/欧洲自由贸易联盟和英国地区的合作伙伴，如果有新客户和现有 CSP 客户首次购买新商务优惠，并且其租户是在 2020 年 5 月 11 日之前创建的，则将以合作伙伴所在地货币对这些购买计费。</span><span class="sxs-lookup"><span data-stu-id="e06fa-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="e06fa-118">位于欧盟/欧洲自由贸易联盟和英国地区以外的合作伙伴将继续以合作伙伴所在地货币计费。</span><span class="sxs-lookup"><span data-stu-id="e06fa-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="e06fa-119">**合作伙伴奖励**：从发票月份结束时间起的 45 天付费。</span><span class="sxs-lookup"><span data-stu-id="e06fa-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="e06fa-120">访问发票和对帐文件</span><span class="sxs-lookup"><span data-stu-id="e06fa-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="e06fa-121">当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e06fa-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="e06fa-122">访问发票和对帐文件：</span><span class="sxs-lookup"><span data-stu-id="e06fa-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="e06fa-123">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="e06fa-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="e06fa-124">在“合作伙伴中心”菜单中，选择“计费”。</span><span class="sxs-lookup"><span data-stu-id="e06fa-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="e06fa-125">选择“定期”和“一次性”选项卡，以及所需货币 。</span><span class="sxs-lookup"><span data-stu-id="e06fa-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="计费":::

4. <span data-ttu-id="e06fa-127">选择“发票”或“对帐文件” 。</span><span class="sxs-lookup"><span data-stu-id="e06fa-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="e06fa-128">若要查看历史发票和对帐文件，请展开下面的“计费历史记录”行。</span><span class="sxs-lookup"><span data-stu-id="e06fa-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="e06fa-129">了解使用情况数据</span><span class="sxs-lookup"><span data-stu-id="e06fa-129">Understanding usage data</span></span> 

1. <span data-ttu-id="e06fa-130">Azure 计划是使用情况的根或顶级容器。</span><span class="sxs-lookup"><span data-stu-id="e06fa-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="e06fa-131">所有使用情况都要关联回单个 Azure 计划。</span><span class="sxs-lookup"><span data-stu-id="e06fa-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="e06fa-132">一个计划中将有一个或多个 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="e06fa-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="e06fa-133">这些容器用于资源管理和部署。</span><span class="sxs-lookup"><span data-stu-id="e06fa-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="e06fa-134">在订阅中，资源组将添加到组资源。</span><span class="sxs-lookup"><span data-stu-id="e06fa-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="e06fa-135">每个资源都将部署到一个资源组。</span><span class="sxs-lookup"><span data-stu-id="e06fa-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="e06fa-136">示例资源包括虚拟机和存储帐户。</span><span class="sxs-lookup"><span data-stu-id="e06fa-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="e06fa-137">资源发出计量：计量是资源的消耗度量，一个资源可能会为多个计量发出使用情况。</span><span class="sxs-lookup"><span data-stu-id="e06fa-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="e06fa-138">计量由 ProductId、SKUId 和 AvailabilityId 标识。</span><span class="sxs-lookup"><span data-stu-id="e06fa-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="e06fa-139">订阅资源组和计量的层次结构</span><span class="sxs-lookup"><span data-stu-id="e06fa-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="e06fa-140">**Azure 帐户（租户）**</span><span class="sxs-lookup"><span data-stu-id="e06fa-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="e06fa-141">订阅 A</span><span class="sxs-lookup"><span data-stu-id="e06fa-141">Subscription A</span></span>
    - <span data-ttu-id="e06fa-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="e06fa-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="e06fa-143">虚拟机（资源）</span><span class="sxs-lookup"><span data-stu-id="e06fa-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="e06fa-144">计算计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-144">Compute meter</span></span>
        - <span data-ttu-id="e06fa-145">虚拟网络（资源）</span><span class="sxs-lookup"><span data-stu-id="e06fa-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="e06fa-146">无计费计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-146">No billing meter</span></span>

    - <span data-ttu-id="e06fa-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="e06fa-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="e06fa-148">虚拟机（资源）</span><span class="sxs-lookup"><span data-stu-id="e06fa-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="e06fa-149">计算机计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-149">Computer meter</span></span>
        - <span data-ttu-id="e06fa-150">高级 SSD 托管磁盘（资源）</span><span class="sxs-lookup"><span data-stu-id="e06fa-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="e06fa-151">存储容量计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-151">Storage capacity meter</span></span>
            - <span data-ttu-id="e06fa-152">存储操作计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-152">Storage operations meter</span></span>

- <span data-ttu-id="e06fa-153">订阅 B   -ResourceGroup 1       - Azure SQL（资源）           - DTU 计量       - VPN 网关（资源）           - VPN 网关计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="e06fa-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="e06fa-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="e06fa-155">虚拟网络接口（资源）</span><span class="sxs-lookup"><span data-stu-id="e06fa-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="e06fa-156">无计费计量</span><span class="sxs-lookup"><span data-stu-id="e06fa-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="e06fa-157">阅读发票</span><span class="sxs-lookup"><span data-stu-id="e06fa-157">Read the invoice</span></span>

1. <span data-ttu-id="e06fa-158">提供发票的日期不会晚于每个月的 8 号。</span><span class="sxs-lookup"><span data-stu-id="e06fa-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="e06fa-159">合作伙伴可在 60 天内汇款。</span><span class="sxs-lookup"><span data-stu-id="e06fa-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="e06fa-160">计费周期涵盖给定的日历月份，例如 10/1 - 10/31。</span><span class="sxs-lookup"><span data-stu-id="e06fa-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="e06fa-161">费用是净调整额（金额是“合作伙伴赚取的托管服务返点”的净额）。</span><span class="sxs-lookup"><span data-stu-id="e06fa-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="e06fa-162">查看发票对帐文件和每日分类的使用情况文件，以了解更多计费详细信息。</span><span class="sxs-lookup"><span data-stu-id="e06fa-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="发票":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="e06fa-164">阅读发票对帐文件</span><span class="sxs-lookup"><span data-stu-id="e06fa-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="e06fa-165">在对帐文件中，每个 Azure 计划和计量组合最多可以有两个计费行。</span><span class="sxs-lookup"><span data-stu-id="e06fa-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="e06fa-166">如果该计量项目符合任何类型的折扣或返点（例如，分级折扣，或合作伙伴赚取的托管服务返点）条件，则对帐文件只包含一个计费行。</span><span class="sxs-lookup"><span data-stu-id="e06fa-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="e06fa-167">PriceAdjusmentDescription 列将引用折扣或赚取的返点。</span><span class="sxs-lookup"><span data-stu-id="e06fa-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="e06fa-168">如果特定计量项目中的资源都不符合折扣或合作伙伴赚取的返点条件，则对帐文件只包含一个计费行，有效单价是零售价（即单价）。</span><span class="sxs-lookup"><span data-stu-id="e06fa-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="e06fa-169">如果该计量项目或发出该计量项目的任何资源在当月的某些日期符合合作伙伴赚取的托管服务返点条件，则对帐文件将包含两个计费行。</span><span class="sxs-lookup"><span data-stu-id="e06fa-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="e06fa-170">其中一行表示该计量项目符合条件的天数，另一行表示该计量项目不符合条件的天数。</span><span class="sxs-lookup"><span data-stu-id="e06fa-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="e06fa-171">阅读每日使用情况文件</span><span class="sxs-lookup"><span data-stu-id="e06fa-171">Read the daily usage file</span></span>

- <span data-ttu-id="e06fa-172">Azure 计划中的订阅计量项目将会分类，并每日累积。</span><span class="sxs-lookup"><span data-stu-id="e06fa-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="e06fa-173">**合作伙伴赚取的托管服务返点** 按日确定和应用。</span><span class="sxs-lookup"><span data-stu-id="e06fa-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="e06fa-174">对于月份中发生了消耗的每个日期，每个订阅计量项目都有对应的一行。</span><span class="sxs-lookup"><span data-stu-id="e06fa-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="e06fa-175">在以下示例中：</span><span class="sxs-lookup"><span data-stu-id="e06fa-175">In the example below:</span></span>

  - <span data-ttu-id="e06fa-176">计量项目在 7/1 - 7/3 符合 **合作伙伴赚取的托管服务返点** 条件（请注意，有效单价为零售价减去合作伙伴获取的返点）。</span><span class="sxs-lookup"><span data-stu-id="e06fa-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="e06fa-177">计量项目在 7/4 - 7/7 不符合 **合作伙伴赚取的托管服务返点** 条件（请注意，有效单价为零售价）。</span><span class="sxs-lookup"><span data-stu-id="e06fa-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="e06fa-178">计量项目在 7/8 - 7/31 符合 **合作伙伴赚取的托管服务返点** 条件（请注意，有效单价为零售价减去合作伙伴获取的返点）。</span><span class="sxs-lookup"><span data-stu-id="e06fa-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="对帐 2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="e06fa-180">采用客户货币的发票</span><span class="sxs-lookup"><span data-stu-id="e06fa-180">Invoice in customer currency</span></span>

<span data-ttu-id="e06fa-181">通过 Azure 计划销售的 Azure 服务按美元定价，并按客户所在国家/地区指定的货币计费。</span><span class="sxs-lookup"><span data-stu-id="e06fa-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="e06fa-182">如果计费货币不是美元，则发票的最后一页上会显示使用的外汇汇率 (FX)。</span><span class="sxs-lookup"><span data-stu-id="e06fa-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="e06fa-183">外汇汇率每月确定，并应用于随后的发票。</span><span class="sxs-lookup"><span data-stu-id="e06fa-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="e06fa-184">有关国家/地区货币的完整列表，请查看[新商务套餐在各个国家/地区的上市情况和客户货币矩阵](https://go.microsoft.com/fwlink/?linkid=2112354)。</span><span class="sxs-lookup"><span data-stu-id="e06fa-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="e06fa-185">Microsoft 按照伦敦证券交易所汇率进行转换。</span><span class="sxs-lookup"><span data-stu-id="e06fa-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="e06fa-186">我们采用的汇率是伦敦证券交易所当月最后一个交易日的最后一秒捕获的汇率。</span><span class="sxs-lookup"><span data-stu-id="e06fa-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="e06fa-187">外汇汇率将在月份最后一日的前一天刷新，然后将会应用。</span><span class="sxs-lookup"><span data-stu-id="e06fa-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="e06fa-188">Azure 预订</span><span class="sxs-lookup"><span data-stu-id="e06fa-188">Azure reservations</span></span>


<span data-ttu-id="e06fa-189">如果通过 Azure 计划[购买 Azure 预订](azure-reservations.md)，则可选择一次性计费或按月计费。</span><span class="sxs-lookup"><span data-stu-id="e06fa-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="e06fa-190">Azure 支出</span><span class="sxs-lookup"><span data-stu-id="e06fa-190">Azure spending</span></span>

<span data-ttu-id="e06fa-191">现有 Azure 支出体验已更新，以支持合作伙伴中心中的新 Azure 计划计费。</span><span class="sxs-lookup"><span data-stu-id="e06fa-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="e06fa-192">这样合作伙伴可以实现以下操作：</span><span class="sxs-lookup"><span data-stu-id="e06fa-192">This enables partners to:</span></span>

- <span data-ttu-id="e06fa-193">查看、管理和接收在客户级设置的预算的警报</span><span class="sxs-lookup"><span data-stu-id="e06fa-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="e06fa-194">查看 Azure 计划的总估算支出（按资源和计量级别细分）</span><span class="sxs-lookup"><span data-stu-id="e06fa-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="e06fa-195">由于通过 Azure 计划销售的 Azure 服务的计费模型是付后使用，因此，为了避免帐单超过预期，合作伙伴可以应用每月预算并跟踪用量百分比。</span><span class="sxs-lookup"><span data-stu-id="e06fa-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="e06fa-196">一次可对一个或多个客户应用预算。</span><span class="sxs-lookup"><span data-stu-id="e06fa-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure 支出":::

## <a name="next-steps"></a><span data-ttu-id="e06fa-198">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e06fa-198">Next steps</span></span>

- <span data-ttu-id="e06fa-199">查看合作伙伴赚取的返点 (PEC) 的计算方式。</span><span class="sxs-lookup"><span data-stu-id="e06fa-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="e06fa-200">登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/)并找到提供的价目表。</span><span class="sxs-lookup"><span data-stu-id="e06fa-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="e06fa-201">了解如何[购买 Azure 计划](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="e06fa-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="e06fa-202">请参阅 [CSP 新商务体验的价目表](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="e06fa-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
