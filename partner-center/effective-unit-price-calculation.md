---
title: 有效单价计算
ms.topic: how-to
ms.date: 04/02/2021
description: 了解有效单价及其计算方式。 本文还包括一个示例计算。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147116"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure 计划消耗量的有效单位价格计算

**适当的角色**：计费管理员

## <a name="the-effective-unit-price"></a>有效单位价格

有效单位价格在计量级别 (相对于资源级别) 计算，根据计量使用情况进行调整。

我们使用以下三个因素来计算有效单位价格：

- 消耗，在整个计费周期中每天监视
- 计量的计费成本
- 分层 (（如果适用）) 

由于我们会在整个计费周期内监视消耗，因此有效单位价格将会波动。 在停止消耗计算并关闭计费周期后，给定计费周期的最终价格将可用。 在第四个或第五个小数位之后，您将看到大部分使用量的变化。

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>了解计量器是否使用分层定价

如果你不知道计量器是否使用分层定价，请使用以下过程来了解。 

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。
2. 选择 " **销售**"，选择 **定价和产品/服务**，然后选择 " **Azure 计划定价**"。
3. 按 ID 查找计量器，然后下载定价数据。 

## <a name="sample-calculation"></a>示例计算

下表提供了一个示例，说明如何在开放期间计算有效单价。

在表中，以下值适用： 

- **UP** = 资源/小时的单位价格 = 0.868

- **BCU** = 计量的计费消耗单位

- **BC** = 计量的计费成本 = BCU * UP * 0.85。 这反映了 15% PEC 折扣的调整。 然后，我们使用 函数的下限将值限制为小数点后的两位数，以便对最小值收费。 

- **有效单价** = BCU/BC

>[!NOTE]

>注意：此示例中的计量器在定价或其他折扣方面没有层，即折扣百分比和其他调整中的有效单价因素。


| 日期 | BCU (计费消耗单位)  | BC (计费成本)  | 有效单价 |
| ------ | ----------- | ----------- | ----------- |  
| 8 月 3 日 | 29 | 21.39 | 0.737586206896552 |
| 8 月 10 日 | 210.950039 | 155.63 | 0.737757626107858 |
| 8 月 25 日 | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>后续步骤

- [计费和税款](billing.md)
