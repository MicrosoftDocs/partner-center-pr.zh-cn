---
title: 将 Dynamics 365 和 Customer Engagement 计划从 Basic （限定产品/服务） 迁移到较新版本 |合作伙伴中心
ms.topic: article
ms.date: 12/12/2018
description: 为销售的 Dynamics 365 Customer Engagement 计划从 Basic （限定提供） 的订阅不能再续订 /。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 产品/服务，续订产品/服务，新的 Dynamics 365 Sku
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134397"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本

**适用于**

-  合作伙伴中心

有效 2019 年 1 月 1 日，客户与销售的 Dynamics 365 Customer Engagement 计划从 Basic （限定提供） 的订阅无法再续订这些旧的产品/服务; /过期时，将不自动续订现有订阅。 在订阅的详细信息页上，订阅状态将从"自动续订于 [date]"更改为"过期日期 [date]"。 


若要为客户确保连续性，应转换那些与受支持的选项，下面列出的即将过期订阅。 建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。

如果使用 API （CREST 或合作伙伴中心），可以找到通过计算结束日期以及自动订阅的过期订阅续订 = False 属性。 相关的订阅将设置为自动续订在 2019 年 1 月 1 日 = False。 你可以随时将客户移到新计划中。 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 提供了即将停用

- Dynamics 365 for 销售 Enterprise Edition CRMOL 基本 （限定产品/服务）
- Dynamics 365 for 教职员工版的销售 Enterprise Edition CRMOL 基本 （限定产品/服务）
- Dynamics 365 for 面向学生的销售 Enterprise Edition CRMOL 基本 （限定产品/服务）
- Dynamics 365 for 销售企业版 （政府定价） CRMOL 基本 （限定产品/服务）
- Dynamics 365 适用于销售的 Enterprise Edition 来自 SA 的 CRM Basic （限定产品/服务）
- Dynamics 365 适用于销售的 Enterprise Edition 来自 SA 的 CRM Basic 教职员工版 （限定产品/服务）
- Dynamics 365 适用于销售的 Enterprise Edition 来自 SA 的 CRM Basic 学生版 （限定产品/服务）
- Dynamics 365 的销售企业版 （政府定价） 来自 SA 的 CRM Basic （限定产品/服务）
- Dynamics 365 的销售企业版外接程序的 CRM Basic （限定产品/服务）
- Dynamics 365 的销售企业版外接程序的 CRM Basic 教职员工版 （限定产品/服务）
- Dynamics 365 的销售企业版外接程序适用于面向学生的 CRM Basic （限定产品/服务）
- Dynamics 365 的销售企业版 （政府定价） 外接程序的 CRM Basic （限定产品/服务）
- Dynamics 365 客户参与计划企业版 CRMOL Basic （限定产品/服务）
- Dynamics 365 客户参与计划企业版 （政府定价） CRMOL Basic （限定产品/服务）
- Dynamics 365 客户参与计划企业版 CRMOL Basic （限定产品/服务） 学生版
- Dynamics 365 客户参与计划企业版 CRMOL Basic （限定产品/服务） 教职员工版
- 来自 SA 的 CRM Basic （限定产品/服务） 的 Dynamics 365 客户参与计划企业版
- Dynamics 365 客户参与计划企业版 （政府定价） 来自 SA 的 CRM Basic （限定产品/服务）
- 从面向学生的 CRM Basic （限定产品/服务） 的 SA 的 Dynamics 365 客户参与计划企业版
- 来自 SA 的 CRM Basic 教职员工版 （限定产品/服务） 的 Dynamics 365 客户参与计划企业版
- Dynamics 365 客户参与计划企业版外接程序的 CRM Basic （限定产品/服务）
- Dynamics 365 客户参与计划企业版 （政府定价） 的外接程序 CRM Basic （限定产品/服务）
- Dynamics 365 客户参与计划企业版外接程序适用于面向学生的 CRM Basic （限定产品/服务）
- Dynamics 365 客户参与计划企业版外接程序的 CRM Basic 教职员工版 （限定产品/服务）



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>为销售的 Dynamics 365 Customer Engagement 计划从 Basic （限定提供） 替换计划 /

**已停用的产品/服务**   

- 从 CRM Basic 或 CRMOL Basic （限定产品/服务） 销售的 Dynamics 365
- Dynamics 365 客户参与计划从 CRM Basic 或 CRMOL Basic （限定产品/服务）

**替换选项**
- Dynamics 365 for Sales 专业版 （新）
- Dynamics 365 for Sales 专业版 （新）
- Dynamics 365 for Customer Service
- Dynamics 365 客户参与计划或
- Dynamics 365 团队成员



## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

将客户从已停用 Sku 移动到较新的需要按以下顺序执行以下步骤：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

## <a name="purchase-the-new-plan-for-your-customer"></a>为您的客户购买新的计划

1. 选择**客户**从左侧导航栏，然后选择你想要将移动到新订阅的客户。
2. 选择**添加订阅**。
3. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。 

您的客户现在将在旧订阅并新建一个。 下一步是重新分配给客户的用户的许可证。

1. 选择**客户**从左侧导航栏，然后选择客户正在移动。
2. 选择**用户和许可证**。
3. 若要重新分配给用户的许可证，选择用户，然后选择**管理许可证**。 
4. 上**管理许可证**页上，清除销售 Dynamics 365 / Basic （限定产品/服务） 中的客户参与计划许可证复选框，然后选择订阅客户移动到新的服务计划。 
5. 选择“提交”。 将为每个用户都需要新许可证来执行此操作。 

一旦您已将的许可证移到新的订阅可以取消旧订阅。 

1. 选择**客户**从左侧导航栏，然后选择客户正在移动。
2. 在订阅详细信息页上，将旧的订阅设置为**Suspended** ，然后选择**提交**。

旧订阅现在已挂起，但新订阅处于活动状态。 暂停的订阅在 120 天后将自动取消预配。 您的客户将产生在旧订阅无额外成本。
 

 



