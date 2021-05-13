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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855873"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="6e7bb-103">了解合作伙伴中心对帐文件中的不同费用类型</span><span class="sxs-lookup"><span data-stu-id="6e7bb-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="6e7bb-104">**适用** 于：合作伙伴中心 |适用于美国政府的 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6e7bb-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6e7bb-105">**适当的角色**：管理代理 |计费管理 |全局管理员</span><span class="sxs-lookup"><span data-stu-id="6e7bb-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="6e7bb-106">本文介绍了发票部分与你的对帐文件上可能的相关费用类型之间的映射。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="6e7bb-107">发票提供费用的摘要。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="6e7bb-108">你的对帐文件提供行项事务的详细细分，包括费用类型。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="6e7bb-109">有关对帐文件的详细信息，请参阅 [如何使用协调文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="6e7bb-110">[基于使用情况的对帐文件](usage-based-recon-files.md)和[基于许可证的对帐文件](license-based-recon-files.md)只显示与使用量相关的事务，并 () 消耗的单位和相关费用的费用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="6e7bb-111">在发票上作为 **调整** 显示的一次性信用额度、折扣或退款不显示在对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="6e7bb-112">将费用类型映射到发票费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="6e7bb-113">若要在发票和对帐文件之间交叉引用费用量，请使用 Microsoft Excel 中的筛选器选项。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="6e7bb-114">按对帐文件上的费用类型进行筛选，以将发票费用映射到对帐文件上的一组费用细分。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="6e7bb-115">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-115">License-based charges</span></span>

<span data-ttu-id="6e7bb-116">若要将这些基于许可证的费用映射到发票，请对基于许可证的文件中的 " **金额** " 列求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="6e7bb-117">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="6e7bb-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6e7bb-118">收费说明</span><span class="sxs-lookup"><span data-stu-id="6e7bb-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6e7bb-119">激活费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-119">Activation fee</span></span> | <span data-ttu-id="6e7bb-120">客户在购买后使用订阅时向客户收取的费用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="6e7bb-121">取消费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-121">Cancel fee</span></span> | <span data-ttu-id="6e7bb-122">更改关联的许可证时，将向客户退还按比例计费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="6e7bb-123">取消实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="6e7bb-123">Cancel instance prorate</span></span> | <span data-ttu-id="6e7bb-124">按月订阅的客户在同一月内暂停订阅并更改关联许可证时，按比例计费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="6e7bb-125">周期费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-125">Cycle fee</span></span> | <span data-ttu-id="6e7bb-126">订阅的定期收费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="6e7bb-127">周期实例按比例计算</span><span class="sxs-lookup"><span data-stu-id="6e7bb-127">Cycle instance prorate</span></span> | <span data-ttu-id="6e7bb-128">更改关联许可证时，从客户评估的按比例收费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="6e7bb-129">按比例计算取消时的费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-129">Prorate fees when cancel</span></span> | <span data-ttu-id="6e7bb-130">取消时服务未使用部分的按比例退款。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="6e7bb-131">从当前产品/服务转换时按比例收费</span><span class="sxs-lookup"><span data-stu-id="6e7bb-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="6e7bb-132">从当前每月订阅转换为年度订阅后按比例收费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="6e7bb-133">转换为新产品/服务时按比例收费</span><span class="sxs-lookup"><span data-stu-id="6e7bb-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="6e7bb-134">将每月订阅转换为新的年度订阅后按比例收费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="6e7bb-135">按比例计算购买时的费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-135">Prorate fees when purchase</span></span> | <span data-ttu-id="6e7bb-136">使用每月或按年计费时订阅的费用类型。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="6e7bb-137">按比例计算续订时的费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-137">Prorate fee when renew</span></span> | <span data-ttu-id="6e7bb-138">订阅续订时按比例计算的费用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="6e7bb-139">续订费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-139">Renew fee</span></span> | <span data-ttu-id="6e7bb-140">续订订阅费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="6e7bb-141">按比例计算激活时的费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-141">Prorate fees when activate</span></span> | <span data-ttu-id="6e7bb-142">从激活到计费周期结束按比例计费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="6e7bb-143">一次费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-143">One-time charges</span></span>

<span data-ttu-id="6e7bb-144">若要将这些一次性费用映射到发票，请对基于许可证的文件中 **"金额** "列求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="6e7bb-145">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="6e7bb-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6e7bb-146">费用说明</span><span class="sxs-lookup"><span data-stu-id="6e7bb-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6e7bb-147">新建</span><span class="sxs-lookup"><span data-stu-id="6e7bb-147">New</span></span> | <span data-ttu-id="6e7bb-148">在新建购买时使用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="6e7bb-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="6e7bb-149">addQuantity</span></span> | <span data-ttu-id="6e7bb-150">用于原始购买退款和增加后的新数量。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="6e7bb-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="6e7bb-151">removeQuantity</span></span> | <span data-ttu-id="6e7bb-152">用于原始购买退款和减少后的新数量。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="6e7bb-153">取消</span><span class="sxs-lookup"><span data-stu-id="6e7bb-153">Cancel</span></span> | <span data-ttu-id="6e7bb-154">在取消订阅时使用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="6e7bb-155">转换</span><span class="sxs-lookup"><span data-stu-id="6e7bb-155">Convert</span></span> | <span data-ttu-id="6e7bb-156">在升级许可证但许可证数量保持不变时使用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="6e7bb-157">使用费</span><span class="sxs-lookup"><span data-stu-id="6e7bb-157">Usage charges</span></span>

<span data-ttu-id="6e7bb-158">若要将这些使用费用映射到发票，请对基于使用情况的文件的 **PretaxCharges** 列求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="6e7bb-159">对帐 (中的 ChargeType 列的费用) </span><span class="sxs-lookup"><span data-stu-id="6e7bb-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6e7bb-160">收费说明</span><span class="sxs-lookup"><span data-stu-id="6e7bb-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6e7bb-161">评估取消时的使用费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="6e7bb-162">在已取消的情况下的访问使用费，针对当前计费周期的未付款使用量。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="6e7bb-163">评估当前周期的使用费用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="6e7bb-164">当前计费周期的访问使用费。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="6e7bb-165">信用</span><span class="sxs-lookup"><span data-stu-id="6e7bb-165">Credits</span></span>

<span data-ttu-id="6e7bb-166">若要将这些信用额度映射到发票：</span><span class="sxs-lookup"><span data-stu-id="6e7bb-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="6e7bb-167">对基于许可证的文件中的 **TotalForCustomer** 求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="6e7bb-168">在基于使用情况的文件中对 **PostTaxTotal** 列求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="6e7bb-169">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="6e7bb-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6e7bb-170">收费说明</span><span class="sxs-lookup"><span data-stu-id="6e7bb-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6e7bb-171">偏移行项</span><span class="sxs-lookup"><span data-stu-id="6e7bb-171">Offset a line item</span></span> | <span data-ttu-id="6e7bb-172">对某个行项的部分或全部退款，包括税款。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="6e7bb-173">基于使用情况的折扣</span><span class="sxs-lookup"><span data-stu-id="6e7bb-173">Usage-based discounts</span></span>

<span data-ttu-id="6e7bb-174">若要将基于使用情况的折扣映射到发票，请对基于使用情况的文件中的 **PretaxCharges** 列求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="6e7bb-175">对帐文件中 ChargeType 列 (收费说明) </span><span class="sxs-lookup"><span data-stu-id="6e7bb-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6e7bb-176">收费说明</span><span class="sxs-lookup"><span data-stu-id="6e7bb-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6e7bb-177">激活折扣</span><span class="sxs-lookup"><span data-stu-id="6e7bb-177">Activation discount</span></span> | <span data-ttu-id="6e7bb-178">激活订阅后应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="6e7bb-179">周期折扣</span><span class="sxs-lookup"><span data-stu-id="6e7bb-179">Cycle discount</span></span> | <span data-ttu-id="6e7bb-180">应用在周期性费用上的折扣。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="6e7bb-181">续订折扣</span><span class="sxs-lookup"><span data-stu-id="6e7bb-181">Renew discount</span></span> | <span data-ttu-id="6e7bb-182">续订订阅时应用的折扣。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="6e7bb-183">取消折扣</span><span class="sxs-lookup"><span data-stu-id="6e7bb-183">Cancel discount</span></span> | <span data-ttu-id="6e7bb-184">取消折扣时应用的费用。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="6e7bb-185">基于许可证的折扣</span><span class="sxs-lookup"><span data-stu-id="6e7bb-185">License-based discounts</span></span>

<span data-ttu-id="6e7bb-186">若要将基于许可证的折扣映射到发票，请对基于许可证的文件中的 **TotalOtherDiscount** 列求和。</span><span class="sxs-lookup"><span data-stu-id="6e7bb-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="6e7bb-187">*基于许可证的折扣可以应用于多种费用类型。*</span><span class="sxs-lookup"><span data-stu-id="6e7bb-187">*License-based discounts may be applied to multiple charge types.*</span></span>
