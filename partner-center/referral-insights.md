---
title: 获取引荐见解
ms.topic: article
ms.date: 04/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在合作伙伴中心定期检查引荐见解数据，了解要处理的趋势或有待改进的方面，从而帮助你实现业务目标。
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5793e865105b59b2772fd6af5187a92115659e1d
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328077"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>在合作伙伴中心获取引荐见解，并了解引荐状况如何

**相应的角色**

- 引荐管理员

通过引荐中“分析”部分下的“联合销售机会”页面，可查看你的引荐表现如何 。 请定期查看这些指标，以识别趋势或需要关注的领域，并推动业务目标的实现。

若要查看联合销售机会见解数据，请从合作伙伴中心菜单，转到“引荐”>“分析”>“联合销售机会”。

> [!Important]
> 交易类型筛选器已预先应用了“联合销售”类型，该类型被选择用于所有数据。 若要分析与私人交易和合作伙伴引荐交易相关的数据，请删除此筛选器。

## <a name="apply-filters"></a>应用筛选器

在“联合销售机会”页面的顶部附近，可选择要显示的数据所属的时间段。 默认选择“3M”（3 个月），但你可选择显示 6 个月或 1 年的数据。 你还可选择“自定义”，查看特定时间段所有引荐的数据。

可选择“筛选器”按钮来打开面板，可在此面板中按客户名称、国家/地区、交易类型、交易方向、解决方案名称和状态筛选此页面上的所有数据。 下面是这些筛选器的详细信息。

- **客户名称**：默认值为“全部”，但你可限制仅查看所选的一名或多名客户的数据。
- **国家/地区**：默认值为“全部”，但你可限制仅查看所选的一个或多个国家/地区的客户的数据。
- **交易类型**：默认值为“联合销售”，但可以选择“全部”，也可以根据你的选择限制仅查看私人交易或合作伙伴引荐交易的数据。
- **交易方向**：默认值为“全部”，但你可选择限制仅查看“传入”引荐（收到的引荐）或“传出”引荐（发送的引荐）的数据  。
- **解决方案名称**：默认值为“全部”，但你可选择限制仅查看包含你所选的一个或多个解决方案的引荐的数据。
- **状态**：默认值为“全部”，但你可选择限制仅查看包含所选的一个或多个引荐状态类型（例如“已创建”、“已接受”、“已拒绝”、“已过期”、“已失去”和“已获得”）的引荐的数据。

除非下面有说明，否则以下列出的所有图表中的信息将反映所选的日期范围和任何筛选器。 某些部分还允许应用额外筛选器，例如按特定的解决方案进行筛选。

## <a name="referrals-summary"></a>引荐摘要

此卡片显示了你的联合销售机会业绩效果的概述。

该图表显示了所选时间段的总交易数、获得的交易数、失去的交易数和总交易量（美元）。

变化百分比指标以红色或绿色显示，带有箭头指示器，它指示所选日期范围内上一个完整月份与该范围内第一个完整月份之间的差 。 例如，假设当前日期是 6 月 15 日，而你选择了“3M”筛选器来显示过去三个月的数据。 在这种情况下，这些指标将显示所选日期范围内，五月（所选时间段内的上一个完整月份）与三月（所选时间段内的第一个完整月份）之间的差是 **3 个月**；比较将在五月份数据与三月份数据之间进行。

:::image type="content" source="images/referrals/cosellanalyticssummary.png" alt-text="显示联合销售机会分析摘要卡的图像。":::

## <a name="conversion-funnel"></a>转化漏斗图

本部分显示一种视觉指示器，它显示你的交易在其生命周期内是如何从一种状态移到另一种状态的。 你可以根据交易量查看整个生命周并根据这个部分的主透视查看交易额（美元）。 第一部分标记有状态和交易类型，它按类型直观显示交易量或交易额。 还有一个名为“历史引荐”的部分，它显示你对其采取了操作（在为报告所选的时间段内接受/拒绝或将其标记为“已获得”/“已失去”）的交易。 可应用筛选器，在交易的生命周期中跨各个阶段查看交易的进度。

联合销售的入站交易可以合并为“已接受”、“已拒绝”或“已过期”，因为合作伙伴必须接受或拒绝入站联合销售交易。

:::image type="content" source="images/referrals/inbound.png" alt-text="图片显示入站引荐的状态。":::

如果合作伙伴创建了伙伴引荐、私人和联合销售出站交易，则这些类型的交易会合并为“已创建”。

:::image type="content" source="images/referrals/outbound.png" alt-text="图片显示出站引荐的状态。":::

