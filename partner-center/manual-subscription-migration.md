---
title: 迁移合格的 Dynamics 365 订阅
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在现有订阅过期之前从合格的基本 Dynamics 365 订阅迁移到新的订阅。
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151638"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本

**适当的角色**：全局管理员 |用户管理管理员 |管理代理 |销售代理

从2019年1月1日起生效，对于来自基本 (合格产品/服务的销售/客户参与计划的365客户，) 订阅不能再续订这些旧产品/服务。现有订阅将不会在过期时自动续订。 在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。 

若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。 建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。

如果 ("CREST" 或 "合作伙伴中心") 使用 API，则可以通过使用 "自动续订 = False" 属性来评估订阅的结束日期，找到过期订阅。 相关订阅将在2019年1月1日设置为自动续订 = False。 你可以随时将客户移到新计划中。 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 产品/服务已停用

- Dynamics 365 for Sales Enterprise Edition CRMOL 基本 (合格提议) 
- 适用于 Sales Enterprise Edition 的 Dynamics 365 CRMOL Basic (限定提议) 教职员
- 适用于 Sales Enterprise Edition 的 Dynamics 365 CRMOL Basic (合格提议) 学生
- Dynamics 365 for Sales Enterprise Edition (政府定价) CRMOL 基本 (合格产品/服务) 
- 来自 SA for CRM Basic (合格的产品/服务的 Dynamics 365 for Sales Enterprise Edition) 
- 用于 CRM Basic (合格产品/) 服务的 SA 的 Dynamics 365 for Sales Enterprise Edition
- 适用于适用于 CRM 的 SA 的 Dynamics 365 for Sales Enterprise Edition (合格的产品/服务) 学生
- 适用于 Sales Enterprise Edition 的 Dynamics 365 (政府定价) ，适用于 CRM 基本 (合格产品/服务) 
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (符合条件的产品/) 
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (符合条件的产品/) 教职员工
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (符合条件的产品/) 学生版
- DYNAMICs 365 for Sales Enterprise Edition (政府定价) Add-On CRM Basic (符合条件的产品/) 
- Dynamics 365 客户参与计划Enterprise Edition CRMOL Basic (符合条件的套餐) 
- Dynamics 365 客户参与计划Enterprise Edition (政府定价) CRMOL Basic (符合条件的套餐) 
- Dynamics 365 客户参与计划 Enterprise Edition CRMOL Basic (学生) 符合条件的产品/服务
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for 教职员工
- Dynamics 365 客户参与计划 Enterprise Edition SA for CRM Basic (符合条件的产品/服务) 
- Dynamics 365 客户参与计划Enterprise Edition (政府定价) 来自 SA for CRM Basic (符合条件的套餐) 
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 客户参与计划 Enterprise Edition SA for CRM Basic (符合条件的产品/服务) 教职员工
- Dynamics 365 客户参与计划Enterprise Edition Add-On CRM Basic (符合条件的套餐) 
- Dynamics 365 客户参与计划Enterprise Edition (CRM Basic) Add-On符合条件的产品/服务 (政府定价) 
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offers) 替换计划

**已停用的优惠**   

- CRM Basic 或 CRMOL Basic 中的 Dynamics 365 for Sales (符合条件的产品/服务) 
- CRM Basic 或 CRMOL Basic 中的 Dynamics 365 客户参与计划 (符合条件的套餐) 

**替换选项**
- Dynamics 365 for Sales Professional (NEW) 
- Dynamics 365 for Sales Professional (NEW) 
- Dynamics 365 for Customer Service
- Dynamics 365 客户参与计划或
- Dynamics 365 团队成员



## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

将客户从已停用的 SKUS 迁移到较新的 SKUS 需要按以下顺序执行以下步骤：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

## <a name="purchase-the-new-plan-for-your-customer"></a>为客户购买新计划

1. 从 **左侧** 导航中选择"客户"，然后选择要移动到新订阅的客户。
2. 选择"**添加订阅"。**
3. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。 

现在，你的客户将同时拥有旧订阅和新订阅。 下一步是为客户的用户重新分配许可证。

1. 从 **左侧** 导航中选择"客户"，然后选择要移动的客户。
2. 选择 **"用户和许可证"。**
3. 若要向用户重新分配许可证，请选择该用户，然后选择"**管理许可证"。** 
4. 在"管理许可证"页上，清除"基本 (合格产品/服务) 许可证"复选框中的"Dynamics 365 for Sales/Customer Engagement 计划"复选框，并选择客户要移动到的订阅的新服务计划。 
5. 选择“提交”。 你将为需要新许可证的每个用户执行此操作。 

将许可证移到新订阅后，可以取消旧订阅。 

1. 从 **左侧** 导航中选择"客户"，然后选择要移动的客户。
2. 在订阅详细信息页上，将旧订阅设置为"已挂起 **"，** 然后选择"提交 **"。**

旧订阅现已暂停，新订阅处于活动状态。 暂停的订阅在 120 天后将自动取消预配。 对于旧订阅，客户不会产生额外的费用。
 

 



