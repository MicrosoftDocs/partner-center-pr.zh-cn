---
title: 了解合作伙伴中心帐单发票
ms.topic: article
ms.date: 05/18/2020
description: 了解发票文件中合作伙伴中心帐单的字段。 包括所有发票字段和一次性费用字段的字段和定义。
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44bda5256b14722f143a5bf937e73b2533b8c9f5
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178895"
---
# <a name="understand-partner-center-billing-invoice-fields"></a><span data-ttu-id="3feea-104">了解合作伙伴中心帐单发票字段</span><span class="sxs-lookup"><span data-stu-id="3feea-104">Understand Partner Center billing invoice fields</span></span>

<span data-ttu-id="3feea-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="3feea-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3feea-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3feea-106">Global admin</span></span>
- <span data-ttu-id="3feea-107">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="3feea-107">User management admin</span></span>
- <span data-ttu-id="3feea-108">计费管理员</span><span class="sxs-lookup"><span data-stu-id="3feea-108">Billing admin</span></span>
- <span data-ttu-id="3feea-109">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="3feea-109">Helpdesk agent</span></span>

<span data-ttu-id="3feea-110">您可以使用下表来了解合作伙伴中心发票文件中的字段。</span><span class="sxs-lookup"><span data-stu-id="3feea-110">You can use the following tables to understand the fields in Partner Center invoice files.</span></span>

## <a name="invoice-file-fields"></a><span data-ttu-id="3feea-111">发票文件字段</span><span class="sxs-lookup"><span data-stu-id="3feea-111">Invoice file fields</span></span>

<span data-ttu-id="3feea-112">发票文件上将显示以下字段。</span><span class="sxs-lookup"><span data-stu-id="3feea-112">The following fields appear on your invoice files.</span></span>

