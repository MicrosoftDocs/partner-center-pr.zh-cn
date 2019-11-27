---
title: 基于使用情况的对帐文件 |合作伙伴中心
ms.topic: article
ms.date: 11/21/2019
description: 了解合作伙伴中心的基于使用情况的对帐文件。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 3cf0f20ed266fa5302264ef07092d47c050a9206
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389775"
---
# <a name="usage-based-file-fields"></a>基于使用情况的文件字段

适用于：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

若要根据客户的使用量来协调您的费用，请将对帐文件中的**ResellerID**、 **ResellerName**和**ResellerBillableAccount**与合作伙伴中心的**客户名称**和**订阅 ID**进行比较。

## <a name="fields-in-usage-based-reconciliation-files"></a>基于使用情况的对帐文件中的字段

以下字段说明已使用的服务和费率。

| 列 | 说明 | 示例值 |
| ------ | ----------- | ------------ |
| PartnerID | 采用 GUID 格式的合作伙伴标识符。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | 伙伴名称。 | *Contoso，有限公司。* |
| PartnerBillableAccountID | 合作伙伴帐户标识符。 | *1010578050* |
| CustomerName | 客户的组织名称，如合作伙伴中心中所报告。 *与系统信息协调发票非常重要。* | *测试客户* |
| MPNID | CSP 合作伙伴的 MPN 标识符。 | *4390934* |
| ResellerMPNID | 订阅的记录分销商的 MPN 标识符。 有关详细信息，请参阅[如何按合作伙伴列举](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)。 | *4390934* |
| InvoiceNumber | 显示执行交易所在的发票号码。 | *D020001IVK* |
| ChargeStartDate | 计费周期的开始日期（在显示先前 uncharged 的潜在使用情况数据的日期时除外）。 时间始终是一天的开始，即 0:00。 | *2/1/2019 0:00* |
| ChargeEndDate | 计费周期的结束日期，但在显示先前 uncharged 的潜在使用情况数据的日期（来自以前的帐单周期）时除外。 时间始终是一天的结束，即 23:59。 | *2/28/2019 23:59* |
| SubscriptionID | Microsoft 帐单平台中订阅的唯一标识符。 与支持人员联系时，确定订阅可能会很有用。 不用于对帐。 *这不同于合作伙伴管理控制台上的**订阅 ID** 。* | *usCBMgAAAAAAAAIA* |
| 订阅名称 | 服务产品的昵称。 | *Microsoft Azure* |
| SubscriptionDescription | 服务产品的业务线。 | *Microsoft Azure* |
| OrderID | Microsoft 帐单平台中订单的唯一标识符。 与支持人员联系时，确定订阅可能会很有用。 不用于对帐。 | *566890604832738111* |
| ServiceName | 存在问题的 Azure 服务的名称。 | *虚拟机* |
| ServiceType | Azure 服务的特定类型。 | *Service Bus-个人或包*、 *SQL Azure 数据库–企业版或 Web 版* |
| ResourceGUID | 所有服务数据和定价结构的特定唯一标识符。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure 资源的名称。 | *数据传输（GB）* ，*数据发送 (GB)* |
| 地区 | 使用情况适用的区域。 主要用于分配数据传输费率，因为费率因区域而异。 | *亚太*、*欧洲*、*拉丁美洲* *北美* |
| SKU | 产品/服务的唯一 Microsoft 标识符。 | *7UD-00001* |
| DetailLineItemId | 为给定计费期间的服务或资源提供不同费率的标识符和数量。 对于 Azure 分层定价，可能会有一种费率达到特定数量的计费单位，然后以该数量为一个不同的费率。 | *1* |
| 已使用数量 | 报表期间使用的服务量（如小时或 GB）。 此外还包括来自以前报告期间任何未开票的使用量。 | *11x17* |
| IncludedQuantity | 作为产品/服务的一部分包含在内的单位。 在 CSP 中通常不存在。 | *0* |
| OverageQuantity | 产品/服务中未包含的单元。 合作伙伴必须支付这些费用。 等于**ConsumedQuantity**减**IncludedQuantity**。 | *11x17* |
| ListPrice | 在订阅的开始日期提供有效价格。 | *$0.0808* |
| PretaxCharges | 等于**ListPrist**乘以**OverageQuantity**，舍入为最接近的美分。 | *$0.085* |
| TaxAmount | 收取的税额。 基于市场的税务规则和特定情况。 | *$0.08* |
| PostTaxTotal | 税后总额（如果税务适用）。 | *$0.93* |
| Currency | 货币类型。 每个计费单位仅使用一种货币。 请检查它是否与第一个发票匹配，然后再更新任何主要的计费平台。 | *EUR* |
| PretaxEffectiveRate | 每一单位的税前价格。 等于**PretaxCharges**除以**OverageQuantity**，舍入为最接近的美分。 | *$0.08* |
| PostTaxEffectiveRate | 每一单位的税后价格。 等于**PostTaxTotal**除以**OverageQuantity**，舍入为最接近的美分。 或等于**PretaxEffectiveRate** + 每个单位的化税率 amoun，舍入为最接近的美分。 | *$0.08* |
| ChargeType | 费用或调整的[类型](recon-file-charge-types.md)。 | 请参阅[费用类型](recon-file-charge-types.md)。 |
| CustomerBillableAccount | Microsoft 计费平台中唯一的帐户标识符。 | *1280018095* |
| UsageDate | 服务部署日期。 | *2/1/2019 0:00* |
| MeteredRegion | 标识区域中数据中心的位置（适用于此值适用和填充的服务）。 | *东亚*、*南东亚*、*北欧*、*西欧*、*美国中北部*、*美国中南部* |
| MeteredService | 标识每个 Azure 服务使用情况（如果未在**ServiceName**列中明确标识）。 例如，数据传输将报告为 Microsoft Azure- **ServiceName**列中的*所有服务*。 | *Accesscontrol-namespace*， *CDN*，*计算*，*数据库*，，*存储* |
| MeteredServiceType | **MeteredService**字段的副标题，提供 Azure 服务使用情况的其他说明。 | *路* |
| 项目 | 客户定义的服务实例名称。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | 在给定日期预配和使用的 Azure 服务总线连接的数量。 | *1.000000 连接/30 天*（如果在30天的时间内有单独预配的连接）、 *25 个连接/30 天–使用： 1.000000* （如果已预配25个 Service Bus 连接，并且在那一天使用了1个） |
| CustomerID | 客户的唯一 Microsoft 标识符，采用 GUID 格式。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | 客户的域名。 该字段在第二个计费周期之前可能会显示为空白。 | *example.onmicrosoft.com* |
| 单位 | 资源**名称**的单位。 | *GB*或*小时* |
