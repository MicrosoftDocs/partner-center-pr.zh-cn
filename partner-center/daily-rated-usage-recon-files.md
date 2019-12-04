---
title: 每日分级使用帐文件 |合作伙伴中心
ms.topic: article
ms.date: 11/27/2019
description: 了解如何在合作伙伴中心读取每日分级使用情况协调文件。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d7de5da8529aefb325961ac5c139a9375b66f7e0
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721856"
---
# <a name="daily-rated-usage-reconciliation-files"></a>每日分级的使用情况协调文件

**适用于**

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

**相应的角色**

- 管理员代理
- 帐单管理员
- 销售代理
- 支持人员代理

本主题说明如何读取每日分级使用情况协调文件。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>每日分级使用帐文件中的字段

| 列 | 描述 |
| ------ | ----------- |
| PartnerId | GUID 格式的合作伙伴标识符。 |
| PartnerName | 伙伴名称。 |
| CustomerId | GUID 格式的客户的唯一 Microsoft 标识符。 |
| CustomerCompanyName | 在合作伙伴中心中报告的客户的组织名称。 *此列对于协调发票与系统信息非常重要。* |
| CustomerDomainName | 客户的域名。 对当前活动不可用。 |
| 客户所在国家/地区 | 客户所在的国家/地区。 |
| MPNID | CSP 合作伙伴的 MPN 标识符。 |
| 经销商 MPNID | 订阅的记录分销商的 MPN 标识符。 对当前活动不可用。 |
| InvoiceNumber | 显示指定交易所在的发票号码。 对当前活动不可用。 |
| ProductId | 产品的标识符。 |
| SkuId | 特定 SKU 的标识符。 |
| AvailabilityId | 特定 SKU 可用性的标识符。 这表明 SKU 是否可在给定的国家/地区、货币、行业段等购买。 |
| SKU 名称 | 特定 SKU 的名称。 |
| PublisherName | 发布服务器的名称。 |
| PublisherID | GUID 格式的发布服务器的标识符。 对当前活动不可用。 |
| 订阅说明 | 客户购买的服务产品的名称，如价目表中所定义。 （这是与**OfferName**相同的字段）。 |
| 订阅 ID | Microsoft 帐单平台中订阅的唯一标识符。 不用于对帐。 *此标识符不同于合作伙伴管理控制台上的**订阅 ID** 。* |
| ChargeStartDate | 计费周期的开始日期（在显示以前的计费周期内先前 uncharged 的潜在使用情况数据的日期时除外）。 时间始终是一天的开始，即 0:00。 |
| ChargeEndDate | 计费周期的结束日期（在显示以前的 biling 循环中先前 uncharged 的潜在使用情况数据的日期时除外）。 时间始终是一天的结束，即 23:59。 |
| 使用日期 | 服务使用日期。 |
| 计量类型 | 计量器的类型。 |
| 计量类别 | 使用的顶级服务。 |
| 计量 Id | 所使用的计量的标识符。 |
| 计量子类别 | Azure 服务的类型，该类型可能会影响费率。 |
| 计量名称 | 所使用的计量的度量单位。 |
| 计量区域 | 此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。 |
| 单位 | 资源**名称**的单位。 |
| 已消耗数量 | 报表期间使用的服务量（如*小时*或*GB*）。 包括以前报告期间的任何未开票使用情况。 |
| 资源位置 | > 计量器正在其中运行的数据中心。 |
| 已使用服务 | 你使用的 Azure 平台服务。 |
| 资源 URI | 所使用资源的 URI。 |
| 费用类型 | 费用或调整的类型。 对当前活动不可用。 |
| 单价 | 在购买时价格列表中发布的每个许可证的价格。 请确保此价格与在协调期间存储在计费系统中的信息相匹配。 |
| 数量 | 许可证数量。 请确保此价格与在协调期间存储在计费系统中的信息相匹配。 |
| 单位类型 | 计量计量器的单位类型。 对当前活动不可用。 |
| 帐单税前税 | 税前的总帐单金额。 |
| 计费货币 | 客户的地理区域中的货币。 |
| 定价 pretax 总计 | 添加税款之前的定价。 |
| 定价货币 | 价目表中的货币。 |
| 服务信息1 | 在给定日期预配和使用的服务总线连接数。 |
| 服务信息2 | 捕获可选的服务特定元数据的旧字段。 |
| 附加信息 | 其他列中未涵盖的任何其他信息。 |
