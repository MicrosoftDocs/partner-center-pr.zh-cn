---
title: 一次性和定期对帐文件
ms.topic: article
ms.date: 05/26/2020
description: 了解合作伙伴中心一次性和定期对帐文件中每个字段或列的含义。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3874d384aa1f4b932832d599f73bd601dc73fb07
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943804"
---
# <a name="one-time-and-recurring-reconciliation-files-in-partner-center"></a>合作伙伴中心的一次性和定期对帐文件

**适用于**

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

**相应的角色**

- 全局管理员
- 用户管理员
- 计费管理员
- 管理员代理
- 销售代理

本文介绍如何在合作伙伴中心读取一次性和定期对帐文件。

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>一次性和定期对帐文件中的字段

| 列 | 说明 |
| ------ | ----------- |
| PartnerId | 特定计费实体的唯一 Azure Active Directory （Azure AD）租户标识符，采用 GUID 格式。 对帐不是必需的。 在所有行中均相同。 |
| CustomerId | GUID 格式的唯一 Azure AD 租户标识符。 标识客户。 |
| CustomerName | 客户的组织名称，如合作伙伴中心中所报告。 |
| CustomerDomainName | 客户的域名。 该字段在第二个计费周期之前可能会显示为空白。 *请勿将此字段用作客户的唯一标识符。客户/合作伙伴可以通过 Office 365 门户更新虚或默认域。* |
| CustomerCountry | 客户所在的国家/地区。 |
| InvoiceNumber | 指定交易显示时对应的发票号。 |
| MpnId | CSP 合作伙伴的 MPN 标识符。 |
| OrderId | Microsoft commerce 平台中订单的唯一标识符。 不用于对帐。 |
| OrderDate | 下达订单的日期。 |
| ProductId | 产品的标识符。 |
| SkuId | 特定 SKU （库存单位）的标识符。 |
| AvailabilityId | 特定 SKU 可用性的标识符。 此字段显示 SKU 是否可用于给定国家/地区、货币、行业段等。 |
| SkuName | 特定 SKU 的名称。 |
| ProductName | 产品的名称。 |
| ChargeType | 费用或调整的类型。 |
| UnitPrice | 在购买时价格列表中已发布的单位价格。 *请确保此字段与在对帐期间存储在计费系统中的信息相匹配。* |
| 数量 | 单位数量。 *请确保此字段与在对帐期间存储在计费系统中的信息相匹配。* |
| SubTotal | 税前总额。 如果有折扣，则检查您的小计是否与预期的合计相符。 |
| TaxTotal | 税费。 基于市场的税务规则和特定情况。 |
| 总计 | 税后总额。 检查你是否在发票中计入了税务。 |
| 货币 | 货币类型。 每个计费实体只有一种货币。 请确保此字段与第一个发票匹配，并在进行任何主要计费平台更新后再次检查。 |
| PriceAdjustmentDescription | 适用于任何适用折扣的说明。 |
| PublisherName | 产品发布者的名称。
| PublisherId | 特定发布服务器的唯一标识符。 |
| SubscriptionDescription | 订阅的友好名称。 |
| SubscriptionId | Microsoft commerce 平台中订阅的唯一标识符。 不用于对帐。 *此标识符不同于合作伙伴管理控制台上的**订阅 ID** 。* |
| ChargeStartDate | 费用的开始日。 该时间始终为一天的起点时间，即 0:00。 |
| ChargeEndDate | 费用的结束日。 时间始终是一天的结束，即 23:59。 |
| TermAndBillingcycle | 采购的术语长度和计费周期（例如，*每月1年*）。 |
| EffectiveUnitPrice | 进行调整后的单位价格。 |
| Unittype.pixel 度量 | 要购买的单位类型。 |
| AlternateId | **订单 ID**的替代标识符。 |
| BillableQuantity | 表示购买或消耗的总单位数。 |
| BillingFrequency | 描述行项是每月还是一次性计费频率。 *此字段目前仅支持 Azure RI，每月支持的值为。如果 RI 是通过一次性计费频率购买的，则侦测文件中的此字段将显示为空白。* |
| PricingCurrency | 资源或产品/服务的定价。 |
| PCToBCExchangeRate | 定价货币应用于计费货币的汇率。 |
| PCToBCExchangeRateDate | 确定计费货币的定价货币的日期。 |
| MeterDescription | 消耗行项的计量说明。 |
