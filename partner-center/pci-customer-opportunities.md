---
title: 合作伙伴中心见解-CloudAscent 电网报告
description: 了解合作伙伴中心仪表板中的 CloudAscent 电网报表。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 510f85b053ec17fa0a2a66217a19c006e7ca2bc9
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2020
ms.locfileid: "90811322"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>合作伙伴中心仪表板中提供的 CloudAscent 电网报表

**相应的角色**
- 主管人员报表查看器
- 报表查看器

合作伙伴中心仪表板提供了 CloudAscent 程序中可下载的电网数据。 数据显示客户电网购买 Microsoft 产品。  本文介绍了此数据的明细，如何利用评分，以及它的含义。

## <a name="summary-definitions"></a>摘要定义

- **SMC 客户**-这是电网下载中的客户总数。  客户由记录的合作伙伴标识。
- **协议过期**–在当前会计年度内，我们将提供过期协议的数量。
- **过期收入**–与过期协议关联的收入。
- **开启过期收入**–与开放式过期协议关联的收入。

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="客户机会概述仪表板的屏幕截图。":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB 分段

中小型企业 (SMB) 段进一步划分为三个不同的子段。

1. **顶级非托管** 用户包括最大的 SMB 客户，其中最有 Microsoft 机会。 典型的顶级非托管客户与托管帐户共享类似的特征、大量的员工、大型 IT 预算和支出，以及大量可能的 Microsoft 收入。

   我们定义了顶层非托管方法：

   - **基于的顶级非托管用户**–包括有300或更多员工的帐户。 基于用户的帐户是首次购买或扩展基于用户的订阅产品（如 M365、D365 或 Surface）的理想目标。
   - **基于顶级非托管计算** –包括 Azure 可能大于 $ 10k 的帐户。 基于计算的帐户包括现有 Azure。 将来可能需要购买 Azure，但可能会有 Azure 大于 $ 10k 的帐户。

2. **中型企业** 包括有25到300名员工的现有客户和客户帐户。

3. **小型企业** 包含25个以上员工的所有剩余企业。

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC 类型的客户。":::

**排名靠前的非托管** 和 **中型企业** Subsegments 为 microsoft 和 microsoft 合作伙伴 (LTV) 客户提供高生存期值。 因此，它们是在此段中推动增长的领导领域。 在这两个 subsegments 中，我们更好地定位了 M365、盈利和 D365/Azure 业务线 (LOB) 应用中的套接字，并为 Microsoft 实现了高 LTV。

现在，我们有两个重要的机会领域–1。 我们的客户增加了增长;pps-2. 尽管我们非常不错地获取 M365 的云套接字，但我们在 D365 和 Azure 中有一个很大的机会。

以下屏幕截图表示市场的三个 SMB Subsegments 和优化路由。 CloudAscent 优先处理所有顶级非托管和中型企业帐户的分析、评分和建模。

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="SMB subsegments 的屏幕截图。":::

## <a name="cloudascent-machine-learning"></a>CloudAscent 机器学习

SMB 使用机器学习技术来推动顶级非托管和中型业务领域中的销售和市场营销客户预测。 如何收集信号并将其转换为电网建议？

- **数据收集**：通过 ping 公司域和监视：博客文章、新闻流和技术论坛，Web 爬网程序扫描和收集数十亿个客户信号。  除了收集到的信号之外，firmographics 信息从内部和外部源（例如 D&B、Microsoft 内部订阅和事务数据）收集。

- **机器学习**：将信号送入机器学习模型，以按云产品和群集输出每个客户的一组结构化数据。  每个客户都使用与 Microsoft 的顶级 SMB （确定客户适合的模式）和机器学习算法（可将客户的联机行为定义为意向）进行评分。 评分会合并到分类中，以显示客户电网购买 Microsoft 云产品。

- **优化**：机器学习系统通过每月使用事务数据并按季度对订阅数据进行优化，来优化模型。  使用 win/丢失数据，机器学习调整算法，并通过将群集建议与在 MSX 中操作的机会进行比较来验证模型是否按预期方式工作。

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 机器学习的屏幕截图。":::

## <a name="cloudascent-propensity"></a>CloudAscent 电网

如何创建电网建议？

使用通过 web 爬网程序收集的信号和来自各种来源的数据，我们合并了 firmographics 数据和客户的社交媒体信号。  评分使用这些信号和比较模型中的数据来适应和评分模型的意图。

1. 客户帐户适合

   - 定义 firmographics 的内部和外部数据点。

   - 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。

   - 按季度更新适合评分

2. 客户帐户意向

   - 与社交媒体和客户的联机行为相关的信号定义意向。

   - 意向计分重叠在一起以定义分类。

   - 意向评分每月更新一次。

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 预测模型。":::

3. 群集功能

   用于拟合和意向的信号合并为聚类分析分数。 CloudAscent 有四个分类：

      - 立即行动-销售就绪客户
      - 评估-市场营销就绪客户
      - 维护-驱动器认知活动
      - 培训-指导和监视意向

   群集允许用户根据分段因素（例如：产品、异地、行业和垂直）针对销售和市场营销计划的特定客户。

   CloudAscent 工作簿中的 **电网模型** 选项卡共享电网和估计的空白收入。 若要定义拟合和意向的聚类分析，请完成以下步骤：

      1. 使用 ML 模型，我们首先计算按100的比例计算客户的分数和意向分数。  确切分数将因 ML 型号而异。  示例评分如下：

         |**分类**|**评分**|
         |---------|:---------|
         |高|75-100|
         |中型|55-74|
         |低|30 - 54|
         |非常低|0 - 29|

      2. 使用以上规则，我们将公司的分类分类为高、中、低和极低，并跨客户调整和意向信号。

      3. 我们在二维矩阵上绘制客户拟合和意向信号，每个交集表示电网。     例如，高位 + 高意向 = A1，表示最高的电网。

      4. 最后，这些分段组构成了分类。  例如，A1、A2、A3、A4 窗体。

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent 模型。":::

   对于这些客户，我们建议以 "立即行动" 为目标并评估客户。

## <a name="cloudascent-products--models"></a>CloudAscent Products & 型号

下图提供了 CloudAscent 中的每个电网模型的视图：

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 电网模型。":::

空白模型由现有 Microsoft 客户的预测构成，这些客户没有产品和/或不是网络的新客户。

追加销售模型使用事务数据来预测在 Azure 和 M365 Sku 中追加销售的潜能。

EOS 为 Win 7、Office 2010、SQL Server 和 Windows Server 共享服务客户的结束时间。 EOS 数据从 MS Sales 中提取，并使用 CloudAscent 电网建模（如果可用）进行重叠。 EOS 数据存在于新式工作和 Azure 销售部。
