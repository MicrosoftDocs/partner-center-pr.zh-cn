---
title: 对帐文件费用类型
ms.topic: article
ms.date: 06/05/2020
description: 了解合作伙伴中心对帐文件中的费用类型 (例如，基于许可证、基于使用情况以及一次性) 、信用额度和折扣。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441586"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="24c11-103">了解合作伙伴中心对帐文件中的不同费用类型</span><span class="sxs-lookup"><span data-stu-id="24c11-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="24c11-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="24c11-104">**Applies to**</span></span>

- <span data-ttu-id="24c11-105">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="24c11-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="24c11-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="24c11-106">**Appropriate roles**</span></span>

- <span data-ttu-id="24c11-107">管理员代理</span><span class="sxs-lookup"><span data-stu-id="24c11-107">Admin agent</span></span>
- <span data-ttu-id="24c11-108">计费管理员</span><span class="sxs-lookup"><span data-stu-id="24c11-108">Billing admin</span></span>
- <span data-ttu-id="24c11-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="24c11-109">Global admin</span></span>

<span data-ttu-id="24c11-110">本文介绍了发票部分与你的对帐文件上可能的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="24c11-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="24c11-111">发票提供费用的摘要。</span><span class="sxs-lookup"><span data-stu-id="24c11-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="24c11-112">你的对帐文件提供行项事务的详细细分，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="24c11-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="24c11-113">有关对帐文件的详细信息，请参阅 [如何使用协调文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="24c11-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="24c11-114">[基于使用情况的对帐文件](usage-based-recon-files.md)和[基于许可证的对帐文件](license-based-recon-files.md)只显示与使用量相关的事务，并 () 消耗的单位和相关费用的费用。</span><span class="sxs-lookup"><span data-stu-id="24c11-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="24c11-115">在发票上作为 **调整** 显示的一次性信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="24c11-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="24c11-116">将费用类型映射到发票费用</span><span class="sxs-lookup"><span data-stu-id="24c11-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="24c11-117">若要在发票和对帐文件之间交叉引用费用量，请使用 Microsoft Excel 中的筛选器选项。</span><span class="sxs-lookup"><span data-stu-id="24c11-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="24c11-118">按对帐文件上的费用类型进行筛选，以将发票费用映射到对帐文件上的一组费用细分。</span><span class="sxs-lookup"><span data-stu-id="24c11-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="24c11-119">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="24c11-119">License-based charges</span></span>

<span data-ttu-id="24c11-120">若要将这些基于许可证的费用映射到发票，请对基于许可证的文件中的 " **金额** " 列求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="24c11-121">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="24c11-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24c11-122">收费说明</span><span class="sxs-lookup"><span data-stu-id="24c11-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24c11-123">激活费用</span><span class="sxs-lookup"><span data-stu-id="24c11-123">Activation fee</span></span> | <span data-ttu-id="24c11-124">客户在购买后使用订阅时向客户收取的费用。</span><span class="sxs-lookup"><span data-stu-id="24c11-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="24c11-125">取消费用</span><span class="sxs-lookup"><span data-stu-id="24c11-125">Cancel fee</span></span> | <span data-ttu-id="24c11-126">更改关联的许可证时，将向客户退还按比例计费。</span><span class="sxs-lookup"><span data-stu-id="24c11-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="24c11-127">取消实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="24c11-127">Cancel instance prorate</span></span> | <span data-ttu-id="24c11-128">按月订阅的客户在同一月内暂停订阅并更改关联许可证时，按比例计费。</span><span class="sxs-lookup"><span data-stu-id="24c11-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="24c11-129">周期费用</span><span class="sxs-lookup"><span data-stu-id="24c11-129">Cycle fee</span></span> | <span data-ttu-id="24c11-130">订阅的定期收费。</span><span class="sxs-lookup"><span data-stu-id="24c11-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="24c11-131">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="24c11-131">Cycle instance prorate</span></span> | <span data-ttu-id="24c11-132">更改关联的许可证时，从客户评估的按比例计费。</span><span class="sxs-lookup"><span data-stu-id="24c11-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="24c11-133">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="24c11-133">Prorate fees when cancel</span></span> | <span data-ttu-id="24c11-134">取消时，未使用的服务部分按比例退款。</span><span class="sxs-lookup"><span data-stu-id="24c11-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="24c11-135">转换远离当前产品/服务的按比例计算费用</span><span class="sxs-lookup"><span data-stu-id="24c11-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="24c11-136">从当前月度订阅转换为年度订阅后按比例计费。</span><span class="sxs-lookup"><span data-stu-id="24c11-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="24c11-137">转换为新产品/服务时的按比例计算费用</span><span class="sxs-lookup"><span data-stu-id="24c11-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="24c11-138">将月度订阅转换为新年度订阅后按比例计费。</span><span class="sxs-lookup"><span data-stu-id="24c11-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="24c11-139">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="24c11-139">Prorate fees when purchase</span></span> | <span data-ttu-id="24c11-140">使用月度或年度计费时的订阅费用类型。</span><span class="sxs-lookup"><span data-stu-id="24c11-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="24c11-141">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="24c11-141">Prorate fee when renew</span></span> | <span data-ttu-id="24c11-142">订阅续订时按比例计费。</span><span class="sxs-lookup"><span data-stu-id="24c11-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="24c11-143">续订费用</span><span class="sxs-lookup"><span data-stu-id="24c11-143">Renew fee</span></span> | <span data-ttu-id="24c11-144">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="24c11-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="24c11-145">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="24c11-145">Prorate fees when activate</span></span> | <span data-ttu-id="24c11-146">从激活中按比例计费，直到计费周期结束。</span><span class="sxs-lookup"><span data-stu-id="24c11-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="24c11-147">一次性费用</span><span class="sxs-lookup"><span data-stu-id="24c11-147">One-time charges</span></span>

