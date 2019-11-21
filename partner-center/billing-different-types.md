---
title: 了解合作伙伴中心中的计费类型 | 合作伙伴中心
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn about different billing types, billing periods, and billing dates you might see in Partner Center.
author: MaggiePucciEvans
ms.author: evansma
keywords: 计费, 付款, 订单, 对帐文件
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 539d3150e571c33114feee2d316611d7ac324f24
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253195"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>了解合作伙伴中心的计费类型

**适用于**

-  合作伙伴中心
-  云解决方案提供商计划中的合作伙伴

根据为客户购买的具体产品类型，你可能会有不同的计费周期，并且我们可能会在同一月内的不同日期向你收费。 本文介绍了从 2019 年 3 月 1 日起进行的更改，以及这些更改将对你造成的影响。

## <a name="billing-for-recurring-charges"></a>定期费用的计费

对于基于许可证和基于使用情况的订阅，这些订阅的定期费用的计费体验不会发生更改。 We'll continue to bill you on the day of the month you selected as your billing date, and your billing period will continue to be the month prior to that date. If you selected the 15th day of the month for your billing date, you'll be billed for all activity from the 15th of one calendar month to the 14th of the next calendar month. 发票和对帐文件通常可以在计费日期后的 2-4 天内获取。

As before, we'll bill you for these products in the currency for the country/region you're located in, regardless of the location of the customer you sold the product to.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>一次性和选择性定期费用的计费

从 2019 年 3 月 1 日开始，我们为 Microsoft 和第三方 ISV 产品的定期和一次性费用引入了新的计费体验。

这些产品的计费周期从日历月的第一天开始，于日历月的最后一天结束。 We'll make your invoice available on the 8th day of the following month. 

换言之，你在 2019 年 5 月 1 日和 5 月 31 日之间进行的任何交易都将显示在 6 月 8 日的发票上。 你在 2019 年 6 月 1 日到 6 月 30 日之间进行的任何交易都将显示在 7 月 8 日的发票上。 我们可能还会在同一张发票上向你收取定期和一次性购买的费用。 

你还可以随时检查你的帐户余额/帐单（例如 5 月 1 日到 6 月 7 日之间的余额/帐单）并且查看最近的帐户活动，而无需等待发票的开具。 请注意，当我们在 8 日发布你的帐单时，此帐单中将包含税费以及任何其他适用的费用和贷记，因此最终金额与你在计费周期期间看到的金额可能会存在出入。 

You'll access your invoices the same way you do now, either in Partner Center or by API. They'll appear before midnight UTC on the 8th day of the month. 

