---
title: 使用 合作伙伴中心 Analytics 进行Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何使用云解决方案提供商计划适用于 Power BI 的合作伙伴中心分析应用 (计划中的直接合作伙伴云解决方案提供商 () 业务) 。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564975"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="08083-103">使用适用于 Microsoft Power BI 的合作伙伴中心分析应用查看你的业务数据</span><span class="sxs-lookup"><span data-stu-id="08083-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="08083-104">**相应的角色**：全局管理员 |“用户管理”管理员 | 管理员代理</span><span class="sxs-lookup"><span data-stu-id="08083-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="08083-105">查看你的业务数据</span><span class="sxs-lookup"><span data-stu-id="08083-105">View your business data</span></span>

<span data-ttu-id="08083-106">使用适用于 Microsoft 合作伙伴中心 的 合作伙伴中心 Analytics 应用获取业务数据的可视化Power BI，包括：</span><span class="sxs-lookup"><span data-stu-id="08083-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="08083-107">你的客户群、订阅和许可证增长情况</span><span class="sxs-lookup"><span data-stu-id="08083-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="08083-108">Office 365、Microsoft Dynamics 和 Microsoft Azure 产品的使用情况</span><span class="sxs-lookup"><span data-stu-id="08083-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="08083-109">最近 60 天每个 Azure 订阅中的每项计量资源的每日消耗量</span><span class="sxs-lookup"><span data-stu-id="08083-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="08083-110">基于最新费率卡的估算成本</span><span class="sxs-lookup"><span data-stu-id="08083-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="08083-111">能够导出数据集并创建自定义报表，包括每个客户。</span><span class="sxs-lookup"><span data-stu-id="08083-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="08083-112">关于合作伙伴中心分析应用预览版</span><span class="sxs-lookup"><span data-stu-id="08083-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="08083-113">此应用仅适用于云解决方案提供商云解决方案提供商 (计划) 合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="08083-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="08083-114">CSP 中的其他合作伙伴（例如，间接经销商）将无法登录。</span><span class="sxs-lookup"><span data-stu-id="08083-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="08083-115">任何估算成本都是税前计费/发票数据，都不具有法律约束力。</span><span class="sxs-lookup"><span data-stu-id="08083-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="08083-116">估算成本只应用于数据洞察。</span><span class="sxs-lookup"><span data-stu-id="08083-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="08083-117">客户信息是以订阅为基础的。</span><span class="sxs-lookup"><span data-stu-id="08083-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="08083-118">最近创建帐户但尚未拥有订阅的任何客户不会包含在计数中。</span><span class="sxs-lookup"><span data-stu-id="08083-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="08083-119">估算成本基于最新费率卡，而它又基于 CSP 定价。</span><span class="sxs-lookup"><span data-stu-id="08083-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="08083-120">天为日历天。</span><span class="sxs-lookup"><span data-stu-id="08083-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="08083-121">业务洞察报告</span><span class="sxs-lookup"><span data-stu-id="08083-121">Business Insights report</span></span>

- <span data-ttu-id="08083-122">**客户租户**：已Azure Active Directory (Azure AD) 客户不同租户数</span><span class="sxs-lookup"><span data-stu-id="08083-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="08083-123">**新客户(最近 30 天)**：最近 30 天内购买至少一个订阅的新客户</span><span class="sxs-lookup"><span data-stu-id="08083-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="08083-124">**过去 (30** 天的流失) ：没有任何"活动"、"宽限期"或"已禁用"订阅的客户</span><span class="sxs-lookup"><span data-stu-id="08083-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="08083-125">**新客户(最近 24 小时)**：最近 24 小时内购买至少一个订阅的新客户</span><span class="sxs-lookup"><span data-stu-id="08083-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="08083-126">**过去 12 个月的估算月成本**：过去 12 个月期间每月累计估算税前发票美元金额环比趋势</span><span class="sxs-lookup"><span data-stu-id="08083-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08083-127">**过去 12 个月按产品排序的估算成本**：按过去 12 个月期间累计估算税前发票美元金额排序的售出产品。</span><span class="sxs-lookup"><span data-stu-id="08083-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="08083-128">此状态表示收入最多的主要产品。</span><span class="sxs-lookup"><span data-stu-id="08083-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="08083-129">**过去 12 个月的客户**：过去 12 个月期间每月累计新客户和改动客户的环比趋势</span><span class="sxs-lookup"><span data-stu-id="08083-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08083-130">**过去 12 个月按客户排序的估算成本**：按过去 12 个月期间累计估算税前发票美元金额排序的客户。</span><span class="sxs-lookup"><span data-stu-id="08083-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="08083-131">此状态表示收入最多的客户。</span><span class="sxs-lookup"><span data-stu-id="08083-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="08083-132">**按产品排序的客户计数**：按管理连客户排序的售出产品。</span><span class="sxs-lookup"><span data-stu-id="08083-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="08083-133">此状态表示向大多数客户销售的热门产品。</span><span class="sxs-lookup"><span data-stu-id="08083-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="08083-134">订阅洞察报告</span><span class="sxs-lookup"><span data-stu-id="08083-134">Subscription Insights report</span></span>

