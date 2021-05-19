---
title: CSP 一次购买的重新确认文件字段
ms.topic: conceptual
ms.date: 01/29/2021
description: 了解云解决方案提供商一次购买对帐文件的所有合作伙伴中心，包括示例值。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146249"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP 一次购买对帐文件字段

**适当角色**：帐户管理员|计费代理

## <a name="using-the-recon-file"></a>使用 recon 文件
下表提供了 CSP 一次购买对帐文件中字段的说明和示例值。

有关对帐文件详细信息，请参阅 [使用对帐文件](use-the-reconciliation-files.md)。

| 列 | 说明 | 示例值 |
| ------ | ----------- | ------------ |
| PartnerId | 特定计费实体的 GUID 格式的唯一标识符。 对帐不需要。 在所有行中均相同。 | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | 采用 GUID 格式的客户的唯一 Microsoft 标识符。 | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | 合作伙伴中心报告的客户的组织名称。 此列对于将发票与系统信息进行对帐非常重要。 | *使用现代 Cust DE2* |
| CustomerDomainName | 客户的域名。 | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | 客户所在的国家/地区。 查看 [你区域的国家](./regional-authorization-overview.md) /地区的完整列表。  | *DE* |
| InvoiceNumber | 与对帐文件关联的发票号。  | *G002297372* |
| MpnId | CSP 合作伙伴的 MPN 标识符。 有关详细信息，请参阅 [如何按合作伙伴列举](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)。 | *6034453* |
| ResellerMpnId | 订阅的记录分销商的 MPN 标识符。 | *6048879* |
| OrderId | 订单在 Microsoft 计费平台中的唯一标识符。 在联系支持人员时，确定订单可能会很有用。 不用于对帐。 | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | 下订单的日期（UTC）。 | *10/3/2020* |
| ProductId | 产品的唯一标识符。 | *DZH318Z0BNZ5* |
| SkuId | SKU 唯一标识符。 | *006G* |
| AvailabilityId | 可用性唯一标识符。 | *DZH318Z08B80* |
| SkuName | SKU 名称。 | *表-LRS* |
| ProductName | 产品名称。 | *表* |
| ChargeType | 费用或调整的 [类型](./recon-file-charge-types.md) 。 | *新建* |
| 单价 | 每个许可证的价格，在购买时在价目表中发布。 请确保这与对帐期间在计费系统中存储的信息匹配。 | *0.045* |
| 数量 | 许可证数。 请确保这与对帐期间在计费系统中存储的信息匹配。 | *1* |
| 小计 | 税前总额。 小计应等于可计费数量乘以有效单价。 | *0* |
| TaxTotal | 税额费用。 根据市场的税务规则和特定情况。 | *0* |
| 总计 | 总金额等于小计加上税额。 | *0* |
| 货币 | 帐单是在客户货币上下文中生成的。 这意味着，如果你是与使用不同的可结算货币的客户进行交易的合作伙伴，那么你将收到每种客户货币类型的发票。  | *EUR* |
| PriceAdjustmentDescription | 单价调整的原因。 这些是主要原因，但不限于确定有效的单价。 | *["15.0% 合作伙伴赚取的托管服务信用额度"]* |
| PublisherName | 产品的发布者。  | *Microsoft* |
| PublisherId | 用于标识合作伙伴中心的唯一标识符。 | *那* |
| SubscriptionDescription | 客户购买的服务产品的名称，如价目表中所定义。 此列与 OfferName 的字段相同。 | *Azure 计划* |
| SubscriptionId | 订阅在 Microsoft 计费平台中的唯一标识符。 不用于对帐。 请注意，此标识符与合作伙伴管理控制台上的订阅 ID 不同。 | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | 订阅的计费周期的开始日期。 | *9/1/2020* |
| ChargeEndDate | 订阅的计费周期的结束日期。 | *2020/9/30* |
| TermAndBillingCycle | 在购买时继续订阅的持续时间。 | *存储 (GB/月) 的数据* |
| EffectiveUnitPrice | 计算计费周期成本的按比例分配的单位价格。 折扣、计费日的调整和其他因素确定了有效单位价格。 有关详细信息，请参阅 [有效单位价格计算](./effective-unit-price-calculation.md)。  | *0.03825* |
| Unittype.pixel 度量 | 计量计量器的单位类型。 | *1 GB/月* |
| AlternateId | 引用的订单行项的备用 ID。 | *6dc5c039750a* |
| BillableQuantity | 要计费的总数量。  | *0.005001* |
| BillingFrequency | 购买时选择的计费计划。 | *那*  |
| PricingCurrency | 价目表中的货币。 | *USD* |
| PCToBCExchangeRate | 将定价货币应用于计费货币的汇率。 | *0.846202666* |
| PCToBCExchangeRateDate | 确定计费货币的定价货币的日期。 | *2020/9/30* |
| MeterDescription | 计量说明。  | *表 - 存储的 LRS (GB/月)* |
| ReservationOrderId | 预留订单 ID。 | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | 额度说明。 | *Azure 消耗额度* |

>[!NOTE]
>可以在一次购买对帐文件中核对 Azure 消耗量。 为此，请转到每日评分使用情况分析文件，并搜索 SubscriptionID。 这将显示与 Azure 计划 ID 关联的所有成本。 Azure SubscriptionID 显示为 EntitlementID。

## <a name="next-steps"></a>后续步骤

- [计费和税款](billing.md)
