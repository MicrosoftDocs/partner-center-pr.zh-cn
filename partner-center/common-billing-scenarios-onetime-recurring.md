---
title: Common billing scenarios for one-time and select recurring purchases | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common billing scenarios in Partner Center for one-time and select recurring purchases (such as purchasing subscriptions, adding more subscriptions, adding and removing seats).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, one-time purchase, recurring purchase, subscriptions, seats
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389635"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>One-time and select recurring purchase billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable to [one-time and select recurring charges](one-time-and-recurring-billing.md) in Partner Center.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Purchase a subscription and add a seat on the same day

在场景 1 中，你于 6 月 11 日以 4 美元的单价购买了一个订阅。 在同一天的晚些时候，你以相同的价格又购买了相同的订阅。

对帐文件将包含以下内容：

- 6 月 10 日 - 7 月 9 日服务期的费用为 4 美元。
- 6 月 11 日 - 6 月 11 日服务期内按比例重新计算的费用为 -4.00 美元。 当你有 1 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 30 x 1 = 4.00。
- 6 月 10 日 - 7 月 9 日服务期内按比例重新计算的费用为 8.00 美元。 当你有 2 个许可证时会出现此期间。 计算 = (4/30) x 30 x 2 = 8.00。

|**购买日期**   |**计费开始日期** |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/09         |4 美元                |1                 |4 美元            |新         |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        |1        | -4 美元       |addQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        | 2      |8 美元         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Purchase a subscription and add more subscriptions later

在场景 2 中，你于 6 月 11 日以 4 美元的单价购买了一个订阅，然后在 6 月 12 日以相同的价格购买了同一产品的另一个订阅。

对帐文件将包含以下内容：

- 6 月 10 日 - 7 月 9 日服务期的费用为 4 美元。
- 6 月 11 日 - 6 月 12 日服务期内按比例重新计算的费用为 -3.87 美元。 当你有 1 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 29 x 1 = 3.87。
- 6 月 12 日 - 7 月 9 日服务期内按比例重新计算的费用为 7.74 美元。 当你有 2 个许可证时会出现此期间。 计算 = (4/30) x 29 x 2 = 7.74。

|**购买日期**   |**计费开始日期** |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11（有一个许可证）     |2019/6/10   |2019/7/09         |4 美元         |1        |4 美元            |新         |
|2019/6/12     | 2019/6/10    |2019/7/09        |4 美元        |1        | -3.87 美元       |addQuantity           |
|2019/6/12     | 2019/6/10    |2019/7/09        |4 美元        | 2      |7\.74 美元       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Purchase a subscription and remove a seat on the same day

在场景 3 中，你于 6 月 11 日以 4 美元的单价购买了同一产品的两个订阅。 在同一天的晚些时候，你删除了一个席位。  

对帐文件将包含以下内容：

- 6 月 10 日 - 7 月 9 日两个许可证的服务期费用为 8 美元。
- 6 月 11 日 - 6 月 11 日服务期内按比例重新计算的费用为 -8.00 美元。 当你有 2 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 30 x 2 = 8.00。
- 6 月 11 日 - 7 月 9 日服务期内按比例重新计算的费用为 4.00 美元。 当你有 1 个许可证时会出现此期间。 计算 = (4/30) x 30 x 1 = 4.00。

|**购买日期**   |**计费开始日期** |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/09         |4 美元                |2                 |8 美元            |新         |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        |2        | -8 美元       |removeQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/09        |4 美元        | 1      |4 美元         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Purchase a subscription and remove seats later

在场景 4 中，你于 6 月 11 日以 4 美元的单价购买了 2 个订阅，然后在 6 月 12 日删除了一个席位。

对帐文件将包含以下内容：

- 6 月 10 日 - 7 月 9 日服务期的费用为 8 美元。
- 6 月 11 日 - 6 月 12 日服务期内按比例重新计算的费用为 -7.74 美元。 当你有 2 个许可证时会出现此期间。 计算 =（每月价格/服务期的总天数）x 按比例计算的服务期天数 x 许可证数量 = (4/30) x 29 x 2 = 7.74。
- 6 月 12 日 - 7 月 9 日服务期内按比例重新计算的费用为 3.87 美元。 当你有 1 个许可证时会出现此期间。 计算 = (4/30) x 29 x 1 = 3.87。

|**购买日期**   |**计费开始日期** |**计费结束日期**  |**单价**  |**数量**  |**金额** |**费用类型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11（有 2 个许可证）     |2019/6/10   |2019/7/09         |4 美元         |2        |8 美元       |新       |
|2019/6/12     | 2019/6/10    |2019/7/09        |4 美元        |2        | -7.74 美元       |removeQuantity           |
|2019/6/12（有 1 个许可证）    | 2019/6/10    |2019/7/09   |4 美元    |1      |3\.87 美元    |removeQuantity |
