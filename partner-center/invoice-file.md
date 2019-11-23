---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389835"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| 字段 | 定义 |
| ----- | ---------- |
| US FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| 客户编号 | 你的客户编号。 |
| 帐单邮寄地址 | 我们发送发票的地址。 You can change your company name and/or address in your Partner Center billing profile. |
| 基于许可证的费用 | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| 基于使用情况的费用 | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| 折扣 | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| 退款额 | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| 小计 | 税前总额以及不含税的费用和退款。 |
| 税 | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| 其他退款 | 不含税的退款。 |
| 当前总费用 | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| 付款指示 | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| 发票编号 | 发票的编号。 |
| 计费周期 | The monthly period leading up to the invoice date. This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count. |
| 发票日期 | The billing date or anniversary date on which your invoice is generated each month. |
| 付款期限 | The payment term. 对于一次性购买，此期限将始终为 60 天。 |
| 付款截止日期 | The date by which your payment must be received. |
| 客户 PO | Your purchase number order. |
| 客户服务 | The website address where you can access customer service. |
| 服务接收方 | The address where the service is being used. (This is the legal company address associated with company vetting.) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| 字段 | 定义 |
| ----- | ---------- |
| 日期 | 购买的日期。 |
| 描述 | 产品名称。 |
| 数量 | The number of products (such as reservations) purchased. |
| 单价 | Price per product (such as a reservation). |
| 折扣 | 任何适用的折扣。 |
| 税前金额 | 税前购物小计。 |
| 销售税 | 税额。 |
| 总计 | Total amount to be paid. |
