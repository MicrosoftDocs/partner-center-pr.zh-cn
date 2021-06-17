---
title: 支出声明
description: 了解付款对帐单和摘要，以及如何查看和导出 Microsoft 合作伙伴中心
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: dc0c720544f4a8a3c95e5b91ec656e65dbce7c80
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276104"
---
# <a name="payout-statements"></a>支出声明

**适当角色**：帐户管理员|全局管理员

付款 **对** 账单概述了通过商业市场销售的产品/服务中的付款。 它显示收益的事务历史记录、估算下一次付款，以及付款趋势。 还可以下载交易历史记录和付款对帐单。 本文介绍如何访问付款对账单，以及你可在其中访问的不同付款页面和合作伙伴中心。

>[!NOTE]
>只会看到与关联的 MPN ID 和程序的数据。 如果想查看其他数据，请与帐户管理员联系以授予权限。 

## <a name="roles-and-permissions"></a>角色和权限

若要访问付款对账单，需要分配帐户 **所有者或****财务参与者** 角色。

| 报表/页 | 帐户所有者 | Manager | 开发人员 | 业务参与者 | 财务参与者 | 营销人员 |
| --- | --- | --- | --- | --- | --- | --- |
| 获取报表（包括准实时数据） | 可以查看 | 可以查看 | 不允许访问 | 不允许访问 | 可以查看 | 不允许访问 |
| 反馈报告/响应 | 可以查看和发送反馈 | 可以查看和发送反馈 | 可以查看和发送反馈 | 不允许访问 | 不允许访问 | 可以查看和发送反馈 |
| 运行状况报告（包括准实时数据） | 可以查看 | 可以查看 | 可以查看 | 可以查看 | 不允许访问 | 不允许访问 |
| 使用情况报告 | 可以查看 | 可以查看 | 可以查看 | 可以查看 | 不允许访问 | 不允许访问 |
| 付款帐户 | 可以更新 | 不允许访问 | 不允许访问 | 不允许访问 | 可以更新 | 不允许访问 |
| 税务资料 | 可以更新 | 不允许访问 | 不允许访问 | 不允许访问 | 可以更新 | 不允许访问 |
| 付款摘要 | 可以查看 | 不允许访问 | 不允许访问 | 不允许访问 | 可以查看 | 不允许访问 |
|

## <a name="access-your-payout-statement"></a>访问付款对账单

