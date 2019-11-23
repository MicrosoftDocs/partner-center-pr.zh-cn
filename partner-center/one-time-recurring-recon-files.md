---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389675"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

适用范围：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| 列 | 描述 |
| ------ | ----------- |
| PartnerId | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. 在所有行中均相同。 |
| Customer Id | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| 客户名称 | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. 该字段在第二个计费周期之前可能会显示为空白。 *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Customer Country | 客户所在的国家/地区。 |
| 发票编号 | 显示指定交易所在的发票号码。 |
| MpnId | MPN identifier of the CSP partner. |
| Reseller MpnId | MPN identifier of the reseller of record for the subscription. |
| 订单编码 | Unique identifier for an order in the Microsoft commerce platform. Not used for reconciliation. |
| 订单日期 | 下达订单的日期。 |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | 特定 SKU 的名称。 |
| 产品名称 | 产品的名称。 |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Subscription Description | Friendly name of a subscription. |
| 订阅 ID | Unique identifier for a subscription in the Microsoft commerce platform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | 费用的开始日。 时间始终是一天的开始，即 0:00。 |
| ChargeEndDate | 费用的结束日。 时间始终是一天的结束，即 23:59。 |
| Term and Billingcycle | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| 费用类型 | 费用或调整的类型。 |
| 单价 | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effective Unit Price | The unit price after adjustments have been made. |
| 数量 | Number of units. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Unit type | The type of unit being purchased. |
| DiscountDetails | An explanation of any applicable discount. |
| Sub Total | 税前总额。 Checks if your subtotal matches your expected total, in case of a discount. |
| Tax Total | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| 总计 | 税后总额。 检查你是否在发票中计入了税务。 |
| 货币 | 货币类型。 每个计费单位仅使用一种货币。 Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
