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
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073792"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP 一次性采购对帐文件字段

**适当的角色**：帐户管理员 |计费代理

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
| OrderDate | 下订单的日期（UTC）。 | *10/3/2020* |
| ProductId | 产品的唯一标识符。 | *DZH318Z0BNZ5* |
| SkuId | SKU 唯一标识符。 | *006G* |
| AvailabilityId | 可用性唯一标识符。 | *DZH318Z08B80* |
| SkuName | SKU 名称。 | *表-LRS* |
| ProductName | 产品名称。 | *表* |
| ChargeType | 费用或调整的 [类型](./recon-file-charge-types.md) 。 | *新建* |
| 单价 | 在购买时价格列表中发布的每个许可证的价格。 请确保此项与在协调期间存储在计费系统中的信息相匹配。 | *0.045* |
| 数量 | 许可证数量。 请确保此项与在协调期间存储在计费系统中的信息相匹配。 | *1* |
| 小计 | 税前总额。 小计应等于可计费的数量乘以有效单价。 | *0* |
| TaxTotal | 税费。 基于市场的税务规则和特定情况。 | *0* |
| 总计 | 总金额等于小计加上税额。 | *0* |
| 货币 | 你的帐单在客户货币的上下文中生成。 这意味着，如果你是与使用不同的可结算货币的客户进行交易的合作伙伴，那么你将收到每种客户货币类型的发票。  | *EUR* |
| PriceAdjustmentDescription | 单位价格调整的原因。 这是主要原因，但并不局限于确定有效单价。 | *["15.0% 合作伙伴获得的服务信用额度"]* |
| PublisherName | 产品发布者。  | *Microsoft* |
| PublisherId | 合作伙伴中心用来标识发布者的唯一标识符。 | *\N\N* |
| SubscriptionDescription | 客户购买的服务产品的名称，如价目表中所定义。 此列与 OfferName 的字段相同。 | *Azure 计划* |
| SubscriptionId | 订阅在 Microsoft 计费平台中的唯一标识符。 不用于对帐。 请注意，此标识符与合作伙伴管理控制台上的订阅 ID 不同。 | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | 订阅计费周期的开始日期。 | *9/1/2020* |
| ChargeEndDate | 订阅的计费周期结束日期。 | *2020/9/30* |
| TermAndBillingCycle | 购买时继续订阅的持续时间承诺。 | *存储的数据 (GB/月)* |
| EffectiveUnitPrice | 用于计算计费周期成本的按比例计算的单价。 折扣、计费天数调整和其他因素决定了有效单价。 有关详细信息，请参阅 [Effective Unit Price Calculation](./effective-unit-price-calculation.md)。  | *0.03825* |
| UnitType | 计量的计费单位类型。 | *1 GB/月* |
| AlternateId | 引用的订单行项的备用 ID。 | *6dc5c039750a* |
| BillableQuantity | 正在计费的总数。  | *0.005001* |
| BillingFrequency | 购买时选择的计费计划。 | *那*  |
| PricingCurrency | 价目表中的货币。 | *USD* |
| PCToBCExchangeRate | 将定价货币应用于计费货币的汇率。 | *0.846202666* |
| PCToBCExchangeRateDate | 确定计费货币的定价货币的日期。 | *2020/9/30* |
| MeterDescription | 计量说明。  | *表 - 存储的 LRS (GB/月)* |
| ReservationOrderId | 预留订单 ID。 | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | 额度说明。 | *Azure 消耗额度* |
| SubscriptionStartDate | 购买订阅的日期。 | *5/1/2021* |
| SubscriptionEndDate | 订阅过期的日期。 | *4/30/2022* |
| ReferenceID | 对升级过程中发生的所有事务进行链接。 | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | 用于了解加载项或试用版购买的标识符。 | *["Add-on"]* |
| PromotionID | 用于提取促销信息的标识符。 | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>可以在一次购买对帐文件中核对 Azure 消耗量。 为此，请转到每日评分使用情况分析文件，并搜索 SubscriptionID。 这将显示与 Azure 计划 ID 关联的所有成本。 Azure SubscriptionID 显示为 EntitlementID。
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>如何将基本订阅与升级后的订阅连接？

你应该使用基本产品的订阅 ID 来查找相应的引用 ID，并使用它们提取所有关联的事务。 与订阅 ID 和引用 ID 相结合，可以连接在单个事件内发生的所有升级。

## <a name="next-steps"></a>后续步骤

- [计费和税款](billing.md)
