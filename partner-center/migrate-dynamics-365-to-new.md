---
title: 迁移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在符合条件的 Dynamics 365 Business Edition 产品/服务过期之前将其迁移到较新版本。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151519"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>将 Dynamics 365 商业版产品/服务迁移到较新版本

**适当的角色**：全局管理员|用户管理管理员|管理代理|销售代理

自 2019 年 1 月 1 日起，具有 Dynamics 365 Business Edition 订阅的客户无法再续订这些旧版产品/服务;现有订阅过期时不会自动续订。 在订阅的详细信息页上，订阅状态从"[日期]自动续订"更改为"[date]过期"。

为了确保客户的连续性，应该将即将过期的订阅转换为下面列出的受支持选项。 我们建议在订阅的每年结束日期之前将客户移动到新订阅，以避免客户发生任何服务中断。

如果使用 CREST (或 合作伙伴中心) API，则可以通过评估订阅的结束日期以及自动续订 = False 属性来查找即将过期的订阅。 有关订阅将在 2019 年 1 月 1 日设置为 auto renew=False。 你可以随时将客户移到新计划中。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>即将停用的 Dynamics 365 商业版

- Dynamics 365 for Finance and Operations Business Edition
- 适用于团队成员的 Dynamics 365，商业版

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - Dynamics 365 Business Edition 新产品/服务

借助新的 Dynamics Business Central 产品/服务，客户可以连接其财务、销售、服务和操作，以简化业务流程、改善客户交互并做出更好的决策。 Dynamics 365 Business Central 基于云的，仅通过云解决方案云解决方案提供商 (CSP) 合作伙伴提供。
在 2020 年 6 月 30 日之前，Dynamics 365 Business Edition 客户有资格享受新的 Business Central 产品/服务的折扣转换定价。

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

 将客户从已停用的 SKUS 迁移到较新的 SKUS 需要按以下顺序执行以下步骤：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

## <a name="purchase-the-new-plan-for-your-customer"></a>为客户购买新计划

1. 从 **左侧** 导航中选择"客户"，然后选择要移动到新订阅的客户。
2. 选择"**添加订阅"。**
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