- <span data-ttu-id="08083-135">**订阅状态**：</span><span class="sxs-lookup"><span data-stu-id="08083-135">**Subscription status**:</span></span>

- <span data-ttu-id="08083-136">活动：属于"活动"或"宽限期"的订阅</span><span class="sxs-lookup"><span data-stu-id="08083-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="08083-137">已挂起：属于"已禁用"状态订阅</span><span class="sxs-lookup"><span data-stu-id="08083-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="08083-138">已取消预配：属于"已取消预配"或"已过期"状态的订阅</span><span class="sxs-lookup"><span data-stu-id="08083-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="08083-139">**过期状态**：</span><span class="sxs-lookup"><span data-stu-id="08083-139">**Expiry status**:</span></span>

  - <span data-ttu-id="08083-140">已过期：已过期（订阅结束日期处于过去）的订阅</span><span class="sxs-lookup"><span data-stu-id="08083-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="08083-141">30 天后过期：将在 30 天后过期的订阅（订阅结束日期在接下来的 30 天后）</span><span class="sxs-lookup"><span data-stu-id="08083-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="08083-142">30 天内过期：将在接下来的 30 天内过期的订阅（订阅结束日期在今天和接下来的 30 天之间）</span><span class="sxs-lookup"><span data-stu-id="08083-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="08083-143">**订阅总数**：处于"活动"、"已宽限期"或"已禁用"状态的订阅</span><span class="sxs-lookup"><span data-stu-id="08083-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="08083-144">**新订阅(最近 30 天)**：客户在最近 30 天内购买的新订阅</span><span class="sxs-lookup"><span data-stu-id="08083-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="08083-145">**新订阅(最近 24 小时)**：客户在最近 24 小时内购买的新订阅</span><span class="sxs-lookup"><span data-stu-id="08083-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="08083-146">**30 天内过期**：将在接下来的 30 天内过期的订阅</span><span class="sxs-lookup"><span data-stu-id="08083-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="08083-147">**过去 (30** 天内) 流失：过去 30 天内已取消预配或已 (已) 订阅</span><span class="sxs-lookup"><span data-stu-id="08083-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="08083-148">**按订阅类型分布**：按许可证和基于使用情况的订阅类型分配订阅总数的百分比</span><span class="sxs-lookup"><span data-stu-id="08083-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="08083-149">**按产品排序的活动订阅计数**：按活动订阅计数排序的售出产品</span><span class="sxs-lookup"><span data-stu-id="08083-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="08083-150">**过去 12 个月的订阅**：过去 12 个月期间每月累计新订阅和改动订阅的环比趋势</span><span class="sxs-lookup"><span data-stu-id="08083-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08083-151">**客户订阅详细信息**：客户、订阅和套餐的详细视图</span><span class="sxs-lookup"><span data-stu-id="08083-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="08083-152">许可证洞察报告：</span><span class="sxs-lookup"><span data-stu-id="08083-152">License Insights report:</span></span>

- <span data-ttu-id="08083-153">**许可证总数**：跨所有基于许可证的订阅聚合的许可证总数</span><span class="sxs-lookup"><span data-stu-id="08083-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="08083-154">**新(最近 30 天)**：最近 30 天内增加的许可证</span><span class="sxs-lookup"><span data-stu-id="08083-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="08083-155">**改动(最近 30 天)**：最近 30 天内减少的许可证</span><span class="sxs-lookup"><span data-stu-id="08083-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="08083-156">**新(最近 24 小时)**：最近 24 小时内增加的许可证</span><span class="sxs-lookup"><span data-stu-id="08083-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="08083-157">**过去 90 天内的许可证**：过去 90 天期间每月累计许可证增加和减少环比趋势</span><span class="sxs-lookup"><span data-stu-id="08083-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="08083-158">**按产品排序的活动许可证计数**：按活动许可证计数排序的售出产品</span><span class="sxs-lookup"><span data-stu-id="08083-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="08083-159">**按客户统计的活动许可证计数**：按活动许可证计数排序的客户</span><span class="sxs-lookup"><span data-stu-id="08083-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="08083-160">**过去 90** 天内的客户许可证事件详细信息：客户、订阅和订阅事件的详细视图，包括事件日期、事件名称、数量和数量变化。</span><span class="sxs-lookup"><span data-stu-id="08083-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="08083-161">许可证使用情况报告：</span><span class="sxs-lookup"><span data-stu-id="08083-161">Licenses Usage report:</span></span>

