---
title: 了解在合作伙伴中心计费的类型 |合作伙伴中心
ms.topic: article
ms.date: 03/01/2019
Description: 有关不同计费类型、 计费句点和计费日期
author: labrenne
ms.author: labrenne
keywords: 计费，付款，订单，对帐文件，对帐文件
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 777a98f8780eb036b4bac99eca9a5621d61da66b
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122286"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>了解在合作伙伴中心计费的类型

**适用范围**

-  合作伙伴中心
-  云解决方案提供商计划中的合作伙伴

具体取决于你的客户购买的产品的类型，你可能有不同的帐单期间和计费的相同月份的不同天。 本文介绍了有何变化开始 2019 年 3 月 1 日，以及所做的更改将影响你。

## <a name="billing-for-recurring-charges"></a>计费定期费用

没有变化的基于许可证和基于使用情况的订阅的定期费用的帐单体验。 我们将继续向你计费在每个月你选择作为你的计费日期，日期和计费周期将继续在该日期之前个月。 如果你选择你的计费日期的月份的第 15 日，将从一个日历月的 15 日到下一个日历月 14 的所有活动向你计费。 发票和对帐文件，则你的计费日期后的公开发布 2-4 天。

如之前，我们将向您的这些产品中正在位于国家/地区的货币，无论客户的位置情况下你销售该产品。

## <a name="billing-for-one-time-and-select-recurring-charges"></a>计费一次性和选择定期费用

我们从开始 2019 年 3 月 1 日，Microsoft 和第三方 ISV 产品引入新计费体验的定期和一次性费用。

对于这些产品，在计费周期开始日历月的第一天，最后一天的日历月份的结束。 我们将使你的发票可在下个月的第 8 天。 

换句话说，任何交易记录使之间 5 月 1 和 2019 年 5 月 31 日，将显示在你的发票上 6 月 8 日。 6 月 1 日和 2019 年 6 月 30 日之间进行任何交易记录将出现在你的发票 7 月 8 日。 可能会定期和一次性购买同一发票上获取向你计费。 

每当你希望 （例如，之间月 1 到 6 月 7 日） 并查看最新的帐户活动，而无需等待发票，你也可以检查你的帐户余额/帐单。 请注意，发布你的帐单后上 8，它将包括税款和任何其他适用的费用和信用额度，因此最终金额可能不同于期间计费周期内看到的内容。 

您可以访问你的发票现在，在合作伙伴中心或通过 API 执行相同的方式。 他们将出现在午夜 UTC 上个月的第 8 天之前。 

|**计费体验**|**产品类型**|**计费日期**|**计费周期**|**计费货币**|**可用的当前活动？**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|基于许可证和基于使用情况的订阅的定期费用 |[联机服务目录](https://partner.microsoft.com/commerce/preferredoffers/list)中的所有产品。 示例包括 Office 365、 Microsoft 365、 Azure Active Directory、 Azure （即付即用）、 Dynamics 365、 PowerBI Pro |创建合作伙伴中心帐户时所选日期 |在你的计费日期之前月份。 |你将位于国家/地区的货币。 例如，如果你的公司位于英国，我们将向您英国英磅 (GBP) 中。 如果你的公司位于印度中，我们将向你计费在印度卢比 (INR)。  |否 |
|Microsoft 和第三方 Isv 产品的定期和一次性费用 |所有 SaaS 订阅、 Azure 预订和 Microsoft 和第三方 Isv 提供的软件 （永久和基于订阅的） 产品。 请参阅在[市场](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)中的可用产品。 示例包括 SUSE Linux 软件 （软件订阅），Windows Server 2019 Essentials （永久软件），Azure ISV SaaS 产品订阅。 |每个月的第 8 天 |从每个日历月的最后一天的第一天 |你的客户位于国家/地区的货币。 这意味着你将收到单独发票和对帐文件中的国家/地区的货币每个计费周期内销售给客户。 |是 |
