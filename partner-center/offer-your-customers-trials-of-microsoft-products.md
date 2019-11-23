---
title: 为客户提供 Microsoft 产品试用版 | 合作伙伴中心
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 你的客户可以试用 Microsoft 订阅产品，为期 30 天。 You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384834"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>为客户提供 Microsoft 产品试用版

适用范围：

- 合作伙伴中心

向客户推荐 Microsoft 新产品的一种好方法是提供 30 天的免费试用版。 就像许多其他联机服务一样，你可以注册目录中的试用版。 所有合作伙伴都可以参与。

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. 例如，他们可以获取 Office 365 商业高级版的一个免费试用版和 Office 365 E3 的一个免费试用版。 However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

以下产品提供免费试用版：

- Office 365 商业高级版
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- 企业移动性和安全性 E5
- Dynamics 365 客户参与度计划 1
- Dynamics 365 for Financials
- Microsoft 365 商业版

我们提供这些产品的免费试用版，因为它们是最全面最热门的商业套餐。 将来，我们可能会增加其他套餐的免费试用版。

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. 进入目录，在**计费频率**中单击**试用版产品/服务**。 这将仅显示免费试用版，不显示其他非免费的产品/服务。 试用版将显示在目录中的**试用版**选项卡内。
3. 选择你想要提供的免费试用版，然后选择**提交**。 所有试用版的期限均为 30 天，在此期间不会向你收取费用。 你还可以在试用期内随时将其转换为付费订阅。

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. 转到客户的订阅页面，并选择免费试用版。
2. 选择 **Convert trial to paid subscription**。
3. 输入所需的许可证数量和计费频率，然后选择**应用**。
4. 付费订阅从转换日期开始计费，并且订阅从转换日期起 12 个月后自动续订。 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [将试用版订阅转换为付费版订阅](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [获取试用版转换产品/服务的列表](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. 最好经常监视这些日期以便在客户达到决策点时对其采取适当的后续行动。

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>计费

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. 如果免费试用版转换为采用按年计费的付费套餐，则订阅续订日期为自转换日期起 12 个月之后。 如果免费试用版转换为采用按月计费的付费套餐，则转换日期之后的计费日期过后 12 个月将为订阅续订日期。

### <a name="invoices"></a>发票

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>奖励

Free trials do not have an impact on incentives.

## <a name="support"></a>支持

For support on free trials, submit a service request through Partner Center.
