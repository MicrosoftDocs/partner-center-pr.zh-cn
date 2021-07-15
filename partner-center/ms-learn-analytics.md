---
title: 合作伙伴中心 Insights Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 利用各个培训、已完成的模块、已完成的学习途径等数据，跟踪公司中的学员。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5d73582d3cfe0aa19483526d9b77e55a4c7e0a0
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989751"
---
# <a name="use-microsoft-learn-analytics-reports"></a>使用 Microsoft Learn 分析报表

**适当的角色**：全局管理员 |MPN 合作伙伴管理员

[Microsoft Learn](/learn/)报表提供了有关公司中的学员的信息，其中包括他们完成的模块以及他们所在的学习路径。 该报表显示每个单独学习器的状态。 公司的全局管理员和 MPN 管理员可以查看数据。

## <a name="how-to-read-the-report"></a>如何读取报表

### <a name="summary-charts"></a>摘要图表

这些图表汇总了训练有素的个人、模块完成和学习路径的计数和每月累积趋势。

**训练有素的个人计数**：在所选日期范围内完成至少一个模块的所有不同学习器的计数 

**训练有素的个人趋势迷你图**：每月活动学习器的累计计数 

**模块完成计数**：在所选日期范围内由合作伙伴公司的学员完成的模块的计数。
例如，如果 "模块 1" 是由15个个体完成的，并且 "模块 2" 已由同一15个人完成，则模块完成计数将为30。 模块完成日期应在选定的日期范围内。

**模块完成趋势迷你图**：每月月完成数的累计计数 

**Learning 路径完成计数**：在所选日期范围内由合作伙伴公司中的学员完成的 Learning 路径的计数。
例如，如果 Learning 路径 "path 1" 由20个个体完成，且 Learning 路径 "path 2" 已由同一20个人完成，则 Learning 路径完成计数将为40。 Learning 路径完成日期应在所选日期范围内。

**Learning 路径完成趋势迷你图**：月份 over 月份完成学习路径的累计计数 

### <a name="trained-individuals-monthly-trend"></a>训练有素的个人每月趋势

此数据是公司用户在该月第一次完成某个模块的趋势。 

**X 轴** 是所选时间筛选器的月份。 

**Y 轴** 是在该月期间已注册了模块)  (首次完成的活动学员的计数。 这不是累积性。

### <a name="module-completions-monthly-trend"></a>模块每月完成趋势

此数据是每个公司用户在该月完成的模块的趋势。  (非累积)  

**X 轴** 是所选时间筛选器的月份。 

**Y 轴** 是在该月期间完成的模块的计数。 这不是累积性。

### <a name="learning-path-completions-monthly-trend"></a>Learning 路径完成每月趋势

此数据是公司用户在该月完成的学习路径的趋势。  (非累积)  

**X 轴** 是所选时间筛选器的月份。 

**Y 轴** 是当月内模块完成的计数。 这不是累积性。

### <a name="learning-path-completion-tabs"></a>Learning 路径完成选项卡

#### <a name="module-tab"></a>模块选项卡

此选项卡包含在公司中由前5个模块名称完成的模块细目分类;模块关联的产品;以及与模块相关的用户角色。  

- 模块完成环形图：) 模块名称的摘要部分中显示的模块完成明细 (计数。

图表中心显示的数字是已完成的模块总数

- 按角色完成：按模块的角色完成模块的细分。 如果模块与多个角色关联，则会将每个角色添加到模块完成的计数中。

图表中心显示的数字是模块完成的不同角色的数目。 

- 按产品完成：模块映射到的产品的模块完成细目。 如果模块与多个产品关联，则每个产品都将添加到模块完成的计数中。    

图表中心显示的数字是模块完成的不同产品数。  

#### <a name="learning-path-tab"></a>Learning 路径 "选项卡

此选项卡包含在公司中按前5个模块名称完成的学习路径细目分类;学习路径映射到的产品;以及与此学习路径相关的角色。  

- Learning 路径完成圆环图： Learning 路径完成 (按名称) 显示在摘要部分中的计数。

- 按角色完成：按角色完成学习路径的细分。 如果模块与多个角色关联，则每个角色都将添加到模块完成的计数中。

- 按产品完成：按将学习路径映射到的产品完成学习路径的细分。 如果模块与多个产品关联，则每个产品都将添加到模块完成的计数中。

### <a name="completions-by-learning-individuals"></a>通过学习个人完成

这列出了公司中训练有素的用户，并详细介绍了其已完成的模块和学习路径。

Microsoft Learn 使用用户对象 ID 标识学员。 在 " **模块" 选项卡** 下，所有学习器都按完成的模块进行排序。 它们显示 Microsoft Learn 用户名、对象 ID 和模块计数。 可以使用用户名进行搜索。 

在 " **Learning 路径" 选项卡** 下，按学习路径完成的所有学习路径都将显示为 "学习器显示名称"、"对象 ID" 和 "模块计数"。

使用用户对象 ID 获取学习器的详细信息： 

1. 登录到[Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer )。  (你必须是公司 Azure AD 租户的全局管理员。 ) 

2. 将用户对象 ID 复制到 Graph 资源管理器 "中[突出显示的区域](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f)。 

## <a name="frequently-asked-questions-faq"></a>常见问题解答 (FAQ)

1. 我看不到我公司的 "了解详细信息"。

   此报告适用于在合作伙伴中心拥有帐户的合作伙伴。 如果你仍处于合作伙伴成员中心，则将无法查看此报表。

2. 公司中的 Who 可以查看此报表？ 

   全局管理员和 MPN 管理员可以查看报表。

3. 如何确保所有用户将其 Microsoft Learn 帐户与其合作伙伴中心帐户相关联？

   *全局管理员添加新用户后*，该用户必须 [Microsoft Learn](/learn/) ，才能将其 Azure Active Directory (AD) 公司帐户或工作帐户与其学习帐户关联。 这可以确保 Insights "Learning" 选项卡会显示正确的课程和技能。
   
   用户需要：
   
   1. 登录 [Microsoft Learn](/learn/)。
   2. 选择他们的个人资料图片，然后选择 **"我的个人资料**"。
   3. 选择“设置”。
   4. 在 " **帐户管理**" 下，将其工作帐户添加到 " **链接的帐户**" 下。

4. 在此报表中，是否可以看到使用 MSA 帐户登录到 Microsoft Learn 的所有公司用户？

   目前，最佳方法是将这些用户添加到 Azure AD 租户，然后将其添加到合作伙伴中心，以便他们可以通过合作伙伴中心的 **"我的个人资料"** 关联他们的 Microsoft Learn 帐户。 

   对于仅使用 MSA 帐户进行培训的用户，在不久的将来，Microsoft Learn 团队将能够将其工作电子邮件关联到其 Microsoft Learn 配置文件。 

## <a name="next-steps"></a>后续步骤

有关更多报表，请参阅[合作伙伴中心 Insights](partner-center-insights.md)。

>[!NOTE] 
> 你可以从 "Insights" 仪表板中的 "下载报表" 部分下载用于打开此报表的原始数据。 [了解详细信息](pci-download-reports.md) 
