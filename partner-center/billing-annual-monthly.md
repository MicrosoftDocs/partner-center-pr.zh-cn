---
title: Monthly and annual billing differences | Partner Center
ms.topic: article
ms.date: 11/21/2019
Description: Differences between monthly and annual billing cycles in Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 4d6b316f55a6d2cd84959d60feed666d657893b8
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389765"
---
# <a name="monthly-and-annual-billing-differences"></a>Monthly and annual billing differences

适用范围：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

This topic explains the differences between **monthly billing** and **annual billing** in Partner Center, including benefits and use cases. You have the option to pay for certain Cloud Solution Provider (CSP) subscriptions on a monthly or annual basis.

## <a name="applicability"></a>适用性

Most licensed-based subscriptions have the option for either monthly or annual billing option. 基于使用情况的订阅只有按月计费选项。

Both annual and monthly billing are **per subscription**, ***not* per license**.

### <a name="find-subscription-applicability"></a>Find subscription applicability

You can identify the available billing frequencies for each offer by using column J in the offer matrix. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="applicable-partners"></a>Applicable partners

All partners and partner types can choose monthly or annual billing.

### <a name="applicable-markets"></a>Applicable markets

Monthly and annual billing (for applicable offers) are available in all markets where the CSP program is currently available.

## <a name="change-billing-frequency"></a>Change billing frequency

You can switch between monthly and annual billing at any time. You may want to change your billing frequency if your business needs change.

When you change the billing frequency to annual, the annual term is updated to reflect the date you changed the billing frequency. A new renewal date is also established.

### <a name="monthly-to-annual-billing"></a>Monthly to annual billing

Switching from monthly billing to annual billing may be useful if you have numerous subscriptions that are billed monthly. When you switch to annual billing, you can align the subscriptions to a common billing date.

### <a name="annual-to-monthly-billing"></a>Annual to monthly billing

Switching from annual billing to monthly billing may be useful if you want to adjust your billing dates to those of your individual customers.

## <a name="annual-billing"></a>Annual billing

按年计费具有以下好处：

- 增加了支付选项的灵活性。
- 与客户的开票方式更好地保持一致。
- 降低了货币波动的影响。
- 减少了计费运营成本。

### <a name="configure-annual-billing"></a>Configure annual billing

If you're planning to switch to annual billing in Partner Center, be sure to consider how your sales motion will be affected. You should inform your team and update your internal processes as necessary. You should also review changes to your invoice and license-based reconciliation file. 

