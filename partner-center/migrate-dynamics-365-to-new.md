---
title: 迁移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将限定的 Dynamics 365 商业版产品/服务迁移到更新的版本，使其过期。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436826"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>将 Dynamics 365 商业版产品/服务迁移到较新版本

**适用于**

- 合作伙伴中心

**相应的角色**
- 全局管理员
- 用户管理员
- 管理员代理
- 销售代理

2019年1月1日生效，具有 Dynamics 365 Business Edition 订阅的客户不再能够续订这些旧产品/服务。现有订阅将不会在过期时自动续订。 在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。

若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。 建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。

如果使用 API （CREST 或合作者中心），可以通过评估订阅的结束日期以及自动续订 = False 属性来找到过期订阅。 相关订阅将在2019年1月1日设置为自动续订 = False。 你可以随时将客户移到新计划中。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>要停用的 Dynamics 365 业务版本

- Dynamics 365 for Finance and Operations Business Edition
- 适用于团队成员的 Dynamics 365，商业版

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central-Dynamics 365 Business Edition 新产品/服务

利用全新的 Dynamics Business Central 产品/服务，你的客户可以连接其财务、销售、服务和操作，以优化业务流程、改善客户交互，并做出更好的决策。 Dynamics 365 Business Central 是基于云的，并且仅可通过云解决方案提供商（CSP）计划合作伙伴获得。
Dynamics 365 Business Edition 客户有资格在2020年6月30日之前获得新的业务中心产品/服务的折扣过渡价格。

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

 将客户从停用的 Sku 转移到新的 Sku 需要按以下顺序执行以下步骤：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

## <a name="purchase-the-new-plan-for-your-customer"></a>为客户购买新计划

1. 从左侧导航栏中选择 "**客户**"，并选择要移动到新订阅的客户。
2. 选择 "**添加订阅**"。
3. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。 

你的客户现在将具有旧订阅和新订阅。 下一步是向客户的用户重新分配许可证。

1. 从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。
2. 选择 "**用户和许可证**"。
3. 若要为用户重新分配许可证，请选择该用户，然后选择 "**管理许可证**"。 
4. 在 "**管理许可证**" 页上，清除 "基本（合格产品/服务）许可证的 Dynamics 365 for Sales/Customer Engagement 计划" 复选框，并为客户要移到的订阅选择新的服务计划。 
5. 选择“提交”。 你将对需要新许可证的每个用户执行此操作。 

将许可证转移到新订阅后，可以取消旧订阅。 

1. 从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。
2. 在 "订阅详细信息" 页上，将旧订阅设置为 "**挂起**"，然后选择 "**提交**"。

旧订阅现已暂停，新订阅处于活动状态。 暂停的订阅在 120 天后将自动取消预配。 你的客户不会对旧订阅产生额外的费用。
