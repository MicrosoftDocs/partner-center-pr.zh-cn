---
title: 基于许可证的对帐文件 |合作伙伴中心
ms.topic: article
ms.date: 01/14/2020
description: 了解合作伙伴中心的基于许可证的对帐文件。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 304c727fea7605f52fc0b99625d21cc6d148a585
ms.sourcegitcommit: fc43ee25d405ef3dc673edd884c877bfc62ad6aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2020
ms.locfileid: "76021731"
---
# <a name="license-based-reconciliation-files"></a>基于许可证的对帐文件

**适用于**

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

**相应的角色**
-   全局管理员
-   用户管理员
-   帐单管理员
-   管理员代理

若要对客户的订单进行协调，请将对帐文件中的**Syndication_Partner_Subscription_Number**与合作伙伴中心的**订阅 ID**进行比较。

## <a name="fields-in-license-based-reconciliation-files"></a>基于许可证的对帐文件中的字段

| 列 | 描述 | 示例值 |
| ------ | ----------- | ------------ |
| PartnerId | 特定计费实体的 GUID 格式的唯一标识符。 对帐不是必需的。 在所有行中均相同。 | *8ddd03642--46b58d356b4e* |
| CustomerId | GUID 格式的客户的唯一 Microsoft 标识符。 | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | 客户的组织名称，如合作伙伴中心中所报告。 *用于使发票与系统信息进行协调的非常重要的字段。* | *测试客户 A* |
| MpnId | CSP 合作伙伴的 MPN 标识符。 请参阅[如何按合作伙伴列举](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)。 | *4390934* |
| ResellerMpnId | 订阅的记录分销商的 MPN 标识符。  |
| OrderId | Microsoft 帐单平台中订单的唯一标识符。 在联系支持人员时，确定订单可能会很有用。 不用于对帐。 | *566890604832738111* |
| SubscriptionId | Microsoft 帐单平台中订阅的唯一标识符。 与支持人员联系时，确定订阅可能会很有用。 不用于对帐。 *此值不同于合作伙伴管理控制台上的**订阅 ID** 。请参阅**SyndicationPartnerSubscriptionNumber** 。* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | 订阅的唯一标识符。 对于同一计划，一个客户可以具有多个订阅。 此列对于协调文件分析非常重要。 此字段映射到合作伙伴管理员控制台中的**订阅 ID** 。 | *fb977ab5--24c8d9591708* |
| OfferID | 唯一产品标识符。 标准产品/服务标识符，如价目表中所定义。 *此值与价目表中的**产品 ID**不匹配。请参阅**DurableOfferID** 。* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | 价目表中定义的唯一持久性提议标识符。 *此值与价目表中的**产品 ID**匹配。* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 客户购买的服务产品的名称，如价目表中所定义。 | *Microsoft Office 365 （Plan E3）* |
| SubscriptionStartDate | 订阅的开始日期。 时间始终是一天的开始，即 0:00。 此字段设置为提交订单后的那一天。 与**subscription.subscriptionenddate**结合使用以确定：客户是否仍在订阅的第一年内，或者是否已续订了下一年的订阅。 | *2/1/2019 0:00* |
| SubscriptionEndDate | 订阅结束日期。 时间始终是一天的开始，即 0:00。 *12 个月 + 开始日期之后的**x**天*，以与合作伙伴的计费日期或*从续订日期起12个月*的时间一致。 续订时，价格将更新为当前价目表。 自动续订之前可能需要与客户进行通信。 | *2/1/2019 0:00* |
| ChargeStartDate | 费用的开始日。 时间始终是一天的开始，即 0:00。 用于在客户更改座位号码时计算每日费用（*pro 每*费用）。 | *2/1/2019 0:00* |
| ChargeEndDate | 费用的结束日。 时间始终是一天的结束，即 23:59。 用于在客户更改座位号码时计算每日费用（*pro 每*费用）。 | *2/28/2019 23:59* |
| ChargeType | 费用或调整的[类型](recon-file-charge-types.md)。 | 请参阅[费用类型](recon-file-charge-types.md)。 |
| UnitPrice | 购买时公布在价目表中的每一席位的价格。 请确保此项与在协调期间存储在计费系统中的信息相匹配。 | *6.82* |
| 数量 | 席位的数量。 请确保此项与在协调期间存储在计费系统中的信息相匹配。 | *2* |
| 金额 | 数量的总价。 用于检查量计算是否与你为客户计算此值的方式匹配。 | *13.32* |
| TotalOtherDiscount | 适用于这些费用的折扣金额。 资格或地图随附的产品许可证，或符合激励条件的新订阅，还将在此列中包含折扣金额。 | *2.32* |
| 小计 | 税前总额。 检查小计是否与预期的总计匹配（如果是折扣）。 | *11* |
| 税 | 税费。 基于市场的税务规则和特定情况。 | *0* |
| TotalForCustomer | 税后总额。 检查你是否在发票中计入了税务。 | *11* |
| 货币 | 货币类型。 每个计费单位仅使用一种货币。 检查它是否与第一个发票匹配。 在进行任何主要计费平台更新后再次检查。 | *EUR* |
| DomainName | 客户的域名。 该字段在第二个计费周期之前可能会显示为空白。 *请勿将此字段用作客户的唯一标识符。客户/合作伙伴可以通过 Office 365 门户更新虚或默认域。* | *example.onmicrosoft.com* |
| SubscriptionName | 订阅昵称。 如果未指定昵称，则合作伙伴中心将使用**OfferName**。 | *项目联机* |
| SubscriptionDescription | 客户购买的服务产品的名称，如价目表中所定义。 （这是与**OfferName**相同的字段。） | *项目在线高级版，无需 PROJECT 客户端* |
| BillingCycleType | 一次性计费频率。| *每月* |