| <span data-ttu-id="3feea-113">字段</span><span class="sxs-lookup"><span data-stu-id="3feea-113">Field</span></span> | <span data-ttu-id="3feea-114">定义</span><span class="sxs-lookup"><span data-stu-id="3feea-114">Definition</span></span> |
| ----- | ---------- |
| <span data-ttu-id="3feea-115">美国 FEIN</span><span class="sxs-lookup"><span data-stu-id="3feea-115">US FEIN</span></span> | <span data-ttu-id="3feea-116">联邦雇主识别码 (FEIN) 。</span><span class="sxs-lookup"><span data-stu-id="3feea-116">Your Federal Employer Identification Number (FEIN).</span></span> <span data-ttu-id="3feea-117">这是美国的联邦税务标识符编号。</span><span class="sxs-lookup"><span data-stu-id="3feea-117">This is your United States federal tax identifier number.</span></span> |
| <span data-ttu-id="3feea-118">客户编号</span><span class="sxs-lookup"><span data-stu-id="3feea-118">Customer number</span></span> | <span data-ttu-id="3feea-119">你的客户编号。</span><span class="sxs-lookup"><span data-stu-id="3feea-119">Your customer number.</span></span> |
| <span data-ttu-id="3feea-120">帐单邮寄地址</span><span class="sxs-lookup"><span data-stu-id="3feea-120">Bill to</span></span> | <span data-ttu-id="3feea-121">我们发送发票的地址。</span><span class="sxs-lookup"><span data-stu-id="3feea-121">The address where we send your invoice.</span></span> <span data-ttu-id="3feea-122">你可以在合作伙伴中心帐单配置文件中更改公司名称和地址。</span><span class="sxs-lookup"><span data-stu-id="3feea-122">You can change your company name and address in your Partner Center billing profile.</span></span> |
| <span data-ttu-id="3feea-123">基于许可证的费用</span><span class="sxs-lookup"><span data-stu-id="3feea-123">License-based charges</span></span> | <span data-ttu-id="3feea-124">已购买的基于使用情况的许可证的按月或每年收费，服务提前向你收费。</span><span class="sxs-lookup"><span data-stu-id="3feea-124">The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service.</span></span> <span data-ttu-id="3feea-125">此数字是基于许可证的对帐文件中 (列 **T**) 的 **分类汇总** 列中所有费用的总和。</span><span class="sxs-lookup"><span data-stu-id="3feea-125">This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file.</span></span> |
| <span data-ttu-id="3feea-126">基于使用情况的费用</span><span class="sxs-lookup"><span data-stu-id="3feea-126">Usage-based charges</span></span> | <span data-ttu-id="3feea-127">你的 Azure 使用情况。</span><span class="sxs-lookup"><span data-stu-id="3feea-127">Your Azure usage.</span></span> <span data-ttu-id="3feea-128">这包括在计费期间启用并使用的新服务或应用程序。</span><span class="sxs-lookup"><span data-stu-id="3feea-128">This includes new services or applications enabled and used during the billing period.</span></span> <span data-ttu-id="3feea-129">此数字是基于使用情况的对帐文件中 **PretaxCharges** 列 (列 **Z**) 的所有费用的总和。</span><span class="sxs-lookup"><span data-stu-id="3feea-129">This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file.</span></span> |
| <span data-ttu-id="3feea-130">折扣</span><span class="sxs-lookup"><span data-stu-id="3feea-130">Discounts</span></span> | <span data-ttu-id="3feea-131">客户从订阅的标准价格接收的折扣。</span><span class="sxs-lookup"><span data-stu-id="3feea-131">The discount that the customer receives from subscription's normal price.</span></span> <span data-ttu-id="3feea-132">此数量显示为 *固定数量*，而不是按单位或许可证的价格显示。</span><span class="sxs-lookup"><span data-stu-id="3feea-132">This number is shown as a *flat amount*, not as a price per unit or license.</span></span> |
| <span data-ttu-id="3feea-133">信用</span><span class="sxs-lookup"><span data-stu-id="3feea-133">Credits</span></span> | <span data-ttu-id="3feea-134">对订阅所做更改的信用或调整 (例如，许可证增加或减少) 。</span><span class="sxs-lookup"><span data-stu-id="3feea-134">Credits or adjustments for changes made to subscriptions (for example, license increases or decreases).</span></span> |
| <span data-ttu-id="3feea-135">小计</span><span class="sxs-lookup"><span data-stu-id="3feea-135">Subtotal</span></span> | <span data-ttu-id="3feea-136">税前总额以及不含税的费用和退款。</span><span class="sxs-lookup"><span data-stu-id="3feea-136">Total before taxes and tax-exclusive charges and credits.</span></span> |
| <span data-ttu-id="3feea-137">税款</span><span class="sxs-lookup"><span data-stu-id="3feea-137">Tax</span></span> | <span data-ttu-id="3feea-138">当前费用的总税款，从发票第2页开始的 **详细信息** 部分中汇总。</span><span class="sxs-lookup"><span data-stu-id="3feea-138">The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice.</span></span> <span data-ttu-id="3feea-139">此数字是基于使用的对帐文件中 " **TaxAmount** " 列 (列 **AA**) 的总费用的总和，以及基于许可证的对帐文件中的 **税款** 列 (列 **U**) 。</span><span class="sxs-lookup"><span data-stu-id="3feea-139">This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file.</span></span> |
| <span data-ttu-id="3feea-140">其他退款</span><span class="sxs-lookup"><span data-stu-id="3feea-140">Other credits</span></span> | <span data-ttu-id="3feea-141">不含税的退款。</span><span class="sxs-lookup"><span data-stu-id="3feea-141">Tax-exclusive credits.</span></span> |
| <span data-ttu-id="3feea-142">当前费用总计</span><span class="sxs-lookup"><span data-stu-id="3feea-142">Total current charges</span></span> | <span data-ttu-id="3feea-143">计费周期的计费币种中到期的金额。</span><span class="sxs-lookup"><span data-stu-id="3feea-143">The amount due in your billing currency for the billing period.</span></span> <span data-ttu-id="3feea-144">这些费用将按支付截止日期到期。</span><span class="sxs-lookup"><span data-stu-id="3feea-144">These charges are due by the payment due date.</span></span> |
| <span data-ttu-id="3feea-145">付款说明</span><span class="sxs-lookup"><span data-stu-id="3feea-145">Payment instructions</span></span> | <span data-ttu-id="3feea-146">介绍如何根据你所在的区域对发票进行付款。</span><span class="sxs-lookup"><span data-stu-id="3feea-146">Description of how to pay your invoice, based on your region.</span></span> <span data-ttu-id="3feea-147">*付款时，请始终确保包含发票号。*</span><span class="sxs-lookup"><span data-stu-id="3feea-147">*Always be sure to include your invoice number when making a payment.*</span></span> |
| <span data-ttu-id="3feea-148">发票编号</span><span class="sxs-lookup"><span data-stu-id="3feea-148">Invoice no</span></span> | <span data-ttu-id="3feea-149">发票的编号。</span><span class="sxs-lookup"><span data-stu-id="3feea-149">The number of your invoice.</span></span> |
| <span data-ttu-id="3feea-150">计费周期</span><span class="sxs-lookup"><span data-stu-id="3feea-150">Billing period</span></span> | <span data-ttu-id="3feea-151">按发票日期的月期间。</span><span class="sxs-lookup"><span data-stu-id="3feea-151">The monthly period leading up to the invoice date.</span></span> <span data-ttu-id="3feea-152">这是使用基于使用情况的服务和基于许可证的服务对许可证计数的任何信用调整或更改进行协调的时间段。</span><span class="sxs-lookup"><span data-stu-id="3feea-152">This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count.</span></span> |
| <span data-ttu-id="3feea-153">发票日期</span><span class="sxs-lookup"><span data-stu-id="3feea-153">Invoice date</span></span> | <span data-ttu-id="3feea-154">每月生成发票的帐单日期或周年周年日。</span><span class="sxs-lookup"><span data-stu-id="3feea-154">The billing date or anniversary date on which your invoice is generated each month.</span></span> |
| <span data-ttu-id="3feea-155">付款期限</span><span class="sxs-lookup"><span data-stu-id="3feea-155">Payment terms</span></span> | <span data-ttu-id="3feea-156">支付期限。</span><span class="sxs-lookup"><span data-stu-id="3feea-156">The payment term.</span></span> <span data-ttu-id="3feea-157">对于一次性购买，此期限将始终为 60 天。</span><span class="sxs-lookup"><span data-stu-id="3feea-157">For one-time purchases this will always be 60 days.</span></span> |
| <span data-ttu-id="3feea-158">付款截止日期</span><span class="sxs-lookup"><span data-stu-id="3feea-158">Payment due date</span></span> | <span data-ttu-id="3feea-159">必须接收付款的截止日期。</span><span class="sxs-lookup"><span data-stu-id="3feea-159">The date by which your payment must be received.</span></span> |
| <span data-ttu-id="3feea-160">客户 PO</span><span class="sxs-lookup"><span data-stu-id="3feea-160">Customer PO</span></span> | <span data-ttu-id="3feea-161">你的采购订单编号。</span><span class="sxs-lookup"><span data-stu-id="3feea-161">Your purchase number order.</span></span> |
| <span data-ttu-id="3feea-162">客户服务</span><span class="sxs-lookup"><span data-stu-id="3feea-162">Customer service</span></span> | <span data-ttu-id="3feea-163">可以访问客户服务的网站地址。</span><span class="sxs-lookup"><span data-stu-id="3feea-163">The website address where you can access customer service.</span></span> |
| <span data-ttu-id="3feea-164">服务接收方</span><span class="sxs-lookup"><span data-stu-id="3feea-164">Service recipient</span></span> | <span data-ttu-id="3feea-165">使用服务的地址。</span><span class="sxs-lookup"><span data-stu-id="3feea-165">The address where the service is being used.</span></span> <span data-ttu-id="3feea-166"> (这是与公司审核相关的合法公司地址 ) </span><span class="sxs-lookup"><span data-stu-id="3feea-166">(This is the legal company address associated with company vetting.)</span></span> |

