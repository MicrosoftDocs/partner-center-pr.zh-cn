---
title: 合作伙伴中心 Insights 概述仪表板
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 查看使用许可证、订阅和 Azure 消耗处理销售和部署、客户增长和收入增长的快照。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e274b0a637c7fd4944a395ba7e38154e36d2a9e3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855193"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>简要介绍合作伙伴中心见解内提供的仪表板报表
 
**适当的角色**：全局管理员|管理代理|报表查看器|执行报表查看器

"见解概述"仪表板提供关键绩效指标（如客户、订阅、Azure 消耗收入、许可证）的快照视图。 可以在"概述"报告中可视化以下图表。

- 摘要  
- 客户、订阅和许可证的地理分布  
- 客户增长趋势 
- 订阅增长趋势 
- Azure 已使用收入增长趋势 
- 许可证增长趋势 

## <a name="summary"></a>摘要

摘要包括有关客户、Azure 已使用收入 (ACR) 、销售的订阅、活动订阅和已部署的许可证的信息。 

:::image type="content" source="images/pci/summary.png" alt-text="摘要许可证":::

有关摘要的每个部分，请参阅以下详细信息。

### <a name="customers"></a>客户

" **客户"** 区域包括：

- 通过不同属性类型和所有云产品与公司关联的至少一个活动订阅的所有客户的当前计数。
- 所选日期范围内客户的增长百分比。
- 该微图表显示所选日期范围内客户计数的每月趋势。

### <a name="azure-consumed-revenue-acr"></a>Azure 已使用收入 (ACR) 

摘要 **Azure 已使用收入 (ACR)** 区域包括：

- 在Azure 已使用收入 (范围内) 的总计值（以美元$表示）。
- 在所选日期范围内，属性化 ACR (在 US $) 增长或拒绝百分比。
- 微图显示了 ACR US $ 在所选日期范围内的按月趋势 

> [!NOTE]
> Azure 消耗收入 (ACR) 数据可用于已分配了 Executive 报表查看器角色的用户 
 
### <a name="subscriptions-sold"></a>销售的订阅

摘要中的 " **订阅销售** " 区域包括：

- 云产品订阅的总当前计数 (活动和非活动) 你出售或管理的。  
- 所选日期范围内的订阅增长或拒绝百分比。
- 微图显示了所选日期范围内订阅总数的月趋势。

### <a name="active-subscriptions"></a>活动订阅

摘要上的 " **活动订阅** " 区域包括：

- 基于产品遥测的活动使用情况的当前云产品订阅计数。 这不包括 Azure 订阅的所有试用订阅。  
- 所选日期范围内活动订阅的百分比增长。
- 微图显示了所选日期范围内活动订阅的每月月趋势。
 
### <a name="licenses-deployed"></a>部署的许可证

摘要上 **部署的许可证** 区域包括：
 
- 在所选时间段内部署在客户订阅中的所有云产品许可证的计数。 
- 在选定的日期范围内，这些许可证的增长百分比或拒绝百分比。 
- 微图显示了这些已分配许可证计数在所选日期范围内的月趋势。

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>客户、订阅和许可证的地理分布

此视图是按客户所在国家/地区的客户、订阅和许可证的地理分布。 选择不同的选项卡，在地图上查看每个见解。 可以在网格中搜索并选择国家/地区，以缩放到地图中的位置。 按地图上的"主页"按钮，还原为原始视图。 单击每个 (选项卡，例如，"客户) "选项卡会显示每个国家/地区的指标值，以及国家/地区总计的百分比。  

:::image type="content" source="images/pci/geosummary.png" alt-text="地理摘要":::

## <a name="customers-growth-trend"></a>客户增长趋势

所选日期范围的总客户计数的每月趋势。 X 轴表示所选日期范围的月份，Y 轴表示该月的总客户计数。 

:::image type="content" source="images/pci/customergrowth.png" alt-text="客户增长趋势":::

## <a name="subscriptions-growth-trend"></a>订阅增长趋势

这表示所选日期范围内客户订阅计数的趋势。 X 轴表示所选日期范围的月份，Y 轴表示所选产品的订阅计数。 滚动图表顶部的滑块，将图表缩放到特定的时间段。 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="订阅增长趋势":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure 已使用收入增长趋势

在所选日期范围内，Azure 已使用收入（美元）的每月趋势。 X 轴表示所选日期范围的月份，Y 轴表示当月归为你的 Azure 使用的总收入 US$ 。

> [!NOTE]
> Azure 已使用收入 (ACR) 仅对分配有"执行报告查看器"角色的用户可见。 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Azure 消耗":::

## <a name="licenses-growth-trend"></a>许可证增长趋势
 
所有客户在所选日期范围内分配的许可证趋势。 X 轴表示所选日期范围内的月份，Y 轴表示所选产品的许可证计数。 在图表顶部滚动遍历滑块，以将图表缩放到特定时间段。  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="许可证":::

## <a name="next-steps"></a>后续步骤

有关更多报表，请参阅 [合作伙伴中心见解](partner-center-insights.md)。
