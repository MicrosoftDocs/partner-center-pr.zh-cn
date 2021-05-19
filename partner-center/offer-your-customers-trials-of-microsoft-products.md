---
title: 为客户提供 Microsoft 产品的试用版
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 让客户试用 Microsoft 订阅产品 30 天。 在目录中注册这些免费试用版，就像注册许多其他联机服务。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151128"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>为客户提供 30 天免费 Microsoft 产品试用版

**适当的角色**：全局管理员|用户管理管理员|销售代理

向客户推荐新 Microsoft 产品的一种好方法是提供 30 天的免费试用版。 就像许多其他联机服务一样，你可以注册目录中的试用版。 所有合作伙伴都可以参与。

## <a name="available-trial-offers"></a>可用的试用版产品/服务

可以在"客户"页上找到所有未完成的 **试用** 产品/服务。 此页列出所有订阅，包括免费试用版和付费订阅。  (此功能目前在中国.) 

每个客户都有权针对每个可用产品/服务获得一个免费试用版。 例如，他们可以获得一个适用于 Microsoft 365 Business Standard 的免费试用版和一个 Office 365 E3 免费试用版。 但是，如果客户已拥有该产品/服务，则他们无法使用该产品/服务的免费试用版。

### <a name="available-products"></a>可用产品

免费试用版适用于最全面、最热门的基于 licesen 的优惠。 新的试用版产品/服务可能每月推出一次。

合作伙伴可以在定价和产品/服务页的每月价目表中查找合作伙伴中心。 试用版产品/服务将在价目表"辅助许可证类型"列中 **列出"TRIAL"。**

目前， **政府产品/服务、** 教育产品/服务或附加产品/服务没有免费试用版。

## <a name="licenses-for-free-trial-offers"></a>免费试用版产品/服务许可证

所有免费试用版提供 25 个许可证。 试用期间不能更改此号码。 不能在免费试用版中添加或删除许可证。 将试用版转换为付费订阅后，你可以向订阅添加更多许可证。

应将试用许可证分配给用户，方法与分配付费服务许可证的方式相同。

## <a name="sign-customers-up-for-trials"></a>为客户注册试用版

在合作伙伴中心获取客户的试用版：

1. 从合作伙伴中心 **销售** ，中转到 " **目录**"。 
2. 在目录中的 " **计费频率**" 下，选择 " **试用产品/服务**"。 这将仅显示免费试用版，不显示其他非免费的产品/服务。 试用版将显示在目录中的 **试用版** 选项卡内。
3. 选择你想要提供的免费试用版，然后选择 **提交**。 所有试用版的期限均为 30 天，在此期间不会向你收取费用。 你还可以在试用期内随时将其转换为付费订阅。

## <a name="converting-trials-to-paid-subscriptions"></a>将试用版转换为付费订阅

免费试用版不会自动转换为付费订阅。 30天后，必须将免费试用版转换为付费订阅，否则它将 [过期](#expiring-offers)。 免费试用版无法扩展。

你需要自己将试用版转换为付费订阅。 可以 [使用合作伙伴中心](#convert-trials-using-partner-center) 或 [合作伙伴中心 api](#convert-trials-using-apis)来实现此目的。

> [!NOTE]
> 云解决方案提供商的免费试用版 (CSP) 程序不能转换为其他程序租户 (例如 EA、Open 或 MOSP) 。

### <a name="convert-trials-using-partner-center"></a>使用合作伙伴中心转换试用版

你可以使用合作伙伴中心将试用版转换为付费订阅：

1. 转到客户的订阅页面，并选择免费试用版。
2. 选择 **Convert trial to paid subscription**。
3. 输入所需的许可证数量和计费频率，然后选择 **应用**。
4. 付费订阅的计费从转换日期开始，订阅将从转换日期自动续订12个月。 

### <a name="convert-trials-using-apis"></a>使用 Api 转换试验

可能需要更改 Api，以适应免费试用版到付费订阅的转换。 有关详细信息，请参阅以下开发人员文档：

- [将试用版订阅转换为付费版订阅](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [获取试用版转换产品/服务的列表](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>不带转换的试用

并非所有试用版都可以转换为付费订阅。 合作伙伴可以使用在到期日期之前没有转换的试用版。 合作伙伴可以购买支持与试用产品/服务相同的服务的兼容产品/服务。  应在试用版过期之前完成此操作，以确保新购买的产品/服务与试用版服务保持一致。 

|**试用**   |**兼容的小型企业产品/服务**   |**兼容的企业产品/服务**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams 商业云 (用户发起的) 试用版   |Microsoft 365 Business Basic、Microsoft 365 Business Standard、Microsoft 365 Business Premium   | F3 (F1) 、Office 365 for Enterprise (E1、E3 和 E5) 、Microsoft 365 F1/F3、Microsoft 365 企业版 (E3)    |

>[!NOTE]
>上述套餐具有类似的服务计划以及类似的功能，但产品/服务之间可能有一些差异。

### <a name="expiring-offers"></a>即将过期的优惠

你将不会收到即将过期产品/服务的通知。 可以使用客户视图在 合作伙伴中心或查询 API 来跟踪即将过期的日期。 最好经常监视这些日期以便在客户达到决策点时对其采取适当的后续行动。

试用过期后，尝试登录到该试用版的客户将看到过期消息。 但是，数据存储符合数据保留标准。 购买具有相同服务计划的新订阅后，可以从新激活的订阅再次访问客户的信息。

## <a name="billing"></a>计费

主权云和公有云中的按年计费和免费试用是相同的。 唯一的区别是在启动时可用的试用 SKUS。

## <a name="billing-for-free-trials"></a>免费试用版计费

免费试用版可用于每月和每年计费订阅。 将试用版转换为付费订阅时，可以选择计费频率。

订阅开始日期基于转换日期。 如果免费试用版转换为付费产品/服务，则订阅续订日期将为转换日期12个月。 如果免费试用版转换为采用按月计费的付费套餐，则转换日期之后的计费日期过后 12 个月将为订阅续订日期。

### <a name="invoices"></a>发票

你不会看到在发票或基于许可证的对帐文件中列出的免费试用版。 仅在将免费试用版转换为付费订阅后，才会在发票和基于许可证的对帐文件中显示免费试用版。 转换后的订阅将以与任何新订阅相同的方式出现。

### <a name="incentives"></a>奖励

免费试用不会对激励产生影响。

## <a name="support"></a>支持

如要免费试用，请通过合作伙伴中心提交服务请求。