You will also need to [update your APIs for annual billing](#required-api-changes).

#### <a name="required-api-changes"></a>Required API changes

为了利用按年计费，需要对你的 API 进行一些更改。

- [Order.BillingCycle property](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Create an order](https://docs.microsoft.com/partner-center/develop/create-an-order)

For more information about Partner Center APIs, see all [Partner Center developer resources and documentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placing orders

The billing frequency type, including the annual billing option, is assigned to the **Offer** as an attribute. There is not a unique offer specifically for orders with annual billing. 但是，你可以使用对客户更友好的名称重命名套餐以进行区分。

### <a name="select-annual-billing"></a>Select annual billing

When you add a new subscription, you will be prompted to choose the billing frequency. 可以在此时选择按年计费选项。 When you select annual billing,all available offers will be displayed.

### <a name="billing-time"></a>Billing time

将在下一个计费日期向你收费。 For example, if your billing date is the 1st of the month and you purchase an annually billed subscription on October 29, 2019, you will be billed on November 1, 2019. Assuming that you make no license changes, you will be billed again on November 1, 2020. If you make a license change you will receive a credit and rebill on your next billing date.

### <a name="annual-renewals"></a>Annual renewals

Your subscription renewal date will be twelve months after the service start date. 服务期从订阅创建之日起开始。  For example, a subscription created on January 10, 2019, will be renewed on January 10, 2020.

将在订阅续订日期之后的下一计费日期向你计费。 例如，如果你在 2018 年 1 月 15 日购买了按年计费订阅，并且计费日期是 1 月 20 日，则订阅续订日期将为 2019 年 1 月 15 日。 将在 2019 年 1 月 20 日针对续订向你计费。

### <a name="split-subscription-billing-frequency"></a>Split subscription billing frequency

It isn't possible to split a **single subscription** so that one part is billed monthly and the other part is billed annually. The entire subscription must have the same billing frequency (either monthly or annual billing).

For customers with **multiple subscriptions** of the same offer, it may be possible to have different billing frequencies per subscription. 对于某些套餐，每个客户仅限拥有一份订阅。 如果套餐不受限制，则每个客户可以拥有相同套餐的多份计费频率不同的订阅。 可以在套餐矩阵的 I 列查找所有套餐限制的详细信息。 You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="free-subscription-period"></a>Free subscription period

Subscriptions with annual billing frequency do not receive a free period. The twelve-month paid term begins on the purchase date. 这不同于采用按月计费频率的订阅，采用按月计费频率的订阅会获得一个从购买日期到下一个计费日期的免费时段。

### <a name="adding-and-removing-licenses"></a>Adding and removing licenses

可以随时更改订阅的许可证数量。 添加其他许可证不会影响计费频率。

可以随时添加或删除许可证。  You will receive a credit and prorated rebill on your next billing date after you change the number of licenses.

If your existing subscription has annual billing, it's not possible to add licenses with monthly billing to that subscription. 购买采用按年计费的订阅之后，任何附加许可证将采用相同的计费频率。 如果以后需要购买采用按月计费的许可证，你将需要购买新的订阅。

### <a name="add-on-offers"></a>Add-on offers

附加订阅将自动采用与父订阅相同的计费频率。 Annual billing is available for add-on offers. 

### <a name="cancelling-subscriptions"></a>Cancelling subscriptions

所有计费频率的取消策略都相同。

For annual billing, if the subscription is cancelled in the first 30 days of the twelve-month paid term you will receive a 100 percent credit on your next billing date. If the subscription is cancelled after 30 days of the twelve-month paid term you will receive a prorated credit on your next billing date.

### <a name="moving-subscriptions-between-partners"></a>Moving subscriptions between partners

Customers can't move subscriptions between from one partner to another. 这适用于按月和按年计费订阅。

新合作伙伴必须代表客户购买新的订阅。 It's not possible to move subscriptions between partners.

### <a name="reactivating-subscriptions"></a>Reactivating subscriptions

You can reactivate a subscription for up to 90 days after the suspension date. 你将在下一个计费日期收到按比例计算的费用。 订阅续订日期保持不变。

## <a name="pricing"></a>定价

### <a name="offer-pricing"></a>Offer pricing

The offer price at time of purchase is guaranteed for the full billed subscription term (one month for monthly billing, twelve months for annual billing). 续订订阅时，价格将基于续订日期的当前价目表。 The new price is guaranteed for the next subscription term.

If an offer price decreases during the billing period, the amount you are billed for doesn't change. The price is set for the full billing period at the time of purchase. This applies to both monthly and annual billing.

### <a name="cancellation-credits"></a>Cancellation credits

Credit for a cancelled license or subscription is calculated as follows:

**Cancellation credit** = ((**monthly price***12)/365) \* **days remaining in the twelve-month term** \* number of licenses cancelled.

## <a name="reconciliation-file"></a>Reconciliation file

### <a name="find-subscriptions-billing-frequency"></a>Find subscription's billing frequency

Review your license-based reconciliation file for information on whether your subscription is billed monthly or annually. This information is in column **AA**.

To find out whether you can change a monthly subscription to annual billing, see [Find subscription applicability](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Reconciliation file changes for annual billing

When you purchase or renew a subscription with annual billing, your license-based reconciliation file will change as follows.

A new row on the license-based reconciliation file on the first billing date following the purchase or a new subscription.

未对订阅进行任何更改，则订阅期限的 2 至 12 个月的对帐文件上将不会显示任何行。 If a change is made to the subscription during the twelve-month term, a credit and prorated rebill will appear on the next reconciliation file after the change is made.

The next change to the reconciliation file will appear when the subscription is renewed. 这将在续订后的第一个计费日期显示。

### <a name="usage-file-changes-for-annual-billing"></a>Usage file changes for annual billing

The following annually billed subscription changes appear in column P of your usage file.

- **Prorate Fees When Purchase**: the initial purchase of an annual subscription.
- **Cycle Instance Prorate**: license changes that result in credit and rebilling.
- **Cancel Fee**: the [cancellation of an annual subscription](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancellation of annual subscription

When an annually billed subscription is cancelled, the reconciliation file will contain one line item for a cancellation credit.

If the cancellation occurs in the first 30 days of the twelve-month term, the subscription will be credited at 100 percent. 如果取消发生在前 30 天后，则将按比例对订阅进行退款。

### <a name="adding-licenses-to-annual-subscription"></a>Adding licenses to annual subscription

When you add licenses to a subscription, the reconciliation file will contain a credit and prorated rebill. This applies to monthly and annually billed subscriptions.

### <a name="price-lists-for-annual-billing"></a>Price lists for annual billing

Partner Center price lists show the monthly prices. There is no annual price listed. 可以将每月价格乘以 12 计算出年度价格。

### <a name="offer-matrix"></a>Offer matrix

Offer IDs in the offer matrix are the same for all billing frequencies. There are no unique IDs for offers that can be billed annually.

## <a name="incentives"></a>奖励

### <a name="incentives-calculation"></a>Incentives calculation

Incentives are calculated based on **billed revenue**, ***not* adjusted revenue**. 赚取的奖励付款将按照我们的云解决方案提供商奖励指南中的政策到帐。

When an annually billed subscription is sold, that subscription's revenue is recognized for the calculation of incentives based on billed revenue.

### <a name="payout"></a>付款

Currently, all incentive payments are made twice a year. 这些付款在半年期结束后 45 天内完成。

### <a name="rates"></a>资费

Partners earn incentives on all eligible transactions, regardless of how a subscription is billed. Incentive earnings are calculated based on the global incentive rate (which is applied to the billed revenue for the period), the local accelerator (for all geographies in which there are local accelerators), and any global campaigns (where applicable).

### <a name="contacts"></a>联系人

For questions about incentives, contact the appropriate regional incentives support team:

| Region | Email address |
| ------ | ------------- |
| 北美 | <ocina@microsoft.com> |
|Latin America & Brazil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excluding Japan) | <ociapgc@microsoft.com> |
| 日本 | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspension

If you suspend an subscription (in Partner Center or through the APIs) within 30 days of purchase, you will receive a 100% credit, regardless of billing frequency.

For annual billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to December 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to December 31st.
3. The reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to December 31st.

For monthly billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to January 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to January 31st.
3. The partner reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to January 31st.
