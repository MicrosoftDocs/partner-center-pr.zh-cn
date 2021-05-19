---
title: 使用订阅见解分析
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心使用分析来更好地了解你的业务，以及你的客户如何使用你购买的许可证。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7dab3469b885f693ba8498e8a07eb120b8f07021
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147201"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a><span data-ttu-id="54770-103">使用分析了解有关订阅收入的详细信息</span><span class="sxs-lookup"><span data-stu-id="54770-103">Use analytics to learn more about subscription revenue</span></span>

<span data-ttu-id="54770-104">**适当的角色**：全局管理员 |MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="54770-104">**Appropriate roles**: Global admin | MPN partner admin</span></span>

<span data-ttu-id="54770-105">规划各种方式来发展 CSP 业务，包括了解客户使用其 Microsoft 产品的方式。</span><span class="sxs-lookup"><span data-stu-id="54770-105">Planning ways to develop your CSP business includes understanding how your customers use their Microsoft products.</span></span> <span data-ttu-id="54770-106">合作伙伴中心中有多个用于收集数据的选项，可以收集有关你的业务的数据，还可以收集你的客户是否在使用以及如何使用所购买的许可证的数据。</span><span class="sxs-lookup"><span data-stu-id="54770-106">You have several options for gathering data in Partner Center, and you can gather data on both your business and on if and how your customers are using the licenses they've purchased.</span></span> <span data-ttu-id="54770-107">如果你使用的是 CSP 直接模式，则还可以安装并使用合作伙伴中心分析应用，以便 Power BI 收集额外数据。</span><span class="sxs-lookup"><span data-stu-id="54770-107">If you are in the CSP direct model, you also have the opportunity to install and use the Partner Center Analytics app for Power BI to gather additional data.</span></span>

## <a name="access-to-the-subscription-analytics"></a><span data-ttu-id="54770-108">访问订阅分析</span><span class="sxs-lookup"><span data-stu-id="54770-108">Access to the Subscription Analytics</span></span>

1. <span data-ttu-id="54770-109">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="54770-109">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>
1. <span data-ttu-id="54770-110">在 "合作伙伴中心" 菜单中，选择 " **分析**"，然后选择 " **订阅分析**"。</span><span class="sxs-lookup"><span data-stu-id="54770-110">From CSP in the Partner Center menu, select **Analyze**, and then select **Subscription analytics**.</span></span>

1. <span data-ttu-id="54770-111">在页面顶部会显示尾随的十二个月的 CSP 收入</span><span class="sxs-lookup"><span data-stu-id="54770-111">The trailing twelve-month CSP revenue will be displayed at the top of the page</span></span>

:::image type="content" source="images/analytics/subscription1.png" alt-text="订阅屏幕":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a><span data-ttu-id="54770-113">尾随 Twelve-Month (TTM) CSP 收入</span><span class="sxs-lookup"><span data-stu-id="54770-113">Trailing Twelve-Month (TTM) CSP Revenue</span></span>

<span data-ttu-id="54770-114">尾随12个月的 CSP 收入代表合作伙伴全局帐户级别的在 USD 中的尾随云解决方案提供商计划收入。</span><span class="sxs-lookup"><span data-stu-id="54770-114">Trailing 12-month CSP revenue represents the trailing Cloud Solution Provider program revenue in USD at a Partner Global Account level.</span></span> <span data-ttu-id="54770-115">数据将在每月的第八个月刷新，以显示前个月之前的12个月的尾随收入。</span><span class="sxs-lookup"><span data-stu-id="54770-115">The data is refreshed on the eighth of every month, to display the trailing twelve-month revenue until the prior month.</span></span> <span data-ttu-id="54770-116">例如，在 9 2020 月9日，你应该能够看到 TTM 的固定时间段上午9月2019到8月2020。</span><span class="sxs-lookup"><span data-stu-id="54770-116">For example, on 9 September 2020, you should be able to see the TTM for the fixed period of September 2019 to August 2020.</span></span>

<span data-ttu-id="54770-117">合作伙伴中心显示的收入是按12个月的固定时间间隔计算的，不能修改为更短的时间范围。</span><span class="sxs-lookup"><span data-stu-id="54770-117">The revenue displayed on Partner Center is calculated for a fixed time interval of 12 months, and cannot be modified to a shorter time frame.</span></span>

<span data-ttu-id="54770-118">若要查看合作伙伴位置帐户级别的收入细目：</span><span class="sxs-lookup"><span data-stu-id="54770-118">To see a breakdown of the revenue at your Partner Location Account level:</span></span>

