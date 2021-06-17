---
title: 排查付款和收益问题
ms.topic: article
ms.date: 02/05/2021
description: 了解如何解决缺失或不正确的收益、资格问题，以及如何协调奖励收益等问题。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ad71a6e02d6472ae844c504491e5acb05d5d6426
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277855"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>排除缺少付款、收入错误和其他问题

**适当的角色**：激励管理员

本文将帮助你解决激励计划中的任何收益或付款问题。 涉及的主题包括付款时间、检查收入资格以及正确设置支出和税务配置文件的重要性。

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>谁可以创建或更新组织的支出和税务配置文件？

在合作伙伴中心获得相关激励计划和 MPN 位置的激励管理员角色的用户可以更新和查看组织的支出和税务配置文件。

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Microsoft 批准待处理付款和/或税务配置文件需要多长时间？

验证最多可能需要 48 小时。 在此期间，“概述”页面上的配置文件状态将显示为“正在验证注册”。 完成此过程后，状态将显示为 "已 **注册** " （如果成功）或 " **需要操作–更新付款" 和/或 "税务详细信息** " （如有必要）。

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>如何得知我是否正确填写了付款和税务配置文件？

注册状态显示在“概述”页面上。 完成配置文件的创建后，状态将为 " **正在验证注册**"。 验证你的信息后，你的状态将更改为 "已 **注册**"。 此状态表示你的支出和税务配置文件以及你的注册已成功完成。

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>为什么需要更新税务配置文件才能将其用于新的激励计划？

我们会根据激励类型从不同位置支付奖励。 根据激励计划规则，这些不同的位置可能需要附加税务信息才能正确处理。

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>如何删除付款和/或税务配置文件？

Microsoft 当前不提供删除现有付款和税务配置文件的选项。

## <a name="my-payment-is-missing-or-incorrect"></a>我的付款已丢失或不正确

付款缺失或不正确通常是由以下某一原因所致：

