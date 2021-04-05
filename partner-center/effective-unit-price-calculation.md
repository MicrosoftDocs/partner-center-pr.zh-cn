---
title: 有效单价计算
ms.topic: how-to
ms.date: 04/02/2021
description: 了解有效单价及其计算方式。 本文还包括一个示例计算。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374378"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="29802-104">Azure 计划消耗量的有效单位价格计算</span><span class="sxs-lookup"><span data-stu-id="29802-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="29802-105">有效单位价格</span><span class="sxs-lookup"><span data-stu-id="29802-105">The effective unit price</span></span>

<span data-ttu-id="29802-106">有效单位价格在计量级别 (相对于资源级别) 计算，根据计量使用情况进行调整。</span><span class="sxs-lookup"><span data-stu-id="29802-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="29802-107">我们使用以下三个因素来计算有效单位价格：</span><span class="sxs-lookup"><span data-stu-id="29802-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="29802-108">消耗，在整个计费周期中每天监视</span><span class="sxs-lookup"><span data-stu-id="29802-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="29802-109">计量的计费成本</span><span class="sxs-lookup"><span data-stu-id="29802-109">Billable cost for the meter</span></span>
- <span data-ttu-id="29802-110">分层 (（如果适用）) </span><span class="sxs-lookup"><span data-stu-id="29802-110">Tiering (if applicable)</span></span>

<span data-ttu-id="29802-111">由于我们会在整个计费周期内监视消耗，因此有效单位价格将会波动。</span><span class="sxs-lookup"><span data-stu-id="29802-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="29802-112">在停止消耗计算并关闭计费周期后，给定计费周期的最终价格将可用。</span><span class="sxs-lookup"><span data-stu-id="29802-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="29802-113">在第四个或第五个小数位之后，您将看到大部分使用量的变化。</span><span class="sxs-lookup"><span data-stu-id="29802-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="29802-114">了解计量器是否使用分层定价</span><span class="sxs-lookup"><span data-stu-id="29802-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="29802-115">如果你不知道计量器是否使用分层定价，请使用以下过程来了解。</span><span class="sxs-lookup"><span data-stu-id="29802-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="29802-116">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="29802-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="29802-117">选择 " **销售**"，选择 **定价和产品/服务**，然后选择 " **Azure 计划定价**"。</span><span class="sxs-lookup"><span data-stu-id="29802-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="29802-118">按 ID 查找计量器，然后下载定价数据。</span><span class="sxs-lookup"><span data-stu-id="29802-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="29802-119">示例计算</span><span class="sxs-lookup"><span data-stu-id="29802-119">Sample calculation</span></span>

<span data-ttu-id="29802-120">下表提供了一个示例，说明如何在开放期间计算有效单价。</span><span class="sxs-lookup"><span data-stu-id="29802-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="29802-121">在表中，以下值适用：</span><span class="sxs-lookup"><span data-stu-id="29802-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="29802-122">**向上** = 资源的单价 = 0.868</span><span class="sxs-lookup"><span data-stu-id="29802-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="29802-123">**BCU** = 计量的计费消耗单位</span><span class="sxs-lookup"><span data-stu-id="29802-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="29802-124">**BC** = 计量器的计费成本 = BCU \* UP \* 0.85。</span><span class="sxs-lookup"><span data-stu-id="29802-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="29802-125">这反映了 15% PEC 折扣的调整。</span><span class="sxs-lookup"><span data-stu-id="29802-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="29802-126">然后，使用函数的下限将该值限制为小数点后两位的数字，以便对最小值进行计费。</span><span class="sxs-lookup"><span data-stu-id="29802-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="29802-127">**有效单价** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="29802-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="29802-128">此示例中的计量器没有定价层。</span><span class="sxs-lookup"><span data-stu-id="29802-128">The meter in this example does not have tiers in pricing.</span></span> <span data-ttu-id="29802-129">折扣百分比和其他调整中的有效单位价格系数。</span><span class="sxs-lookup"><span data-stu-id="29802-129">The Effective Unit Price factors in discount percentages and other adjustments.</span></span>

| <span data-ttu-id="29802-130">日期</span><span class="sxs-lookup"><span data-stu-id="29802-130">Date</span></span> | <span data-ttu-id="29802-131">BCU (计费消耗单位) </span><span class="sxs-lookup"><span data-stu-id="29802-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="29802-132">BC (计费成本) </span><span class="sxs-lookup"><span data-stu-id="29802-132">BC (Billable cost)</span></span> | <span data-ttu-id="29802-133">有效单价</span><span class="sxs-lookup"><span data-stu-id="29802-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="29802-134">3-8 月</span><span class="sxs-lookup"><span data-stu-id="29802-134">3-Aug</span></span> | <span data-ttu-id="29802-135">29</span><span class="sxs-lookup"><span data-stu-id="29802-135">29</span></span> | <span data-ttu-id="29802-136">21.39</span><span class="sxs-lookup"><span data-stu-id="29802-136">21.39</span></span> | <span data-ttu-id="29802-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="29802-137">0.737586206896552</span></span> |
| <span data-ttu-id="29802-138">10-8 月</span><span class="sxs-lookup"><span data-stu-id="29802-138">10-Aug</span></span> | <span data-ttu-id="29802-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="29802-139">210.950039</span></span> | <span data-ttu-id="29802-140">155.63</span><span class="sxs-lookup"><span data-stu-id="29802-140">155.63</span></span> | <span data-ttu-id="29802-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="29802-141">0.737757626107858</span></span> |
| <span data-ttu-id="29802-142">25-8 月</span><span class="sxs-lookup"><span data-stu-id="29802-142">25-Aug</span></span> | <span data-ttu-id="29802-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="29802-143">555.950039</span></span> | <span data-ttu-id="29802-144">410.17</span><span class="sxs-lookup"><span data-stu-id="29802-144">410.17</span></span> | <span data-ttu-id="29802-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="29802-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="29802-146">后续步骤</span><span class="sxs-lookup"><span data-stu-id="29802-146">Next steps</span></span>

- [<span data-ttu-id="29802-147">计费和税款</span><span class="sxs-lookup"><span data-stu-id="29802-147">Billing and taxes</span></span>](billing.md)
