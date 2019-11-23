---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
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
# <a name="understand-charge-types"></a><span data-ttu-id="49f19-103">Understand charge types</span><span class="sxs-lookup"><span data-stu-id="49f19-103">Understand charge types</span></span>

<span data-ttu-id="49f19-104">适用范围：</span><span class="sxs-lookup"><span data-stu-id="49f19-104">Applies to:</span></span>

- <span data-ttu-id="49f19-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="49f19-105">Partner Center</span></span>
- <span data-ttu-id="49f19-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="49f19-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="49f19-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="49f19-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="49f19-108">Your invoice provides a summary of charges.</span><span class="sxs-lookup"><span data-stu-id="49f19-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="49f19-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="49f19-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="49f19-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="49f19-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="49f19-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span><span class="sxs-lookup"><span data-stu-id="49f19-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="49f19-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="49f19-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="49f19-113">Map charge types to invoice charges</span><span class="sxs-lookup"><span data-stu-id="49f19-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="49f19-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="49f19-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="49f19-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="49f19-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="49f19-116">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="49f19-116">License-based charges</span></span>

<span data-ttu-id="49f19-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="49f19-118">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="49f19-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49f19-119">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="49f19-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49f19-120">激活费用</span><span class="sxs-lookup"><span data-stu-id="49f19-120">Activation fee</span></span> | <span data-ttu-id="49f19-121">The amount charged to the customer when they use the subscription after purchase.</span><span class="sxs-lookup"><span data-stu-id="49f19-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="49f19-122">取消费用</span><span class="sxs-lookup"><span data-stu-id="49f19-122">Cancel fee</span></span> | <span data-ttu-id="49f19-123">Prorated charges refunded to the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="49f19-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="49f19-124">周期费用</span><span class="sxs-lookup"><span data-stu-id="49f19-124">Cycle fee</span></span> | <span data-ttu-id="49f19-125">Periodic charges for a subscription.</span><span class="sxs-lookup"><span data-stu-id="49f19-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="49f19-126">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="49f19-126">Cycle instance prorate</span></span> | <span data-ttu-id="49f19-127">Prorated charges assessed from the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="49f19-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="49f19-128">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="49f19-128">Prorate fees when cancel</span></span> | <span data-ttu-id="49f19-129">Prorated refund for unused portion of service upon cancellation.</span><span class="sxs-lookup"><span data-stu-id="49f19-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="49f19-130">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="49f19-130">Prorate fees when purchase</span></span> | <span data-ttu-id="49f19-131">The charge type for a subscription when using annual billing.</span><span class="sxs-lookup"><span data-stu-id="49f19-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="49f19-132">购买费用</span><span class="sxs-lookup"><span data-stu-id="49f19-132">Purchase fee</span></span> | <span data-ttu-id="49f19-133">The charge type for a subscription when using monthly billing.</span><span class="sxs-lookup"><span data-stu-id="49f19-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="49f19-134">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="49f19-134">Prorate fee when renew</span></span> | <span data-ttu-id="49f19-135">Prorated fees upon subscription renewal.</span><span class="sxs-lookup"><span data-stu-id="49f19-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="49f19-136">续订费用</span><span class="sxs-lookup"><span data-stu-id="49f19-136">Renew fee</span></span> | <span data-ttu-id="49f19-137">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="49f19-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="49f19-138">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="49f19-138">Prorate fees when activate</span></span> | <span data-ttu-id="49f19-139">>Prorated fees from activation until end of billing period.</span><span class="sxs-lookup"><span data-stu-id="49f19-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="49f19-140">One-time charges</span><span class="sxs-lookup"><span data-stu-id="49f19-140">One-time charges</span></span>

