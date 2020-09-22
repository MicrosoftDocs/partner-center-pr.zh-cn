---
title: 为客户提供 Microsoft 产品的试用版
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 让客户试用 Microsoft 订阅产品30天。 在目录中注册这些免费试用，就像许多其他联机服务一样。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a51504a5e560f8a8041c448c3e5d9e7f0cfdae07
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999211"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>为客户授予为期30天的免费试用版 Microsoft 产品

**适用于**

- 合作伙伴中心

**相应的角色**
-   全局管理员 
-   用户管理员
-   销售代理

向客户推荐新 Microsoft 产品的一种好方法是提供 30 天的免费试用版。 就像许多其他联机服务一样，你可以注册目录中的试用版。 所有合作伙伴都可以参与。

## <a name="available-trial-offers"></a>可用试用优惠

可以在 **客户** 页上找到所有未完成的试用版产品/服务。 此页列出所有订阅，包括免费试用版和付费订阅。  (此功能目前在中国不可用。 ) 

每个客户都有权使用每个可用产品/服务的免费试用版。 例如，他们可以为 Microsoft 365 商业版标准版和 Office 365 E3 免费试用版获取一个免费试用版。 但是，如果客户已拥有该产品/服务，则不能使用该产品/服务的免费试用版。

### <a name="available-products"></a>可用产品

免费试用版适用于基于 licesen 的更为全面的产品/服务。 每月可能会引入新的试用版产品/服务。

合作伙伴可以在合作伙伴中心的 " **定价和优惠** " 页上找到每月价目表中的试用版。 试用版产品/服务的 "价目表" **辅助许可证类型** 列中列出了 "试用"。

目前，政府产品/服务、教育产品/服务或附加产品/服务没有 **免费试用** 版。

## <a name="licenses-for-free-trial-offers"></a>免费试用版许可证

所有免费试用版均提供25个许可证。 你无法在试用期间更改此数字。 不能在免费试用版中添加或删除许可证。 将试用版转换为付费订阅后，你可以向订阅添加其他许可证。

应将试用许可证分配给用户，方法与分配付费服务许可证的方式相同。

## <a name="sign-customers-up-for-trials"></a>为客户注册试用版

在合作伙伴中心获取客户的试用版：

1. 从合作伙伴中心 **销售** ，中转到 " **目录**"。 
2. 进入目录，在**计费频率**中单击**试用版产品/服务**。 这将仅显示免费试用版，不显示其他非免费的产品/服务。 试用版将显示在目录中的**试用版**选项卡内。
3. 选择你想要提供的免费试用版，然后选择**提交**。 所有试用版均为30天，在此期间不会计费。 你还可以在试用期内随时将其转换为付费订阅。

## <a name="converting-trials-to-paid-subscriptions"></a>将试用版转换为付费订阅

免费试用版不会自动转换为付费订阅。 三十天后，必须将免费试用版转换为付费订阅，否则它将 [过期](#expiring-offers)。 免费试用版无法扩展。

你需要自己将试用版转换为付费订阅。 可以 [使用合作伙伴中心](#convert-trials-using-partner-center) 或 [合作伙伴中心 api](#convert-trials-using-apis)来实现此目的。

> [!NOTE]
> 云解决方案提供商的免费试用版 (CSP) 程序不能转换为其他程序租户 (例如 EA、Open 或 MOSP) 。

### <a name="convert-trials-using-partner-center"></a>使用合作伙伴中心转换试用版

你可以使用合作伙伴中心将试用版转换为付费订阅：

1. 转到客户的订阅页面，并选择免费试用版。
2. 选择 **Convert trial to paid subscription**。
3. 输入所需的许可证数量和计费频率，然后选择**应用**。
4. 付费订阅的计费从转换日期开始，订阅从转换日期 autorenews 12 个月。 

### <a name="convert-trials-using-apis"></a>使用 Api 转换试验

可能需要更改 Api，以适应免费试用版到付费订阅的转换。 有关详细信息，请参阅以下开发人员文档：

- [将试用版订阅转换为付费版订阅](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [获取试用版转换产品/服务的列表](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>无转换的试验

并非所有试用都可以转换为付费订阅。 合作伙伴可以使用在到期日期之前没有转换的试用版。 合作伙伴可以购买支持与试用产品/服务相同的服务的兼容产品/服务。  此操作应在试用版到期之前完成，以确保新购买的产品/服务与试用版服务保持一致。 

|**试用**   |**兼容的小型企业产品**   |**兼容的企业产品**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft 团队商业云 (用户启动) 试用版   |Microsoft 365 商业版基本、Microsoft 365 商业版标准 Microsoft 365 商业版高级   | F3 (以前的 F1) ，Office 365 for Enterprise (E1、E3 和 E5) 、M365 F1/F3、M365 Enterprise (E3)    |

>[!NOTE]
>上述产品/服务具有类似功能的类似服务计划，但产品/服务之间可能存在一些差异。

### <a name="expiring-offers"></a>即将过期

将不会向你通知即将过期的产品/服务。 您可以使用合作伙伴中心的客户视图或通过查询 API 来跟踪即将到期的到期日期。 最好经常监视这些日期以便在客户达到决策点时对其采取适当的后续行动。

试用期到期后，尝试登录该试用版的客户将看到过期消息。 但数据存储在数据保留标准的行中。 在使用相同的服务计划购买新订阅后，可以再次从新激活的订阅访问客户信息。

## <a name="billing"></a>计费

在主权云和公有云中，年度计费和免费试用版是相同的。 唯一的区别是在启动时可以使用试用 Sku。

## <a name="billing-for-free-trials"></a>免费试用计费

免费试用版可用于每月和每年计费订阅。 将试用版转换为付费订阅时，可以选择计费频率。

订阅开始日期基于转换日期。 如果免费试用版转换为采用按年计费的付费套餐，则订阅续订日期为自转换日期起 12 个月之后。 如果免费试用版转换为采用按月计费的付费套餐，则转换日期之后的计费日期过后 12 个月将为订阅续订日期。

### <a name="invoices"></a>发票

你不会看到在发票或基于许可证的对帐文件中列出的免费试用版。 仅在将免费试用版转换为付费订阅后，才会在发票和基于许可证的对帐文件中显示免费试用版。 转换后的订阅将以与任何新订阅相同的方式出现。

### <a name="incentives"></a>奖励

免费试用不会对激励产生影响。

## <a name="support"></a>支持

如要免费试用，请通过合作伙伴中心提交服务请求。