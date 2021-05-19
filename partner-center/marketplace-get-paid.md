---
title: 在合作伙伴中心付费
description: 了解如何以 Microsoft 合作伙伴的形式接收收入付款，例如通过商业 marketplace 产品/服务、激励计划和云解决方案提供商计划。 包括支出策略、付出的支出状态和付出的支出。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 3dc8b728ef20da77b9a6d2a925ebb0388ea53837
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146487"
---
# <a name="getting-paid-in-partner-center"></a>在合作伙伴中心付费

**适当的角色**：帐户管理员 |全局管理员

本文包含有关接收产品/服务、外接程序和广告收入的付款的重要信息。 它汇总了费用策略、获得付费之前所需的步骤以及对帐单概述。

## <a name="payout-policies-and-agreements"></a>支出政策和协议

付费要求遵守协议和支出政策。

- [Microsoft Azure 市场发布者协议](/legal/marketplace/msft-publisher-agreement)：获得付费之前，必须接受此发布者协议。 本协议介绍你与 Microsoft 之间的关系，因为它与商业应用商店中的卖方产品/服务有关，其中包括 Microsoft 对每个销售所收取的存储费用。
- [支出策略](payout-policy-details.md) 显示包括支付计划和付款方式的费用支付政策。 策略还介绍了客户非付款过程。
- [税收详细](tax-details-marketplace.md) 说明了在 Microsoft [发布者协议](/legal/marketplace/msft-publisher-agreement)下价格选择和税务责任的税务注意事项。
- **商店费用** 在发布者协议中正式定义。 商店费用适用于由商业应用商店收集的所有产品/服务（包括外接程序）。
- 每月支付一次 **支付** (前提是已满足支付阈值) 。 我们通常会在指定月份内按该月的第15天发送任何付款。 支付费用通常需要3到10个额外的工作日内才能联系到你的帐户。 有关详细信息，请参阅[付款阈值、方法和期限](payment-thresholds-methods-timeframes.md)。

## <a name="prerequisite-steps-before-getting-paid"></a>获得付费之前的先决条件步骤

首次付款之前，必须设置付款帐户并填写必要的银行和税务表单。 在银行和税务表单中，你将提供首选付款方式和预扣税的税单。 在我们可以付款之前，需要提供银行和税务表单。 有关详细信息，请参阅 [设置付款帐户和税务表单](set-up-your-payout-account.md)。

### <a name="payout-hold-status"></a>付款暂停状态

默认情况下，我们将按如上所述按月发送付款。 但是，你可以暂停计划付款，Microsoft 不会将付款释放到你的帐户。 如果选择暂停付款，我们将继续在"付款"页中记录 **任何** 收益。 但是，在删除暂停状态之前，我们不会向你的帐户发送任何付款。

若要暂停付款，请选择右上角的"设置"齿轮图标，然后选择"帐户 **设置"。** 在 **左侧菜单中** 选择"付款和税务"，在"付款和税务配置文件分配"部分中，找到要持有付款的计划。 选中" **保留我的付款** "复选框以保存此计划的付款。 你随时都可以更改付款暂停状态，但你的决策将影响下一个每月付款。 例如，如果要暂停四月付款，请确保在三月底之前将付款暂停状态设置为“打开”。

将付款暂停状态设置为 **"** 开"后，此计划的所有付款都将暂停，直到将复选框清除为"**关闭"。** 这样做时，将在下一个每月付款周期包含 (只要满足付款阈值) 。 如果你的付款已暂停，但想在 6 月生成付款，请在 5 月底之前将复选框清除为 **"** 关"。

>[!Note]
> 付款暂停状态适用于每个计划， (Microsoft Store、广告、Azure 市场等) 。 如果要保留所有计划的付款，请单独保留每个计划的付款。

## <a name="payout-statements"></a>支出声明

付款对账单显示交易历史记录中产品/服务销售额和加载项的收入。 还可以查看付款详细信息，并下载 tsv 或 csv 格式的报告。 若 [要详细](payout-statement.md) 了解如何访问支出报表和交易记录和付款报表的详细信息，请参阅费用报表。 此外，还可以使用 [合作伙伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts) 来系统地拉取支出报表。

## <a name="next-steps"></a>后续步骤

- [合作伙伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [支出常见问题解答](payout-faq.md)