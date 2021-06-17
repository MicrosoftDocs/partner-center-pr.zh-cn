---
title: 见解培训仪表板
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 浏览合作伙伴中心仪表板。 "培训"是"合作伙伴中心 INSIGHTs (PCI) 报告之一。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6af4f5f82c145aa932c03a176dbf8592d095a930
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276274"
---
# <a name="trainings-dashboard"></a>培训仪表板

**适当角色**：执行报表查看器|报表查看器

"培训"仪表板提供有关公司员工公司提供的认证、评估和审核的见解。 "培训"仪表板包括以下部分：

- 总结
- 按认证、评估、考试划分的训练性能
- 个人（如认证、评估、考试）的凭据
- 活动详细信息

>[!NOTE] 
>此报表在 合作伙伴中心 中的 Insights 中心下提供。 若要查看此报表，应分配有"报表查看器"或"执行报表查看器"角色。 只有作为执行报表查看者的用户才能看到此报表的少数部分。 有关见解报表的访问控制详细信息，请参阅 [PCI 角色](pci-roles.md)。

## <a name="summary"></a>总结

摘要部分提供与训练相关的各种性能指标的数字快照视图。 各种绩效指标包括认证个人、认证、具有考试凭据的个人、考试凭据、具有评估凭据的个人和评估凭据。 本部分中数据根据所选日期范围（可以是三个月 (3M) 、六个月 (6M) 和 12 个月 (1Y) 或自定义数据范围 (自定义) ）刷新。 

:::image type="content" source="images/pci/td-summary.png" alt-text="总结。":::

- **具有认证的个人**：表示公司中具有认证的个人数。
- **认证计数**：表示公司中个人参加的认证总数。
- **具有评估的个人**：表示公司中具有评估凭据的个体数。 
- **评估计数**：表示公司中个人进行评估的总数。
- **具有检查凭据** 的个人：表示公司中具有检查凭据的个体数。 
- **检查计数**：表示公司中个人接受的考试总数。

## <a name="training-performance"></a>训练性能

培训绩效显示个人每月计数和公司中个人完成的培训。 它按认证、评估和考试拆分，格式为所选日期范围的图表。 X 轴表示所选日期范围的月份。 Y 轴表示所选训练类型的个人非重复计数和训练次数。 选择图表上方相应的选项卡，按训练类型查看明细。 可以通过所选日期范围的 .tsv 格式的下载图标下载图表数据。

:::image type="content" source="images/pci/td-training-performance.png" alt-text="训练性能。":::

## <a name="individuals-performance"></a>个人绩效

"个人绩效"部分显示公司中个人针对所选日期范围进行的培训的详细信息。 在部分左侧面板中搜索并选择个人姓名。 所选个人的训练详细信息将显示在该部分右侧面板上。

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="个人性能。":::

>[!NOTE] 
> "个人性能"部分仅适用于执行报表查看者。 

## <a name="next-steps"></a>后续步骤

[合作伙伴中心 Insights 中的报表](partner-center-insights.md)

>[!NOTE] 
> 可以从见解仪表板中的"下载报表"部分下载为此报表提供电源的原始数据。 [了解详细信息](pci-download-reports.md)