---
title: 每日分级的使用情况协调文件
ms.topic: article
ms.date: 06/12/2020
description: 了解如何在合作伙伴中心读取每日分级使用情况协调文件。 包含侦测文件中特定字段的说明。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147269"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>了解如何在合作伙伴中心读取每日分级使用情况协调文件

**适用** 于：合作伙伴中心 |适用于美国政府的 Microsoft 云合作伙伴中心

**适当的角色**：管理代理 |计费管理 |销售代理 |支持人员代理

本文介绍如何读取每日按比例使用帐文件。

>[!NOTE]
>每日评级使用情况通常需要24小时才会显示在合作伙伴中心，或通过 API 访问。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>每日分级使用帐文件中的字段

| 列 | 说明 |
| ------ | ----------- |
| PartnerId | GUID 格式的合作伙伴标识符。 |
| PartnerName | 合作伙伴名称。 |
| CustomerId | GUID 格式的客户的唯一 Microsoft 标识符。 |
| CustomerName | 合作伙伴中心报告的客户的组织名称。 *此列对于协调发票与系统信息非常重要。* |
| CustomerDomainName | 客户的域名。 |
| CustomerCountry | 客户所在的国家/地区。 |
| MpnId | CSP 合作伙伴的 MPN 标识符。 |
| Tier2MpnId | 订阅的记录分销商的 MPN 标识符。 |
| InvoiceNumber | 指定交易显示时对应的发票号。 |
| ProductId | 产品的标识符。 |
| SkuId | 特定 SKU 的标识符。 |
| AvailabilityId | 特定 SKU 可用性的标识符。 此列显示了 SKU 是否可用于给定国家/地区、货币、行业段等。 |
| SkuName | 特定 SKU 的名称。 |
| ProductName | 产品的名称。 |
| PublisherName | 发行者的名称。 |
| PublisherId | 以 GUID 格式表示的发布服务器标识符。 |
| SubscriptionDescription | 客户购买的服务产品的名称，如价目表中所定义。  (此列与 **OfferName** 字段相同) 。 |
| SubscriptionId | 订阅在 Microsoft 计费平台中的唯一标识符。 不用于对帐。 *此标识符与合作伙伴管理控制台 **上的订阅 ID** 不同。* |
| ChargeStartDate | 计费周期的开始日期 (之前计费周期中未计费的潜在使用情况数据的日期除外) 。 该时间始终为一天的起点时间，即 0:00。 |
| ChargeEndDate | 计费周期的结束日期 (，除非显示上一计费周期中以前未计费的潜在使用情况数据) 。 时间始终是一天的结束，即 23:59。 |
| UsageDate | 服务使用日期。 |
| MeterType | 计量的类型。 |
| MeterCategory | 用量对应的顶级服务。 |
| 计量 ID | 所使用的计量的标识符。 |
| MeterSubCategory | Azure 服务的类型，可能会影响费率。 |
| MeterName | 所消耗计量的度量单位。 |
| MeterRegion | 此列标识计量区域适用的服务区域内的数据中心位置并填充。 |
| 计价单位 | 资源名称 **的单位。** |
| ResourceLocation | 运行计量的数据中心。 |
| ConsumedService | 使用的 Azure 平台服务。 |
| ResourceGroup | 表示保存 Azure 解决方案相关资源的容器。 |
| ResourceURI | 所使用的资源的 URI。 |
| ChargeType | 费用或调整的类型。  |
| 单价 | 每个许可证的价格，在购买时在价目表中发布。 请确保此价格与对帐期间在计费系统中存储的信息匹配。 |
| 数量 | 许可证数。 请确保此价格与对帐期间在计费系统中存储的信息匹配。 |
| Unittype.pixel 度量 | 计量计量器的单位类型。  |
| BillingPreTaxTotal | 税前的总帐单金额。<br/> _**BillingPreTaxTotal** = 楼层 ( ( [ @EffectiveUnitPrice ]*[ @Quantity*] [] @PCToBCExchangeRate ) ，2)_ |
| BillingCurrency | 客户的地理区域中的货币。 |
| PricingPreTaxTotal | 添加税之前的定价。 |
| PricingCurrency | 价目表中的货币。 |
| ServiceInfo1 | 在给定日期预配和使用的服务总线连接数。 |
| ServiceInfo2 | 捕获可选的服务特定元数据的旧字段。 |
| 标记 | 表示由用户设置的 Azure 资源的逻辑组织。 |
| AdditionalInfo | 其他列中未包括的任何其他信息。 |
| EffectiveUnitPrice | 按单位收费的实际值，包括任何折扣、获得的信用额度等。 |
| PCToBCExchangeRate | 定价货币应用于计费货币的汇率。 |
| PCToBCExchangeRateDate | 确定计费货币的定价货币的日期。 |
| EntitlementId | 表示 Azure 订阅 ID。 |
| EntitlementDescription | 表示 Azure 订阅 ID 的名称。 |
| PartnerEarnedCreditPercentage | 显示行项的 PartnerEarnedCredit。 赚取的额度为 0% 或 15% |
| CreditPercentage | 显示 Azure 消耗额度。 赚取的额度为 0 或 100%。 |
| CreditType | 额度的类型。 例如 **，Azure Credit Applied。** |
>[!NOTE]
>每日评分使用情况通常需要 24 小时才能显示在合作伙伴中心 API 访问。


