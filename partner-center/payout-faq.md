---
title: Microsoft 商业应用商店的支出
description: 获取有关商业应用商店中付款的常见问题的解答。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335646"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>有关商业 marketplace 付款的常见问题

本文解答了有关商业应用商店中的付款的常见问题。

## <a name="earnings-incorrect-or-missing"></a>收入不正确或缺失

#### <a name="why-are-my-earnings-missing"></a>为什么缺少收入？

- 客户订单可能不符合要求。 对于非企业客户订单，Microsoft 必须在发布者收益生效之前获得客户付款。 对于企业客户订单，收入将在采购订单日期之后1-2 天可用。 验证 [订单报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的订单状态。
- 事务历史记录报表中不显示在2019年7月之前的事务的收入。 查看正在进行的 [下载](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)的历史记录语句。
- 检查 [付出的时间范围](payment-thresholds-methods-timeframes.md) 并了解你的收入应出现在付出的时间范围内。

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>为什么收入金额不同于我的预期？

- 如果订单已部分支付给客户，则您的收入金额将基于扣除费用和相应税款后的部分支付金额。
- 按国家/地区检查减税责任。 如果国家/地区的税务为 Microsoft 负责任，Microsoft 将从出版商收益中收集并 deducts 税款。 该语句中显示的交易金额为税额后。 请参阅 [税务详细信息](tax-details-marketplace.md)。
- SaaS 和 IaaS 产品/服务的折扣率为10%，而不是标准20%，而收入率为90%。 此促销在2021年6月30日之前有效。

**进一步阅读**： [商业市场出版商协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出政策详细信息](payout-policy-details.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)、 [在商业市场中支付的](marketplace-get-paid.md)费用 [详细信息、费用详细信息](tax-details-marketplace.md)、费用 [报表](payout-statement.md)和 [商业 marketplace 分析中的订单仪表板](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>收入对帐
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>如何实现在分析中对费用报表和使用情况报表进行协调
使用 "记录订单" 和 "使用情况报告" 的 "对事务历史记录进行支出" 报表中显示的 AssetID、订单 ID 和行项 ID 使用以下映射：

- 付出的交易历史记录。 AssetID = order。订单
- 对事务历史记录进行支出 & LineItem = UsageReferenceID [订单 Id： LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>如何实现知道何时应向客户订单付款？
- 首先，使用 assetID，检查 [订单报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的客户订单。
- 在客户 [报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)中检查客户的客户渠道。
- 对于企业客户，发布者收益显示在采购订单日期之后的1-2 天内。
- 对于非企业客户，发布者收益在收到客户付款后的1-2 天内显示。

**进一步阅读**：[商业 marketplace 分析中的](/azure/marketplace/partner-center-portal/orders-dashboard)[支出报表](payout-statement.md)和订单仪表板

## <a name="payout-policies"></a>支出策略

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>如何实现找出当前机构费用和付出比率？

- 查看商业 marketplace 发布者协议。 标准代理商费为20%。 SaaS 共同销售符合条件的交易的折扣费用为10%。 检查是否有任何促销机构费用的公告。
- 在您的费用声明中，收益率指定给定交易的实际付出费率。

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>在我的语句上出现收入后，我应从 Microsoft 支付一次款项？
- 如果你的赢利处于未处理状态，你可以查看该月的到期日期，以便支付收入。 支付准备就绪后，你的收益状态将更改为 "已处理"。  Microsoft 将按成熟月15日发布付款。
- 对于信用卡支付的订单，Microsoft 保留30天的付款，直到收益得到成熟。

 **进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出详细信息](payout-policy-details.md)、 [税务详细信息](tax-details-marketplace.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>付款和调整

#### <a name="why-is-my-payment-missing"></a>为何我的付款丢失？

- 确保在 "[概述" 页](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)上，您的支出状态和税务配置文件状态显示为*有效*。
- 你可能未满足支付的最小阈值。 收入必须至少为 $50 美元才能获得支付。


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>如何实现将我的帐户设置为不接收支付？
你可以在费用 [配置文件](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)中保留付款;只需选中 " **保存**"。 在你发布保留期之前，Microsoft 会向你收取费用。

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>为什么接收到的货币与购买货币不同？

付出的货币基于您在付出的配置文件中选择的货币。 采购币种基于客户支付的货币。

#### <a name="how-do-i-reconcile-adjustments"></a>如何实现协调调整？

支付调整是用于适应补偿调整（如系统问题）的付款更正。 在支出语句中，ReasonCode 将指定调整的原因。 这并不是要直接与单独的事务进行协调。

**进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出详细信息](payout-policy-details.md)、 [税务详细信息](tax-details-marketplace.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>税款

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>如何确定支出报表中的 Microsoft 或出版社之间的减税责任？

在 "事务历史记录" 下载中，查找 "税务模型" 列。 这显示了 MS 托管或 ISV 管理的。 请参阅特定于国家/地区的税务规则和支出 [详细信息](tax-details-marketplace.md)影响。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何实现下载服务费用纳税表单？

依次前往 " **支出支付** " 页和 " **付款** " 部分列表。 对于具有服务费用税率的付款，将显示一个指向服务费用的链接。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何实现下载 PDF 格式的预缴税金窗体？

依次前往 " *支出支付* " 页和 " **付款** " 部分列表。 付款旁边将显示预缴税金窗体的链接。

#### <a name="where-do-i-find-year-end-tax-forms"></a>在哪里查找年末税务表格？

请在 " [配置文件" 页](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) 上查看您的年末税务表。

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>如何实现为交易查找预缴税金？
预缴税金适用于归档了 i-9 窗体的美国出版商。 预缴税金按月支付计算。

**进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)， [详细信息策略详细信息](payout-policy-details.md)

## <a name="payout-statement-access"></a>对帐单访问权限

#### <a name="how-do-i-access-a-payout-statement"></a>如何实现访问支出报表？

1. 检查你的角色。 您必须拥有 *财务参与者* 或 *帐户所有者* 角色才能访问付出的支出。
2. 在右上方导航中，选择 " **支出** " 图标以查看支出报表。 选择 " **事务历史记录**"、" **付款**" 和 " **下载**"。

**进一步阅读**： [支出角色和权限](payout-statement.md#roles-and-permissions)， [付出额外帐单](payout-statement.md) 

## <a name="payout-statement-report"></a>支出报表报表

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>事务下载中的每个字段是什么意思？

有关属性及其 [含义的详细列表，请参阅](payout-statement.md) 详细说明。

#### <a name="what-is-earning-status"></a>什么是收益状态？

这会显示 "未处理"、"已处理" 或 "已发送" 收入。

- 未**处理–收入**在到期日之前处于保管期内。
- 已**处理**–收入已成熟，并已准备好每月支付。 支付每月15号发布。
- 已**发送**–付款已成功地根据你的支出配置文件发布到银行。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何实现下载服务费用纳税表单？

依次前往 " **支出支付** " 页和 " **付款** " 部分列表。 对于具有服务费用税率的付款，将显示一个指向服务费用的链接。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何实现下载 PDF 格式的预缴税金窗体？

依次前往 " **支出支付** " 页和 " **付款** " 部分列表。 付款旁边将显示预缴税金窗体的链接。

#### <a name="where-do-i-find-year-end-tax-forms"></a>在哪里查找年末税务表格？

请在 " [配置文件" 页](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) 上查看您的年末税务表。

**进一步阅读**： [支出报表](payout-statement.md)、 [事务历史记录下载](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>历史对帐单

#### <a name="how-do-i-view-historical-information"></a>如何实现查看历史信息？

历史记录语句将显示2019年10月的支出数据的快照。 遗憾的是，此处的支出信息不会刷新。 若要接收最新信息，请提交最新数据的支持票证。

**进一步阅读**： [支出报表](payout-statement.md)、 [事务历史记录下载](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>支出导出 API

#### <a name="how-do-i-download-payout-data"></a>如何实现下载支出数据？

使用 [合作伙伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)。

## <a name="next-steps"></a>后续步骤

- [在商业市场中获得付款](marketplace-get-paid.md)
