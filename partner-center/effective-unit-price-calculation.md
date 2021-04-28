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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172211"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="11d68-104">Azure 计划消耗量的有效单位价格计算</span><span class="sxs-lookup"><span data-stu-id="11d68-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="11d68-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="11d68-105">**Appropriate roles**</span></span>

- <span data-ttu-id="11d68-106">计费管理员</span><span class="sxs-lookup"><span data-stu-id="11d68-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="11d68-107">有效单位价格</span><span class="sxs-lookup"><span data-stu-id="11d68-107">The effective unit price</span></span>

<span data-ttu-id="11d68-108">有效单位价格在计量级别 (相对于资源级别) 计算，根据计量使用情况进行调整。</span><span class="sxs-lookup"><span data-stu-id="11d68-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="11d68-109">我们使用以下三个因素来计算有效单位价格：</span><span class="sxs-lookup"><span data-stu-id="11d68-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="11d68-110">消耗，在整个计费周期中每天监视</span><span class="sxs-lookup"><span data-stu-id="11d68-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="11d68-111">计量的计费成本</span><span class="sxs-lookup"><span data-stu-id="11d68-111">Billable cost for the meter</span></span>
- <span data-ttu-id="11d68-112">分层 (（如果适用）) </span><span class="sxs-lookup"><span data-stu-id="11d68-112">Tiering (if applicable)</span></span>

<span data-ttu-id="11d68-113">由于我们会在整个计费周期内监视消耗，因此有效单位价格将会波动。</span><span class="sxs-lookup"><span data-stu-id="11d68-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="11d68-114">在停止消耗计算并关闭计费周期后，给定计费周期的最终价格将可用。</span><span class="sxs-lookup"><span data-stu-id="11d68-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="11d68-115">在第四个或第五个小数位之后，您将看到大部分使用量的变化。</span><span class="sxs-lookup"><span data-stu-id="11d68-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="11d68-116">了解计量器是否使用分层定价</span><span class="sxs-lookup"><span data-stu-id="11d68-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="11d68-117">如果你不知道计量器是否使用分层定价，请使用以下过程来了解。</span><span class="sxs-lookup"><span data-stu-id="11d68-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="11d68-118">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="11d68-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="11d68-119">选择 " **销售**"，选择 **定价和产品/服务**，然后选择 " **Azure 计划定价**"。</span><span class="sxs-lookup"><span data-stu-id="11d68-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="11d68-120">按 ID 查找计量器，然后下载定价数据。</span><span class="sxs-lookup"><span data-stu-id="11d68-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="11d68-121">示例计算</span><span class="sxs-lookup"><span data-stu-id="11d68-121">Sample calculation</span></span>

<span data-ttu-id="11d68-122">下表提供了一个示例，说明如何在开放期间计算有效单价。</span><span class="sxs-lookup"><span data-stu-id="11d68-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="11d68-123">在表中，以下值适用：</span><span class="sxs-lookup"><span data-stu-id="11d68-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="11d68-124">**向上** = 资源的单价 = 0.868</span><span class="sxs-lookup"><span data-stu-id="11d68-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="11d68-125">**BCU** = 计量的计费消耗单位</span><span class="sxs-lookup"><span data-stu-id="11d68-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="11d68-126">**BC** = 计量器的计费成本 = BCU \* UP \* 0.85。</span><span class="sxs-lookup"><span data-stu-id="11d68-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="11d68-127">这反映了 15% PEC 折扣的调整。</span><span class="sxs-lookup"><span data-stu-id="11d68-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="11d68-128">然后，使用函数的下限将该值限制为小数点后两位的数字，以便对最小值进行计费。</span><span class="sxs-lookup"><span data-stu-id="11d68-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="11d68-129">**有效单价** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="11d68-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="11d68-130">注意：在此示例中，此指标没有按定价百分比或其他价格计算的有效单位价格系数。</span><span class="sxs-lookup"><span data-stu-id="11d68-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="11d68-131">日期</span><span class="sxs-lookup"><span data-stu-id="11d68-131">Date</span></span> | <span data-ttu-id="11d68-132">BCU (计费消耗单位) </span><span class="sxs-lookup"><span data-stu-id="11d68-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="11d68-133">BC (计费成本) </span><span class="sxs-lookup"><span data-stu-id="11d68-133">BC (Billable cost)</span></span> | <span data-ttu-id="11d68-134">有效单价</span><span class="sxs-lookup"><span data-stu-id="11d68-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="11d68-135">3-8 月</span><span class="sxs-lookup"><span data-stu-id="11d68-135">3-Aug</span></span> | <span data-ttu-id="11d68-136">29</span><span class="sxs-lookup"><span data-stu-id="11d68-136">29</span></span> | <span data-ttu-id="11d68-137">21.39</span><span class="sxs-lookup"><span data-stu-id="11d68-137">21.39</span></span> | <span data-ttu-id="11d68-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="11d68-138">0.737586206896552</span></span> |
| <span data-ttu-id="11d68-139">10-8 月</span><span class="sxs-lookup"><span data-stu-id="11d68-139">10-Aug</span></span> | <span data-ttu-id="11d68-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="11d68-140">210.950039</span></span> | <span data-ttu-id="11d68-141">155.63</span><span class="sxs-lookup"><span data-stu-id="11d68-141">155.63</span></span> | <span data-ttu-id="11d68-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="11d68-142">0.737757626107858</span></span> |
| <span data-ttu-id="11d68-143">25-8 月</span><span class="sxs-lookup"><span data-stu-id="11d68-143">25-Aug</span></span> | <span data-ttu-id="11d68-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="11d68-144">555.950039</span></span> | <span data-ttu-id="11d68-145">410.17</span><span class="sxs-lookup"><span data-stu-id="11d68-145">410.17</span></span> | <span data-ttu-id="11d68-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="11d68-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="11d68-147">后续步骤</span><span class="sxs-lookup"><span data-stu-id="11d68-147">Next steps</span></span>

- [<span data-ttu-id="11d68-148">计费和税款</span><span class="sxs-lookup"><span data-stu-id="11d68-148">Billing and taxes</span></span>](billing.md)
