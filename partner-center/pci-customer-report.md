---
title: 合作伙伴中心见解 - 客户报表
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 发现改进业务的方法。 按地理位置、产品和其他属性查看特定客户趋势。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9207e793865bcf7fa2f205fc69b0b5def65b4d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152896"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>来自 合作伙伴中心 Insights 的客户仪表板报表

**适当的角色**：全局管理员|管理代理|报表查看器|执行报表查看器

"客户"仪表板显示通过你获取云产品（如 Office、Azure、Dynamics 等）的客户的数据，或让你在租户中部署和管理这些产品的客户的数据。 
 
"客户"仪表板包含以下部分： 

- 总结  
- 客户的地理分布 
- 客户添加/流失趋势 
- 按合作伙伴位置、客户细分、销售渠道、合作伙伴归属类型进行客户分布 
- 按产品的客户分布 
- 按合作伙伴位置、客户细分、定价模型、合作伙伴归属类型分类的客户分布趋势 
- 活跃客户趋势 

## <a name="summary"></a>总结

摘要部分提供与客户相关的各种 KPI 的快照视图，例如客户、活跃客户、订阅、添加的客户、客户流失以及每个产品的客户。 页面级筛选器适用于每个部分。

:::image type="content" source="images/pci/customerproduct.png" alt-text="&quot;客户摘要&quot;仪表板的屏幕截图，其中显示了处于活动状态、最近添加、丢失/流失或按特定产品统计的客户数的条形图和数量。":::

### <a name="customers"></a>客户

- 组织的所有客户的当前计数通过跨所有云产品（如 Office、Azure、Dynamics 等）的不同属性类型关联。如果客户至少有一个订阅处于"活动"状态，则进行计数。  
- 在所选日期范围内拒绝客户百分比 
- 微图表显示所选日期范围内客户计数的月份趋势

### <a name="active-customers"></a>活跃客户

- 任何活动产品使用情况的客户的当前计数，例如任何云产品的活跃使用情况。
- 所选时段内活动客户的增长或下降百分比
- 微图表显示所选日期范围内活跃客户计数的每月趋势。

### <a name="customers-added"></a>已添加客户

- 所选时段内添加的所有客户的计数。
- 所选服务范围内添加的客户的增长或下降百分比。
- 微图表显示所选日期范围内添加的客户每月趋势。

### <a name="customers-churned"></a>客户流失
- 所选时段内每月流失的所有客户的计数。 如果客户没有具有活动状态的单个订阅，则认为客户已丢失。 
- 所选日期范围内流失的客户百分比 
- 微图表显示所选时段内客户流失的月份趋势 
 
### <a name="customers-by-products"></a>按产品的客户

- 跨各种云产品（例如 O365、Azure、Dynamics 等）分布的客户的当前计数。  

## <a name="geographical-spread-of-your-customers"></a>客户的地理分布

当前客户、当前活跃客户和所选日期范围内新添加的客户计数使用客户的国家/地区进行异地映射。 该指标下方显示的百分比表示该国家/地区占该指标总计的百分比。 可以将鼠标悬停在地图上以查看该国家/地区的总活跃新客户。 可以在网格中搜索并选择国家/地区，以缩放到地图中的位置。 选择地图上的"主页 **"按钮，** 还原为原始视图。 可对网格中的所有列进行排序。  

:::image type="content" source="images/pci/customersgeo.png" alt-text="按地域列出的合作伙伴中心见解客户报表的屏幕截图显示世界地图和按区域列出的总计、添加和新客户的列表。":::

## <a name="customer-adds-and-churns"></a>客户添加和 churns

细分为所选日期范围的新的、现有的和改动的客户趋势。 X 轴表示所选日期范围内的月份，Y 轴表示客户计数。 改动客户在 Y 轴的负比例上表示。 堆积柱形图显示了当月的新客户、现有客户和改动客户细分情况。 您可以通过在图例中选择特定的堆栈项来重新生成柱形图。 您可以在图表顶部利用滑块来放大到特定时间段。 

:::image type="content" source="images/pci/customerslost.png" alt-text="使用条形图的合作伙伴中心见解客户报表的屏幕截图显示了在特定时间段内添加、丢失或改动的客户数。":::

## <a name="customer-distribution"></a>客户分发

你的当前客户通过你的 MPN 位置、客户细分市场、销售渠道/Azure 定价模型以及归属)  (的细分。 选择图表上方的各个选项卡，按这些类别查看细目。 通过选择/取消选择特定维度，可以通过选择图例项来重新生成图表。 

## <a name="customers-by-products"></a>按产品的客户

按产品和 Sku/计划对当前客户计数的细分。 选择 product 细分情况饼图中的产品，查看其旁边的图表中的 "Sku/计划" 细分情况。

:::image type="content" source="images/pci/customerbyprod.png" alt-text="按产品列出的客户的屏幕截图显示两个放射图-一个按产品分类，另一个与客户按 SKU 细分。":::

## <a name="customer-distribution-trend"></a>客户分布趋势 

在所选日期范围内，客户在所选日期范围内分布的每月趋势：市场、段、MPN 位置和产品。 在图表中选择相应的选项卡，按这些类别查看趋势。 X 轴表示所选日期范围的月份，Y 轴具有所选类别的客户计数 (选项卡) 。 可以将鼠标悬停在图表列上，以查看每个堆栈的值分解。 可以利用图表顶部的滑块放大到特定的时间段。   

:::image type="content" source="images/pci/customerdistri.png" alt-text="&quot;客户分布趋势&quot;报表的屏幕截图，其中显示了可以按市场、细分市场、合作伙伴位置或产品查看的条形图。":::

## <a name="active-customers"></a>活跃客户

每月趋势图，比较所选日期范围的活动客户和总客户。 列表示每月的活动客户计数，行表示每月的总客户数。 

:::image type="content" source="images/pci/activecustomer.png" alt-text="Insights 合作伙伴中心活动客户报表的屏幕截图，其中显示了活动客户一段时间的条形图。":::

## <a name="next-steps"></a>后续步骤

有关更多报表，请参阅[合作伙伴中心 Insights。](partner-center-insights.md)

>[!NOTE]
> 可以从见解仪表板中的"下载报表"部分下载为此报表提供电源的原始数据。 [了解详细信息](pci-download-reports.md) 
