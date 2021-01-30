---
title: 用于 CSP 一次性购买的侦测文件字段
ms.topic: conceptual
ms.date: 01/29/2021
description: 了解 "合作伙伴中心" 中的 CSP 一次性采购对帐文件中的所有项目，包括示例值。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: f1606cceaf9dec1f04850fd85b3924ef75bbfda0
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098799"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP 一次性采购对帐文件字段

## <a name="using-the-recon-file"></a>使用侦测文件
下表提供了针对 CSP 一次性购买的对帐文件中的字段的说明和示例值。

有关对帐文件的详细信息，请参阅 [使用对帐文件](use-the-reconciliation-files.md)。

| 列 | 说明 | 示例值 |
| ------ | ----------- | ------------ |
| PartnerId | 特定计费实体的 GUID 格式的唯一标识符。 对帐不是必需的。 在所有行中均相同。 | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | GUID 格式的客户的唯一 Microsoft 标识符。 | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | 合作伙伴中心报告的客户的组织名称。 此列对于协调发票与系统信息非常重要。 | *Johnny 新式的 DE2* |
| CustomerDomainName | 客户的域名。 | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | 你的客户所在的国家/地区。 查看你所在地区的完整 [国家/地区列表](./regional-authorization-overview.md) 。  | *取消* |
| InvoiceNumber | 与该对帐文件关联的发票号。  | *G002297372* |
| MpnId | CSP 合作伙伴的 MPN 标识符。 有关详细信息，请参阅 [如何按合作伙伴列举](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)。 | *6034453* |
| ResellerMpnId | 订阅的记录分销商的 MPN 标识符。 | *6048879* |
| OrderId | 订单在 Microsoft 计费平台中的唯一标识符。 在联系支持人员时，确定订单可能会很有用。 不用于对帐。 | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | 订单的放置日期。 | *10/3/2020* |
| ProductId | 产品的唯一标识符。 | *DZH318Z0BNZ5* |
| SkuId | SKU 唯一标识符。 | *006G* |
| AvailabilityId | 可用性唯一标识符。 | *DZH318Z08B80* |
| SkuName | SKU 名称。 | *表-LRS* |
| ProductName | 产品名称。 | *表* |
| ChargeType | 费用或调整的 [类型](./recon-file-charge-types.md) 。 | *新建* |
| UnitPrice | 在购买时价格列表中发布的每个许可证的价格。 请确保此项与在协调期间存储在计费系统中的信息相匹配。 | *0.045* |
| 数量 | 许可证数量。 请确保此项与在协调期间存储在计费系统中的信息相匹配。 | *1* |
| 小计 | 税前总额。 小计应等于可计费的数量乘以有效单价。 | *0* |
| TaxTotal | 税费。 基于市场的税务规则和特定情况。 | *0* |
| 总计 | 总金额等于小计加上税额。 | *0* |
| 货币 | 你的帐单在客户货币的上下文中生成。 这意味着，如果你是与使用不同的可结算货币的客户进行交易的合作伙伴，那么你将收到每种客户货币类型的发票。  | *EUR* |
| PriceAdjustmentDescription | 单位价格调整的原因。 这是主要原因，但并不局限于确定有效单价。 | *["15.0% 合作伙伴获得的服务信用额度"]* |
| PublisherName | 产品发布者。  | *Microsoft* |
| PublisherId | 合作伙伴中心用来标识发布者的唯一标识符。 | *\N\N* |
| SubscriptionDescription | 客户购买的服务产品的名称，如价目表中所定义。 此列是与 OfferName 相同的字段。 | *Azure 计划* |
| SubscriptionId | 订阅在 Microsoft 计费平台中的唯一标识符。 不用于对帐。 请注意，此标识符不同于合作伙伴管理控制台上的订阅 ID。 | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | 合作伙伴中心收取订阅费用的日期。 如果使用年度计费条款和每月计费计划购买订阅，则在第一个对帐文件中，这是购买订阅的那一天。 从下一个对帐文件开始，将按30天递增。 | *9/1/2020* |
| ChargeEndDate | 订阅的计费周期的结束日期。 如果使用年度计费条款和每月计费计划购买订阅，则在第一个对帐文件中，这是购买订阅后的30天。 从下一个对帐文件开始，将按30天递增。 | *2020/9/30* |
| TermAndBillingCycle | 在购买时继续订阅的持续时间。 | *存储 (GB/月) 的数据* |
| EffectiveUnitPrice | 计算计费周期成本的按比例分配的单位价格。 折扣、计费日的调整和其他因素确定了有效单位价格。 有关详细信息，请参阅 [有效单位价格计算](./effective-unit-price-calculation.md)。  | *0.03825* |
| Unittype.pixel 度量 | 计量计量器的单位类型。 | *1 GB/月* |
| AlternateId | 引用的订单行项的备用 ID。 | *6dc5c039750a* |
| BillableQuantity | 要计费的总数量。  | *0.005001* |
| BillingFrequency | 在购买时选择的计费计划。 | *\N\N*  |
| PricingCurrency | 价目表中的货币。 | *USD* |
| PCToBCExchangeRate | 定价货币应用于计费货币的汇率。 | *0.846202666* |
| PCToBCExchangeRateDate | 确定计费货币的定价货币的日期。 | *2020/9/30* |
| MeterDescription | 计量说明。  | *表-存储 (GB/月) 的 LRS 数据* |
| ReservationOrderId | 预订订单 Id。 | *E21A6344E398FFC1C4D7...* |

>[!NOTE]
>可在一次性购买侦测文件中协调 Azure 消耗。 若要执行此操作，请在每日按比例使用侦测文件并搜索 SubscriptionID。 这将显示与 Azure 计划 ID 关联的所有成本。 你的 Azure 订阅将显示为 "EntitlementID"。

## <a name="next-steps"></a>后续步骤

- [计费和税款](billing.md)