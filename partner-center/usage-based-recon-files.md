---
title: 基于使用情况的对帐文件
ms.topic: article
ms.date: 06/08/2020
description: 了解合作伙伴中心的基于使用情况的对帐文件上的所有项目。 包含几个示例。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9a84ca15cd51c02a3b5c53ad4478d72343add284
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909115"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>了解基于使用情况的对帐文件及其在合作伙伴中心的特定字段

适用于：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

若要根据客户的使用量来协调您的费用，请将对帐文件中的**ResellerID**、 **ResellerName**和**ResellerBillableAccount**与合作伙伴中心的**客户名称**和**订阅 ID**进行比较。

## <a name="fields-in-usage-based-reconciliation-files"></a>基于使用情况的对帐文件中的字段

以下字段说明已使用的服务和费率。

| 列 | 说明 | 示例值 |
| ------ | ----------- | ------------ |
| PartnerId | 采用 GUID 格式的合作伙伴标识符。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | 合作伙伴名称。 | *Contoso，有限公司。* |
| PartnerBillableAccountId | 合作伙伴帐户标识符。 | *1010578050* |
| CustomerCompanyName | 客户的组织名称，如合作伙伴中心中所报告。 *与系统信息协调发票非常重要。* | *测试客户* |
| MpnId | CSP 合作伙伴的 MPN 标识符。 | *4390934* |
| ResellerMpnId | 订阅的记录分销商的 MPN 标识符。  |
| InvoiceNumber | 指定交易显示时对应的发票号。 | *D020001IVK* |
| ChargeStartDate | 计费周期的开始日期，之前未付款的潜在使用数据（来自上一个计费周期）的显示日期除外。 该时间始终为一天的起点时间，即 0:00。 | *2/1/2019 0:00* |
| ChargeEndDate | 计费周期的结束日期，之前未付款的潜在使用数据（来自上一个计费周期）的显示日期除外。 时间始终是一天的结束，即 23:59。 | *2/28/2019 23:59* |
| SubscriptionId | 订阅在 Microsoft 计费平台中的唯一标识符。 与支持人员联系时，确定订阅可能会很有用。 不用于对帐。 *这不同于合作伙伴管理控制台上的**订阅 ID** 。* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | 服务产品的昵称。 | *Microsoft Azure* |
| SubscriptionDescription | 服务产品的业务线。 | *Microsoft Azure* |
| OrderID | 订单在 Microsoft 计费平台中的唯一标识符。 与支持人员联系时，确定订阅可能会很有用。 不用于对帐。 | *566890604832738111* |
| ServiceName | 存在问题的 Azure 服务的名称。 | *虚拟机* |
| ServiceType | Azure 服务的特定类型。 | *Service Bus-个人或包*、 *SQL Azure 数据库–企业版或 Web 版* |
| ResourceGuid | 针对所有服务数据和定价结构的具体的唯一标识符。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure 资源的名称。 | *数据传输（GB）*，*数据发送 (GB)* |
| 区域 | 使用情况适用的区域。 主要用于分配数据传输费率，因为费率因区域而异。 | *亚太*、*欧洲*、*拉丁美洲**北美* |
| SKU | 产品/服务的唯一 Microsoft 标识符。 | *7UD-00001* |
| DetailLineItemId | 为给定计费期间的服务或资源提供不同费率的标识符和数量。 对于 Azure 分层定价，可能会有一种费率达到特定数量的计费单位，然后以该数量为一个不同的费率。 | *1* |
| ConsumedQuantity | 报表期间使用的服务量（如小时或 GB）。 也包括以前的报告周期中未计费的使用量。 | *11* |
| IncludedQuantity | 包括在套餐中的单元数。 在 CSP 中通常不存在。 | *0* |
| OverageQuantity | 产品/服务中未包含的单元。 合作伙伴必须支付这些费用。 等于**ConsumedQuantity**减**IncludedQuantity**。 | *11* |
| ListPrice | 在订阅的开始日期提供有效价格。 | *$0.0808* |
| PretaxCharges | 等于**ListPrist**乘以**OverageQuantity**，舍入为最接近的美分。 | *$0.085* |
| TaxAmount | 收取的税额。 基于市场的税务规则和特定情况。 | *$0.08* |
| PostTaxTotal | 税后总计（如果需纳税）。 | *$0.93* |
| 货币 | 货币类型。 每个计费实体只有一种货币。 请检查它是否与第一个发票匹配，然后再更新任何主要的计费平台。 | *EUR* |
| PretaxEffectiveRate | 税前单价。 等于**PretaxCharges**除以**OverageQuantity**，舍入为最接近的美分。 | *$0.08* |
| PostTaxEffectiveRate | 税后单价。 等于**PostTaxTotal**除以**OverageQuantity**，舍入为最接近的美分。 或者，等于**PretaxEffectiveRate**加上每单位金额的税率，舍入为最接近的美分。 | *$0.08* |
| ChargeType | 费用或调整的[类型](recon-file-charge-types.md)。 | 请参阅[费用类型](recon-file-charge-types.md)。 |
| CustomerId | 客户的唯一 Microsoft 标识符，采用 GUID 格式。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | 客户的域名。 该字段在第二个计费周期之前可能会显示为空白。 | *example.onmicrosoft.com* |
| BillingCycleType | 时间计费频率。| **每月**  |
| 计价单位 | 资源**名称**的单位。 | *GB*或*小时* |
| CustomerBillableAccount | Microsoft 计费平台中唯一的帐户标识符。 | *1280018095* |
| UsageDate | 服务部署的日期。 | *2/1/2019 0:00* |
| MeteredRegion | 标识区域中数据中心的位置（适用于此值适用和填充的服务）。 | *东亚*、*南东亚*、*北欧*、*西欧*、*美国中北部*、*美国中南部* |
| MeteredService | 标识每个 Azure 服务使用情况（如果未在**ServiceName**列中明确标识）。 例如，数据传输将报告为 Microsoft Azure- **ServiceName**列中的*所有服务*。 | *Accesscontrol-namespace*， *CDN*，*计算*，*数据库*， *ServiceBus*，*存储* |
| MeteredServiceType | **MeteredService**字段的副标题，提供 Azure 服务使用情况的其他说明。 | *路* |
| Project | 客户为其服务实例定义的名称。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | 在给定日期预配和使用的 Azure 服务总线连接的数量。 | *1.000000 连接/30 天*（如果在30天的时间内有单独预配的连接）、 *25 个连接/30 天–使用： 1.000000* （如果已预配25个 Service Bus 连接，并且在那一天使用了1个） |
