---
title: 付款计划和流程
description: 了解付款和交易，例如商业市场和其他事务的付款计划和重新付款流程。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146946"
---
# <a name="payout-schedules-and-processes"></a>付款计划和流程

**适当角色**：帐户管理员|全局管理员

本文讨论 Microsoft 的付款计划、在何处查找付款状态以及客户未付款的过程。

## <a name="payment-schedules"></a>付款计划

以下部分介绍了我们针对信用卡企业协议 **发票交易付款流程**。 

### <a name="enterprise-agreement-transactions"></a>企业协议事务

当客户使用现有 Microsoft 企业协议 Microsoft AppSource 或 Azure 市场 购买产品进行交易时，我们将在下一个付款周期中在客户发票后的 30 天内发出付款。 客户使用信用卡的事务在付款前有 30 天的持有期。

在 Microsoft 从客户收取付款之前，通常会进行付款。 请参阅 [下面的客户未付款](#process-for-customer-non-payment) 流程，了解如果客户未能支付 Microsoft 付款但我们已经发出了付款，我们采取的操作。

| 事件 | 说明 | 报表可见性 | 计时* |
| --- | --- | --- | --- |
| 使用情况或交易月份 | 客户使用或购买服务。 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [订单](/azure/marketplace/partner-center-portal/orders-dashboard) 仪表板 | **月份 1** |
| Microsoft 计算计费金额 | 确定总使用量、总事务数 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [订单](/azure/marketplace/partner-center-portal/orders-dashboard) 仪表板 | **第 2 个月** |
| 已发布付款 | 确定机构费和支出收益 | 在[付出](payout-statement.md)的交易历史记录中被标记为未处理 | **第3个月 (第一周)** |
| 准备支出 | 收益已准备好每月支付 | 在[支出表](payout-statement.md)的事务历史记录中标记为即将推出 | **第3个月 (第一周)** |
| **已发送支出** | **支付将发送到发布服务器** | **在事务历史记录中标记为 "已发送"，在费用 [声明](payout-statement.md)的 "付款" 部分** | **第3个月 (不晚于 15)** |
| 按客户付款的发票 | Microsoft 收集客户的付款 | 没有变化 | **第4个月到第12个月** |
|

\* 付出日期为太平洋标准时间 (PST) 。

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="企业协议客户的付款时间线。":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>具有信用卡或发票的交易 (选中/线路) 

使用信用卡或月度发票的所有购买都有30天的保留期，以确保从客户那里收集资金。

| 事件 | 说明 | 报告可见性 | 时机 |
| --- | --- | --- | --- |
| 使用情况或交易月份 | 客户使用或购买服务。 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [订单](/azure/marketplace/partner-center-portal/orders-dashboard) 仪表板 | **月份 1** |
| 客户支付发票 | 确定总使用量、总交易值和客户付款发票 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [订单](/azure/marketplace/partner-center-portal/orders-dashboard) 仪表板 | **第 2 个月** |
| 已发布付款 | 确定代理费和付款收益 | 在付款对账单的事务历史记录中标记为"未 [处理"](payout-statement.md) | **第 2 个月** |
| 30 天保持期 | 确保收集资金、可能的退款和退款请求 | 在付款对账单的事务历史记录中标记为"未 [处理"](payout-statement.md) | **第 3 个月** |
| 准备付款 | 准备每月付款的收入 | 在付款对账单的"交易历史记录"中标记为 ["即将发布"](payout-statement.md) | **第 4 (第 1 周)** |
| **已发送支出** | **支付将发送到发布服务器** | **在事务历史记录中标记为 "已发送"，在费用 [声明](payout-statement.md)的 "付款" 部分** | **第4个月 (不晚于 15)** |
|

\* 付出日期为太平洋标准时间 (PST) 。

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="信用卡和发票客户的付款时间线。":::

## <a name="process-for-customer-non-payment"></a>客户非付款过程

在极少数情况下，Microsoft 无法收集客户对其商业市场购买的付款。 当客户无法根据其计费计划向 Microsoft 付款时，我们开始进行集合过程。 此过程大约需要四个月的时间，并涉及与 Microsoft 的持久通信。 如果此过程结束后未收到付款，则 Microsoft 会将资金作为 uncollectable 写出。

根据此处所述的支出过程，Microsoft 可能已向发布者支付了资金， (你) 最终 uncollectable 的。 因此，我们有一个流程来协调这些金额。 为了确保你的 (已收到) 付款可能会对你发出警报，你将在客户处于收款过程中时收到通知，并且可能会写出采购。

Microsoft 将使用以下方法之一收回已支付给你的任何付款： (1) Microsoft 可以从未来的付款中减去未支付的金额;例如，如果付款中的 $1000 被视为 uncollectable 并写出，则将来的付款将被预扣到 $1000 恢复，或者 (2) Microsoft 可能会请求支付任何未收集金额的退款或发票出版商。

下面的计划是一个示例：

| 事件 | 估计日期 * | 合作伙伴可见性 |
| --- | --- | --- |
| 示例付出日期 | 10/15/2020 | 在" **交易** 历史记录"和"付款仪表板"的"付款"部分标记为"已发送" |
| <font color="red">如果客户不支付 Microsoft 费用</font> | 12/2/2020 – 12/5/2020 | 无更改，与上面相同 |
| 客户收到第一封延迟付款电子邮件 | 12/6/2020 | 无 |
| 客户收到紧急性增加的定期电子邮件 | 12/7/2020 – 1/31/2021 | 无 |
| 发布服务器可能会收到注销通知 | 1/7/2021 | 发送给发布者的电子邮件通知，告知其客户尚未发送付款。 包括事务 ID 和美元金额。 |
| 客户收到终止通知 | 2/1/2021 | 无 |
| 收集过程结束/资金被注销 | 2/15/2021 | 发送给发布者的电子邮件通知，指出资金已注销。 包括事务 ID 和美元金额。 |
| 付款已减去 | 2021/3/1 | 发布者将在付款对账单合作伙伴中心负交易 |
| 预扣支出 | 3/15/2021 | 未来的付款将显示在合作伙伴中心支出报表中。 在余额不再为负值之前，发布者将不会收到支付。  |
|||

\* 付出日期为太平洋标准时间 (PST) 。

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>支付给支出帐户的付款天数

通常，我们会在该月的第15天，在给定的月份发送任何付款，但支付该费用需要另一段时间才能联系到你的帐户。 天数取决于我们为帐户使用的付款方式，如下所述。

> [!NOTE]
> 下面显示的日期大致为近似值;任何支付可能需要更多或更少的时间才能联系到你的帐户。

| 付款方式     | 到达付款帐户的天数     |
|--------------------|--------------------------------------------|
| PayPal             | 1 个工作日                             |
| ACH/SEPA           | 2-3 个工作日                          |
| 电汇      | 7-10 个工作日                         |
|

## <a name="next-steps"></a>后续步骤

- [税项详细信息](tax-details-marketplace.md)
