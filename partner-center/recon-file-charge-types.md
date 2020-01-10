---
title: 对帐文件费用类型 |合作伙伴中心
ms.topic: article
ms.date: 01/06/2020
description: 合作伙伴中心对帐文件的费用类型（基于许可证、基于使用情况的和一次性）、信用额度和折扣。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b18a2a7d53e2f9d35baac2412c1710c21d6d98eb
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716868"
---
# <a name="understand-charge-types"></a><span data-ttu-id="2b40e-103">了解费用类型</span><span class="sxs-lookup"><span data-stu-id="2b40e-103">Understand charge types</span></span>

<span data-ttu-id="2b40e-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="2b40e-104">**Applies to**</span></span>

- <span data-ttu-id="2b40e-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2b40e-105">Partner Center</span></span>
- <span data-ttu-id="2b40e-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2b40e-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="2b40e-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="2b40e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="2b40e-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="2b40e-108">Admin agent</span></span>
- <span data-ttu-id="2b40e-109">帐单管理员</span><span class="sxs-lookup"><span data-stu-id="2b40e-109">Billing admin</span></span>
- <span data-ttu-id="2b40e-110">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2b40e-110">Global admin</span></span>

<span data-ttu-id="2b40e-111">本主题介绍了发票部分与可能在对帐文件上的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="2b40e-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="2b40e-112">发票提供费用的摘要。</span><span class="sxs-lookup"><span data-stu-id="2b40e-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="2b40e-113">你的对帐文件提供行项事务的详细细分，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="2b40e-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="2b40e-114">有关对帐文件的详细信息，请参阅[如何使用协调文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="2b40e-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="2b40e-115">[基于使用情况的对帐文件](usage-based-recon-files.md)和[基于许可证的对帐文件](license-based-recon-files.md)只显示与使用相关的事务和费用（单位消耗和相关费用）。</span><span class="sxs-lookup"><span data-stu-id="2b40e-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="2b40e-116">在发票上作为**调整**显示的一次性信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="2b40e-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="2b40e-117">将费用类型映射到发票费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="2b40e-118">若要在发票和对帐文件之间交叉引用费用量，请使用 Microsoft Excel 中的筛选器选项。</span><span class="sxs-lookup"><span data-stu-id="2b40e-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="2b40e-119">按对帐文件上的费用类型进行筛选，以将发票费用映射到对帐文件上的一组费用细分。</span><span class="sxs-lookup"><span data-stu-id="2b40e-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="2b40e-120">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-120">License-based charges</span></span>

<span data-ttu-id="2b40e-121">若要将这些基于许可证的费用映射到发票，请对基于许可证的文件中的 "**金额**" 列求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="2b40e-122">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="2b40e-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="2b40e-123">收费说明</span><span class="sxs-lookup"><span data-stu-id="2b40e-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="2b40e-124">激活费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-124">Activation fee</span></span> | <span data-ttu-id="2b40e-125">客户在购买后使用订阅时向客户收取的费用。</span><span class="sxs-lookup"><span data-stu-id="2b40e-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="2b40e-126">取消费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-126">Cancel fee</span></span> | <span data-ttu-id="2b40e-127">当关联的座位发生变化时，将向客户退还按比例计费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="2b40e-128">取消实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="2b40e-128">Cancel instance prorate</span></span> | <span data-ttu-id="2b40e-129">按月订阅的客户在同一月内暂停订阅并更改关联座位时，按比例计费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-129">Prorated charges cancelled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="2b40e-130">周期费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-130">Cycle fee</span></span> | <span data-ttu-id="2b40e-131">订阅的定期收费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="2b40e-132">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="2b40e-132">Cycle instance prorate</span></span> | <span data-ttu-id="2b40e-133">相关座位发生变化时，从客户评估的按比例计费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="2b40e-134">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-134">Prorate fees when cancel</span></span> | <span data-ttu-id="2b40e-135">取消时，未使用的服务部分按比例退款。</span><span class="sxs-lookup"><span data-stu-id="2b40e-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="2b40e-136">转换远离当前产品/服务的按比例计算费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="2b40e-137">从当前月度订阅转换为年度订阅后按比例计费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="2b40e-138">转换为新产品/服务时的按比例计算费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="2b40e-139">将月度订阅转换为新年度订阅后按比例计费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="2b40e-140">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-140">Prorate fees when purchase</span></span> | <span data-ttu-id="2b40e-141">使用年度计费时的订阅费用类型。</span><span class="sxs-lookup"><span data-stu-id="2b40e-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="2b40e-142">购买费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-142">Purchase fee</span></span> | <span data-ttu-id="2b40e-143">使用月度帐单时的订阅费用类型。</span><span class="sxs-lookup"><span data-stu-id="2b40e-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="2b40e-144">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-144">Prorate fee when renew</span></span> | <span data-ttu-id="2b40e-145">订阅续订时按比例计费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="2b40e-146">续订费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-146">Renew fee</span></span> | <span data-ttu-id="2b40e-147">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="2b40e-148">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-148">Prorate fees when activate</span></span> | <span data-ttu-id="2b40e-149">从激活 > 按比例计费，直到计费期结束。</span><span class="sxs-lookup"><span data-stu-id="2b40e-149">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="2b40e-150">一次性费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-150">One-time charges</span></span>

