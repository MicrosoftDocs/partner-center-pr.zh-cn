---
title: 付款计划和流程
description: 了解付款和事务，例如适用于商业市场和其他交易的付款计划和 recoupment 过程。
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f4d31a5cf0752d03248b0efddb98ce621f9174f9
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086169"
---
# <a name="payout-schedules-and-processes"></a>付款计划和流程

**相应的角色**

- 帐户管理员
- 全局管理员

本文介绍了 Microsoft 的付款计划，在何处可以找到费用的状态，以及客户非付款过程。

## <a name="payment-schedules"></a>付款计划

以下部分介绍了用于 **企业协议** 和 **信用卡/发票** 交易的付款流程。

### <a name="enterprise-agreement-transactions"></a>企业协议事务

当客户使用其现有的 Microsoft 企业协议用于交易来从 Microsoft AppSource 或 Azure Marketplace 购买产品时，我们将在下一次付出的费用周期30天后发出客户发票。 客户使用信用卡的交易在支出前有30天的保留期。

通常，在 Microsoft 从客户处收集付款之前会发生费用。 如果客户未能向 Microsoft 付款，但我们已支付费用，请参阅下面的 [客户非支付过程](#process-for-customer-non-payment) 。

| 事件 | 说明 | 报告可见性 | 时机 |
| --- | --- | --- | --- |
| 事务的使用或月份 | 客户使用或购买服务。 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [排序](/azure/marketplace/partner-center-portal/orders-dashboard) 面板 | **第1个月** |
| Microsoft 计算计费金额 | 确定总用量、总事务数 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [排序](/azure/marketplace/partner-center-portal/orders-dashboard) 面板 | **第2个月** |
| 已发布比率 | 确定机构费和支出收益 | 在[付出](payout-statement.md)的交易历史记录中被标记为未处理 | **第3个月 (第一周)** |
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
| 事务的使用或月份 | 客户使用或购买服务。 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [排序](/azure/marketplace/partner-center-portal/orders-dashboard) 面板 | **第1个月** |
| 按客户付款的发票 | 确定总用量、总事务值和客户支付开票 | [使用情况](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [排序](/azure/marketplace/partner-center-portal/orders-dashboard) 面板 | **第2个月** |
| 已发布比率 | 确定机构费和支出收益 | 在[付出](payout-statement.md)的交易历史记录中被标记为未处理 | **第2个月** |
| 30天的保留期 | 确保资金收集、可能的退款和退款请求 | 在[付出](payout-statement.md)的交易历史记录中被标记为未处理 | **第3个月** |
| 准备支出 | 收益已准备好每月支付 | 在[支出表](payout-statement.md)的事务历史记录中标记为即将推出 | **第4个月 (第一周)** |
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
| 示例付出日期 | 10/15/2020 | 已标记为 "在事务历史记录中 **发送** " 和 "支出" 面板中 |
| <font color="red">如果客户不向 Microsoft 付款</font> | 12/2/2020 –12/5/2020 | 无更改，如上所述 |
| 客户首先收到延迟支付的电子邮件 | 12/6/2020 | None |
| 客户收到不断增加的紧急性电子邮件 | 12/7/2020 –1/31/2021 | None |
| 发布者通知写入可能 | 1/7/2021 | 发送给发布者的电子邮件通知，其客户尚未发送付款。 包括交易记录 ID 和美元金额。 |
| 客户收到终止通知 | 2/1/2021 | None |
| 收集过程结束/资金已写出 | 2/15/2021 | 发送给发布者的电子邮件通知已写出。 包括交易记录 ID 和美元金额。 |
| 扣减支出 | 2021/3/1 | 发布者将在合作伙伴中心支出报表中看到消极事务 |
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