- **您可能不符合条件。**  仅当你满足运营资格要求（即在相应的计划收入期内处于注册状态）时，收益才可用。
- **您可能尚未满足要求。**  检查以确定是否已满足所需激励的资格和合格收入规则。

  **检查您的资格**

  1. 登录 [合作伙伴奖励](https://partner.microsoft.com/membership/partner-incentives)。

  2. 向下滚动到程序的文档。
  
  3. 选择所需的文档链接，然后查看各个部分 

**合作伙伴资格** 和 **符合条件的收入规则**。

- **你的付款配置文件可能不完整。** 奖励收益开始日期将是你满足所有资格要求（包括加入时需要填写付款和税务详细信息）的当月的第一天。 对于填写付款和税务信息之前的几个月，你将不会获得任何收益。 例如，如果你在 2020 年 4 月满足了所有要求，则收益开始日期为 2020 年 4 月 1 日。
- **您可能有一个未完成的操作**。  这可能是由于奖励没有得到处理，因为你有待处理的未完成操作。

  **查看未完成的操作**

  1. 登录 [合作伙伴奖励](https://partner.microsoft.com/membership/partner-incentives)。
  2. 打开 " **事务历史记录** " 页。 查看此页中的字段，以查看要完成的任何未完成的操作，如 **待定税务配置文件**、 **挂起的付款配置文件** 或 **待定的税务发票提交**。

如果这些操作没有帮助，但你的付款仍缺失或不正确，请联系 [支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="how-can-i-reconcile-my-adjustments"></a>如何协调调整？

您可以通过下载您的赢利和交易细节来找到并协调调整。

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。
2. 在顶部导航栏上，选择 "货币" 图标，然后选择 " **事务历史记录**"。
3. 应用适当的筛选器。  (参阅下面的 **重要** 说明。 ) 
4. 筛选数据后，选择 " **开始下载**"，然后选择 " **导出数据**"。 你的数据将在 CSV 文件中打开。
5. 在 CSV 文件中，导航到第 P 列： " **收入类型**"。
6. 筛选此列以进行 **调整-返利**。 您可以在列中看到每个调整的月份。

>[!IMPORTANT]
>应用了调整的月份的收入中将不会显示应用于先前收益期的调整。 调整将始终在应用了调整的月份的收入报表中反映出来。
>
>例如，在9月2019日处理的2019年9月收益的调整将不会反映9月2019日的收入金额。 但是，在收到九月2019年9月的付款时，它将包括9月2019的调整时间。 在这种情况下，需要下载2019年1月的事务详细信息，以查看已应用的调整。
>
>设置日期筛选器时，请记住这一点。 如上所述，对前一个期间的调整仅在应用了调整的月份中可见。 仔细检查所选日期范围是否与要尝试查找的调整的月份相对应。 可能需要选择 " **全部清除** " 来删除筛选器，然后应用新的筛选器。

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>为什么我的合作申请款项采用了两种不同的货币支付？

在合作资金是从不同的 Microsoft 实体赚取的情况下，款项会以每一实体的当地货币支付。  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>为什么我的款项是以合作申请货币以外的货币支付的？

每一激励计划都有在设置期间创建的一个银行配置文件。 该配置文件中指定的货币是付款所采用的货币。

## <a name="i-dont-see-earnings-for-a-certain-period"></a>我看不到某个时间段的收入

如果看不到预期的时间段，通常是由以下问题之一导致的：

- **您可能不符合条件。**  仅当你满足运营资格要求（即在相应的计划收入期内处于注册状态）时，收益才可用。

- **你的付款配置文件可能不完整。**  奖励收益开始日期将是你满足所有资格要求（包括加入时需要填写付款和税务详细信息）的当月的第一天。 对于填写付款和税务信息之前的几个月，你将不会获得任何收益。 例如，如果你在 2020 年 4 月满足了所有要求，则收益开始日期为 2020 年 4 月 1 日。

如果你已经完成了符合性要求，其中包含有关时间的支出和税务详细信息，但仍找不到收入，请联系 [支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="my-earnings-are-missing-or-incorrect"></a>我的收入缺失或不正确

收益缺失或不正确可能由下列某个问题导致：

- **你可能没有满足相应要求。**  请检查你是否具备[资格](#my-payment-is-missing-or-incorrect)以及是否符合所需奖励的合格收益规则。

- **可能存在差异。**  如果你同时满足 [节目资格](incentives-determined-your-program-eligibility.md) 和 [收益资格](incentives-confirm-your-earnings-eligibility.md) 要求并且你的收入似乎不正确，以下信息可帮助你检索数据。

收益显示在 " **事务历史记录** " 页和 " **付款** " 页上。 可以通过选择 "合作伙伴中心" 中导航栏上的 " **支出** " 图标来访问这两个页面。

:::image type="content" source="images/incentives/paymenticon.png" alt-text="事务信息。":::

交易历史记录视图中的每月收益量可能与特定月份收到的付款金额不符。 这是因为在未来的支付期内进行了重新计算和调整。

例如，9月2019日处理的2019年9月收益的调整将不会反映在9月2019的收入金额中;但是，在收到九月2019年9月的付款时，它将包括9月2019的调整时间。

在这种情况下，您需要下载事务详细信息，以获得您的付款中包含的所有收益的完整视图。  此外，您还可以导航到 "付款" 视图以下载每个付款的交易。

### <a name="transaction-history"></a>交易历史记录

此视图按月显示收入和付款趋势，按状态显示收益和交易详细信息以及每个交易的付款状态。 数据仅对您是其激励用户或管理员的程序和 MPN Id 可见。

### <a name="payments"></a>支付

此视图允许查看所有程序和 MPN Id 的付款。 数据仅对您是其激励用户或管理员的程序和 MPN Id 可见。从此视图中，你可以下载汇款或按付款查看事务详细信息。

| 要执行此操作 | 请转到此处 |
| ------ | :----------- | 
| 按行查看付款信息，包括以本地货币表示的收入和付款金额  | 请参阅 **付款列表** 字段   |
| 下载信信   |  选择 **"付款付款"**  |
| 查看特定付款的事务级别详细信息 |  选择 **"视图"**  |
| 将事务详细信息导出到 Excel  |  选择 **"开始下载**"，然后选择"**导出数据"。** 所有选定的筛选器都将应用于导出的数据。 状态更改为"已完成"后，选择"下载"并按照提示导出详细的事务报告。 如果状态在 5 分钟内未更新，请刷新页面。  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>收益和付款缺失或不正确

如果找不到付款或交易详细信息，请检查是否已应用正确的筛选器。 由于某些计划名称 (例如，CSP 1T 直接合作伙伴现已CSP Direct Bill Partner) ，因此可能需要使用多个选择。

如果仍然找不到你的收益或认为显示的收入不正确，请联系 [支持部门](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="how-do-i-reconcile-my-earnings"></a>如何实现我的收入？

如果收益存在差异，请完成以下步骤：

1. 验证你是否符合获取收益的资格。  只有在满足计划资格和收益资格时，[](incentives-determined-your-program-eligibility.md)[才能获得收益](incentives-confirm-your-earnings-eligibility.md)。

2. 验证是否已完成你的付款配置文件。  奖励收益开始日期将是你满足所有资格要求（包括加入时需要填写付款和税务详细信息）的当月的第一天。 对于填写付款和税务信息之前的几个月，你将不会获得任何收益。 例如，如果你在 2020 年 4 月满足了所有要求，则收益开始日期为 2020 年 4 月 1 日。 

3. 验证你是否满足要求。  检查你是否满足奖励 [计划的资格](#my-payment-is-missing-or-incorrect) 和符合条件的收入规则。

如果这些操作没有帮助，并且你的收益仍未协调，请联系 [支持](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)部门。

## <a name="where-can-i-find-my-rates"></a>在哪里可以找到我的费率？

1. 登录到 [合作伙伴奖励](https://partner.microsoft.com/membership/partner-incentives)。

2. 向下滚动以访问程序的文档。

3. 选择相应程序的文档链接。

4. 在文档中，请参阅计划结构和 **费率部分**。

## <a name="next-steps"></a>后续步骤

- [管理合作声明](incentives-managing-co-op-claims.md)