<span data-ttu-id="2b40e-151">若要将这些一次性费用映射到你的发票，请对基于许可证的文件中的 "**金额**" 列求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="2b40e-152">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="2b40e-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="2b40e-153">收费说明</span><span class="sxs-lookup"><span data-stu-id="2b40e-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="2b40e-154">“新建”</span><span class="sxs-lookup"><span data-stu-id="2b40e-154">New</span></span> | <span data-ttu-id="2b40e-155">创建新购买时使用。</span><span class="sxs-lookup"><span data-stu-id="2b40e-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="2b40e-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="2b40e-156">addQuantity</span></span> | <span data-ttu-id="2b40e-157">用于原始购买的退款和增加后的新数量。</span><span class="sxs-lookup"><span data-stu-id="2b40e-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="2b40e-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="2b40e-158">removeQuantity</span></span> | <span data-ttu-id="2b40e-159">用于原始购买的退款和减少后的新数量。</span><span class="sxs-lookup"><span data-stu-id="2b40e-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="2b40e-160">“取消”</span><span class="sxs-lookup"><span data-stu-id="2b40e-160">Cancel</span></span> | <span data-ttu-id="2b40e-161">取消订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="2b40e-161">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="2b40e-162">转换</span><span class="sxs-lookup"><span data-stu-id="2b40e-162">Convert</span></span> | <span data-ttu-id="2b40e-163">升级许可证时使用，但座位数保持不变。</span><span class="sxs-lookup"><span data-stu-id="2b40e-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="2b40e-164">使用情况费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-164">Usage charges</span></span>

<span data-ttu-id="2b40e-165">若要将这些用量费用映射到发票，请将**PretaxCharges**列与基于使用情况的文件进行求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="2b40e-166">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="2b40e-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="2b40e-167">收费说明</span><span class="sxs-lookup"><span data-stu-id="2b40e-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="2b40e-168">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="2b40e-169">在已取消的情况下的访问使用费，针对当前计费周期的未付款使用量。</span><span class="sxs-lookup"><span data-stu-id="2b40e-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="2b40e-170">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="2b40e-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="2b40e-171">当前计费周期的访问使用费。</span><span class="sxs-lookup"><span data-stu-id="2b40e-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="2b40e-172">退款额</span><span class="sxs-lookup"><span data-stu-id="2b40e-172">Credits</span></span>

<span data-ttu-id="2b40e-173">若要将这些信用额度映射到发票：</span><span class="sxs-lookup"><span data-stu-id="2b40e-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="2b40e-174">对基于许可证的文件中的**TotalForCustomer**求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="2b40e-175">在基于使用情况的文件中对**PostTaxTotal**列求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="2b40e-176">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="2b40e-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="2b40e-177">收费说明</span><span class="sxs-lookup"><span data-stu-id="2b40e-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="2b40e-178">偏移行项</span><span class="sxs-lookup"><span data-stu-id="2b40e-178">Offset a line item</span></span> | <span data-ttu-id="2b40e-179">对某个行项的部分或全部退款，包括税款。</span><span class="sxs-lookup"><span data-stu-id="2b40e-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="2b40e-180">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="2b40e-180">Usage-based discounts</span></span>

<span data-ttu-id="2b40e-181">若要将基于使用情况的折扣映射到发票，请对基于使用情况的文件中的**PretaxCharges**列求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="2b40e-182">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="2b40e-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="2b40e-183">收费说明</span><span class="sxs-lookup"><span data-stu-id="2b40e-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="2b40e-184">激活折扣</span><span class="sxs-lookup"><span data-stu-id="2b40e-184">Activation discount</span></span> | <span data-ttu-id="2b40e-185">激活订阅后应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="2b40e-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="2b40e-186">周期折扣</span><span class="sxs-lookup"><span data-stu-id="2b40e-186">Cycle discount</span></span> | <span data-ttu-id="2b40e-187">应用在周期性费用上的折扣。</span><span class="sxs-lookup"><span data-stu-id="2b40e-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="2b40e-188">续订折扣</span><span class="sxs-lookup"><span data-stu-id="2b40e-188">Renew discount</span></span> | <span data-ttu-id="2b40e-189">续订订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="2b40e-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="2b40e-190">取消折扣</span><span class="sxs-lookup"><span data-stu-id="2b40e-190">Cancel discount</span></span> | <span data-ttu-id="2b40e-191">取消折扣后应用的费用。</span><span class="sxs-lookup"><span data-stu-id="2b40e-191">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="2b40e-192">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="2b40e-192">License-based discounts</span></span>

<span data-ttu-id="2b40e-193">若要将基于许可证的折扣映射到发票，请对基于许可证的文件中的**TotalOtherDiscount**列求和。</span><span class="sxs-lookup"><span data-stu-id="2b40e-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="2b40e-194">*基于许可证的折扣可以应用于多种费用类型。*</span><span class="sxs-lookup"><span data-stu-id="2b40e-194">*License-based discounts may be applied to multiple charge types.*</span></span>
