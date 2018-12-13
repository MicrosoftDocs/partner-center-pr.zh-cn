---
title: 迁移到较新版本的 Dynamics 365 企业版产品/服务 |合作伙伴中心
ms.topic: article
ms.date: 12/12/2018
description: 可以不再续订 Dynamics 365 企业版订阅。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: 11f0d9262856d28adb4d67871503d86f2d4945ac
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968278"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>迁移到较新版本的 Dynamics 365 企业版产品/服务 

**适用范围**

- 合作伙伴中心

Dynamics 365 企业版订阅有效于 2019 年 1 月 1 日，客户可以不再续订这些旧的产品/服务。当它们到期时，现有订阅将不会自动续订。 订阅的详细信息页面上的订阅状态将从"自动续订 [日期]"更改为"[日期] 过期"。

若要确保客户服务连续性，你应该过渡那些到支持的选项，下面列出的订阅快过期。 建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。

如果你使用 API （CREST 或合作伙伴中心），你可以找到通过评估以及自动订阅的结束日期即将到期订阅续订 = False 属性。 问题的订阅将设置为自动续订 = False 于 2019 年 1 月 1 日。 你可以随时将客户移到新计划中。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>被停用的 Dynamics 365 企业版

- Dynamics 365 Finance and Operations 企业版的
- Dynamics 365 for Team Members、 企业版

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics 业务中央-Dynamics 365 企业版的新产品/服务

使用新的 Dynamics 业务中央产品/服务，你的客户可以连接其 financials、 销售、 服务和操作来优化业务流程，提高客户交互，并使更好的决策。 Dynamics 365 业务中心是基于云的和可通过云解决方案提供商 (CSP) 计划合作伙伴。
Dynamics 365 企业版客户有资格获得新的业务中央打折的过渡定价提供直到于 2020 年 6 月 30 日。

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

 从已停用的 Sku 的客户移动到较新的需要按此顺序执行以下步骤：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

## <a name="purchase-the-new-plan-for-your-customer"></a>为客户购买新计划

1. 从左侧导航中选择**客户**，然后选择你想要移动到新订阅的客户。
2. 选择**添加订阅**。
3. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。 

你的客户现在将具有旧订阅和新。 下一步是许可证重新分配到客户的用户。

1. 从左侧导航中选择**客户**，然后选择你要移动的客户。
2. 选择**用户和许可证**。
3. 若要重新分配用户许可证，选择用户，然后选择**管理许可证**。 
4. 在**管理许可证**页上，清除 Dynamics 365 for Sales/从基本 （限定产品/服务） 的客户参与度计划许可证复选框，然后选择客户要迁移到的订阅的新服务计划。 
5. 选择**提交**。 将每个用户都需要新许可证来执行此操作。 

你已移许可证的新订阅后您可以取消旧订阅。 

1. 从左侧导航中选择**客户**，然后选择你要移动的客户。
2. 在订阅详细信息页上，设置为**已暂停**的旧订阅，并选择**提交**。

旧订阅现在暂停，并且新订阅处于活动状态。 暂停的订阅在 120 天后将自动取消预配。 你的客户将产生的旧订阅任何额外成本。