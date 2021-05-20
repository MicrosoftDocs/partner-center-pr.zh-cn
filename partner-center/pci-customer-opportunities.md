---
title: 合作伙伴中心见解 - CloudAscent 属性报告
description: 了解云中的 CloudAscent 属性合作伙伴中心。 包括有关客户购买 Microsoft 产品倾向的信息。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153032"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>可从仪表板获得 CloudAscent 属性合作伙伴中心报表

**适当角色**：执行报表查看器|报表查看器

仪表板合作伙伴中心 CloudAscent 程序提供可下载的属性数据。 数据显示客户购买 Microsoft 产品的可能性。  本文介绍此数据的细分、如何使用评分以及它的含义。

## <a name="summary-definitions"></a>摘要定义

- **SMC 客户**- 这是推动下载的客户总数。  客户由记录合作伙伴标识。
- **过期协议**- 在当前会计年度内，我们将提供即将到期的协议数。
- **未到期收入**- 与开放式到期协议关联的收入。

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="&quot;客户机会摘要&quot;仪表板的屏幕截图。":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB 分段

SMB 服务 (中) 分为三个不同的子段。

1. **顶级非托管包括** Microsoft 机会最大的 SMB 客户。 典型的顶级非托管客户具有与托管帐户类似的特征，包括大量员工、大量 IT 预算和支出，以及 Microsoft 的大量潜在收入。

   我们以两种方式定义顶级非托管：

   - **基于顶级非托管用户**- 包括具有 300 名或更多员工的帐户。 User-Based 帐户是首次购买或扩展基于用户的订阅产品（如 Microsoft 365、Dynamics 365 或 Surface）的理想目标。
   - **基于顶级非托管计算** –包括 Azure 可能大于 $ 10k 的帐户。 基于计算的帐户包括现有 Azure。 将来可能需要购买 Azure，但可能会有 Azure 大于 $ 10k 的帐户。

2. **中型企业** 包括有25到300名员工的现有客户和客户帐户。

3. **小型企业** 包含10-25 员工的企业。

4. **非常小的企业** 包含1-9 员工的企业。

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC 类型的客户。":::

**排名靠前的非托管** 和 **中型企业** Subsegments 为 microsoft 和 microsoft 合作伙伴 (LTV) 客户提供高生存期值。 因此，它们是在此段中推动增长的领导领域。 在这两个 subsegments 中，我们更好地定位到 Microsoft 365，使用 D365/Azure 业务线 (LOB) 应用程序获取套接字，并为 Microsoft 实现高 LTV。

现在，我们有两个重要的机会领域–1。 我们的客户增加了增长;pps-2. 尽管我们非常不错地获取 Microsoft 365 的云套接字，但我们在 Dynamics 365 和 Azure 中提供了巨大的机会。

下面的屏幕截图表示四个 SMB Subsegments。 CloudAscent 优先处理所有顶级非托管和中型企业帐户的分析、评分和建模。

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB subsegments 的屏幕截图。":::

## <a name="cloudascent-machine-learning"></a>CloudAscent 机器学习

SMB 使用机器学习技术来推动顶级非托管和中型业务领域中的销售和市场营销客户预测。 如何收集信号并将其转换为电网建议？

- **数据收集：Web** 爬网程序通过 ping 公司域、监视博客文章、新闻发布、社交流和技术论坛来扫描和收集数十亿客户信号。  除了收集的信号之外，还从内部和外部源（例如 D&B、Microsoft 内部订阅和事务数据）收集公司图信息。

- **机器学习**：信号将馈入机器学习模型，该模型按云产品和群集输出每个客户的销售和市场营销预测的结构化数据集。  每个客户都使用 Microsoft 顶级 SMB 的类似模型进行评分，该模型确定客户的拟合度，而集成客户的联机行为的机器学习算法将 定义为意向。 评分合并到群集中，这些群集显示客户购买 Microsoft 云产品的需求。

- **优化**：机器学习系统通过每月使用事务数据和每季度订阅数据来优化模型。  机器学习使用 win/loss 数据调整算法，通过将群集建议与 MSX 中处理的机会进行比较来验证模型是否按预期工作。

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 机器学习的屏幕截图。":::

## <a name="cloudascent-propensity"></a>CloudAscent 属性

如何创建属性建议？

使用通过 Web 爬网程序收集的信号以及从各种源提供的数据，我们合并了公司图数据和客户的社交媒体信号。  评分在比较模型中使用这些信号和数据，为意向使用拟合模型和评分模型。

1. 客户帐户拟合

   - 定义公司图的内部和外部数据点。

   - 拟合评分使用与最佳 SMB 相似的模型来比较客户，并查看它们是否适合 Microsoft 云产品。

   - 拟合评分每季度更新一次

2. 客户帐户意向

   - 与社交媒体和客户联机行为相关的信号定义了意向。

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

      2. 使用上述规则，我们将公司分类为"高、中、低"和"非常低"，包括"客户适应"和"意向信号"。

      3. 我们在 2D 矩阵上绘制客户拟合和意向信号，每个交集都表示属性。 例如，高拟合 + 高意向 = A1，表示最高属性。

      4. 最后，这些段分组为形成群集。  例如，A1、A2、A3、A4 构成了"立即行动"群集。

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent 模型。":::

   对于这些客户，我们建议以"立即行动"和"评估客户"为目标。

## <a name="cloudascent-products--models"></a>CloudAscent 产品&模型

下图提供了 CloudAscent 中每个属性模型的视图：

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 属性模型。":::

空白模型由现有 Microsoft 客户的预测组成，这些客户没有产品和/或全新的潜在客户客户。

Upsell 模型使用事务数据来预测在 Azure 中向上销售的可能性，Microsoft 365 SK。

这些客户已拥有 Azure 或 Microsoft 365，而 upsell 模型显示他们可能会购买更多现有 SKU。

EOS 与 Win 7、Office 2010、SQL Server 和 Windows Server (EOS) 共享服务结束。 EOS 数据从 MS Sales 拉取，并叠加在 CloudAscent 属性建模（如果可用）中。 EOS 数据在 Modern Work 和 Azure Sales 中提供。