:::image type="content" source="images/referrals/cosell-analytics-funnel-v2.png" alt-text="显示引荐转化漏斗图的图像。":::

## <a name="deals-by-geography"></a>按地理位置列出的交易

本部分显示了产生交易的国家/地区，以及每个国家/地区的详细信息。 有一个表视图显示了每个国家/地区的交易详细信息，还有一个地图视图显示了所有国家/地区。 可选择表中的特定国家/地区，或选择地图视图，缩放定位到特定国家/地区。

:::image type="content" source="images/referrals/cosell-analytics-geo-distribution-v2.png" alt-text="显示引荐的地理分布情况的图像。":::

## <a name="deals-by-solutions"></a>按解决方案列出的交易

在此图表中，可查看哪些解决方案正在促成大部分引荐和最高的交易额。 表具有三种透视：联合销售、合作伙伴引荐和私人。
根据你的透视选择，你可查看按解决方案聚合的交易绩效。

> [!NOTE]
> 如果一笔交易中包含了多个解决方案，该表将显示针对所有这些解决方案计数的同一交易。 不得将与这些解决方案相关的交易额相加并与其他引荐交易量指标进行比较。 此视图旨在帮助你通过解决方案透视了解交易绩效。

表中显示了其中包含解决方案的全部交易、相应的状态（例如已获得交易、已失去交易、交易已过期），以及已获得和已失去的总交易额（美元）。 表的右侧还有一个交易趋势图，其中根据所选的解决方案显示总交易数和已获交易额（美元）。 默认选择是“所有解决方案”。

:::image type="content" source="images/referrals/cosell-analytics-solutions-v2.png" alt-text="显示解决方案绩效的图像。":::

## <a name="declined--lost-reasons"></a>拒绝和损失原因

本部分将帮助你分析交易为何要被你的公司标记为“已拒绝”或“已失去” 。 这些表述中的选项与你的卖方在结束交易并将交易标记为“已拒绝”或“已失去”时选择的原因相同。

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="显示合作伙伴在拒绝交易或将交易标记为“已失去”时选择的原因的图像。":::

## <a name="comparison-charts"></a>比较图

比较部分将帮助你根据透视（单位为美元）中已获得的交易量和交易额的多个维度，对与引荐相关的数据进行比较。 可选择 3 个维度来比较数据，它们是：

- 交易类型
- 市场
- 解决方案

如果选择了交易类型，则可比较联合销售机会、合作伙伴引荐交易和私人交易方面的引荐表现情况。 对于市场和解决方案，可最多选择 3 个不同的选项来比较它们的表现情况。 第一个图是条形图，它将根据主透视（已获得的交易量或交易额）显示数据和月度环比趋势。 条形图右侧还有一个饼图，它显示同一数据的分布情况百分比。

:::image type="content" source="images/referrals/cosell-analytics-compare-v2.png" alt-text="显示比较部分的图像。":::

## <a name="raw-data-table"></a>原始数据表

下表中有与联合销售机会相关的所有原始数据，它将帮助你快速导出数据来进行你想要执行的任何详细或自定义分析。

:::image type="content" source="images/referrals/cosellanalyticsrawdata.png" alt-text="显示引荐的原始数据表的图像。":::

## <a name="no-data"></a>无数据

有很多原因会导致你在访问下述联合销售分析时获得如下所示的空白图表。

- 此帐户没有数据。 请尝试创建交易来填充此报告。
- 存在某种网络连接问题。 请检查你的 Internet 连接，然后重试。
- 在加载页面，但采用了针对联合销售交易的默认筛选器。 如果你只有私人交易，则请重置交易类型筛选器。
- 没有与你应用的筛选器相匹配的记录。 尝试重置筛选器。
- 分析报告中机会状态更改域机会状态更新之间存在延迟。 请在 24 小时后查看报告。

:::image type="content" source="images/referrals/nodata.png" alt-text="显示引荐没有数据可视化的图像。":::

> [!NOTE]
> “引荐见解”页仅显示在合作伙伴中心内生成的引荐的数据。 它不显示通过 [Partner Sales Connect](psc-to-pc.md) 或任何其他机制生成的引荐的数据。

> [!TIP]
> 若要了解你的企业档案在[查找解决方案提供商](https://www.microsoft.com/solution-providers/home)体验中的表现，请查看[企业档案见解页](analyze-your-marketing-profile.md)。

## <a name="next-steps"></a>后续步骤

- [借助 Microsoft 引荐拓展业务](referrals.md)
- [分析潜在客户](analyze-your-marketing-profile.md)