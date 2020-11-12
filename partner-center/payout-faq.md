---
title: Microsoft 商业应用商店的支出
description: 获取有关商业应用商店中付款的常见问题的解答。 包括有关收入为何与预期不同的解答。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532015"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>有关商业 marketplace 付款的常见问题

本文解答了有关商业应用商店中的付款的常见问题。

## <a name="earnings-incorrect-or-missing"></a>收入不正确或缺失

#### <a name="why-are-my-earnings-missing"></a>为何我的收入缺失？

- 客户订单可能还不符合付款条件。 对于非企业客户订单，Microsoft 必须先收到客户付款，然后发布者才能获得收入。 对于企业客户订单，你的收入将在采购订单日期之后的 1-2 天内提供。 请在[订单报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中验证订单状态。
- 交易历史记录报表中可能不显示 2019 年 7 月之前的交易的收入。 请在[付款下载](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)中检查历史对账单。
- 检查 [付出的时间范围](payment-thresholds-methods-timeframes.md) 并了解你的收入应出现在付出的时间范围内。

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>为什么收入金额不同于我的预期？

- 如果订单已部分支付给客户，则您的收入金额将基于扣除费用和相应税款后的部分支付金额。
- 按国家/地区检查减税责任。 在税款由 Microsoft 负责的国家/地区，Microsoft 将从发布者收入中收集并扣除税款。 对账单中显示的交易金额为税后金额。 请参阅[税项详细信息](tax-details-marketplace.md)。
- SaaS 和 IaaS 产品/服务的折扣率为10%，而不是标准20%，而收入率为90%。 此促销在 2021 年 6 月 30 日之前有效。

**进一步阅读** ： [商业市场出版商协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出政策详细信息](payout-policy-details.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)、 [在商业市场中支付的](marketplace-get-paid.md)费用 [详细信息、费用详细信息](tax-details-marketplace.md)、费用 [报表](payout-statement.md)和 [商业 marketplace 分析中的订单仪表板](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>收入对帐
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>如何在分析中将付款对账单与订单或使用情况报表进行对帐？
使用 "记录订单" 和 "使用情况报告" 的 "对事务历史记录进行支出" 报表中显示的 AssetID、订单 ID 和行项 ID 使用以下映射：

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>如何知道何时会有客户订单付款？
- 首先，使用 assetID，检查 [订单报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的客户订单。
- 在客户 [报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)中检查客户的客户渠道。
- 对于企业客户，发布者收益显示在采购订单日期之后的1-2 天内。
- 对于非企业客户，发布者收益在收到客户付款后的1-2 天内显示。

**进一步阅读** ： [商业 marketplace 分析中的](/azure/marketplace/partner-center-portal/orders-dashboard)[支出报表](payout-statement.md)和订单仪表板

## <a name="payout-policies"></a>付款策略

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>如何查找当前的代理费和付款比率？

- 检查商业市场发布者协议。 标准代理费为 20%。 SaaS Co-Sell 符合条件的事务的折扣费用为10%。 检查是否有任何促销代理费的公告。
- 在您的费用声明中，收益率指定给定交易的实际付出费率。

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>在收入出现在我的对账单上后，多长时间可以收到 Microsoft 的付款？
- 当你的收入处于未处理状态之后，你可以检查将处理你的收入以进行付款的月份的到期日期。 支付准备就绪后，你的收益状态将更改为 "已处理"。  Microsoft 将在每个到期月份的 15 号之前发放付款。
- 对于信用卡支付的订单，Microsoft 保留30天的付款，直到收益得到成熟。

 **进一步阅读** ： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出详细信息](payout-policy-details.md)、 [税务详细信息](tax-details-marketplace.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>付款和调整

#### <a name="why-is-my-payment-missing"></a>为何我的付款缺失？

- 确保在 " [概述" 页](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)上，您的支出状态和税务配置文件状态显示为 *有效* 。
- 你可能未满足付款的最小阈值。 收入必须至少为 50 美元才能获得付款。


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>如何实现将我的帐户设置为不接收支付？
你可以在费用 [配置文件](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)中保留付款;只需选中 " **保存** "。 在你发布保留期之前，Microsoft 会向你收取费用。

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>为什么我收到的货币与购买货币不同？

付款货币基于你在付款配置文件中选择的货币。 购买货币基于客户支付的货币。

#### <a name="how-do-i-reconcile-adjustments"></a>如何对调整进行对帐？

付款调整是用于容纳补偿调整（例如系统问题）的付款更正。 在付款对账单中，原因代码会指定调整原因。 它们不用于直接与各个交易进行对帐。

**进一步阅读** ： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出详细信息](payout-policy-details.md)、 [税务详细信息](tax-details-marketplace.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>税款

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>我们如何在付款对账单中识别 Microsoft 和发布者之间的税务减免责任？

在交易历史记录下载中，找到“税模型”列。 此时会显示“MS 管理”或“ISV 管理”。 请参阅[税详细信息](tax-details-marketplace.md)中特定于国家/地区的税务规则和实际付款。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何下载服务费用纳税表单？

依次转到“付款支付”和“付款列表”部分。 对于具有服务费用税的付款，将显示指向服务费用纳税表单的链接。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何下载 PDF 格式的预缴税金表单？

依次转到“付款支付”和“付款列表”部分。 付款旁边将显示预缴税金表单的链接。

#### <a name="where-do-i-find-year-end-tax-forms"></a>在哪里可以找到年末纳税表单？

请转到[“配置文件”页](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)以查看你的年末纳税表单。

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>如何查找某个交易的预缴税金？
预缴税金适用于提交了 W-9 表单的美国发布者。 预缴税金是按照每月付款计算的。

**进一步阅读** ： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)， [详细信息策略详细信息](payout-policy-details.md)

## <a name="payout-statement-access"></a>对帐单访问权限

#### <a name="how-do-i-access-a-payout-statement"></a>如何访问付款对账单？

1. 请检查你的角色。 你必须具有“财务参与者”或“帐户所有者”角色才能访问付款对账单 。
2. 在右上方导航中，选择 " **支出** " 图标以查看支出报表。 选择 " **事务历史记录** "、" **付款** " 和 " **下载** "。

**进一步阅读** ： [支出角色和权限](payout-statement.md#roles-and-permissions)， [付出额外帐单](payout-statement.md) 

## <a name="payout-statement-report"></a>支出报表报表

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>交易下载内容中的每个字段是什么意思？

有关属性及其 [含义的详细列表，请参阅](payout-statement.md) 详细说明。

#### <a name="what-is-earning-status"></a>什么是收入状态？

这会显示 "未处理"、"已处理" 或 "已发送" 收入。

- 未 **处理–收入** 在到期日之前处于保管期内。
- 已 **处理** –收入已成熟，并已准备好每月支付。 支付每月15号发布。
- 已 **发送** –付款已成功地根据你的支出配置文件发布到银行。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何下载服务费用纳税表单？

依次转到“付款支付”和“付款列表”部分。 对于具有服务费用税的付款，将显示指向服务费用纳税表单的链接。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何实现下载 PDF 格式的预缴税金窗体？

依次转到“付款支付”和“付款列表”部分。 付款旁边将显示预缴税金表单的链接。

#### <a name="where-do-i-find-year-end-tax-forms"></a>在哪里可以找到年末纳税表单？

请转到[“配置文件”页](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)以查看你的年末纳税表单。

**进一步阅读** ： [支出报表](payout-statement.md)、 [事务历史记录下载](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>历史对帐单

#### <a name="how-do-i-view-historical-information"></a>如何实现查看历史信息？

历史对账单会显示截止到 2019 年 10 月的付款数据的快照。 遗憾的是，此处的支出信息不会刷新。 若要接收最新信息，请提交最新数据的支持票证。

**进一步阅读** ： [支出报表](payout-statement.md)、 [事务历史记录下载](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>支出导出 API

#### <a name="how-do-i-download-payout-data"></a>如何下载付款数据？

使用 [合作伙伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)。

## <a name="next-steps"></a>后续步骤

- [在商业市场中获得付款](marketplace-get-paid.md)
