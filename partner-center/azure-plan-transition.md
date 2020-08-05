---
title: 将客户从当前的 Azure 产品/服务迁移到 Azure 计划
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解云解决方案提供商合作伙伴如何使用合作伙伴中心将客户从现有的云解决方案提供商 Azure 产品/服务迁移到 Azure 计划下的 Azure 服务。
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: bcc6534995a7550f0f09d1da2d52cbf676b66c40
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527503"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>将客户从现有的云解决方案提供商 Azure 产品/服务迁移到 Azure 计划

**相应的角色**

- 管理员代理
- 计费管理员
- 全局管理员
- 支持人员代理
- 销售代理
- “用户管理”管理员

间接提供商和直接计费合作伙伴可以转换到 Azure 的 Microsoft 云服务提供商计划 (CSP) 中提供的新商务体验。 （间接经销商需通过其间接提供商才能实现此转换。）然后，客户可以通过简便的方式来购买云服务，无论是从合作伙伴、Microsoft 经销商还是直接在 Web 上购买。

转换功能仅适用于要转换到 Azure 新商务体验且已签署 Microsoft 客户协议的客户，而不适用于 CSP 中的其他套餐（例如 Office 365 或 Dynamics 365）。

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>将现有的 CSP 套餐过渡到 Azure 计划

可以在合作伙伴中心内部，将客户从其现有 CSP 套餐过渡到 CSP 计划中新商务体验的 Azure 计划下的 Azure 服务。 为此，合作伙伴和客户必须已通过合作伙伴中心建立了分销商关系，并且客户必须已签署 Microsoft 客户协议。

### <a name="select-transition-to-azure-plan"></a>选择过渡到 Azure 计划

1. 选择适用于客户的 Azure 计划。

2. 选择“将计费过渡到 Azure 计划”。

   :::image type="content" source="images/azure/transition1.png" alt-text="显示基于使用情况的订阅报告信息的屏幕截图，其中包含一个名为“将 Azure 订阅计费过渡到 Azure 计划”的可选选项。":::

3. 选择“继续”

   :::image type="content" source="images/azure/transition2.png" alt-text="标题为“过渡到 Azure 计划”的对话框，其中包含有关过渡的含义以及两个用于选择的选项：“继续”或“取消”。":::

   客户将过渡到 Azure 计划。

   **过渡工作流会自动完成前提步骤**：

   - 购买 Azure 计划
   - Direct CSP 方案中每个客户有一个计划  
   - 每个分销商有一个计划  

   例如，某家合作伙伴购买了两个 Microsoft Azure 套餐，并在购买时包含了两个不同的 POR。 在这种情况下，过渡工作流将购买两个 Azure 计划（每个分销商有一个），并自动映射到 Azure 计划下的相应 Azure 订阅。  

   **将 Azure 订阅映射到 Azure 计划**

   购买 Azure 计划后，我们的系统会将现有的 Azure 订阅映射到 Azure 计划。 可以在 Azure 门户以及合作伙伴中心查看进度。

4. 返回到客户的合作伙伴中心“订阅”页，使用其本地货币更新其预算限制。

   :::image type="content" source="images/azure/transition3.png" alt-text="合作伙伴中心“订阅”页面的分部视图，其中已针对计费周期设置了预算限制（以本地货币形式）。":::

   >[!NOTE]
   >在合作伙伴中心设置的预算不会传播到 Azure 门户。 还应在 Azure 门户中设置预算和警报。

   过渡到 Azure 计划后，不再可为此客户购买 Azure 订阅。 在 Azure 门户的 Azure 计划下创建订阅。

   >[!NOTE]
   > 所有通过 RBAC 在 Azure 计划下购买的 Azure 订阅都将按当地货币定价和计费。 不会使用外汇汇率。

### <a name="track-your-transition-details"></a>跟踪过渡详细信息

可以在 Azure 门户以及合作伙伴中心跟踪过渡进度。

:::image type="content" source="images/azure/details1.png" alt-text="显示包含每个订阅过渡详细信息列表的表的屏幕截图 - 包括订阅 ID、过渡日期和过渡状态。":::

### <a name="billing-impact-to-partners"></a>对合作伙伴的计费影响

如果从现有的 CSP Azure 套餐过渡客户，将产生以下计费影响：

- 在退出原始 CSP Azure 订阅之前，将在现有 CSP 发票中计收所有使用费。

- 如果你对现有 CSP 订阅拥有管理员访问权限，则在迁移该订阅时继续拥有访问权限。

若要将直接企业协议过渡到 CSP，并将服务器和云注册过渡到 Azure 服务，请阅读[获取 Microsoft 合作伙伴协议的 Azure 订阅计费所有权](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>审核日志

若要核对计费，请查看“订阅”页上的“Microsoft Azure”(0145P) 订阅历史记录。

“Microsoft Azure”(0145P) 订阅由两个部分组成：

1. 商务订阅
2. Azure 订阅（权利）

过渡完成后，Azure 订阅将移到新的 Azure 计划下，商务订阅将会暂停，以便不再报告其使用情况。  

>[!NOTE]
>在 CSP 中购买 Microsoft Azure (0145P) 订阅时，商务订阅和 Azure 订阅（权利）具有相同的值。 仅当计费所有权发生更改或转移时，值才会不同。

### <a name="transition-issues"></a>过渡问题

转换期间预计不会发生任何问题。 但如果失败，我们将在过渡工作流本身中提供最新信息。 Azure 的使用不会受到干扰。  

## <a name="next-steps"></a>后续步骤

- [管理 Azure 计划中的订阅和资源](azure-plan-manage.md)

- [合作伙伴赚取的返点 - 概述](partner-earned-credit.md)
