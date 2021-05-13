---
title: 查看激励和计划详细信息
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 使用这些页面查看和管理激励计划状态
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 798fde02b87e8f8105dad6d00c32b050fb90097e
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818739"
---
# <a name="view-your-incentives-program-details"></a>查看奖励计划详细信息

**适当的角色**：激励管理 |奖励用户 |全局管理员 |MPN 合作伙伴管理员

本文介绍了 " **我的奖励概述** " 页，其中显示了激励计划的总体状态以及每个位置的每个程序的状态。 它还提供不同的注册状态。

>[!NOTE]
>若要详细了解合作伙伴中心的奖励和激励功能，请参阅)  (登录所需的 [合作伙伴投资和奖励](https://partner.microsoft.com/membership/partner-incentives) 。

## <a name="access-the-incentives-overview-page"></a>访问奖励概述页

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard)。
1. 选择 " **激励**"，然后从菜单中选择 " **概述** "。
1. 在页面顶部查看“收益和付款摘要”，并在下表中查看更多详细信息。 还可以对随附的表进行排序、分组和扩展：

   - 若要按列排序，请选择列名称。
   - 若要按程序分组，请选择表上方的 " **按程序** " 选项卡。
   - 若要按位置分组，请选择表上方的 " **按位置** " 选项卡。
   - 若要查看有关特定组内的注册的详细信息，请选择给定行末尾的 v 形符号。 这 v 形将展开您的视图。
1. 如果需要执行更多操作才能在计划中注册，则此信息将出现在“状态”列中。 在这种情况下，请选择 V 形符号以了解需要执行的后续步骤。

## <a name="enrollment-status"></a>注册状态

下表说明了 " **状态** " 列中显示的不同注册状态。

| **Status**         | **出现时间** |
|:------------------------------------|:------------------|
| 必需的操作  | 合作伙伴已接受邀请来注册激励计划，但可能需要更新银行或税务信息。 有关后续步骤的详细信息，请参阅 " **所需操作** " 列，或者在合作伙伴中心更新银行或税务信息的链接。 |
| 已中断  | 奖励系统中不再提供特定激励计划。 |
| 已注册  | 所有税务和银行信息均已验证。 合作伙伴无需执行进一步的注册操作。 |
| 正在注册  | 用户不是奖励管理员，并且注册状态为"需要 **操作"** 或" **正在验证注册"** 状态。|
| 非活动/不符合要求 | 奖励计划目前可能未开放注册，或者合作伙伴不符合当前注册或重新注册资格。 <br><br> 如果状态为 **"不符合"，** 则合作伙伴不满足该计划的当前资格要求;选择 **注册状态下的** "查看资格要求"链接将显示资格要求以及满足这些要求中的哪一项。 <br><br> 对于不再在奖励计划中处于活动状态的虚拟组织 (VORG) 或合作伙伴全局帐户 (PGA) 注册，还可能会看到非活动状态。  |
| 已邀请  | 新的奖励计划注册邀请已发送给合作伙伴，但合作伙伴尚未开始注册过程。 相邻的" **需要操作"** 列显示下一步骤和任何相关链接。  |
| 验证注册  | 合作伙伴已完成或更新了新注册或现有注册的银行和税务信息，正在等待 Microsoft 验证此信息。 在验证过程中， **验证注册** 可能最多出现 48 小时。  |

## <a name="see-your-payment-information"></a>查看付款信息

选择屏幕右上角的付款图标，访问以下不同的摘要：

- 交易历史记录
- 支付
- 导出数据

:::image type="content" source="images/payouts/payout-overview.png" alt-text="说明门户右上角的&quot;付款&quot;合作伙伴中心图标":::

此信息包括自你注册奖励计划以来的奖励收益和付款总额。 此页还包括按位置或计划显示的收益和付款，以及在特定位置注册计划时可能需要执行的任何其他操作。 

还可使用合作伙伴付款 [API](https://apidocs.microsoft.com/services/partnerpayouts) 直接连接和获取付款交易和付款数据。 有关详细信息 [，请参阅付款](payout-statement.md) 对帐单。

## <a name="next-steps"></a>后续步骤

- [支出声明](payout-statement.md)