- <span data-ttu-id="54770-119">选择 "下载详细信息" 链接并下载一个 tsv 文件，其中显示了所有位置的 TTM 收入。</span><span class="sxs-lookup"><span data-stu-id="54770-119">Select the ‘Download Details’ link and download a .tsv file that displays the TTM revenue across all your locations.</span></span>

>[!NOTE] 
><span data-ttu-id="54770-120">在 tsv 文件中跨 MPN Id 汇总单独的 TTM 收入数字可能看起来比你在合作伙伴中心显示的总体 TTM 收入大。</span><span class="sxs-lookup"><span data-stu-id="54770-120">Summing up the individual TTM Revenue numbers across MPN IDs in the .tsv file may appear to be greater than the overall TTM revenue you see displayed on Partner Center.</span></span> <span data-ttu-id="54770-121">这是因为在下载的文件中，可能会为具有多个合作伙伴归属的订阅计算收入。</span><span class="sxs-lookup"><span data-stu-id="54770-121">This is because the revenue may be double counted for subscriptions with multiple partner attributions in the downloaded file.</span></span>

## <a name="subscription-summary"></a><span data-ttu-id="54770-122">订阅摘要</span><span class="sxs-lookup"><span data-stu-id="54770-122">Subscription Summary</span></span>

<span data-ttu-id="54770-123">屏幕的下半部分显示订阅摘要。</span><span class="sxs-lookup"><span data-stu-id="54770-123">The lower half of the screen displays a summary of the subscriptions.</span></span> <span data-ttu-id="54770-124">使用以下筛选器查看必要的订阅详细信息：</span><span class="sxs-lookup"><span data-stu-id="54770-124">Use the following filters to see the necessary subscription details:</span></span>  

1. <span data-ttu-id="54770-125">**持续时间**：可以选择查看的订阅摘要</span><span class="sxs-lookup"><span data-stu-id="54770-125">**Duration**: You may opt to see the subscription summary for</span></span> 

- <span data-ttu-id="54770-126">30D – 过去 30 天</span><span class="sxs-lookup"><span data-stu-id="54770-126">30D – Last 30 days</span></span>
- <span data-ttu-id="54770-127">3M – 过去 3 个月</span><span class="sxs-lookup"><span data-stu-id="54770-127">3M – Last 3 months</span></span>
- <span data-ttu-id="54770-128">6M – 过去 6 个月</span><span class="sxs-lookup"><span data-stu-id="54770-128">6M – Last 6 months</span></span>
- <span data-ttu-id="54770-129">12M – 过去 12 个月</span><span class="sxs-lookup"><span data-stu-id="54770-129">12M – Last 12 months</span></span>

2. <span data-ttu-id="54770-130">**产品类型**：</span><span class="sxs-lookup"><span data-stu-id="54770-130">**Product Type**:</span></span>
 
- <span data-ttu-id="54770-131">Office 365</span><span class="sxs-lookup"><span data-stu-id="54770-131">Office 365</span></span>
- <span data-ttu-id="54770-132">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="54770-132">Microsoft 365</span></span>
- <span data-ttu-id="54770-133">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="54770-133">Dynamics 365</span></span>
- <span data-ttu-id="54770-134">EMS</span><span class="sxs-lookup"><span data-stu-id="54770-134">EMS</span></span>

<span data-ttu-id="54770-135">应用这些筛选器不会影响此报表顶部的 TTM 收入指标。</span><span class="sxs-lookup"><span data-stu-id="54770-135">Applying these filters will not impact the TTM revenue metric at the top of this report.</span></span>


 
## <a name="next-steps"></a><span data-ttu-id="54770-136">后续步骤</span><span class="sxs-lookup"><span data-stu-id="54770-136">Next steps</span></span>

- [<span data-ttu-id="54770-137">分析客户如何使用他们购买的许可证</span><span class="sxs-lookup"><span data-stu-id="54770-137">Analyze how your customers are using the licenses they purchased</span></span>](increasing-adoption-and-satisfaction.md)  
- [<span data-ttu-id="54770-138">查看客户活动日志</span><span class="sxs-lookup"><span data-stu-id="54770-138">View customer activity logs</span></span>](activity-logs.md)
- [<span data-ttu-id="54770-139">适用于 Power BI 的合作伙伴中心分析应用</span><span class="sxs-lookup"><span data-stu-id="54770-139">Partner Center Analytics app for Power BI</span></span>](power-bi-app-for-direct-partners.md)






