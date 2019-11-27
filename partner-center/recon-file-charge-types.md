---
title: 对帐文件费用类型 |合作伙伴中心
ms.topic: article
ms.date: 08/26/2019
description: 合作伙伴中心对帐文件的费用类型（基于许可证、基于使用情况的和一次性）、信用额度和折扣。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389805"
---
# <a name="understand-charge-types"></a><span data-ttu-id="010e4-103">了解费用类型</span><span class="sxs-lookup"><span data-stu-id="010e4-103">Understand charge types</span></span>

<span data-ttu-id="010e4-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="010e4-104">Applies to:</span></span>

- <span data-ttu-id="010e4-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="010e4-105">Partner Center</span></span>
- <span data-ttu-id="010e4-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="010e4-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="010e4-107">本主题介绍了发票部分与可能在对帐文件上的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="010e4-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="010e4-108">发票提供费用的摘要。</span><span class="sxs-lookup"><span data-stu-id="010e4-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="010e4-109">你的对帐文件提供行项事务的详细细分，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="010e4-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="010e4-110">有关对帐文件的详细信息，请参阅[如何使用协调文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="010e4-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="010e4-111">[基于使用情况的对帐文件](usage-based-recon-files.md)和[基于许可证的对帐文件](license-based-recon-files.md)只显示与使用相关的事务和费用（单位消耗和相关费用）。</span><span class="sxs-lookup"><span data-stu-id="010e4-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="010e4-112">在发票上作为**调整**显示的一次性信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="010e4-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="010e4-113">将费用类型映射到发票费用</span><span class="sxs-lookup"><span data-stu-id="010e4-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="010e4-114">若要在发票和对帐文件之间交叉引用费用量，请使用 Microsoft Excel 中的筛选器选项。</span><span class="sxs-lookup"><span data-stu-id="010e4-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="010e4-115">按对帐文件上的费用类型进行筛选，以将发票费用映射到对帐文件上的一组费用细分。</span><span class="sxs-lookup"><span data-stu-id="010e4-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="010e4-116">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="010e4-116">License-based charges</span></span>

<span data-ttu-id="010e4-117">若要将这些基于许可证的费用映射到发票，请对基于许可证的文件中的 "**金额**" 列求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="010e4-118">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="010e4-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="010e4-119">收费说明</span><span class="sxs-lookup"><span data-stu-id="010e4-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="010e4-120">激活费用</span><span class="sxs-lookup"><span data-stu-id="010e4-120">Activation fee</span></span> | <span data-ttu-id="010e4-121">客户在购买后使用订阅时向客户收取的费用。</span><span class="sxs-lookup"><span data-stu-id="010e4-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="010e4-122">取消费用</span><span class="sxs-lookup"><span data-stu-id="010e4-122">Cancel fee</span></span> | <span data-ttu-id="010e4-123">当关联的座位发生变化时，将向客户退还按比例计费。</span><span class="sxs-lookup"><span data-stu-id="010e4-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="010e4-124">周期费用</span><span class="sxs-lookup"><span data-stu-id="010e4-124">Cycle fee</span></span> | <span data-ttu-id="010e4-125">订阅的定期收费。</span><span class="sxs-lookup"><span data-stu-id="010e4-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="010e4-126">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="010e4-126">Cycle instance prorate</span></span> | <span data-ttu-id="010e4-127">相关座位发生变化时，从客户评估的按比例计费。</span><span class="sxs-lookup"><span data-stu-id="010e4-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="010e4-128">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="010e4-128">Prorate fees when cancel</span></span> | <span data-ttu-id="010e4-129">取消时，未使用的服务部分按比例退款。</span><span class="sxs-lookup"><span data-stu-id="010e4-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="010e4-130">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="010e4-130">Prorate fees when purchase</span></span> | <span data-ttu-id="010e4-131">使用年度计费时的订阅费用类型。</span><span class="sxs-lookup"><span data-stu-id="010e4-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="010e4-132">购买费用</span><span class="sxs-lookup"><span data-stu-id="010e4-132">Purchase fee</span></span> | <span data-ttu-id="010e4-133">使用月度帐单时的订阅费用类型。</span><span class="sxs-lookup"><span data-stu-id="010e4-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="010e4-134">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="010e4-134">Prorate fee when renew</span></span> | <span data-ttu-id="010e4-135">订阅续订时按比例计费。</span><span class="sxs-lookup"><span data-stu-id="010e4-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="010e4-136">续订费用</span><span class="sxs-lookup"><span data-stu-id="010e4-136">Renew fee</span></span> | <span data-ttu-id="010e4-137">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="010e4-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="010e4-138">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="010e4-138">Prorate fees when activate</span></span> | <span data-ttu-id="010e4-139">从激活 > 按比例计费，直到计费期结束。</span><span class="sxs-lookup"><span data-stu-id="010e4-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="010e4-140">一次性费用</span><span class="sxs-lookup"><span data-stu-id="010e4-140">One-time charges</span></span>

