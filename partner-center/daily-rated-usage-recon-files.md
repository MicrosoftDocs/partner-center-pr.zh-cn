---
title: Daily-rated usage reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand daily-rated usage reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389695"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Daily-rated usage reconciliation files

适用范围：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

This topic explains how to read daily-rated usage reconciliation files.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Fields in daily-rated usage reconciliation files

| 列 | 描述 |
| ------ | ----------- |
| PartnerId | Partner identifier in GUID format. |
| PartnerName | Partner name. |
| CustomerId | Unique Microsoft identifier for the customer in GUID format. |
| CustomerCompanyName | 在合作伙伴中心中报告的客户的组织名称。 *This column is very important for reconciling the invoice with your system information.* |
| CustomerDomainName | The customer's domain name. Not available for current activity. |
| Customer country | 客户所在的国家/地区。 |
| MPNID | MPN identifier of the CSP partner. |
| Reseller MPNID | MPN identifier of the reseller of record for the subscription. Not available for current activity. |
| InvoiceNumber | 显示指定交易所在的发票号码。 Not available for current activity. |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU. |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | 特定 SKU 的名称。 |
| PublisherName | The name of the publisher. |
| PublisherID | The identifier of the publisher in GUID format. Not available for current activity. |
| Subscription Description | 客户购买的服务产品的名称，如价目表中所定义。 (This is an identical field to **OfferName**). |
| 订阅 ID | Microsoft 帐单平台中订阅的唯一标识符。 Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Start date of the billing cycle (except when presenting dates of previously uncharged latent usage data from the previous billing cycle). 时间始终是一天的开始，即 0:00。 |
| ChargeEndDate | End date of billing cycle (except when presenting dates of previously uncharged latent usage data from the previous biling cycle). 时间始终是一天的结束，即 23:59。 |
| Usage Date | Date of service usage. |
| Meter Type | The type of meter. |
| Meter Category | The top-level service for the usage. |
| Meter Id | The identifier for the meter being used. |
| Meter Sub-category | The type of Azure service, which can affect the rate. |
| Meter Name | The unit of measure for the meter being consumed. |
| Meter Region | 此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。 |
| 单位 | The unit of the resource **Name**. |
| Consumed Quantity | The amount of service consumed (such as *hours* or *GB*) during the reporting period. Includes any unbilled usage from previous reporting periods. |
| Resource Location | >The data center where the meter is running. |
| Consumed Service | The Azure platform service that you used. |
| Resource URI | The URI of the resource being used. |
| 费用类型 | 费用或调整的类型。 Not available for current activity. |
| 单价 | Price per license, as published in the price list at the time of purchase. Make sure this price matches the information stored in your billing system during reconciliation. |
| 数量 | Number of licenses. Make sure this price matches the information stored in your billing system during reconciliation. |
| Unit type | The type of unit the meter is charged in. Not available for current activity. |
| Billing pre tax | Total billing amount before taxes. |
| Billing currency | The currency in the customer's geographic region. |
| Pricing pretax total | The pricing before taxes are added. |
| Pricing currency | The currency in the price list. |
| Service Info 1 | The number of Service Bus connections that were provisioned and utilized on a given day. |
| Service Info 2 | A legacy field that captures optional service-specific metadata. |
| Additional Info | Any additional information not covered in other columns. |
