---
title: Common monthly billing scenarios | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common scenarios in Partner Center when you use monthly billing (such as adding new subscriptions, changing license quantity, and suspending subscriptions.)
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, monthly billing, subscriptions, reconciliation file
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389615"
---
# <a name="monthly-billing-scenarios"></a>Monthly billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable if you use monthly billing in Partner Center.

## <a name="new-monthly-subscription"></a>New monthly subscription

你的计费日期是每个月的 15 日。 1 月 13 日，你以一个许可证每月 4 美元的价格购买了新订阅，并选择按月计费。 1 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |周期费用   |4.00       |1        |4.00 |

2 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |周期费用   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Change license quantity

你的计费日期是每个月的 15 日。 1 月 13 日，你以一个许可证每月 4 美元的价格购买了新订阅，并选择按月计费。 1 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |周期费用   |4.00       |1        |4.00    |

2 月 1 日，你将许可证数量从一个增加到了两个。 2 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |周期实例按比例计算   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | 周期实例按比例计算   |2.45       |1        |2.45    |
|2/1/2018         |2/12/2018    | 周期实例按比例计算   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | 周期实例按比例计算   |4.00       |2        |8.00    |

每月价格为 4.00 并且服务期 1/13/2018 – 2/12/2018 共 31 天。 这相当于每日价格为 0.129 (4/31)。

按比例计算的服务期 1/13/2018 – 1/31/2018 共 19 天。

按比例计算的单价 = 2.451 = 19 x 0.129

按比例计算的服务期 2/1/2018 – 2/12/2018 共 12 天。

按比例计算的单价 = 1.54 = 12 x 0.129

## <a name="suspend-before-30-days"></a>Suspend before 30 days

你的计费日期是每个月的 15 日。 1 月 13 日，你以一个许可证每月 4 美元的价格购买了新订阅，并选择按月计费。 1 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |周期费用   |4.00       |1        |4.00    |

On February 1 you suspend a subscription. 2 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|取消费用|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Suspend after 30 days

你的计费日期是每个月的 15 日。 1 月 13 日，你以一个许可证每月 4 美元的价格购买了新订阅，并选择按月计费。 1 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|周期费用|4.00|1|4.00

2 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|周期费用|4.00|1|4.00

3 月 1 日，你暂停了订阅。 3 月 15 日的基于许可证的对帐文件将包含以下计费行：

|费用开始日期 |费用结束日期 |费用类型 |单价 |数量 |金额 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|取消费用|-1.72|1|-1.72

每月价格为 4.00 并且服务期 2/13/2018 – 3/12/2018 共 28 天。 这相当于每日价格为 0.143 (4/28)。

单价 = 服务期中的天数 x 每日价格 x 许可证数。

取消期间 3/1/2018 – 3/12/2018 共 12 天。

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).
