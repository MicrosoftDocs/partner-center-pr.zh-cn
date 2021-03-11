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
ms.openlocfilehash: 4c4b3a9a71027f5fb02bc29566c20c214e3df371
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022802"
---
# <a name="view-your-incentives-program-details"></a>查看奖励计划详细信息

**相应的角色**

- 激励管理员
- 奖励用户
- 全局管理员
- MPN 合作伙伴管理员

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

| **状态**         | **出现在** |
|:------------------------------------|:------------------|
| 必需的操作  | 合作伙伴已接受邀请来注册激励计划，但可能需要更新银行或税务信息。 有关后续步骤的详细信息，请参阅 " **所需操作** " 列，或者在合作伙伴中心更新银行或税务信息的链接。 |
| 已中断  | 奖励系统中不再提供特定激励计划。 |
| 已注册  | 所有税务和银行信息均已验证。 合作伙伴无需进一步的注册操作。 |
| 正在注册  | 用户不是激励管理员，注册处于 **所需的操作** 或 **验证注册** 状态。|
| 非活动/不符合要求 | 此时，激励计划可能未开放，或者合作伙伴不满足注册或重新注册的当前资格。 <br><br> 如果状态为 " **不符合"，则** 合作伙伴不满足计划的当前资格要求;选择 "注册状态" 下的 " **查看资格要求** " 链接将显示符合条件的要求以及满足了哪些要求。 <br><br> 你还可能会看到虚拟组织 (VORG) 或合作伙伴全局帐户的 **非** 活动状态，该)  (帐户在激励计划中不再处于活动状态。  |
| 已邀请  | 新的激励计划注册邀请已发送给合作伙伴，但合作伙伴尚未开始注册过程。 相邻的 " **必需操作** " 列显示后续步骤和任何相关的链接。  |
| 正在验证注册  | 合作伙伴已经完成或更新了新的或现有注册的银行和税务信息，正在等待 Microsoft 验证此信息。 在验证过程中， **验证注册** 可能会长达48小时。  |

## <a name="see-your-payment-information"></a>查看你的付款信息

选择屏幕右上角的 "支出" 图标以访问这些不同的摘要：

- 交易历史记录
- 支付
- 导出数据

:::image type="content" source="images/payouts/payout-overview.png" alt-text="说明合作伙伴中心门户右上角的支出图标":::

此信息包括自你注册奖励计划以来的奖励收益和付款总额。 此页还包括按位置或计划显示的收益和付款，以及在特定位置注册计划时可能需要执行的任何其他操作。 

你还可以使用 [合作伙伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts) 来连接并直接获取支出交易和付款数据。 有关详细信息，请参阅 [付出](payout-statement.md) 进一步的了解。

## <a name="next-steps"></a>后续步骤

- [支出声明](payout-statement.md)