<span data-ttu-id="010e4-141">若要将这些一次性费用映射到你的发票，请对基于许可证的文件中的 "**金额**" 列求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="010e4-142">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="010e4-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="010e4-143">收费说明</span><span class="sxs-lookup"><span data-stu-id="010e4-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="010e4-144">新增</span><span class="sxs-lookup"><span data-stu-id="010e4-144">New</span></span> | <span data-ttu-id="010e4-145">创建新购买时使用。</span><span class="sxs-lookup"><span data-stu-id="010e4-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="010e4-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="010e4-146">addQuantity</span></span> | <span data-ttu-id="010e4-147">用于原始购买的退款和增加后的新数量。</span><span class="sxs-lookup"><span data-stu-id="010e4-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="010e4-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="010e4-148">removeQuantity</span></span> | <span data-ttu-id="010e4-149">用于原始购买的退款和减少后的新数量。</span><span class="sxs-lookup"><span data-stu-id="010e4-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="010e4-150">取消</span><span class="sxs-lookup"><span data-stu-id="010e4-150">Cancel</span></span> | <span data-ttu-id="010e4-151">取消订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="010e4-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="010e4-152">转换</span><span class="sxs-lookup"><span data-stu-id="010e4-152">Convert</span></span> | <span data-ttu-id="010e4-153">升级许可证时使用，但座位数保持不变。</span><span class="sxs-lookup"><span data-stu-id="010e4-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="010e4-154">使用情况费用</span><span class="sxs-lookup"><span data-stu-id="010e4-154">Usage charges</span></span>

<span data-ttu-id="010e4-155">若要将这些用量费用映射到发票，请将**PretaxCharges**列与基于使用情况的文件进行求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="010e4-156">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="010e4-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="010e4-157">收费说明</span><span class="sxs-lookup"><span data-stu-id="010e4-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="010e4-158">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="010e4-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="010e4-159">在当前计费周期内对未支付的使用情况取消时，访问使用费。</span><span class="sxs-lookup"><span data-stu-id="010e4-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="010e4-160">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="010e4-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="010e4-161">当前计费周期的访问费。</span><span class="sxs-lookup"><span data-stu-id="010e4-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="010e4-162">退款额</span><span class="sxs-lookup"><span data-stu-id="010e4-162">Credits</span></span>

<span data-ttu-id="010e4-163">若要将这些信用额度映射到发票：</span><span class="sxs-lookup"><span data-stu-id="010e4-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="010e4-164">对基于许可证的文件中的**TotalForCustomer**求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="010e4-165">在基于使用情况的文件中对**PostTaxTotal**列求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="010e4-166">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="010e4-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="010e4-167">收费说明</span><span class="sxs-lookup"><span data-stu-id="010e4-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="010e4-168">偏移行项</span><span class="sxs-lookup"><span data-stu-id="010e4-168">Offset a line item</span></span> | <span data-ttu-id="010e4-169">对行项的部分或全部退款，包括税金。</span><span class="sxs-lookup"><span data-stu-id="010e4-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="010e4-170">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="010e4-170">Usage-based discounts</span></span>

<span data-ttu-id="010e4-171">若要将基于使用情况的折扣映射到发票，请对基于使用情况的文件中的**PretaxCharges**列求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="010e4-172">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="010e4-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="010e4-173">收费说明</span><span class="sxs-lookup"><span data-stu-id="010e4-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="010e4-174">激活折扣</span><span class="sxs-lookup"><span data-stu-id="010e4-174">Activation discount</span></span> | <span data-ttu-id="010e4-175">激活订阅后应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="010e4-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="010e4-176">周期折扣</span><span class="sxs-lookup"><span data-stu-id="010e4-176">Cycle discount</span></span> | <span data-ttu-id="010e4-177">应用于定期费用的折扣。</span><span class="sxs-lookup"><span data-stu-id="010e4-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="010e4-178">续订折扣</span><span class="sxs-lookup"><span data-stu-id="010e4-178">Renew discount</span></span> | <span data-ttu-id="010e4-179">续订订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="010e4-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="010e4-180">取消折扣</span><span class="sxs-lookup"><span data-stu-id="010e4-180">Cancel discount</span></span> | <span data-ttu-id="010e4-181">取消折扣后应用的费用。</span><span class="sxs-lookup"><span data-stu-id="010e4-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="010e4-182">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="010e4-182">License-based discounts</span></span>

<span data-ttu-id="010e4-183">若要将基于许可证的折扣映射到发票，请对基于许可证的文件中的**TotalOtherDiscount**列求和。</span><span class="sxs-lookup"><span data-stu-id="010e4-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="010e4-184">*基于许可证的折扣可以应用于多种费用类型。*</span><span class="sxs-lookup"><span data-stu-id="010e4-184">*License-based discounts may be applied to multiple charge types.*</span></span>
