---
title: 在 合作伙伴中心
description: 了解如何作为 Microsoft 合作伙伴接收收益付款，例如通过商业市场产品/服务、奖励计划和云解决方案提供商计划。 包括付款策略、付款保留状态和付款对帐单。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: cc01a1aada6c6665d3fd8f6efc6e5ef873736bdc
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684383"
---
# <a name="getting-paid-in-partner-center"></a>在 合作伙伴中心

**适当角色**：帐户管理员|全局管理员

本文提供有关接收产品/服务、加载项和广告收益的付款的重要信息。 它汇总了付款策略、付款前所需的步骤和付款对账单概述。

## <a name="payout-policies-and-agreements"></a>付款策略和协议

获取付款要求你遵守协议和付款策略。

- [Microsoft Azure市场Publisher](/legal/marketplace/msft-publisher-agreement)协议：在付费之前，必须接受此发布者协议。 本协议解释了你与 Microsoft 之间的关系，因为它与商业市场中的卖家产品/服务相关，包括 Microsoft 针对每次销售收取的商店费用。
- [付款策略](payout-policy-details.md) 显示付款付款策略，包括付款计划以及付款方式。 策略还说明了客户未付款的过程。
- [税务详细信息](tax-details-marketplace.md)解释了 Microsoft 税务协议 下的价格选择和税务Publisher[注意事项](/legal/marketplace/msft-publisher-agreement)。
- **存储费用** 在协议协议Publisher定义。 商店费用适用于商业市场收集的所有产品/服务销售，包括加载项。
- **付款** 按月进行， (达到付款阈值时) 。 我们通常会在给定月份的第 15 天之前发送任何应付款。 付款通常需要额外 3 到 10 个工作日，以到达付款帐户。 有关详细信息，请参阅[付款阈值、方法和期限](payment-thresholds-methods-timeframes.md)。

## <a name="prerequisite-steps-before-getting-paid"></a>付款前的先决条件步骤

首次付款之前，必须设置付款帐户并填写必要的银行和税务表单。 在银行和税务表单中，你将提供首选付款方式和预扣税的税单。 在我们可以付款之前，需要提供银行和税务表单。 有关详细信息，请参阅 [设置付款帐户和税务表单](set-up-your-payout-account.md)。

### <a name="payout-hold-status"></a>付款暂停状态

默认情况下，我们将按如上所述按月发送付款。 但是，你可以暂停计划付款，Microsoft 不会将付款释放到你的帐户。 如果选择暂停付款，我们将继续在"付款"页中记录 **任何** 收益。 但是，在删除暂停状态之前，我们不会向你的帐户发送任何付款。

若要暂停付款，请选择右上角设置齿轮图标，然后选择"帐户 **设置"。** 在 **左侧菜单中** 选择"付款和税务"，在"付款和税务配置文件分配"部分中，找到要持有付款的计划。 选中" **保留我的付款** "复选框以保存此计划的付款。 你随时都可以更改付款暂停状态，但你的决策将影响下一个每月付款。 例如，如果要暂停四月付款，请确保在三月底之前将付款暂停状态设置为“打开”。

将付款暂停状态设置为 **"** 开"后，此计划的所有付款都将暂停，直到将复选框清除为"**关闭"。** 这样做时，将在下一个每月付款周期包含 (只要满足付款阈值) 。 如果你的付款已暂停，但想在 6 月生成付款，请在 5 月底之前将复选框清除为 **"** 关"。

>[!Note]
> 付款暂停状态适用于每个计划， (Microsoft Store、广告、Azure 市场等) 。 如果要保留所有计划的付款，请单独保留每个计划的付款。

## <a name="payout-statements"></a>支出声明

付款对账单显示交易历史记录中产品/服务销售额和加载项的收入。 还可以查看付款详细信息，并下载 tsv 或 csv 格式的报告。 请参阅 [付款](payout-statement.md) 对帐单，详细了解如何访问付款对帐单以及交易历史记录和付款报表的详细信息。 此外，可以使用合作伙伴付款 [API](https://apidocs.microsoft.com/services/partnerpayouts) 系统地拉取付款报表。

## <a name="next-steps"></a>后续步骤

- [合作伙伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [支出常见问题解答](payout-faq.yml)