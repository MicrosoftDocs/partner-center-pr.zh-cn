---
title: 对帐文件费用类型
ms.topic: article
ms.date: 06/05/2020
description: 发现费用类型 (，例如，基于许可证、基于使用情况和一) 、信用额度和折扣合作伙伴中心文件中。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989768"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="9fbb9-103">了解对帐文件中合作伙伴中心类型</span><span class="sxs-lookup"><span data-stu-id="9fbb9-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="9fbb9-104">**适用于**：合作伙伴中心 | Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="9fbb9-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="9fbb9-105">相应的角色：管理员代理 | 计费管理员 | 全局管理员</span><span class="sxs-lookup"><span data-stu-id="9fbb9-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="9fbb9-106">本文介绍发票部分与可能位于对帐文件上的关联费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="9fbb9-107">发票提供费用摘要。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="9fbb9-108">对帐文件提供行项交易的详细明细，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="9fbb9-109">有关对帐文件详细信息，请参阅 [如何使用对帐文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="9fbb9-110">基于 [使用情况的对帐文件和](usage-based-recon-files.md) 基于许可证的 [对](license-based-recon-files.md) 帐文件都只显示与使用情况相关的交易和费用 (单位数和相关费用) 。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="9fbb9-111">发票上显示为"调整"的一次额度、折扣或 **退款不会显示在** 对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="9fbb9-112">将费用类型映射到发票费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="9fbb9-113">若要在发票和对帐文件之间交叉引用费用金额，请使用发票中的筛选Microsoft Excel。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="9fbb9-114">按对帐文件上的费用类型进行筛选，将发票费用映射到对帐文件上的一组费用明细。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="9fbb9-115">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-115">License-based charges</span></span>

<span data-ttu-id="9fbb9-116">若要将这些基于许可证的费用映射到发票，请对基于许可证的文件的 **"金额** "列求和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="9fbb9-117">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="9fbb9-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9fbb9-118">费用说明</span><span class="sxs-lookup"><span data-stu-id="9fbb9-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9fbb9-119">激活费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-119">Activation fee</span></span> | <span data-ttu-id="9fbb9-120">客户在购买后使用订阅时收取的金额。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="9fbb9-121">取消费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-121">Cancel fee</span></span> | <span data-ttu-id="9fbb9-122">更改关联的许可证时，按比例退款给客户。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="9fbb9-123">取消实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="9fbb9-123">Cancel instance prorate</span></span> | <span data-ttu-id="9fbb9-124">当具有月度订阅的客户在同一个月内暂停订阅并更改关联的许可证时，取消了按比例计算的费用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="9fbb9-125">周期费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-125">Cycle fee</span></span> | <span data-ttu-id="9fbb9-126">订阅的定期费用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="9fbb9-127">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="9fbb9-127">Cycle instance prorate</span></span> | <span data-ttu-id="9fbb9-128">更改关联许可证时，从客户评估的按比例收费。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="9fbb9-129">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-129">Prorate fees when cancel</span></span> | <span data-ttu-id="9fbb9-130">取消时服务未使用部分的按比例退款。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="9fbb9-131">从当前产品/服务转换时按比例收费</span><span class="sxs-lookup"><span data-stu-id="9fbb9-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="9fbb9-132">从当前每月订阅转换为年度订阅后按比例收费。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="9fbb9-133">转换为新产品/服务时按比例收费</span><span class="sxs-lookup"><span data-stu-id="9fbb9-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="9fbb9-134">将每月订阅转换为新的年度订阅后按比例收费。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="9fbb9-135">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-135">Prorate fees when purchase</span></span> | <span data-ttu-id="9fbb9-136">使用每月或按年计费时订阅的费用类型。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="9fbb9-137">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-137">Prorate fee when renew</span></span> | <span data-ttu-id="9fbb9-138">订阅续订时按比例计算的费用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="9fbb9-139">续订费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-139">Renew fee</span></span> | <span data-ttu-id="9fbb9-140">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="9fbb9-141">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-141">Prorate fees when activate</span></span> | <span data-ttu-id="9fbb9-142">从激活到计费周期结束按比例计费。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="9fbb9-143">一次费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-143">One-time charges</span></span>

<span data-ttu-id="9fbb9-144">若要将这些一次性费用映射到发票，请对基于许可证的文件中 **"金额** "列求和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="9fbb9-145">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="9fbb9-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9fbb9-146">费用说明</span><span class="sxs-lookup"><span data-stu-id="9fbb9-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9fbb9-147">new</span><span class="sxs-lookup"><span data-stu-id="9fbb9-147">new</span></span> | <span data-ttu-id="9fbb9-148">在新建购买时使用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="9fbb9-149">续订</span><span class="sxs-lookup"><span data-stu-id="9fbb9-149">renew</span></span> | <span data-ttu-id="9fbb9-150">在期限结束后续订订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-150">Used when a subscription is renewed after the end of the term.</span></span> |
| <span data-ttu-id="9fbb9-151">addQuantity</span><span class="sxs-lookup"><span data-stu-id="9fbb9-151">addQuantity</span></span> | <span data-ttu-id="9fbb9-152">用于原始购买退款和增加后的新数量。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-152">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="9fbb9-153">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="9fbb9-153">removeQuantity</span></span> | <span data-ttu-id="9fbb9-154">用于原始购买退款和减少后的新数量。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-154">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="9fbb9-155">cancelImmediate</span><span class="sxs-lookup"><span data-stu-id="9fbb9-155">cancelImmediate</span></span> | <span data-ttu-id="9fbb9-156">在取消订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-156">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="9fbb9-157">convert</span><span class="sxs-lookup"><span data-stu-id="9fbb9-157">convert</span></span> | <span data-ttu-id="9fbb9-158">在升级许可证时使用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-158">Used when a license is upgraded.</span></span> |
| <span data-ttu-id="9fbb9-159">customerCredit</span><span class="sxs-lookup"><span data-stu-id="9fbb9-159">customerCredit</span></span> | <span data-ttu-id="9fbb9-160">在针对 (提供信用额度（例如 Azure、SLA 等) 时使用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-160">Used when credits (e.g., Azure, SLA, etc.) are given against a transaction.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="9fbb9-161">使用费</span><span class="sxs-lookup"><span data-stu-id="9fbb9-161">Usage charges</span></span>

<span data-ttu-id="9fbb9-162">若要将这些使用费用映射到发票，请对基于使用情况的文件的 **PretaxCharges** 列求和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="9fbb9-163">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="9fbb9-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9fbb9-164">费用说明</span><span class="sxs-lookup"><span data-stu-id="9fbb9-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9fbb9-165">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="9fbb9-166">在已取消的情况下的访问使用费，针对当前计费周期的未付款使用量。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="9fbb9-167">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="9fbb9-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="9fbb9-168">当前计费周期的访问使用费。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="9fbb9-169">致谢</span><span class="sxs-lookup"><span data-stu-id="9fbb9-169">Credits</span></span>

<span data-ttu-id="9fbb9-170">若要将这些额度映射到发票：：</span><span class="sxs-lookup"><span data-stu-id="9fbb9-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="9fbb9-171">基于 **许可证的文件中 TotalForCustomer** 的总和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="9fbb9-172">对 **基于使用情况的文件的 PostTaxTotal** 列求和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="9fbb9-173">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="9fbb9-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9fbb9-174">费用说明</span><span class="sxs-lookup"><span data-stu-id="9fbb9-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9fbb9-175">偏移行项</span><span class="sxs-lookup"><span data-stu-id="9fbb9-175">Offset a line item</span></span> | <span data-ttu-id="9fbb9-176">对某个行项的部分或全部退款，包括税款。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="9fbb9-177">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="9fbb9-177">Usage-based discounts</span></span>

<span data-ttu-id="9fbb9-178">若要将这些基于使用情况的折扣映射到发票，请对基于使用情况的文件的 **PretaxCharges** 列求和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="9fbb9-179">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="9fbb9-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="9fbb9-180">费用说明</span><span class="sxs-lookup"><span data-stu-id="9fbb9-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="9fbb9-181">激活折扣</span><span class="sxs-lookup"><span data-stu-id="9fbb9-181">Activation discount</span></span> | <span data-ttu-id="9fbb9-182">激活订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="9fbb9-183">周期折扣</span><span class="sxs-lookup"><span data-stu-id="9fbb9-183">Cycle discount</span></span> | <span data-ttu-id="9fbb9-184">应用在周期性费用上的折扣。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="9fbb9-185">续订折扣</span><span class="sxs-lookup"><span data-stu-id="9fbb9-185">Renew discount</span></span> | <span data-ttu-id="9fbb9-186">续订订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="9fbb9-187">取消折扣</span><span class="sxs-lookup"><span data-stu-id="9fbb9-187">Cancel discount</span></span> | <span data-ttu-id="9fbb9-188">取消折扣时应用的费用。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="9fbb9-189">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="9fbb9-189">License-based discounts</span></span>

<span data-ttu-id="9fbb9-190">若要将基于许可证的折扣映射到发票，请对基于许可证的文件 **的 TotalOtherDiscount** 列求和。</span><span class="sxs-lookup"><span data-stu-id="9fbb9-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="9fbb9-191">*基于许可证的折扣可应用于多种费用类型。*</span><span class="sxs-lookup"><span data-stu-id="9fbb9-191">*License-based discounts may be applied to multiple charge types.*</span></span>
