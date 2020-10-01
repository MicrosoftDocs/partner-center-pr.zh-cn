---
title: 在商业市场中获得付款
description: 了解如何在商业市场-Azure Marketplace 中接收收入支付。
ms.service: marketplace
ms.topic: conceptual
ms.date: 09/28/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: bcd1b6d2ea82a6302ccdad7619f9c1bdabb4aead
ms.sourcegitcommit: 0005e8917ac997f6952b2f57bda326c711b524b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "91591069"
---
# <a name="getting-paid-in-the-commercial-marketplace"></a>在商业市场中获得付款

本文包含有关接收产品/服务、外接程序和广告收入的付款的重要信息。 它汇总了费用策略、获得付费之前所需的步骤以及对帐单概述。

## <a name="commercial-marketplace-payout-policies-and-agreements"></a>商业市场支出政策和协议

付费要求遵守协议和支出政策。

- [Microsoft Azure 市场发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)：获得付费之前，必须接受此发布者协议。 本协议介绍你与 Microsoft 之间的关系，因为它与商业应用商店中的卖方产品/服务有关，其中包括 Microsoft 对每个销售所收取的存储费用。
- [支出策略](payout-policy-details.md) 显示包括支付计划和付款方式的费用支付政策。 策略还介绍了客户非付款过程。
- [税收详细](tax-details-marketplace.md) 说明了在 Microsoft [发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)下价格选择和税务责任的税务注意事项。
- **商店费用** 在发布者协议中正式定义。 商店费用适用于由商业应用商店收集的所有产品/服务（包括外接程序）。
- 每月支付一次**支付** (前提是已满足支付阈值) 。 我们通常会在该月的第15天的给定月份内发送任何付款。 支付费用通常需要3到10个额外的工作日内才能联系到你的帐户。 有关详细信息，请参阅[付款阈值、方法和期限](payment-thresholds-methods-timeframes.md)。

## <a name="prerequisite-steps-before-getting-paid"></a>获得付费之前的先决条件步骤

在第一次获得付费之前，必须设置您的费用科目并完成必需的银行和税务表。 在银行和税务窗体中，你将为预缴税金提供首选支付方法和税务形式。 必须填写银行和税务表格才能支付费用。 有关详细信息，请参阅 [设置你的帐户和税务表](set-up-your-payout-account.md)。

### <a name="payout-hold-status"></a>付款暂停状态

默认情况下，我们将按如上所述按月发送付款。 不过，你可以选择将你的付款放在某个程序上，并且 Microsoft 不会向你的帐户发放你的付款。 如果选择将付款置于保持状态，我们将继续在 **付款** 页中记录任何收入。 但是，在删除暂停状态之前，我们不会向你的帐户发送任何付款。

若要暂停付款，请转到“帐户设置”。 在“付款和税务”下的“付款和税务配置文件分配”部分中，找到要对其暂停付款的计划。 选中 " **保持我的付款** " 复选框，以保留此计划的付款。 你可以随时更改你的支出保留状态，但你的决定会影响下一次的月额度。 例如，如果要暂停四月付款，请确保在三月底之前将付款暂停状态设置为“打开”。

将 "支出保留" 状态设置为 **"打开**" 后，该程序的所有付款都将处于暂停状态，直到清除此复选**框。** 当你执行此操作时，你将在下一个每月费用周期内包含 (前提是已满足支付阈值) 。 如果你已有付款，但想要在6月生成付出的比率，请在 "可能" **结束之前清除** 复选框。

>[!Note]
> 付出的支出状态适用于每个节目，分别 (Microsoft Store、广告、Azure Marketplace 等) 上。 如果要对所有程序进行支付，请分别在每个节目上保存付款。

## <a name="payout-statements"></a>支出声明

支出报表显示你在交易历史记录中的产品/服务和外接程序的销售收入。 你还可以查看付款详细信息，并以 tsv 或 csv 格式下载报表。 若 [要详细](payout-statement.md) 了解如何访问支出报表和交易记录和付款报表的详细信息，请参阅费用报表。 此外，还可以使用 [合作伙伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts) 来系统地拉取支出报表。

## <a name="next-steps"></a>后续步骤

- [合作伙伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [市场付款常见问题解答](payout-faq.md)
