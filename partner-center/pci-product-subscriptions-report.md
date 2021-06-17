---
title: 合作伙伴中心 Insights 订阅报表
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解你表现良好，以及在哪里可以改进为客户销售或管理的云订阅。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf2663122ca95e8d610c8be792a26682ae1718bf
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276308"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>可从 合作伙伴中心 Insights 仪表板获取的产品订阅报表

**适当的角色**：全局管理员|管理代理|报表查看器|执行报表查看器

"产品订阅"报表提供已销售或为客户管理的云订阅的分析。 这是特定于产品的报表，其中包含与云产品（如 Office 365、Azure、Dynamics 等）关联的订阅的性能。

可以从"产品订阅"报表查看以下部分。

- 总结
- 订阅的地理分布
- 订阅添加/改动趋势
- 按合作伙伴位置、销售渠道、SKUS、合作伙伴附加类型、细分市场划分的订阅分发
- 按订阅状态呈现的趋势
- 产品趋势

 > [!NOTE]
 > 此报表可从见解仪表板获取。 若要查看此报表，必须在全局管理员、帐户合作伙伴中心、报表查看器或执行报表查看器等角色中分配特定角色。 有关详细信息，请参阅公司的全局管理员。此报告中的特定数据类型可能也仅可供具有执行报告查看器特权的用户使用。

## <a name="summary"></a>总结

摘要部分提供与客户销售或管理的订阅 (KPI) 的关键绩效指标的快照视图。  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="订阅报表摘要。":::

有关摘要的每个部分的详细信息，请参阅以下内容：

- 订阅：
  - 你销售或管理的云产品订阅的当前计数。
  - 所选日期范围内订阅的增长或拒绝百分比。
  - Micro 图表显示所选日期范围内订阅计数的每月趋势。

- 活动订阅：
  - 云产品订阅的当前计数，其活动使用情况基于产品遥测进行度量。 对于 Azure 订阅，这将排除所有试用订阅。
  - 所选时段内活动订阅的百分比增长或下降。
  - Micro 图表显示所选日期范围内活动订阅的月趋势。

- 已添加订阅：
  - 所选日期范围内 (销售或) 客户订阅总数。 状态为 **"活动"或** " **已续订** "的新订阅计为"已添加的订阅"。
  - 与前一个月相比，上一个完整月份添加的订阅的增长或下降百分比。
  - Micro 图表显示所选日期范围内添加的订阅的每月趋势。

- 改动的订阅：
  - 所选日期范围内客户订阅变动总数。 当月状态 **为"已取消预配**"或"已暂停"的订阅将计为变动订阅。  
  - 所选日期范围内变动的订阅的百分比。
  - Micro 图表显示所选日期范围内流失的订阅的每月趋势。

- 按产品划分的订阅数：按云产品划分的当前订阅计数明细。

## <a name="geographical-spread-of-subscriptions"></a>订阅的地理分布

" **按地理位置划分的订阅** "视图显示按客户市场划分的总订阅的地理分布。 订阅总数包括销售的订阅和活动的订阅。

" **国家/地区** 数量"表显示你拥有订阅的国家/地区总数，以及每个国家/地区的总订阅和有效订阅量。

可以在网格中搜索并选择国家/地区，以缩放到地图中的位置。 按 **地图上** 的"主页"选项可还原为原始视图。 将鼠标悬停在地图上可查看按国家/地区显示的所有订阅和活动订阅。 网格上的两个字段都是可排序的。

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="按地理位置的订阅。":::

## <a name="subscription-addschurns"></a>订阅添加/改动

此视图显示订阅的趋势。 对于所选日期范围，这些类别 ("新建"、"现有) "类别。 X 轴表示所选日期范围的月份。 Y 轴表示订阅计数。 变动的订阅以 Y 轴的负比例表示。 

堆积柱形图显示当月的新订阅、现有订阅和变动订阅的明细。 可以重新生成柱形图，并细分为特定的堆栈项。 为此，请在图例中选择这些特定项。 还可使用图表顶部的滑块放大特定时间段。

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="订阅添加和改动。":::

## <a name="subscription-distribution"></a>订阅分发

此视图按 MPN 位置、客户细分、销售渠道/Azure 定价模型以及属性类型（例如 DPOR、DAP 等）显示当前订阅的 (例如 DPOR、DAP 和其他) 。 选择相应的选项卡以查看按这些类别划分的明细。 若要生成包含特定项类别的明细的饼图，请在图例中选择这些项类别。

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="订阅分发。":::

## <a name="subscription-state-distribution"></a>订阅状态分布

此视图按订阅状态或状态显示当前客户订阅的分布情况。 这包括以下订阅状态：Active、Disabled、Deprovisioned、Open、InGracePeriod、Closed和其他 。     

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="订阅状态分布。":::

## <a name="products-trend"></a>产品趋势

此视图显示条形图和两个饼图。 条形图显示按商业产品（例如 Azure、Office、Dynamics 等）细分的每月订阅趋势。

这两个饼图显示当前客户订阅的细分。 第一个饼图按产品对订阅进行分解。 第二个饼图按 SKUS 或计划分解订阅。 在按产品饼图细分中选择产品时，相邻饼图将显示该产品订阅的明细（按 SKUS）。

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="产品趋势。":::

> [!NOTE]
 > 按 SKUS 细分的订阅计数可能并不总是与该产品的总订阅计数匹配。 如果客户在同一产品订阅下购买了多个 SKUS，则可能会发生这种情况。

## <a name="next-steps"></a>后续步骤

- 有关更多报表，请参阅[合作伙伴中心 Insights。](partner-center-insights.md)

>[!NOTE] 
> 可以从见解仪表板中的"下载报表"部分下载为此报表提供电源的原始数据。 [了解详细信息](pci-download-reports.md) 
