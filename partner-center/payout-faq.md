---
title: 付款和税务配置文件常见问题
description: 获取有关合作伙伴中心的付款和税务详细信息的常见问题的解答。 包括有关收入为何与预期不同的解答。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 11/25/2020
ms.openlocfilehash: 3b09f0a08cd974f88afe5c5708df307830491f3f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492579"
---
# <a name="common-questions-about-payouts-and-taxes"></a>有关付款和税款的常见问题

**适当的角色**：

- 帐户管理员
- 全局管理员
- 奖励管理员

本文解答了有关合作伙伴中心的付款和税务详细信息的常见问题。所涉及的主题包括付款时间、检查收入资格以及正确设置支出和税务配置文件的重要性。

## <a name="profile-management"></a>配置文件管理

#### <a name="why-do-i-need-to-provide-or-update-my-payout-andor-tax-details"></a>为什么需要提供或更新支出和/或税务详细信息？

在新程序中注册的所有合作伙伴都必须提供有效的支出和税务详细信息，才能完成注册和接收付款。 仅在 Microsoft 验证支出和税务配置文件后，才会将注册视为已完成。

如果程序的规则发生更改，或者配置文件的各个方面过期或过期，则可能还需要更新信息。 如果发生这种情况，"概述" 页将显示 "需要执行操作" 的状态 **–更新银行和/或税务配置文件**。

#### <a name="how-do-i-find-set-up-or-update-payout-and-tax-details"></a>如何实现查找、设置或更新支出和税务详细信息？

有关如何更新合作伙伴中心的付款和税务详细信息的详细信息，请参阅 [设置你的帐户和税务表](set-up-your-payout-account.md)。

#### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>为什么在分配付款和税务配置文件时看不到注册？

这可能是因为你没有适当的权限，或者你使用不具有这些权限的帐户登录。 例如，只有 MPN 位置的激励管理员可以创建或管理支出和税务配置文件。 请与你的组织管理员联系，以管理银行和税务的权限。

#### <a name="im-only-able-to-sign-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>我只能用我的 @onmicrosoft.com 域登录。 应采取何种操作？

请联系你的帐户管理员，将其他域添加到 AAD 帐户。
 
#### <a name="my-organization-is-participating-in-multiple-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>我的组织正在参与多个计划。 我是否需要多次提供我的付款和税务配置文件？

这取决于组织的需求。 付款配置文件是在组织级别创建的，它允许将同一银行配置文件分配到组织内的多个 MPN ID 和计划。 在大多数情况下，可以重复使用现有的配置文件或创建新的配置文件。

但可能也有例外，例如将银行配置文件应用于不同的国家或地区时，因为当地银行或税务规定可能会适用。

当同一个 MPN 位置参与另一个程序时，将重新使用为 MPN 位置创建的税配置文件，并自动填充。 但是可能存在例外情况。 例如，新的奖励计划的付款规则可能需要其他的税务配置文件详细信息。

#### <a name="can-i-use-the-same-bank-and-tax-details-for-all-incentive-programs-at-microsoft"></a>能否对 Microsoft 中的所有激励计划使用同一银行和税务详细信息？

如果你的公司邀请了多个程序，则可以为所有程序使用相同的付款帐户，也可以选择为不同的程序使用不同的付款帐户。


#### <a name="how-does-microsoft-ensure-that-the-bank-information-is-indeed-that-of-the-company-and-not-a-personal-bank-account-for-an-employee"></a>Microsoft 如何保证银行信息确实是公司的信息，而不是员工的个人银行帐户？

公司负责确保激励管理员的角色（具有编辑此信息的权限）仅提供给相应的员工。

#### <a name="my-tax-profile-has-expired-how-do-i-fix-this"></a>税配置文件已过期。 如何修复此问题？

使用 [创建或更新税务配置文件](set-up-your-payout-account.md#create-or-update-your-tax-profile) 中的步骤来更新你的税务配置文件。 在 " **税务配置文件** " 页上，您可以在 " **到期日期** " 列中查看已过期或即将过期的配置文件。 

## <a name="earnings-incorrect-or-missing"></a>收入不正确或缺失

#### <a name="why-are-my-earnings-missing"></a>为何我的收入缺失？

- 客户订单可能还不符合付款条件。 对于非企业客户订单，Microsoft 必须先收到客户付款，然后发布者才能获得收入。 对于企业客户订单，你的收入将在采购订单日期之后的 1-2 天内提供。 请在[订单报表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中验证订单状态。
- 交易历史记录报表中可能不显示 2019 年 7 月之前的交易的收入。 请在[付款下载](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)中检查历史对账单。
- 检查 [付出的时间范围](payment-thresholds-methods-timeframes.md) 并了解你的收入应出现在付出的时间范围内。

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>为什么收入金额不同于我的预期？

- 如果订单已部分支付给客户，则您的收入金额将基于扣除费用和相应税款后的部分支付金额。
- 按国家/地区检查减税责任。 在税款由 Microsoft 负责的国家/地区，Microsoft 将从发布者收入中收集并扣除税款。 对账单中显示的交易金额为税后金额。 请参阅[税项详细信息](tax-details-marketplace.md)。
- SaaS 和 IaaS 产品/服务的折扣率为10%，而不是标准20%，而收入率为90%。 此促销在 2021 年 6 月 30 日之前有效。

**进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出策略详细信息](payout-policy-details.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)、 [付费](marketplace-get-paid.md)、 [税务详细信息](tax-details-marketplace.md)、额外 [帐单](payout-statement.md)

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

**进一步阅读**：[商业 marketplace 分析中的](/azure/marketplace/partner-center-portal/orders-dashboard)[支出报表](payout-statement.md)和订单仪表板

## <a name="payments-and-adjustments"></a>付款和调整

#### <a name="why-is-my-payment-missing"></a>为何我的付款缺失？

- 确保在 "[概述" 页](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)上，您的支出状态和税务配置文件状态显示为 *有效*。
- 你可能未满足付款的最小阈值。 收入必须至少为 50 美元才能获得付款。


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>如何实现将我的帐户设置为不接收支付？
你可以在费用 [配置文件](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)中保留付款;只需选中 " **保存**"。 在你发布保留期之前，Microsoft 会向你收取费用。

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>为什么我收到的货币与购买货币不同？

