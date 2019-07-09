---
title: Microsoft 了解分析 |合作伙伴中心
ms.topic: article
ms.date: 07/05/2019
description: 若要了解你的学习分析了解如何
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09d4ca14c1b407e9010ab26bccaf612f9caad732
ms.sourcegitcommit: bd83621eb29fafbda341ad41814a9ae5c1e78b00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2019
ms.locfileid: "67622525"
---
# <a name="microsoft-learn-analytics-report"></a>Microsoft 了解分析报表

Microsoft 了解报表提供已完成的模块以及他们位于的学习路径包括你公司中的学习器的信息。 报表显示每个单独的学习器的状态。 全局管理员和你的公司的 MPN 管理员可以查看数据。

## <a name="how-to-read-the-report"></a>如何阅读报告

### <a name="summary-charts"></a>摘要图表

**训练个人计数**:所有非重复的学习器已完成所选的日期范围内的至少一个模块计数 

**训练的个人趋势微型图表**:月同比月累计计数的活动的学习器 

**模块完成计数**:模块计数完成合作伙伴的公司中的学习器通过所选的日期范围内。
例如，如果 15 个人，可以通过"模块 1"和"模块 2" 已完成的相同的 15 个人，模块完成计数将为 30。 在所选日期范围应倒下模块完成日期。

**模块完成趋势微型图表**:月同比月累计计数的模块完成 

**学习路径完成计数**:计数的学习路径由合作伙伴的公司中的学习器完成所选的日期范围内。
例如，如果按 20 个人和学习路径完成学习路径"路径 1"，则"已由同一 20 个人完成路径 2"、 学习路径完成计数将为 40。 学习路径完成日期应在所选的日期范围内。

**学习路径完成趋势微型图表**:月同比月累计计数的学习路径完成 

### <a name="trained-individuals-monthly-trend"></a>训练的个人月趋势

**X 轴**是月，提供选定时间筛选器。 

**Y 轴**是活动的学习器已在该月中注册 （模块的第一次完成） 的计数。 这不是累积的。

### <a name="module-completions-monthly-trend"></a>模块完成每月趋势

**X 轴**是月，提供选定时间筛选器。 

**Y 轴**在该月期间是模块完成的计数。 这不是累积的。

### <a name="learning-path-completions-monthly-trend"></a>学习路径完成每月趋势

**X 轴**是月，提供选定时间筛选器。 

**Y 轴**是该月份内的模块完成的计数。 这不是累积的。

### <a name="learning-path-completion-tabs"></a>学习路径完成选项卡 

- 模块选项卡

**模块完成环形图**： 细分模块完成 （显示在摘要部分中的计数） 由模块名称。

在图表的中心中显示的数字是已完成的总模块

**按角色完成**： 角色的模块的模块完成的细分。 如果模块是与多个角色关联，然后每个角色添加到模块完成的计数。

环形图中心中显示的数是模块完成不同的角色数。 

**按产品完成**: 模块映射到产品模块完成的细分。 如果模块是与多个产品相关联，则每个产品被添加到模块完成的计数。    

环形图的中间显示数字是模块完成的非重复产品数。  

- 学习路径选项卡    

**学习路径完成环形图**： 学习路径完成 （显示在摘要部分中的计数） 的明细的名称。

**按角色完成**： 细分的学习路径完成角色。 如果模块是与多个角色关联，然后每个角色添加到模块完成的计数。

**按产品完成**： 细分的学习路径完成学习路径映射到的产品。 如果模块是与多个产品相关联，则每个产品被添加到模块完成的计数。

### <a name="completions-by-learning-individuals"></a>通过学习个人完成

Microsoft 了解标识学习器具有一个用户对象 id。 下**选项卡模块**，所有学习器将按已完成的模块。 将显示使用其 Microsoft 了解用户名、 对象 ID 和模块计数中。 可以使用用户名进行搜索。

若要获取使用用户对象 ID 的学习器的详细信息： 

1. 登录到[图形资源管理器](https://developer.microsoft.com/graph/graph-explorer )。 （您必须是公司的 Azure AD 租户的全局管理员）。

2. 将复制到的用户对象 ID[突出显示的区域](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f)图形资源管理器中。 