登录到 [合作伙伴中心并选择](https://partner.microsoft.com/dashboard/home) 屏幕右上角的付款图标，以访问以下不同的摘要：

- 交易历史记录
- 支付
- 导出数据

:::image type="content" source="images/payouts/payout-overview.png" alt-text="展示了合作伙伴中心门户右上角的“付款”图标。":::

还可使用合作伙伴付款 [API](https://apidocs.microsoft.com/services/partnerpayouts) 直接连接和获取付款交易和付款数据。


## <a name="transaction-history"></a>交易历史记录

" **交易历史记录** "页显示过去 36 个月的收益摘要、下一次付款的估计以及收益和付款趋势。 还可以从本部分下载事务详细信息。<br><br>此报表显示符合付款条件的所有收益，包括尚未发送的付款。 当 ISV 在 合作伙伴中心 中完成所有银行和税务信息、赚取了 >$50、ISV 帐户处于活动状态，并且客户已针对 EA 交易) 或已收到针对非 EA 交易) 的付款 ( (，则符合付款条件。

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="事务概述。":::

- **今年发送的收入** - 已支付且将在下个月支付的总收益和收益明细。
- **估计付款月份** - 预期未来几个月的总收益。
- **收益和付款趋势** - 过去 36 个月的每月收入与付款金额。
- **下载** - 以 .tsv .csv下载事务详细信息。

使用页面右上角的日期范围选择来筛选页面的输出，以显示过去 3 个月、6 个月、12 个月或 36 个月。 或者，选择一个自定义日期范围（最多 36 个月）。 默认日期范围为 12 个月。 还可以按"注册 ID"、"计划"、"付款 ID"、"收入类型"、"锁定"和"状态"进行筛选。 数据可用于 7 月 1 (6 月 30) 和前两个会计年度的当前会计年度。

:::image type="content" source="images/payouts/search-filter.png" alt-text="页面右上方的搜索筛选器。":::

若要查看关于收入的更多详情，请选择页面右侧的向下箭头。 这样做将显示控制器、收入金额、产品和客户。 如果出于某种原因此数据不可用，但你需要访问这些数据，请联系支持人员。 如果收入是调整的结果，而不是交易的结果，则不显示"产品"和"客户"字段。

### <a name="transaction-history-summary"></a>事务历史记录摘要

此视图显示收入详细信息，包括产品销售收入日期、状态和估计付款月份的收入来源。

:::image type="content" source="images/payouts/transaction-history.png" alt-text="事务历史记录。":::

- **赚取的日期** - 购买日期。
- **收入类型** - 收入类型，例如"销售"、"收入"或"合作"。
- **总计** - 净收入金额。 在商业市场中，这意味着在减去标准市场费用之后。
- **状态** – 有三个选项：
    - **即将推出的** – 收益正在等待冷却期。
    - **已** 处理 - 收入已准备好进行下一次付款。
    - **已** 发送 - 已支付收益。
- **估计付款月份** - 预期支付收益的月份。 有关详细信息 [，请参阅](#estimated-payment-month) 下一部分。

当交易满足付款资格后，会显示收入交易。 若要了解可能缺少或意外收益的原因，请参阅有关商业 [市场付款的常见问题](payout-faq.md#why-are-my-earnings-missing)。

#### <a name="estimated-payment-month"></a>估计付款月份

"交易历史记录"页现在包含一个表，其中显示了未来几个月的估计付款金额。 还可以在事务历史记录和摘要报表导出中查看和下载此信息。 此信息使对帐和付款预测更容易。

估计付款月份是根据计划配置规则和时间线计算的，将在下一个/即将进行的付款周期中处理。

预计付款月当前可用于除合作之外的所有收入类型，这将显示为"**不适用"。** 对于 2020 年 7 月 1 日之前的收入，估计付款月份将显示为 **"不可用"。**

下表显示了估计的付款月份示例。

| Month | 金额 |
| ------ | :-----------: |
|  2020 年 9 月 |  $7，273.99   |
|  2020 年 10 月 | $8，692.30  |
|  2020 年 11 月 | $107.89  |

由于多种原因，估计金额可能与实际金额不同：

- 收入重述：如果重新计算收益，实际金额将有所不同
- 调整：实际金额因发生的或提交的调整而异。
- 规则更改：规则更改可能会反映实际支付金额的重新计算
- 付款：如果付款失败，实际金额可能不同

请注意，只有在满足计划的阈值和付款资格规则时，你的付款才在预计月份释放。 这些规则包括但不限于以下列表：

- 税务配置文件必须是最新的
- 你的收益必须满足或超过计划指南中定义的最低收入阈值。
- 暂停付款：如果在配置文件分配页上选择"保留我的付款"选项。
- 付款工具不可用：付款或/和税务配置文件未完成。

### <a name="transaction-history-download"></a>事务历史记录下载

若要了解有关收入的详细信息，请选择 **页面** 顶部的"下载"。 下表说明了报表的每一列。

>[!NOTE]
>截至 2020 年 8 月，事务历史记录下载导出有两个新字段：
>
>- **lastPaymentCurrency**  当前登录的合作伙伴有权访问的所有 MMP 中收到最近付款的货币。 如果未收到付款，则最后一个付款货币将为美元。
>- **earningAmountInLastPaymentCurrency**  最后一个付款货币的收入金额。

| 列名称 | 说明 | 奖励计划/市场的适用性 |
| --- | --- | --- |
| AgreementEndDate | 协议结束日期 | 激励 - 仅某些计划 |
| agreementNumber | 协议编号 | 激励 - 仅某些计划 |
| AgreementStartDate | 协议开始日期 | 激励 - 仅某些计划 |
| calculationDate | 在系统中计算收入的日期 | All |
| claimId | 索赔的唯一标识符 | 激励 - 仅某些计划 |
| customerCountry | 客户所在国家/地区 | marketplaces |
| customerEmail |  |  |
| customerName | 可能为空 | 奖励计划仅 (例外情况：OEM) 和市场。 对于 CSP 事务，市场将显示 CSP 的名称 |
| customerTenantId |  |  |
| distributorId | 分销商标识符 | 激励 - 仅某些计划 |
| distributorName | 分销商名称 | 激励 - 仅某些计划 |
| earningAmount | 收入金额（以原始交易币种为单位） | All |
| earningAmountInLastPaymentCurrency | 上一付款币种的收入金额（如果之前没有付款，则字段将为空） |  |
| earningAmountUSD | 收入金额（以美元为单位） | All |
| earningDate | 收入日期 | All |
| earningExchangeRate | 用于显示相应金额（以美元为单位）的汇率 | All |
| earningId | 每笔收入的唯一标识符 | All |
| earningRate | 对交易金额应用的奖励费率以生成收入 | All |
| earningType | 表示是否是费用、返点、合作收入、销售收入等 | All |
| exchangeRateDate | 用于计算 EarningAmount（以美元为单位）的汇率日期 | All |
| externalReferenceId | 计划的唯一标识符 | 直销计划 (激励和市场)  |
| externalReferenceIdLabel | 唯一标识符标签 | 直销计划 (激励和市场)  |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | 发票编号 (适用于仅适用于企业的)  | 激励和市场-仅限一些程序 |
| lastPaymentCurrency | 上一付款币种（如果之前没有付款，则字段将为空） |  |
| lever | 表示收入的业务规则 | All |
| LicensingProgramName | 许可计划的名称 |  |
| LineItemId | 客户发票中的单个行 |  |
| localProviderSeller | 记录的本地提供商/卖家 |  |
| 成熟度月 | 估计的付款月 | 全部 |
| OrderId | 与客户的发票相关  | marketplaces |
| parentProductId | 唯一父产品标识符。 如果交易没有父产品，则父产品 ID = 产品 ID。 | marketplaces |
| parentProductName | 父产品名称。 如果交易没有父产品，则父产品名称 = 产品名称。 | marketplaces |
| participantID | 计划下合作伙伴收入的主要标识 | All |
| participantIdType | 奖励计划和卖方的主要计划 ID （如果针对市场） | All |
| participantName | 收入合作伙伴的名称 | All |
| partnerCountryCode | 收入合作伙伴所在的位置/国家/地区 | All |
| partNumber | 始终为空白 | 某些激励计划和市场 |
| paymentId | 用于将事务报表中的所有事务与付款报表中的特定付款关联的唯一标识符 | 全部 |
| paymentStatus | 付款状态 | All |
| paymentStatusDescription | 付款状态的易记说明 | All |
| productId | 唯一产品标识符 | marketplaces |
| productName | 与交易关联的产品名称 | 全部 |
| productType | 产品类型（如应用、加载项和游戏） | marketplaces |
| Program Code | 要与计划名称一起映射的字符串 |  |
| programName | 激励计划/应用商店计划的名称 | All |
| purchaseOrderCoverageEndDate | 始终为空白 | 激励计划 - CRI |
| purchaseOrderCoverageStartDate | 始终为空白 | 激励计划 - CRI |
| purchaseOrderType | 始终为空白 | 激励计划 - CRI |
| purchaseTypeCode | 始终为空白 | 激励计划 - CRI |
| quantity | 因计划而异。 表示交易计划的已计费数量 | All |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | 经销商标识符 | 激励 - 仅某些计划 |
| resellerName | 经销商名称 |  |
| SkuId | 发布期间定义的 SKU ID。 一个产品/服务可能有许多 SKU，但一个 SKU 只能与一个产品/服务关联。 激励 - 仅某些计划 |  |
| storeFee | Microsoft 保留金额，用于支付在应用商店中提供应用或加载项的费用 | marketplaces |
| subscriptionEndDate | 订阅结束日期 | 激励 - 仅某些计划 |
| subscriptionId | 与客户关联的订阅标识符 | 激励 - 仅某些计划 |
| subscriptionStartDate | 订阅开始日期 | 激励 - 仅某些计划 |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | 汇出税款（销售税、使用税或 VAT/GST 税）的责任方 | marketplaces |
| taxRemitted | 汇出的税款金额（销售税、使用税或 VAT/GST 税） | marketplaces |
| taxState | 客户所在的州/省 |  |
| taxZipCode | 客户的邮政编码 |  |
| tpan | 表示第三方广告网络 | 仅市场广告 |
| transactionAmount | 交易金额（以产生收入的原始交易币种为单位） | All |
| transactionAmountUSD | 交易金额（以美元为单位） | All |
| transactionCountryCode | 发生交易的国家/地区代码 |  |
| transactionCurrency | 原始客户交易发生时使用的币种（这不是合作伙伴所在位置的币种） | All |
| transactionDate | 交易日期。 适用于多次交易促成一笔收入的计划 | All |
| transactionExchangeRate | 用于显示相应交易金额（以美元为单位）的汇率日期 | All |
| transactionId | 交易的唯一标识符 | All |
| transactionPaymentMethod | 用于交易的客户付款方式（如银行卡、移动运营商计费或 PayPal） | marketplaces |
| TransactionType | 交易类型（如购买、退款、冲销或退单） | marketplaces |
| workload | 工作负荷 | 激励 - 仅某些计划 |
|

### <a name="transaction-adjustment-codes"></a>事务调整代码

下表列出了调整的原因代码及其说明。

|**原因代码**   |**说明**   |
|------------------|:-------------------------------------|
| AR 符合性 | 在合作伙伴未及时支付 Microsoft 发票时减少收益的调整。 |
| 合作滚动更新 | 将合作收益转移到另一个周期或将合作收益转换为盈利的调整。 |
| Ops 调整 | 用于更正 Microsoft 系统计算错误的调整。 |
| Ops 调整 Microsoft 错误的计算 | 用于更正错误计算调整。 |
| Ops 调整 Microsoft 注册不正确 | 与注册相关的错误计算调整。 |
| MCI/CSP (合作伙伴) 映射 | 用于更正订阅未对齐的调整。 |
| 策略异常 | 替代程序规则的调整。  |
| 上一周期收益 | 调整当前收入期外的收入。 |

## <a name="payments"></a>支付

" **付款** "页详细说明了你通过 Microsoft 赚取的收入。 它还显示付款时间以及付款时间。

>[!Note]
> 你的收款必须达到 50 美元的[付款阈值](payment-thresholds-methods-timeframes.md)，才符合成为付款的条件。 有关详细信息，请参阅 Microsoft [发布者协议](/legal/marketplace/msft-publisher-agreement)。

:::image type="content" source="images/payouts/payments-overview.png" alt-text="付款概述屏幕。":::

- **今年付款总额** - 所有计划今年支付的总付款总额（美元）。
- **下一次** 估计付款 - 即使即将 (其他付款，) 以美元为单位。
- **上次付款** – (付款的美元) 计划名称和计划。
- **按源付款** – (12 个月内按计划) 美元付款金额。

### <a name="payments-list"></a>付款列表

" **付款列表"** 表显示已付款和待付款。 可以下载 PDF 格式的服务费用税务信息，并查看给定付款的收入详细信息。

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="导出事务历史记录。":::

- **付费** - 已成功发送所有付款。 在下拉菜单中选择年份，以筛选该年份发布的付款。
- **挂起** - 即将付款。
- **服务费用 (PDF 格式)** - 适用于收取服务费用税的付款。 服务费用税显示在"其他 **税款"中**。
- **视图** - 重定向到交易历史记录，其中列出了付款中包含的收益。

若要了解可能缺少或意外收益的原因，请参阅有关商业 [市场付款的常见问题](payout-faq.md#why-are-my-earnings-missing)。

### <a name="payment-status"></a>付款状态

下表说明了不同的收入状态。

| 收入状态 | 原因 | 合作伙伴是否需要采取行动？ |
| --- | --- | --- |
| 未处理 | 收入符合成为付款的条件。 它保持此状态，以冷却期，如设备计划指南奖励计划。 | 否 |
| 即将处理 | 处理付款之前生成的付款订单挂起的内部评审。 | 否 |
| 等待纳税发票 | 税务发票不完整或无效。 | 必须更新纳税发票，才能收到付款 |
| 审查期间被拒绝 | 付款在审查期间被拒绝。 | 有关详细信息，请联系 Microsoft 支持人员 |
| 已失败 | 由于 Microsoft 系统错误，付款失败。 | 有关详细信息，请联系 Microsoft 支持部门 |
| 正在学习 | 付款正在进行中。 | 否 |
| 付款不正确 | 付款重新付款正在进行中。 | 否 |
| 已发送 | 付款已发送到银行。 | 否 |
| 正在重新处理 | 付款遇到 Microsoft 系统错误，正在重新处理。 | 否 |
| Reversed | 付款被银行撤销，将在下一个付款周期中再次发送。 | 否 |
| 纳税发票被拒绝 | 纳税发票在审查期间被拒绝了。 在纳税发票审查完成之前，所有挂起的付款都将处于暂停状态。 | 有关详细信息，请联系 Microsoft 支持部门 |
| 正在审查纳税发票 | 正在审查纳税发票。 一旦纳税发票获准，就会发放付款。 | 否 |
| 已拒绝 | 银行拒绝了付款。 | 有关详细信息，请联系银行。 |
|

### <a name="payments-download"></a>付款下载

 下表说明了报表的每一列。 若要了解有关付款的更多详细信息，请选择"付款 **"** 页顶部的"下载"。

| 列名称 | 说明 |
| --- | --- |
| participantID | 计划下合作伙伴收入的主要标识 |
| participantIdType | 通常，奖励计划的计划 ID 和商店计划的卖家 ID |
| participantName | 收入合作伙伴的名称 |
| programName | 奖励/商店计划名称 |
| earned | 计划/participantID 赚取的金额（以付款币种为单位） |
| earnedUSD | 计划/participantID 赚取的金额（以美元为单位） |
| withheldTax | 计划/participantID 的预扣税款金额（以付款币种为单位） |
| salesTax | 计划/参与者 ID 计划的销售税总额（以付款币种表示 (仅适用于奖励计划)  |
| serviceFeeTax | 计划/participantID 的 serviceFeeTax 总金额（以付款币种为单位）（仅适用于应用商店计划和 Azure 市场） |
| totalPayment | 计划/participantID 的总付款（以本国币种为单位），不含预扣税款，但包括销售税（若有） |
| currencyCode | 付款币种代码 |
| paymentMethod | 向合作伙伴付款的方式（例如，电子银行转帐、贷方通知单） |
| paymentID | 付款的唯一标识符。 此编号通常显示在银行对帐单中（仅适用于 SAP 付款）。 |
| paymentStatus | 付款状态 |
| paymentStatusDescription | 付款状态的易记说明 |
| paymentDate | Microsoft 发放付款的日期 |
|

## <a name="export-data"></a>导出数据

" **导出数据** "页不会自行刷新。 你可能需要手动刷新此页，才能看到最新数据。 从三个选项卡中选择以 **导出"事务** 历史记录"、"**付款"、"****事务摘要**"或 **"历史语句"。**

筛选器可能会导致"无 **可用数据"** 错误。 如果将默认时间段选择为三个月，然后从超出该期限的收入中选择了付款 ID，则可能会发生这种情况。 如果发生这种情况，请展开时间段，然后重试。

下面是付款导出示例：

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="导出付款报表。":::

### <a name="historical-statements"></a>历史对帐单

导出 **数据** 摘要还提供对历史语句的访问。

> [!NOTE]
> 历史语句是快照，不会刷新。 如果需要 [，请联系](https://partner.microsoft.com/support/v2/?stage=1) 支持部门并请求最新数据。

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="导出历史语句。":::

- 2019 年 7 月 1 日后的事务历史记录单独处理，并使用以后历史记录报告中的不同字段。
- 旧事务历史记录有一个称为"Reserved"的列，该列对应于现代历史记录中的"收益"列，只不过它不包括状态等于"已发送付款"的所有收益。
- 3M、6M 或 12M 等筛选器不适用于“历史对帐单”部分。

### <a name="historical-statement-downloads"></a>历史语句下载

下表解释了历史语句的每一列。

| 字段名称 | 说明 |
| --- | --- |
| 收入来源 | 收入来源，取决于发生交易的位置，如 Microsoft Store、Windows Phone 应用商店、Microsoft Store 8 或广告 |
| 订单 ID | 唯一订单标识符。 使用此 ID，可以识别购买交易及其各自的非购买交易（如退款或退单）。 两者具有相同的订单 ID。 此外，如果存在拆分费用，其中对单个购买使用了多种付款方式，则允许链接购买交易。 |
| Transaction ID | 唯一交易标识符。 |
| 交易日期/时间 | 交易发生的日期和时间 (UTC)。 |
| 父产品 ID | 唯一父产品标识符。 如果交易没有父产品，则父产品 ID = 产品 ID。 |
| 产品 ID | 唯一产品标识符。 |
| 父产品名称 | 父产品名称。 如果交易没有父产品，则父产品名称 = 产品名称。 |
| 产品名称 | 产品名称 |
| 产品类型 | 产品类型（如应用、加载项和游戏） |
| 数量 | 当“收入来源”为“适用于企业的 Microsoft Store”时，“数量”表示购买的许可证数量。 对于其他所有收入来源，“数量”始终为“1”。 即使因为使用了两种不同的付款方式而将一项交易拆分为两个行项，每个行项也都显示值为“1”的“数量”。 |
| 事务类型 | 交易类型（如购买、退款、冲销或退单） |
| 付款方式 | 用于交易的客户付款方式（如银行卡、移动运营商计费或 PayPal） |
| 国家/地区 | 发生交易的国家/地区 |
| 本地提供商/卖家 | 记录的本地提供商/卖家 |
| 交易币种 | 交易币种 |
| 交易金额 | 交易金额 |
| 汇出税款 | 汇出的税款金额（销售税、使用税或 VAT/GST 税） |
| 净收入 | 交易金额减去汇出的税款金额 |
| 应用商店费用 | Microsoft 保留的净收入百分比，用于支付在应用商店中提供应用或加载项的费用 |
| 应用收款 | 净收入减去应用商店费用 |
| 预扣税款 | 预扣的所得税金额（不包含在“预留”CSV 文件中） |
| 付款 | 应用收款减去任何相应所得税预扣金额（金额以交易币种显示）。 不包含在“预留”CSV 文件中。 |
| 外汇汇率 | 用于将交易币种转换为付款币种的外汇汇率 |
| 付款币种 | 付款使用的币种 |
| 转换后的付款 | 使用外汇汇率转换为付款币种的付款金额 |
| 税款汇出模型 | 汇出税款（销售税、使用税或 VAT/GST 税）的责任方 |
| 资格日期/时间 | 交易收款符合成为付款的条件的日期和时间 (UTC)。 在付款创建后，它包括“资格日期/时间”先于付款创建日期的交易收款（只包含在“预留”CSV 文件中）。 |
| Charges | 显示“交易金额”列中聚合的所有费用详细信息的细目（只对 Azure 市场包括，不包括在“预留”CSV 文件中）。 |
|||

## <a name="next-steps"></a>后续步骤

- [合作伙伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [付款策略详细信息](payout-policy-details.md)
- 有关计费支持，请联系商业市场[发布者支持](https://partner.microsoft.com/support/v2/?stage=1)。