<span data-ttu-id="49f19-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="49f19-142">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="49f19-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49f19-143">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="49f19-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49f19-144">新</span><span class="sxs-lookup"><span data-stu-id="49f19-144">New</span></span> | <span data-ttu-id="49f19-145">Used when a new purchase is created.</span><span class="sxs-lookup"><span data-stu-id="49f19-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="49f19-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="49f19-146">addQuantity</span></span> | <span data-ttu-id="49f19-147">Used in both the refund of the original purchase and the new quantity after an increase.</span><span class="sxs-lookup"><span data-stu-id="49f19-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="49f19-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="49f19-148">removeQuantity</span></span> | <span data-ttu-id="49f19-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span><span class="sxs-lookup"><span data-stu-id="49f19-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="49f19-150">“取消”</span><span class="sxs-lookup"><span data-stu-id="49f19-150">Cancel</span></span> | <span data-ttu-id="49f19-151">Used when a subscription is cancelled.</span><span class="sxs-lookup"><span data-stu-id="49f19-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="49f19-152">转换</span><span class="sxs-lookup"><span data-stu-id="49f19-152">Convert</span></span> | <span data-ttu-id="49f19-153">Used when a license is upgraded but the number of seats remains unchanged.</span><span class="sxs-lookup"><span data-stu-id="49f19-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="49f19-154">使用情况费用</span><span class="sxs-lookup"><span data-stu-id="49f19-154">Usage charges</span></span>

<span data-ttu-id="49f19-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="49f19-156">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="49f19-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49f19-157">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="49f19-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49f19-158">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="49f19-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="49f19-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span><span class="sxs-lookup"><span data-stu-id="49f19-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="49f19-160">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="49f19-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="49f19-161">Access usage fee for the current billing period.</span><span class="sxs-lookup"><span data-stu-id="49f19-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="49f19-162">退款额</span><span class="sxs-lookup"><span data-stu-id="49f19-162">Credits</span></span>

<span data-ttu-id="49f19-163">To map these credits to your invoice:</span><span class="sxs-lookup"><span data-stu-id="49f19-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="49f19-164">Sum the **TotalForCustomer** from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="49f19-165">Sum the **PostTaxTotal** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="49f19-166">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="49f19-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49f19-167">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="49f19-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49f19-168">偏移行项</span><span class="sxs-lookup"><span data-stu-id="49f19-168">Offset a line item</span></span> | <span data-ttu-id="49f19-169">Partial or whole refund to a line item, including taxes.</span><span class="sxs-lookup"><span data-stu-id="49f19-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="49f19-170">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="49f19-170">Usage-based discounts</span></span>

<span data-ttu-id="49f19-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="49f19-172">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="49f19-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49f19-173">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="49f19-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49f19-174">激活折扣</span><span class="sxs-lookup"><span data-stu-id="49f19-174">Activation discount</span></span> | <span data-ttu-id="49f19-175">Discount applied when subscription activated.</span><span class="sxs-lookup"><span data-stu-id="49f19-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="49f19-176">周期折扣</span><span class="sxs-lookup"><span data-stu-id="49f19-176">Cycle discount</span></span> | <span data-ttu-id="49f19-177">Discount applied on periodic charges.</span><span class="sxs-lookup"><span data-stu-id="49f19-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="49f19-178">续订折扣</span><span class="sxs-lookup"><span data-stu-id="49f19-178">Renew discount</span></span> | <span data-ttu-id="49f19-179">Discount applied when subscription renewed.</span><span class="sxs-lookup"><span data-stu-id="49f19-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="49f19-180">取消折扣</span><span class="sxs-lookup"><span data-stu-id="49f19-180">Cancel discount</span></span> | <span data-ttu-id="49f19-181">Charges applied when discounts cancelled.</span><span class="sxs-lookup"><span data-stu-id="49f19-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="49f19-182">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="49f19-182">License-based discounts</span></span>

<span data-ttu-id="49f19-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="49f19-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="49f19-184">*License-based discounts may be applied to multiple charge types.*</span><span class="sxs-lookup"><span data-stu-id="49f19-184">*License-based discounts may be applied to multiple charge types.*</span></span>
