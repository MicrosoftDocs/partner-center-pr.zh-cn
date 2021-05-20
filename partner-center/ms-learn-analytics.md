---
title: 合作伙伴中心见解Microsoft Learn分析
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 利用单个培训、已完成的模块、已完成的学习路径等数据来跟踪公司中的学员。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 132583352e1697a2f9dfa624eb9532692be6d734
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152624"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Microsoft Learn 分析报告显示贵公司学员的状态

**适当的角色**：全局管理员|MPN 合作伙伴管理员

该Microsoft Learn报告提供有关公司中学员的信息，包括他们已完成的模块及其学习路径。 报表显示每个单独学习器的状态。 公司的全局管理员和 MPN 管理员可以查看数据。

## <a name="how-to-read-the-report"></a>如何读取报表

### <a name="summary-charts"></a>摘要图表

这些图表汇总了已训练个体、模块完成和学习路径的计数和每月累积趋势。


**已训练的个人计数**：在所选日期范围内至少完成一个模块的所有不同学习者的计数 

**已训练的个人趋势迷你图**：活动学习者的月累计计数 

**模块完成计数**：所选日期范围内合作伙伴公司中学员的模块完成计数。
例如，如果"模块 1"由 15 个人完成，并且"模块 2"已由同一 15 个人完成，则模块完成计数将为 30。 模块完成日期应属于所选日期范围。

**模块完成趋势迷你图**：模块完成月份累积计数 

**学习路径完成计数**：所选日期范围内合作伙伴公司中学员的学习路径完成计数。
例如，如果学习路径"路径 1"由 20 个人完成，并且学习路径"路径 2"已由同一 20 个人完成，则学习路径完成计数将为 40。 学习路径完成日期应位于所选日期范围内。

**学习路径完成趋势迷你图**：每月累计学习路径完成计数 

### <a name="trained-individuals-monthly-trend"></a>已训练的个人每月趋势

此数据是公司用户在该月第一次完成某个模块的趋势。 

**X 轴** 是所选时间筛选器的月份。 

**Y 轴** 是在该月期间已注册了模块)  (首次完成的活动学员的计数。 这不是累积性。

### <a name="module-completions-monthly-trend"></a>模块每月完成趋势

此数据是每个公司用户在该月完成的模块的趋势。  (非累积)  

**X 轴** 是所选时间筛选器的月份。 

**Y 轴** 是在该月期间完成的模块的计数。 这不是累积性。

### <a name="learning-path-completions-monthly-trend"></a>学习路径每月完成趋势

此数据是公司用户在该月完成的学习路径的趋势。  (非累积)  

**X 轴** 是所选时间筛选器的月份。 

**Y 轴** 是当月内模块完成的计数。 这不是累积性。

### <a name="learning-path-completion-tabs"></a>学习路径完成选项卡 

**模块选项卡**

此选项卡包含在公司中由前5个模块名称完成的模块细目分类;模块关联的产品;以及与模块相关的用户角色。  

- 模块完成环形图：) 模块名称的摘要部分中显示的模块完成明细 (计数。

图表中心显示的数字是已完成的模块总数

- 按角色完成：按模块的角色完成模块的细分。 如果模块与多个角色关联，则会将每个角色添加到模块完成的计数中。

图表中心显示的数字是模块完成的不同角色的数目。 

- 按产品完成：模块映射到的产品的模块完成细目。 如果模块与多个产品关联，则每个产品都将添加到模块完成的计数中。    

图表中心显示的数字是模块完成的不同产品数。  

**学习路径选项卡**   

此选项卡包含在公司中按前5个模块名称完成的学习路径细目分类;学习路径映射到的产品;以及与此学习路径相关的角色。  

- 学习路径完成环形图：按名称) 汇总部分中显示的学习路径完成明细 (计数。

- 按角色进行的完成 *：按角色完成的学习路径的细分。 如果模块与多个角色关联，则会将每个角色添加到模块完成的计数中。

- 按产品完成：按将学习路径映射到的产品完成学习路径的细分。 如果模块与多个产品关联，则每个产品都将添加到模块完成的计数中。

### <a name="completions-by-learning-individuals"></a>通过学习个人完成

这列出了公司中训练有素的用户，并详细介绍了其已完成的模块和学习路径。

Microsoft Learn 使用用户对象 ID 标识学员。 在 " **模块" 选项卡** 下，所有学习器都按完成的模块进行排序。 它们显示 Microsoft Learn 用户名、对象 ID 和模块计数。 可以使用用户名进行搜索。 

在" **学习路径"选项卡** 下，所有按已完成的学习路径排序的学习器都将显示为学习器显示名称、对象 ID 和模块计数。

若要使用用户对象 ID 获取学员的详细信息，请执行以下操作： 

1. 登录到 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer )。  (必须是公司租户租户.Azure AD的全局) 

2. 将用户对象 ID 复制到图形 [资源管理器中](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) 突出显示的区域。 

## <a name="faq"></a>FAQ

1. 我看不到公司的"学习详细信息"。

此报表适用于在 合作伙伴中心 中拥有帐户的合作伙伴。 如果仍处于Partner Membership Center，将看不到此报表。

2.  公司中的谁可以查看此报表？ 

全局管理员和 MPN 管理员可以查看报表。

3. 如何确保所有用户将其帐户与Microsoft Learn帐户关联合作伙伴中心帐户？

全局管理员添加新用户后，该用户需要转到其 **我的个人资料以将其** Microsoft Learn帐户。

- 选择 **仪表板右上角** 的"帐户"图标，然后选择"我的个人资料"。  

-  在 **"你的** 学习"下，用户将能够关联其Microsoft Learning帐户，并将其Microsoft 帐户 Partner University。

3. 在此报告中，我能否看到使用 MSA Microsoft Learn登录公司的所有用户？

目前，最佳方法就是将这些用户添加到 Azure AD 租户，然后将他们添加到 合作伙伴中心，以便他们可以在 合作伙伴中心 中通过 我的个人资料 关联其 Microsoft Learn 帐户。  

对于仅使用 MSA 帐户进行训练的用户，在不久的将来，Microsoft Learn 团队将使他们能够将工作电子邮件关联到其Microsoft Learn配置文件。 

## <a name="next-steps"></a>后续步骤

有关更多报表，请参阅[合作伙伴中心 Insights。](partner-center-insights.md)

>[!NOTE] 
> 可以从见解仪表板中的"下载报表"部分下载为此报表提供电源的原始数据。 [了解详细信息](pci-download-reports.md) 