## <a name="one-time-charges-fields"></a><span data-ttu-id="3feea-167">一次性费用字段</span><span class="sxs-lookup"><span data-stu-id="3feea-167">One-time charges fields</span></span>

<span data-ttu-id="3feea-168">以下字段仅适用于合作伙伴中心的 **一次性费用** ：</span><span class="sxs-lookup"><span data-stu-id="3feea-168">The following fields only apply to **one-time charges** in Partner Center:</span></span>

| <span data-ttu-id="3feea-169">字段</span><span class="sxs-lookup"><span data-stu-id="3feea-169">Field</span></span> | <span data-ttu-id="3feea-170">定义</span><span class="sxs-lookup"><span data-stu-id="3feea-170">Definition</span></span> |
| ----- | ---------- |
| <span data-ttu-id="3feea-171">Date</span><span class="sxs-lookup"><span data-stu-id="3feea-171">Date</span></span> | <span data-ttu-id="3feea-172">购买的日期。</span><span class="sxs-lookup"><span data-stu-id="3feea-172">Date of purchase.</span></span> |
| <span data-ttu-id="3feea-173">说明</span><span class="sxs-lookup"><span data-stu-id="3feea-173">Description</span></span> | <span data-ttu-id="3feea-174">产品名称。</span><span class="sxs-lookup"><span data-stu-id="3feea-174">Product name.</span></span> |
| <span data-ttu-id="3feea-175">数量</span><span class="sxs-lookup"><span data-stu-id="3feea-175">Quantity</span></span> | <span data-ttu-id="3feea-176">采购)  (的产品数。</span><span class="sxs-lookup"><span data-stu-id="3feea-176">The number of products (such as reservations) purchased.</span></span> |
| <span data-ttu-id="3feea-177">单价</span><span class="sxs-lookup"><span data-stu-id="3feea-177">Unit price</span></span> | <span data-ttu-id="3feea-178">按产品定价 (如预订) 。</span><span class="sxs-lookup"><span data-stu-id="3feea-178">Price per product (such as a reservation).</span></span> |
| <span data-ttu-id="3feea-179">折扣</span><span class="sxs-lookup"><span data-stu-id="3feea-179">Discounts</span></span> | <span data-ttu-id="3feea-180">任何适用的折扣。</span><span class="sxs-lookup"><span data-stu-id="3feea-180">Any applicable discounts.</span></span> |
| <span data-ttu-id="3feea-181">税前金额</span><span class="sxs-lookup"><span data-stu-id="3feea-181">Pre-tax amount</span></span> | <span data-ttu-id="3feea-182">税前采购的小计。</span><span class="sxs-lookup"><span data-stu-id="3feea-182">Subtotal of the purchases before taxes.</span></span> |
| <span data-ttu-id="3feea-183">销售税</span><span class="sxs-lookup"><span data-stu-id="3feea-183">Sales tax</span></span> | <span data-ttu-id="3feea-184">税额。</span><span class="sxs-lookup"><span data-stu-id="3feea-184">Tax amount.</span></span> |
| <span data-ttu-id="3feea-185">总计</span><span class="sxs-lookup"><span data-stu-id="3feea-185">Total</span></span> | <span data-ttu-id="3feea-186">要支付的总金额。</span><span class="sxs-lookup"><span data-stu-id="3feea-186">Total amount to be paid.</span></span> |