|**计费体验**|**产品类型**|**计费日期**|**计费周期**|**计费货币**|**当前活动是否可用？**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|基于许可证和基于使用情况的订阅的定期费用 |[在线服务目录](https://partner.microsoft.com/commerce/preferredoffers/list)中的所有产品。 例如，Office 365、Microsoft 365、Azure Active Directory、Azure（即用即付）、Dynamics 365、PowerBI Pro |创建合作伙伴中心帐户时选择的日期 |计费日期之前的那个月。 |The currency of the country/region you're located in. For example, if your company is located in the United Kingdom, we'll bill you in British pounds sterling (GBP). If your company is located in India, we'll bill you in India Rupees (INR).  |无 |
|Microsoft 和第三方 ISV 产品的定期和一次性费用 |Microsoft 和第三方 ISV 提供的所有 SaaS 订阅、Azure 预订和软件（永久软件和基于订阅的软件）产品。 请参阅[市场](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)中的可用产品。 例如，SUSE Linux 软件（软件订阅）、Windows Server 2019 Essentials（永久软件）、Azure ISV SaaS 产品订阅。 |每月 8 日 |每个日历月的第一天起到最后一天 |你的客户所在国家/地区的货币。 This means you'll receive separate invoices and reconciliation files in the currency of the country/region each customer you sold to in the billing period. |“是” |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>一次性和定期购买的计费场景
### <a name="scenario-1---purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Scenario 1 - Purchase a subscription and then add a seat on the same day

在场景 1 中，你于 6 月 11 日以 4 美元的单价购买了一个订阅。 在同一天的晚些时候，你以相同的价格又购买了相同的订阅。 

对帐文件将包含以下内容： 
-   $4 bill for service period June 10 - July 9. 
-   $-4.00 prorated rebill for service period June 11 - June 11. 当你有 1 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 30 x 1 = 4.00。
-   $8.00 prorated rebill for service period June 10 - July 9. 当你有 2 个许可证时会出现此期间。 计算 = (4/30) x 30 x 2 = 8.00。

|**购买日期**   |**计费开始日期**  |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/09         |4 美元                |1                 |4 美元            |新         |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        |1        | -4 美元       |addQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        | 2      |8 美元         |addQuantity           |

### <a name="scenario-2---purchase-a-subscription-and-then-add-more-later"></a>Scenario 2 - Purchase a subscription and then add more later

在场景 2 中，你于 6 月 11 日以 4 美元的单价购买了一个订阅，然后在 6 月 12 日以相同的价格购买了同一产品的另一个订阅。 

对帐文件将包含以下内容： 
-   $4 bill for service period June 10 - July 9. 
-   $-3.87 prorated rebill for service period June 11 - June 12. 当你有 1 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 29 x 1 = 3.87。
-   $7.74 prorated rebill for service period June 12 - July 9. 当你有 2 个许可证时会出现此期间。 计算 = (4/30) x 29 x 2 = 7.74。

|**购买日期**   |**计费开始日期**  |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11（有一个许可证）     |2019/6/10   |2019/7/09         |4 美元         |1        |4 美元            |新         |
|2019/6/12     | 2019/6/10    |2019/7/09        |4 美元        |1        | -3.87 美元       |addQuantity           |
|2019/6/12     | 2019/6/10    |2019/7/09        |4 美元        | 2      |7\.74 美元       |addQuantity           |

### <a name="scenario-3---purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Scenario 3 - Purchase a subscription and then remove a seat on the same day

在场景 3 中，你于 6 月 11 日以 4 美元的单价购买了同一产品的两个订阅。 在同一天的晚些时候，你删除了一个席位。  

对帐文件将包含以下内容： 
-   $8 bill for two licenses for service period June 10 - July 9. 
-   $-8.00 prorated rebill for service period June 11 - June 11. 当你有 2 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 30 x 2 = 8.00。
-   $4.00 prorated rebill for service period June 11 - July 9. 当你有 1 个许可证时会出现此期间。 计算 = (4/30) x 30 x 1 = 4.00。

|**购买日期**   |**计费开始日期**  |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/09         |4 美元                |2                 |8 美元            |新         |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        |2        | -8 美元       |removeQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        | 1      |4 美元         |removeQuantity           |

### <a name="scenario-4---purchase-a-subscription-and-then-remove-seats-later"></a>Scenario 4 - Purchase a subscription and then remove seats later

在场景 4 中，你于 6 月 11 日以 4 美元的单价购买了 2 个订阅，然后在 6 月 12 日删除了一个席位。 

对帐文件将包含以下内容： 
-   $8 bill for service period June 10 - July 9. 
-   $-7.74 prorated rebill for service period June 11 - June 12. 当你有 2 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 29 x 2 = 7.74。
-   $3.87 prorated rebill for service period June 12 - July 9. 当你有 1 个许可证时会出现此期间。 计算 = (4/30) x 29 x 1 = 3.87。

|**购买日期**   |**计费开始日期**  |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11（有 2 个许可证）     |2019/6/10   |2019/7/09         |4 美元         |2        |8 美元       |新       |
|2019/6/12     | 2019/6/10    |2019/7/09        |4 美元        |2        | -7.74 美元       |removeQuantity           |
|2019/6/12（有 1 个许可证）    | 2019/6/10    |2019/7/09   |4 美元    |1      |3\.87 美元    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>基于许可证的免费试用版 SaaS 交易的计费场景
### <a name="scenario-5---renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Scenario 5 - Renew a license-based free trial SaaS subscription to a paid subscription at the end of the free trial period

在此场景中，你于 6 月 10 日购买了一个基于许可证的免费试用版 SaaS（软件即服务）订阅，此订阅在免费试用期结束时自动续订为付费订阅。 

对帐文件将包含以下内容： 
- $0 bill for service period June 10 - July 9 
- $2 bill for service period July 10 - August 9

|**购买日期**   |**计费开始日期**  |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/10（有 1 个许可证）      |2019/6/10   |2019/7/09         |0 美元                |1                 |0 美元            |新         |
|2019/7/10（有 1 个许可证）     | 2019/7/10    |2019/8/09        |2 美元        |1        | 2 美元       |续订           |

### <a name="scenario-6---cancel-a-license-based-free-trial-saas-subscription"></a>Scenario 6 - Cancel a license-based free trial SaaS subscription

即使在免费试用期间，你也可以随时取消基于许可证的免费试用版 SaaS（软件即服务）订阅。 

在此场景中，你于 7 月 1 日购买了一个基于许可证的免费试用版 SaaS 订阅，随后立即在合作伙伴中心中取消了此订阅。 

对帐文件将包含以下内容： 
- $0 bill for service period June 10th  - July 9th  for the new purchase
- $0 bill for service period July 10th  - July 9th for the cancelation

|**购买日期**   |**计费开始日期**  |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/10（有 11 个许可证）      |2019/6/10   |2019/7/09         |0 美元                |11                |0 美元            |新         |
|2019/6/10（没有许可证）     | 2019/6/10    |2019/7/09        |0 美元        |11       | 0 美元       |取消           |

### <a name="scenario-7---convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Scenario 7 - Convert a custom meter SaaS subscription from one SKU to another for the same product on the same day

在此场景中，你购买了一个产品下的某一 SKU（银牌服务），并在同一天将其转换为此产品下其他可用的 SKU（铜牌服务）。 

对帐文件将包含以下内容： 
- $20 bill of Silver for service period June 10th, 2019 - July 9th, 2020
- $20 prorated rebill for Silver for service period June 10th, 2019 - July 9th, 2020
- $10 bill of Bronze for service period June 10th, 2019 - July 9th, 2020

|**购买日期**   |**SKU**   |**计费开始日期**   |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|2019/6/10（有 1 个许可证） |银牌     |2019/6/10   |2019/6/10         |20 美元        |1         |20 美元            |新      |
|2019/6/10（有 1 个许可证） |银牌    | 2019/6/10    |2019/6/10        |20 美元        |1       | -20 美元       |转换           |
|2019/6/10（有 1 个许可证） |铜牌服务    | 2019/6/10    |2019/6/10        |10 美元        |1       | 10 美元       |转换           |

### <a name="scenario-8---purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Scenario 8 - Purchase and cancel a custom meter SaaS subscription from the Azure portal on the same day 

在此场景中，你在 Azure 门户上购买了一个自定义计量 SaaS 订阅，然后在同一天取消了该订阅。 

|**购买日期**   |**SKU**   |**计费开始日期**   |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|2019/6/10（有 1 个许可证） |铜牌服务     |2019/6/10   |2019/6/10         |10 美元        |1         |10 美元            |新      |
|2019/6/10（没有许可证） |铜牌服务    | 2019/6/10    |2019/6/10        |10 美元        |1       | -10 美元       |CancelImmediate  |

## <a name="billing-under-the-azure-plan"></a>Billing under the Azure plan

- **Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).

- **Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1 - 10/31, 11/1 - 11/30).

- **Charge service periods**: Charges will align to the calendar month. 例如，如果计费合作伙伴在 10/15 通过 Azure 计划添加了 Azure 服务，而客户在 10/15 开始使用 Azure 服务，则计费合作伙伴将在 11/8 收到客户在服务周期 10/15 - 10/31 的使用费发票/对帐文件。 The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.

- **Invoice payment term**: Net 60 days.

- **Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency. 例如，如果计费合作伙伴位于爱尔兰，而客户位于英国、挪威和德国，则计费合作伙伴将收到英镑、挪威克朗和欧元货币的发票/对帐文件。

- **Partner incentives**: Paid 45 days from the end of the invoice month.

For information on the Azure plan see:

- [Azure plan - overview](azure-plan-get-started.md)

- [Azure plan - billing](azure-plan-billing.md)