付款货币基于你在付款配置文件中选择的货币。 购买货币基于客户支付的货币。

#### <a name="how-do-i-reconcile-adjustments"></a>如何对调整进行对帐？

付款调整是用于容纳补偿调整（例如系统问题）的付款更正。 在付款对账单中，原因代码会指定调整原因。 它们不用于直接与各个交易进行对帐。

**进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出详细信息](payout-policy-details.md)、 [税务详细信息](tax-details-marketplace.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)

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

**进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)， [详细信息策略详细信息](payout-policy-details.md)

## <a name="payout-statement-access"></a>对帐单访问权限

#### <a name="how-do-i-access-a-payout-statement"></a>如何访问付款对账单？

1. 请检查你的角色。 你必须具有“财务参与者”或“帐户所有者”角色才能访问付款对账单 。
2. 在右上方导航中，选择 " **支出** " 图标以查看支出报表。 选择 " **事务历史记录**"、" **付款**" 和 " **下载**"。

**进一步阅读**： [支出角色和权限](payout-statement.md#roles-and-permissions)， [付出额外帐单](payout-statement.md) 

## <a name="payout-statement-report"></a>支出报表报表

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>交易下载内容中的每个字段是什么意思？

有关属性及其 [含义的详细列表，请参阅](payout-statement.md) 详细说明。

#### <a name="what-is-earning-status"></a>什么是收入状态？

这会显示 "未处理"、"已处理" 或 "已发送" 收入。

- 未 **处理–收入** 在到期日之前处于保管期内。
- 已 **处理**–收入已成熟，并已准备好每月支付。 支付每月15号发布。
- 已 **发送**–付款已成功地根据你的支出配置文件发布到银行。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何下载服务费用纳税表单？

依次转到“付款支付”和“付款列表”部分。 对于具有服务费用税的付款，将显示指向服务费用纳税表单的链接。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何实现下载 PDF 格式的预缴税金窗体？

依次转到“付款支付”和“付款列表”部分。 付款旁边将显示预缴税金表单的链接。

#### <a name="where-do-i-find-year-end-tax-forms"></a>在哪里可以找到年末纳税表单？

请转到[“配置文件”页](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)以查看你的年末纳税表单。

**进一步阅读**： [支出报表](payout-statement.md)、 [事务历史记录下载](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>历史对帐单

#### <a name="how-do-i-view-historical-information"></a>如何实现查看历史信息？

历史对账单会显示截止到 2019 年 10 月的付款数据的快照。 遗憾的是，此处的支出信息不会刷新。 若要接收最新信息，请提交最新数据的支持票证。

**进一步阅读**： [支出报表](payout-statement.md)、 [事务历史记录下载](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>支出导出 API

#### <a name="how-do-i-download-payout-data"></a>如何下载付款数据？

使用 [合作伙伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)。

## <a name="commercial-marketplace-payout-policies"></a>商业市场支出策略

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>如何查找当前的代理费和付款比率？

- 检查商业市场发布者协议。 标准代理费为 20%。 SaaS Co-Sell 符合条件的事务的折扣费用为10%。 检查是否有任何促销代理费的公告。
- 在您的费用声明中，收益率指定给定交易的实际付出费率。

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>在收入出现在我的对账单上后，多长时间可以收到 Microsoft 的付款？
- 当你的收入处于未处理状态之后，你可以检查将处理你的收入以进行付款的月份的到期日期。 支付准备就绪后，你的收益状态将更改为 "已处理"。  Microsoft 将在每个到期月份的 15 号之前发放付款。
- 对于信用卡支付的订单，Microsoft 保留30天的付款，直到收益得到成熟。

 **进一步阅读**： [商业 Marketplace 发布者协议](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支出详细信息](payout-policy-details.md)、 [税务详细信息](tax-details-marketplace.md)、 [支付阈值、方法和时间范围](payment-thresholds-methods-timeframes.md)

## <a name="next-steps"></a>后续步骤

- [获取付款](marketplace-get-paid.md)
- [设置付款帐户和纳税表单](set-up-your-payout-account.md)