<span data-ttu-id="24c11-148">若要将这些一次性费用映射到你的发票，请对基于许可证的文件中的 " **金额** " 列求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="24c11-149">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="24c11-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24c11-150">收费说明</span><span class="sxs-lookup"><span data-stu-id="24c11-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24c11-151">新建</span><span class="sxs-lookup"><span data-stu-id="24c11-151">New</span></span> | <span data-ttu-id="24c11-152">创建新购买时使用。</span><span class="sxs-lookup"><span data-stu-id="24c11-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="24c11-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="24c11-153">addQuantity</span></span> | <span data-ttu-id="24c11-154">用于原始购买的退款和增加后的新数量。</span><span class="sxs-lookup"><span data-stu-id="24c11-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="24c11-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="24c11-155">removeQuantity</span></span> | <span data-ttu-id="24c11-156">用于原始购买的退款和减少后的新数量。</span><span class="sxs-lookup"><span data-stu-id="24c11-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="24c11-157">取消</span><span class="sxs-lookup"><span data-stu-id="24c11-157">Cancel</span></span> | <span data-ttu-id="24c11-158">取消订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="24c11-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="24c11-159">转换</span><span class="sxs-lookup"><span data-stu-id="24c11-159">Convert</span></span> | <span data-ttu-id="24c11-160">升级许可证时使用，但许可证数量保持不变。</span><span class="sxs-lookup"><span data-stu-id="24c11-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="24c11-161">使用费</span><span class="sxs-lookup"><span data-stu-id="24c11-161">Usage charges</span></span>

<span data-ttu-id="24c11-162">若要将这些用量费用映射到发票，请将 **PretaxCharges** 列与基于使用情况的文件进行求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="24c11-163">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="24c11-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24c11-164">收费说明</span><span class="sxs-lookup"><span data-stu-id="24c11-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24c11-165">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="24c11-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="24c11-166">在已取消的情况下的访问使用费，针对当前计费周期的未付款使用量。</span><span class="sxs-lookup"><span data-stu-id="24c11-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="24c11-167">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="24c11-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="24c11-168">当前计费周期的访问使用费。</span><span class="sxs-lookup"><span data-stu-id="24c11-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="24c11-169">信用</span><span class="sxs-lookup"><span data-stu-id="24c11-169">Credits</span></span>

<span data-ttu-id="24c11-170">若要将这些信用额度映射到发票：</span><span class="sxs-lookup"><span data-stu-id="24c11-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="24c11-171">对基于许可证的文件中的 **TotalForCustomer** 求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="24c11-172">在基于使用情况的文件中对 **PostTaxTotal** 列求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="24c11-173">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="24c11-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24c11-174">收费说明</span><span class="sxs-lookup"><span data-stu-id="24c11-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24c11-175">偏移行项</span><span class="sxs-lookup"><span data-stu-id="24c11-175">Offset a line item</span></span> | <span data-ttu-id="24c11-176">对某个行项的部分或全部退款，包括税款。</span><span class="sxs-lookup"><span data-stu-id="24c11-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="24c11-177">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="24c11-177">Usage-based discounts</span></span>

<span data-ttu-id="24c11-178">若要将基于使用情况的折扣映射到发票，请对基于使用情况的文件中的 **PretaxCharges** 列求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="24c11-179">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="24c11-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24c11-180">收费说明</span><span class="sxs-lookup"><span data-stu-id="24c11-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24c11-181">激活折扣</span><span class="sxs-lookup"><span data-stu-id="24c11-181">Activation discount</span></span> | <span data-ttu-id="24c11-182">激活订阅后应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="24c11-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="24c11-183">周期折扣</span><span class="sxs-lookup"><span data-stu-id="24c11-183">Cycle discount</span></span> | <span data-ttu-id="24c11-184">应用在周期性费用上的折扣。</span><span class="sxs-lookup"><span data-stu-id="24c11-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="24c11-185">续订折扣</span><span class="sxs-lookup"><span data-stu-id="24c11-185">Renew discount</span></span> | <span data-ttu-id="24c11-186">续订订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="24c11-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="24c11-187">取消折扣</span><span class="sxs-lookup"><span data-stu-id="24c11-187">Cancel discount</span></span> | <span data-ttu-id="24c11-188">取消折扣时应用的费用。</span><span class="sxs-lookup"><span data-stu-id="24c11-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="24c11-189">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="24c11-189">License-based discounts</span></span>

<span data-ttu-id="24c11-190">若要将基于许可证的折扣映射到发票，请对基于许可证的文件中的 **TotalOtherDiscount** 列求和。</span><span class="sxs-lookup"><span data-stu-id="24c11-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="24c11-191">*基于许可证的折扣可以应用于多种费用类型。*</span><span class="sxs-lookup"><span data-stu-id="24c11-191">*License-based discounts may be applied to multiple charge types.*</span></span>
