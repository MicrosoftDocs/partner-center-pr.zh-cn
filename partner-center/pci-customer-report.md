---
title: 合作伙伴中心见解-客户报表
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解提高业务的方式。 按地域、产品和其他属性查看特定客户趋势。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1ec30db0d568c7477b6fba9639e6481ffecaaf5
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565519"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>合作伙伴中心见解中的客户仪表板报表

**适当的角色**：全局管理员 |管理代理 |报表查看器 |Executive 报表查看器

客户仪表板显示已获取云产品（如 Office、Azure 和 Dynamics）的客户的数据。 你或使用你在其租户中部署和管理这些产品。 
 
客户仪表板包含以下部分： 

- 总结  
- 客户的地理分布 
- 客户添加/改动趋势 
- 按合作伙伴地点、客户群、销售渠道、合作伙伴归属类型分类的客户分销 
- 按产品的客户分发 
- 按合作伙伴地点、客户群、定价模型、合作伙伴归属类型分类的客户分布趋势 
- 活动客户趋势 

## <a name="summary"></a>总结

"摘要" 部分提供了一个快照视图，其中列出了与客户相关的各种关键性能指标 (Kpi) ，如客户、活动客户、订阅、添加的客户、客户改动和每个产品的客户。 页面级筛选器适用于每个部分。

:::image type="content" source="images/pci/customerproduct.png" alt-text="&quot;客户摘要&quot; 仪表板的屏幕截图显示条形图以及活动、最近添加、丢失/改动或特定产品的客户数。":::

### <a name="customers"></a>客户

- 组织通过各种云产品（如 Office、Azure 和 Dynamics）中的不同归属类型关联的所有客户的当前计数。 如果客户的至少一个订阅的状态为 "活动"，则将对其进行计数。  
- 在所选日期范围内拒绝客户的百分比 
- 微图按月显示客户在所选日期范围内计数的趋势

### <a name="active-customers"></a>活动客户

- 具有任何活动产品使用情况的客户的当前计数，例如任何云产品上的可用使用率。
- 所选时间段内活动客户的增长或拒绝百分比
- 微图显示了在所选日期范围内活动客户数的月趋势。

### <a name="customers-added"></a>添加的客户

- 在选定时间段内添加的所有客户的计数。
- 在选定的状态范围内添加的客户的增长或拒绝百分比。
- 微图显示了在所选日期范围内添加的客户的月趋势。

### <a name="customers-churned"></a>客户改动
- 所选时间段内每个月改动的所有客户的计数。 如果客户不具有具有活动状态的单一订阅，则会被视为丢失。 
- 所选日期范围内改动的客户的百分比 
- 微图显示了改动在所选时间段内的客户的月趋势 
 
### <a name="customers-by-products"></a>按产品的客户

- 跨各种云产品（如 Office 365、Azure 和 Dynamics）分发的客户的当前计数。  

## <a name="geographical-spread-of-your-customers"></a>客户的地理分布

在所选日期范围内，当前客户、当前活动客户和客户的计数是使用客户所在国家/地区进行地理映射的。 指标下显示的百分比表示该指标的该国家/地区的总贡献百分比。 您可以将鼠标悬停在地图上，以查看该国家/地区的活动、新客户总数。 您可以在网格中搜索和选择国家/地区，以便缩放到地图中的位置。 通过选择地图上的 " **主页** " 按钮，还原到原始视图。 可对网格中的所有列进行排序。  

:::image type="content" source="images/pci/customersgeo.png" alt-text="按地域列出的合作伙伴中心见解客户报表的屏幕截图显示世界地图和按区域列出的总计、添加和新客户的列表。":::

## <a name="customer-adds-and-churns"></a>客户添加和 churns

细分为所选日期范围的新的、现有的和改动的客户趋势。 X 轴表示所选日期范围内的月份，Y 轴表示客户计数。 改动客户在 Y 轴的负比例上表示。 堆积柱形图显示了当月的新客户、现有客户和改动客户细分情况。 您可以通过在图例中选择特定的堆栈项来重新生成柱形图。 您可以在图表顶部利用滑块来放大到特定时间段。 

:::image type="content" source="images/pci/customerslost.png" alt-text="使用条形图的合作伙伴中心见解客户报表的屏幕截图显示了在特定时间段内添加、丢失或改动的客户数。":::

## <a name="customer-distribution"></a>客户分发

Microsoft 合作伙伴网络 (MPN) 位置、客户段、销售渠道/Azure 定价模型和归属类型的当前客户的细分。 选择图表上方的各个选项卡，按这些类别查看细目。 通过选择/取消选择特定维度，可以通过选择图例项来重新生成图表。 

## <a name="customers-by-products"></a>按产品的客户

按产品和 Sku/计划对当前客户计数的细分。 选择 product 细分情况饼图中的产品，查看其旁边的图表中的 "Sku/计划" 细分情况。

:::image type="content" source="images/pci/customerbyprod.png" alt-text="按产品列出的客户的屏幕截图显示两个放射图-一个按产品分类，另一个与客户按 SKU 细分。":::

## <a name="customer-distribution-trend"></a>客户分布趋势 

在所选日期范围内，客户在所选日期范围内分布的每月趋势：市场、段、MPN 位置和产品。 选择图表中的各个选项卡以查看这些类别的趋势。 X 轴表示所选日期范围的月份，Y 轴包含所选类别 (选项卡选择) 的客户计数。 您可以将鼠标悬停在图表列上以查看每个堆栈的细分情况值。 您可以在图表顶部利用滑块来放大到特定时间段。   

:::image type="content" source="images/pci/customerdistri.png" alt-text="&quot;客户分发趋势&quot; 报表的屏幕截图，显示可以按市场、段、合作伙伴位置或产品查看的条形图。":::

## <a name="active-customers"></a>活动客户

每月趋势图表比较了所选日期范围内的活动客户和客户总数。 列表示每个月的活动客户计数，行代表每个月的客户总数。 

:::image type="content" source="images/pci/activecustomer.png" alt-text="合作伙伴中心见解活动客户报表显示一段时间内活动客户的条形图的屏幕截图。":::

## <a name="next-steps"></a>后续步骤

有关更多报表，请参阅 [合作伙伴中心见解](partner-center-insights.md)。

>[!NOTE]
> 你可以从见解仪表板中的 "下载报表" 部分下载此报表的原始数据。 [了解详细信息](pci-download-reports.md) 
