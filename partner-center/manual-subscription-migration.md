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
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132734"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本

**相应的角色**

- 全局管理员
- “用户管理”管理员
- 管理员代理
- 销售代理

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
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (合格提议) 
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (合格提议) 教职员
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (合格提议) 学生
- Dynamics 365 for Sales Enterprise Edition (政府定价) Add-On，适用于 CRM 基本 (合格提议) 
- Dynamics 365 客户参与计划企业版 CRMOL 基本 (合格提议) 
- Dynamics 365 客户参与计划 Enterprise Edition (政府定价) CRMOL 基本 (合格产品/服务) 
- Dynamics 365 客户参与计划企业版 CRMOL 基本 (合格提议) 学生
- Dynamics 365 客户参与计划企业版 CRMOL 基本 (合格提议) 教职员
- Dynamics 365 的客户参与计划企业版（来自 SA for CRM Basic (合格的产品/服务）) 
- Dynamics 365 客户参与计划 Enterprise Edition (政府定价) 来自 SA for CRM Basic (合格产品/服务) 
- Dynamics 365 客户参与计划企业版（来自 SA for CRM Basic (合格提议) 学生）
- Dynamics 365 客户参与计划企业版（来自 SA for CRM Basic (合格提议) 教职员）
- Dynamics 365 客户参与计划 Enterprise Edition Add-On for CRM Basic (合格产品/) 服务
- Dynamics 365 客户参与计划 Enterprise Edition (政府定价) Add-On，适用于 CRM 基本 (合格提议) 
- Dynamics 365 客户参与计划 Enterprise Edition Add-On for CRM Basic (合格产品/服务) 学生
- Dynamics 365 客户参与计划 Enterprise Edition Add-On for CRM Basic (合格产品/服务) 教职员



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer Engagement Plan from Basic (合格的产品/服务) 更换计划

**停用的产品**   

- CRM Basic 或 CRMOL 基本 (合格产品/服务的销售额的 Dynamics 365) 
- CRM Basic 或 CRMOL 基本 (合格产品/服务的 Dynamics 365 客户参与计划) 

**替换选项**
- Dynamics 365 for Sales Professional (NEW) 
- Dynamics 365 for Sales Professional (NEW) 
- Dynamics 365 for Customer Service
- Dynamics 365 客户参与计划或
- Dynamics 365 团队成员



## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

将客户从停用的 Sku 转移到新的 Sku 需要按以下顺序执行以下步骤：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

## <a name="purchase-the-new-plan-for-your-customer"></a>为客户购买新计划

1. 从左侧导航栏中选择 " **客户** "，并选择要移动到新订阅的客户。
2. 选择 " **添加订阅**"。
3. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。 

你的客户现在将具有旧订阅和新订阅。 下一步是向客户的用户重新分配许可证。

1. 从左侧导航栏中选择 " **客户** "，然后选择要移动的客户。
2. 选择 " **用户和许可证**"。
3. 若要为用户重新分配许可证，请选择该用户，然后选择 " **管理许可证**"。 
4. 在 " **管理许可证** " 页上，清除 "基本 (合格产品/服务) 许可证" 复选框中的 "Dynamics 365 for Sales/Customer Engagement 计划"，然后为客户要移到的订阅选择新的服务计划。 
5. 选择“提交”。 你将对需要新许可证的每个用户执行此操作。 

将许可证移至新订阅后，可以取消旧订阅。 

1. 从左侧导航栏中选择 " **客户** "，然后选择要移动的客户。
2. 在 "订阅详细信息" 页上，将旧订阅设置为 " **挂起** "，然后选择 " **提交**"。

旧订阅现已暂停，新订阅处于活动状态。 暂停的订阅在 120 天后将自动取消预配。 你的客户不会对旧订阅产生额外的费用。
 

 



