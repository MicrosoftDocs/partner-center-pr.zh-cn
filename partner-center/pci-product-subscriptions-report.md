---
title: 合作伙伴中心见解订阅报表
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解你的工作效果，以及你可以在哪些方面改进你为客户销售或管理的云订阅。
keywords: PCI，性能，量化，客户成功，云订阅，分析，报告
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bc9b306e635a27e1bf19f945341f9d8aab834782
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948804"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>合作伙伴中心见解仪表板中提供的产品订阅报表

**相应的角色**
- 全局管理员
- 管理员代理
- 报表查看器
- Executive 报表查看器

"产品订阅" 报表显示已销售的或为客户管理的云订阅的分析。 这是特定于产品的报表，其中包括与云产品（如 Office 365、Azure、Dynamics 等）关联的订阅的性能。

您可以从 "产品订阅" 报表中查看以下部分。

- 总结
- 订阅的地理分布
- 订阅添加/改动趋势
- 按合作伙伴地点、销售渠道、Sku、合作伙伴附加类型、段划分的订阅分发
- 按订阅状态的趋势
- 产品趋势

 > [!NOTE]
 > 此报告可从见解仪表板中获取。 若要查看此报表，您必须在合作伙伴中心分配有特定的角色，例如全局管理员、帐户管理员、报表查看器或执行报表查看器。 有关详细信息，请参阅公司的全局管理员。此报表中特定类型的数据也可能仅对具有 Executive 报表查看器权限的用户可用。

**摘要**

"摘要" 部分显示了与为客户销售或管理的订阅相关的关键绩效指标（Kpi）的快照视图。  

- 订阅：你销售或管理的云产品订阅的当前计数。
所选日期范围内的订阅增长或拒绝百分比。

微图显示在所选日期范围内订阅计数的月月趋势。

- 活动订阅：基于产品遥测的活动使用情况的当前云产品订阅计数。 这不包括 Azure 订阅的所有试用订阅。
所选时间段内活动订阅的增长百分比或拒绝百分比。

微图显示在所选日期范围内活动订阅的每月月趋势。

- 添加的订阅：在所选日期范围内添加（销售或管理）的客户订阅总数。 新订阅的状态为 "**活动**" 或 "已**续订**"，被计为添加的订阅。
与第一个完整月份相比，最后一个完整月份中添加的订阅百分比增长或拒绝。

微图显示在所选日期范围内添加的订阅的每月趋势。

- 订阅改动：在所选日期范围内改动的客户订阅总数。 在该月中状态为**取消预配**或**挂起**的订阅将计为改动订阅。  
所选日期范围内改动的订阅百分比。

微图显示了在所选日期范围内改动订阅的每月趋势。

- 按产品划分的订阅：按云产品对当前订阅计数的细分。

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="订阅报告摘要":::

**订阅的地理分布**

"**按地理位置**划分的订阅" 视图显示按客户市场列出的订阅总数的地理分布。 订阅总数包括销售的订阅和活动订阅。

"**国家/地区/区域数量**" 表显示了订阅的总国家/地区，以及每个国家/地区的总和活动订阅。

您可以在网格中搜索和选择国家/地区，以便缩放到地图中的位置。 按下地图上的**Home**选项，恢复到原始视图。 将鼠标悬停在地图上，以查看按国家/地区划分的所有订阅和活动订阅。 网格中的两个字段均可排序。

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="地域订阅":::

**订阅添加/churns**

此视图显示订阅的趋势。 这些将细分为所选日期范围内的不同类别（新的、现有的改动）。 X 轴表示所选日期范围内的月份。 Y 轴表示订阅计数。 改动订阅在 Y 轴的负刻度上表示。 

堆积柱形图显示了该月的新的、现有的和改动的订阅的细分。 您可以重新生成与特定堆栈项分离的柱形图。 为此，请选择图例中的特定项。 您还可以利用图表顶部的滑块来缩小特定时间段。

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="订阅添加和 churns":::

**订阅分发**

此视图按 MPN 位置、客户细分市场、销售渠道/Azure 定价模型和归属类型（例如 DPOR、进行等）显示当前订阅的细目。 单击相应的选项卡，按这些类别查看细目。 若要生成包含特定项类别细目的饼图，请在图例中选择这些项目类别。

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="订阅分发":::

**订阅状态分发**

此视图按订阅状态显示当前客户订阅的分布情况。 这包括以下订阅状态： "**活动**"、"**已禁用**"、"**取消预配**" **、"已****打开**"、"**已关闭**" 和**其他**。

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="订阅状态分发":::

**产品趋势**

此视图显示一个条形图和两个饼图。 条形图显示了按商业产品（如 Azure、Office、Dynamics 等）细分的订阅的每月趋势。

这两个饼图显示了当前客户订阅的细目分类。 第一个饼图按产品分解订阅。 第二个饼图按 Sku 或计划分解订阅。 当你在 "**按产品**分类的细分" 饼图中选择产品时，相邻饼图将显示 sku 对该产品的订阅的细分。

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="产品趋势":::

> [!NOTE]
 > 由 Sku 分解的订阅计数可能并不总是与该产品的总订阅数相匹配。 如果客户在同一产品订阅下购买了多个 Sku，则可能会发生这种情况。

## <a name="next-steps"></a>后续步骤

- 有关更多报表，请参阅[合作伙伴中心见解](partner-center-insights.md)。