- <span data-ttu-id="08083-162">**按产品排序的已分配许可证**：按许可证分配计数排序的售出产品</span><span class="sxs-lookup"><span data-stu-id="08083-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="08083-163">**按产品排序的正在使用的许可证**：按许可证使用计数排序的产品</span><span class="sxs-lookup"><span data-stu-id="08083-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="08083-164">**已分配许可证的客户分布**：按许可证分配百分比的 20% 范围划分的客户总数百分比分布</span><span class="sxs-lookup"><span data-stu-id="08083-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="08083-165">**正在使用的许可证的客户分布**：按许可证使用情况百分比的 20% 范围划分的客户总数百分比分布</span><span class="sxs-lookup"><span data-stu-id="08083-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="08083-166">**按客户排序的已分配许可证**：按客户和产品排序的售出许可证和已分配许可证的详细视图</span><span class="sxs-lookup"><span data-stu-id="08083-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="08083-167">**按客户排序的正在使用的许可证**：按客户和产品排序的售出许可证和正在使用的许可证的详细视图</span><span class="sxs-lookup"><span data-stu-id="08083-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="08083-168">Azure 洞察报告：</span><span class="sxs-lookup"><span data-stu-id="08083-168">Azure Insights report:</span></span>

- <span data-ttu-id="08083-169">**过去 12** 个月基于使用情况的客户：过去 12 个月内每月聚合的基于使用情况的新客户和基于使用量的客户每月趋势</span><span class="sxs-lookup"><span data-stu-id="08083-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08083-170">**过去 12** 个月基于使用情况的订阅：过去 12 个月内每月聚合的基于使用情况的新订阅和流失的基于使用情况的订阅的月份趋势</span><span class="sxs-lookup"><span data-stu-id="08083-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08083-171">**过去 60** 天内客户使用的估计成本：基于使用情况的客户，按过去 60 天内聚合的税前发票金额估算排序。</span><span class="sxs-lookup"><span data-stu-id="08083-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="08083-172">此状态表示基于使用情况的客户收入最高</span><span class="sxs-lookup"><span data-stu-id="08083-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="08083-173">**过去 60** 天内按类别估算的使用成本：基于使用情况的订阅的计量类别，按过去 60 天内聚合的税前发票美元金额估算排序。</span><span class="sxs-lookup"><span data-stu-id="08083-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="08083-174">**过去 60** 天内按订阅估算的使用成本：基于使用情况的订阅，按过去 60 天内聚合的税前发票美元金额估算。</span><span class="sxs-lookup"><span data-stu-id="08083-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="08083-175">**按费用预算排序的客户估算使用成本**：按当前使用费用预算超出阈值 (100%) 的百分比排序的客户。</span><span class="sxs-lookup"><span data-stu-id="08083-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="08083-176">Azure 资源使用情况报告：</span><span class="sxs-lookup"><span data-stu-id="08083-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="08083-177">**所选时段的按** 天使用 Azure 资源：过去 60 天内每个基于使用情况的订阅中每个按用量计费的资源的每日消耗单位。</span><span class="sxs-lookup"><span data-stu-id="08083-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="08083-178">**所选时段的 Azure** 资源估计使用成本：基于最近 60 天内每个基于使用情况的订阅中每个按流量计费的资源的最新费率卡估算的成本。</span><span class="sxs-lookup"><span data-stu-id="08083-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="08083-179">后续步骤</span><span class="sxs-lookup"><span data-stu-id="08083-179">Next steps</span></span>

- [<span data-ttu-id="08083-180">适用于 Power BI 的合作伙伴中心分析应用概述</span><span class="sxs-lookup"><span data-stu-id="08083-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="08083-181">安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用</span><span class="sxs-lookup"><span data-stu-id="08083-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
