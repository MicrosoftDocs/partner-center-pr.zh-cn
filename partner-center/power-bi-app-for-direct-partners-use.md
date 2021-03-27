---
title: 将合作伙伴中心分析用于 Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何使用合作伙伴中心分析应用查看你的业务数据，以便在 CSP) 中为直接伙伴 Power BI (。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633856"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="fbbe4-103">使用适用于 Microsoft Power BI 的合作伙伴中心分析应用查看你的业务数据</span><span class="sxs-lookup"><span data-stu-id="fbbe4-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="fbbe4-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="fbbe4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fbbe4-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="fbbe4-105">Global admin</span></span>
- <span data-ttu-id="fbbe4-106">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="fbbe4-106">User management admin</span></span>
- <span data-ttu-id="fbbe4-107">销售代理</span><span class="sxs-lookup"><span data-stu-id="fbbe4-107">Sales agent</span></span>
- <span data-ttu-id="fbbe4-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="fbbe4-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="fbbe4-109">查看你的业务数据</span><span class="sxs-lookup"><span data-stu-id="fbbe4-109">View your business data</span></span>

<span data-ttu-id="fbbe4-110">借助适用于 Power BI 的合作伙伴中心分析应用获得业务数据的直观表示，包括：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="fbbe4-111">你的客户群、订阅和许可证增长情况</span><span class="sxs-lookup"><span data-stu-id="fbbe4-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="fbbe4-112">Office 365、Microsoft Dynamics 和 Microsoft Azure 产品的使用情况</span><span class="sxs-lookup"><span data-stu-id="fbbe4-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="fbbe4-113">最近 60 天每个 Azure 订阅中的每项计量资源的每日消耗量</span><span class="sxs-lookup"><span data-stu-id="fbbe4-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="fbbe4-114">基于最新费率卡的估算成本</span><span class="sxs-lookup"><span data-stu-id="fbbe4-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="fbbe4-115">能够导出数据集和创建自定义报表，包括每个客户。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="fbbe4-116">关于合作伙伴中心分析应用预览版</span><span class="sxs-lookup"><span data-stu-id="fbbe4-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="fbbe4-117">此应用仅适用于云解决方案提供商计划中的直接合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="fbbe4-118">CSP 中的其他合作伙伴（例如，间接经销商）将无法登录。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="fbbe4-119">任何估算成本都是税前计费/发票数据，都不具有法律约束力。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="fbbe4-120">估算成本只应用于数据洞察。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="fbbe4-121">客户信息是以订阅为基础的。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="fbbe4-122">您最近创建帐户的任何客户，但没有订阅的客户不包括在计数中。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="fbbe4-123">估算成本基于最新费率卡，而它又基于 CSP 定价。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="fbbe4-124">天为日历天。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="fbbe4-125">业务洞察报告</span><span class="sxs-lookup"><span data-stu-id="fbbe4-125">Business Insights report</span></span>

- <span data-ttu-id="fbbe4-126">**客户租户**：已购买订阅的不同客户 Azure AD 租户的数量</span><span class="sxs-lookup"><span data-stu-id="fbbe4-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="fbbe4-127">**新客户(最近 30 天)**：最近 30 天内购买至少一个订阅的新客户</span><span class="sxs-lookup"><span data-stu-id="fbbe4-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="fbbe4-128">**(过去30天) 的改动**：不含任何 "活动"、"宽限期" 或 "已禁用" 订阅的客户</span><span class="sxs-lookup"><span data-stu-id="fbbe4-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="fbbe4-129">**新客户(最近 24 小时)**：最近 24 小时内购买至少一个订阅的新客户</span><span class="sxs-lookup"><span data-stu-id="fbbe4-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="fbbe4-130">**过去 12 个月的估算月成本**：过去 12 个月期间每月累计估算税前发票美元金额环比趋势</span><span class="sxs-lookup"><span data-stu-id="fbbe4-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="fbbe4-131">**过去 12 个月按产品排序的估算成本**：按过去 12 个月期间累计估算税前发票美元金额排序的售出产品。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="fbbe4-132">此状态表示最重要的产品收入。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="fbbe4-133">**过去 12 个月的客户**：过去 12 个月期间每月累计新客户和改动客户的环比趋势</span><span class="sxs-lookup"><span data-stu-id="fbbe4-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="fbbe4-134">**过去 12 个月按客户排序的估算成本**：按过去 12 个月期间累计估算税前发票美元金额排序的客户。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="fbbe4-135">此状态表明排名最高的客户。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="fbbe4-136">**按产品排序的客户计数**：按管理连客户排序的售出产品。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="fbbe4-137">此状态表示销售给大多数客户的热门产品。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="fbbe4-138">订阅洞察报告</span><span class="sxs-lookup"><span data-stu-id="fbbe4-138">Subscription Insights report</span></span>

- <span data-ttu-id="fbbe4-139">**订阅状态**：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-139">**Subscription status**:</span></span>

- <span data-ttu-id="fbbe4-140">活动：属于 "活动" 或 "处于宽限期" 状态的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="fbbe4-141">已挂起：属于 "已禁用" 状态的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="fbbe4-142">取消预配：属于 "取消预配" 或 "已过期" 状态的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="fbbe4-143">**过期状态**：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-143">**Expiry status**:</span></span>

  - <span data-ttu-id="fbbe4-144">已过期：已过期（订阅结束日期处于过去）的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="fbbe4-145">30 天后过期：将在 30 天后过期的订阅（订阅结束日期在接下来的 30 天后）</span><span class="sxs-lookup"><span data-stu-id="fbbe4-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="fbbe4-146">30 天内过期：将在接下来的 30 天内过期的订阅（订阅结束日期在今天和接下来的 30 天之间）</span><span class="sxs-lookup"><span data-stu-id="fbbe4-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="fbbe4-147">**订阅总数**： "活动"、"已启用" 或 "已禁用" 状态下的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="fbbe4-148">**新订阅(最近 30 天)**：客户在最近 30 天内购买的新订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="fbbe4-149">**新订阅(最近 24 小时)**：客户在最近 24 小时内购买的新订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="fbbe4-150">**30 天内过期**：将在接下来的 30 天内过期的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="fbbe4-151">**改动(最近 30 天)**：过去 30 天内取消预配或暂停（禁用）的订阅</span><span class="sxs-lookup"><span data-stu-id="fbbe4-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="fbbe4-152">**按订阅类型分发**：按基于许可证的订阅和基于使用情况的订阅类型的订阅总数的百分比</span><span class="sxs-lookup"><span data-stu-id="fbbe4-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="fbbe4-153">**按产品排序的活动订阅计数**：按活动订阅计数排序的售出产品</span><span class="sxs-lookup"><span data-stu-id="fbbe4-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="fbbe4-154">**过去 12 个月的订阅**：过去 12 个月期间每月累计新订阅和改动订阅的环比趋势</span><span class="sxs-lookup"><span data-stu-id="fbbe4-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="fbbe4-155">**客户订阅详细信息**：客户、订阅和产品/服务的详细视图</span><span class="sxs-lookup"><span data-stu-id="fbbe4-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="fbbe4-156">许可证洞察报告：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-156">License Insights report:</span></span>

- <span data-ttu-id="fbbe4-157">**许可证总数**：跨所有基于许可证的订阅聚合的许可证总数</span><span class="sxs-lookup"><span data-stu-id="fbbe4-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="fbbe4-158">**新(最近 30 天)**：最近 30 天内增加的许可证</span><span class="sxs-lookup"><span data-stu-id="fbbe4-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="fbbe4-159">**改动(最近 30 天)**：最近 30 天内减少的许可证</span><span class="sxs-lookup"><span data-stu-id="fbbe4-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="fbbe4-160">**新(最近 24 小时)**：最近 24 小时内增加的许可证</span><span class="sxs-lookup"><span data-stu-id="fbbe4-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="fbbe4-161">**过去 90 天内的许可证**：过去 90 天期间每月累计许可证增加和减少环比趋势</span><span class="sxs-lookup"><span data-stu-id="fbbe4-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="fbbe4-162">**按产品排序的活动许可证计数**：按活动许可证计数排序的售出产品</span><span class="sxs-lookup"><span data-stu-id="fbbe4-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="fbbe4-163">**按客户排列的活动许可证计数**：按活动许可证计数排序的客户</span><span class="sxs-lookup"><span data-stu-id="fbbe4-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="fbbe4-164">**过去90天的客户许可证事件详细信息**：客户、订阅和订阅事件的详细视图，包括事件日期、事件名称、数量和数量更改。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="fbbe4-165">许可证使用情况报告：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-165">Licenses Usage report:</span></span>

- <span data-ttu-id="fbbe4-166">**按产品排序的已分配许可证**：按许可证分配计数排序的售出产品</span><span class="sxs-lookup"><span data-stu-id="fbbe4-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="fbbe4-167">**按产品排序的正在使用的许可证**：按许可证使用计数排序的产品</span><span class="sxs-lookup"><span data-stu-id="fbbe4-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="fbbe4-168">**已分配许可证的客户分布**：按许可证分配百分比的 20% 范围划分的客户总数百分比分布</span><span class="sxs-lookup"><span data-stu-id="fbbe4-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="fbbe4-169">**正在使用的许可证的客户分布**：按许可证使用情况百分比的 20% 范围划分的客户总数百分比分布</span><span class="sxs-lookup"><span data-stu-id="fbbe4-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="fbbe4-170">**按客户排序的已分配许可证**：按客户和产品排序的售出许可证和已分配许可证的详细视图</span><span class="sxs-lookup"><span data-stu-id="fbbe4-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="fbbe4-171">**按客户排序的正在使用的许可证**：按客户和产品排序的售出许可证和正在使用的许可证的详细视图</span><span class="sxs-lookup"><span data-stu-id="fbbe4-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="fbbe4-172">Azure 洞察报告：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-172">Azure Insights report:</span></span>

- <span data-ttu-id="fbbe4-173">**过去12个月内基于使用情况的客户**：基于使用情况的新客户和改动基于使用情况的客户在过去12个月的时间段内每月聚合的每月趋势</span><span class="sxs-lookup"><span data-stu-id="fbbe4-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="fbbe4-174">**过去12个月的基于使用情况的订阅**：在过去12个月的时间段内每月聚合的基于使用情况的新订阅和改动基于使用情况的订阅的月趋势</span><span class="sxs-lookup"><span data-stu-id="fbbe4-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="fbbe4-175">**客户超过过去60天的预计用量成本**：基于使用情况的客户，按在过去60天的时间内聚合的预计税前发票金额进行排序。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="fbbe4-176">此状态表示最常使用的基于使用情况的客户带来了收入</span><span class="sxs-lookup"><span data-stu-id="fbbe4-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="fbbe4-177">**在过去60天内按类别列出的预计用量成本**：基于使用情况的订阅的计数类别，按在过去60天的时间内聚合的预计预纳税发票美元金额排序。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="fbbe4-178">**订阅在过去60天的预计用量成本**：基于使用情况的订阅，按过去60天内聚合的估计预纳税发票美元金额计算。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="fbbe4-179">**按费用预算排序的客户估算使用成本**：按当前使用费用预算超出阈值 (100%) 的百分比排序的客户。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="fbbe4-180">Azure 资源使用情况报告：</span><span class="sxs-lookup"><span data-stu-id="fbbe4-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="fbbe4-181">**按天对所选时间段使用 Azure 资源**：过去60天内所选时间段内每个基于使用量的订阅中每个按流量计费的资源的每日消耗单位。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="fbbe4-182">**所选时间段的 Azure 资源预计使用成本**：在过去60天内所选时间段内每个基于使用量的订阅中每个基于使用情况的订阅中每个按流量计费的资源的预估成本。</span><span class="sxs-lookup"><span data-stu-id="fbbe4-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="fbbe4-183">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fbbe4-183">Next steps</span></span>

- [<span data-ttu-id="fbbe4-184">适用于 Power BI 的合作伙伴中心分析应用概述</span><span class="sxs-lookup"><span data-stu-id="fbbe4-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="fbbe4-185">安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用</span><span class="sxs-lookup"><span data-stu-id="fbbe4-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
