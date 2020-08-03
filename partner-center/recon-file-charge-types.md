---
title: 对帐文件费用类型
ms.topic: article
ms.date: 06/05/2020
description: 了解合作伙伴中心对帐文件中的费用类型（例如，基于许可证、基于使用情况和一次性）、信用额度和折扣。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2020
ms.locfileid: "87479110"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="3c3f5-103">了解合作伙伴中心对帐文件中的不同费用类型</span><span class="sxs-lookup"><span data-stu-id="3c3f5-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="3c3f5-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="3c3f5-104">**Applies to**</span></span>

- <span data-ttu-id="3c3f5-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="3c3f5-105">Partner Center</span></span>
- <span data-ttu-id="3c3f5-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="3c3f5-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="3c3f5-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="3c3f5-107">**Appropriate roles**</span></span>

- <span data-ttu-id="3c3f5-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="3c3f5-108">Admin agent</span></span>
- <span data-ttu-id="3c3f5-109">计费管理员</span><span class="sxs-lookup"><span data-stu-id="3c3f5-109">Billing admin</span></span>
- <span data-ttu-id="3c3f5-110">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3c3f5-110">Global admin</span></span>

<span data-ttu-id="3c3f5-111">本主题介绍了发票部分与可能在对帐文件上的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="3c3f5-112">发票提供费用的摘要。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="3c3f5-113">你的对帐文件提供行项事务的详细细分，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="3c3f5-114">有关对帐文件的详细信息，请参阅[如何使用协调文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="3c3f5-115">[基于使用情况的对帐文件](usage-based-recon-files.md)和[基于许可证的对帐文件](license-based-recon-files.md)只显示与使用相关的事务和费用（单位消耗和相关费用）。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="3c3f5-116">在发票上作为**调整**显示的一次性信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="3c3f5-117">将费用类型映射到发票费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="3c3f5-118">若要在发票和对帐文件之间交叉引用费用量，请使用 Microsoft Excel 中的筛选器选项。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="3c3f5-119">按对帐文件上的费用类型进行筛选，以将发票费用映射到对帐文件上的一组费用细分。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="3c3f5-120">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-120">License-based charges</span></span>

<span data-ttu-id="3c3f5-121">若要将这些基于许可证的费用映射到发票，请对基于许可证的文件中的 "**金额**" 列求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="3c3f5-122">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="3c3f5-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3c3f5-123">收费说明</span><span class="sxs-lookup"><span data-stu-id="3c3f5-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3c3f5-124">激活费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-124">Activation fee</span></span> | <span data-ttu-id="3c3f5-125">客户在购买后使用订阅时向客户收取的费用。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="3c3f5-126">取消费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-126">Cancel fee</span></span> | <span data-ttu-id="3c3f5-127">更改关联的许可证时，将向客户退还按比例计费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="3c3f5-128">取消实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="3c3f5-128">Cancel instance prorate</span></span> | <span data-ttu-id="3c3f5-129">按月订阅的客户在同一月内暂停订阅并更改关联许可证时，按比例计费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="3c3f5-130">周期费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-130">Cycle fee</span></span> | <span data-ttu-id="3c3f5-131">订阅的定期收费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="3c3f5-132">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="3c3f5-132">Cycle instance prorate</span></span> | <span data-ttu-id="3c3f5-133">更改关联的许可证时，从客户评估的按比例计费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="3c3f5-134">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-134">Prorate fees when cancel</span></span> | <span data-ttu-id="3c3f5-135">取消时，未使用的服务部分按比例退款。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="3c3f5-136">转换远离当前产品/服务的按比例计算费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="3c3f5-137">从当前月度订阅转换为年度订阅后按比例计费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="3c3f5-138">转换为新产品/服务时的按比例计算费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="3c3f5-139">将月度订阅转换为新年度订阅后按比例计费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="3c3f5-140">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-140">Prorate fees when purchase</span></span> | <span data-ttu-id="3c3f5-141">使用月度或年度计费时的订阅费用类型。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="3c3f5-142">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-142">Prorate fee when renew</span></span> | <span data-ttu-id="3c3f5-143">订阅续订时按比例计费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="3c3f5-144">续订费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-144">Renew fee</span></span> | <span data-ttu-id="3c3f5-145">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="3c3f5-146">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-146">Prorate fees when activate</span></span> | <span data-ttu-id="3c3f5-147">从激活中按比例计费，直到计费周期结束。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="3c3f5-148">一次性费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-148">One-time charges</span></span>

<span data-ttu-id="3c3f5-149">若要将这些一次性费用映射到你的发票，请对基于许可证的文件中的 "**金额**" 列求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="3c3f5-150">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="3c3f5-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3c3f5-151">收费说明</span><span class="sxs-lookup"><span data-stu-id="3c3f5-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3c3f5-152">新建</span><span class="sxs-lookup"><span data-stu-id="3c3f5-152">New</span></span> | <span data-ttu-id="3c3f5-153">创建新购买时使用。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="3c3f5-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="3c3f5-154">addQuantity</span></span> | <span data-ttu-id="3c3f5-155">用于原始购买的退款和增加后的新数量。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="3c3f5-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="3c3f5-156">removeQuantity</span></span> | <span data-ttu-id="3c3f5-157">用于原始购买的退款和减少后的新数量。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="3c3f5-158">取消</span><span class="sxs-lookup"><span data-stu-id="3c3f5-158">Cancel</span></span> | <span data-ttu-id="3c3f5-159">取消订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="3c3f5-160">转换</span><span class="sxs-lookup"><span data-stu-id="3c3f5-160">Convert</span></span> | <span data-ttu-id="3c3f5-161">升级许可证时使用，但许可证数量保持不变。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="3c3f5-162">使用费</span><span class="sxs-lookup"><span data-stu-id="3c3f5-162">Usage charges</span></span>

<span data-ttu-id="3c3f5-163">若要将这些用量费用映射到发票，请将**PretaxCharges**列与基于使用情况的文件进行求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="3c3f5-164">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="3c3f5-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3c3f5-165">收费说明</span><span class="sxs-lookup"><span data-stu-id="3c3f5-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3c3f5-166">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="3c3f5-167">在已取消的情况下的访问使用费，针对当前计费周期的未付款使用量。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="3c3f5-168">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="3c3f5-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="3c3f5-169">当前计费周期的访问使用费。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="3c3f5-170">致谢</span><span class="sxs-lookup"><span data-stu-id="3c3f5-170">Credits</span></span>

<span data-ttu-id="3c3f5-171">若要将这些信用额度映射到发票：</span><span class="sxs-lookup"><span data-stu-id="3c3f5-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="3c3f5-172">对基于许可证的文件中的**TotalForCustomer**求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="3c3f5-173">在基于使用情况的文件中对**PostTaxTotal**列求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="3c3f5-174">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="3c3f5-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3c3f5-175">收费说明</span><span class="sxs-lookup"><span data-stu-id="3c3f5-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3c3f5-176">偏移行项</span><span class="sxs-lookup"><span data-stu-id="3c3f5-176">Offset a line item</span></span> | <span data-ttu-id="3c3f5-177">对某个行项的部分或全部退款，包括税款。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="3c3f5-178">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="3c3f5-178">Usage-based discounts</span></span>

<span data-ttu-id="3c3f5-179">若要将基于使用情况的折扣映射到发票，请对基于使用情况的文件中的**PretaxCharges**列求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="3c3f5-180">费用说明（对帐文件中的 ChargeType 列）</span><span class="sxs-lookup"><span data-stu-id="3c3f5-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="3c3f5-181">收费说明</span><span class="sxs-lookup"><span data-stu-id="3c3f5-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="3c3f5-182">激活折扣</span><span class="sxs-lookup"><span data-stu-id="3c3f5-182">Activation discount</span></span> | <span data-ttu-id="3c3f5-183">激活订阅后应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="3c3f5-184">周期折扣</span><span class="sxs-lookup"><span data-stu-id="3c3f5-184">Cycle discount</span></span> | <span data-ttu-id="3c3f5-185">应用在周期性费用上的折扣。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="3c3f5-186">续订折扣</span><span class="sxs-lookup"><span data-stu-id="3c3f5-186">Renew discount</span></span> | <span data-ttu-id="3c3f5-187">续订订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="3c3f5-188">取消折扣</span><span class="sxs-lookup"><span data-stu-id="3c3f5-188">Cancel discount</span></span> | <span data-ttu-id="3c3f5-189">取消折扣时应用的费用。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="3c3f5-190">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="3c3f5-190">License-based discounts</span></span>

<span data-ttu-id="3c3f5-191">若要将基于许可证的折扣映射到发票，请对基于许可证的文件中的**TotalOtherDiscount**列求和。</span><span class="sxs-lookup"><span data-stu-id="3c3f5-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="3c3f5-192">*基于许可证的折扣可以应用于多种费用类型。*</span><span class="sxs-lookup"><span data-stu-id="3c3f5-192">*License-based discounts may be applied to multiple charge types.*</span></span>
