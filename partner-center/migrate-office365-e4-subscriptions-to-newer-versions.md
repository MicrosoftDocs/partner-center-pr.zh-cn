---
title: 将 Office 365 E4 订阅迁移到较新的 Office 365 版本 |合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 企业版 E4 版本自 2017 年 4 月 7 日起已停用。 了解如何将你的客户订阅迁移到较新版本的 Office 365。
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: ead92169ce7b3f1c2e697b6d4e983603c17d39fc
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390876"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>将 Office 365 E4 订阅迁移到较新的 Office 365 版本

**适用于**

-  合作伙伴中心

**相应的角色**
-   全局管理员
-   用户管理员
-   管理员代理
-   销售代理

Office 365 企业版 E4 计划已停用，停用的生效日期为 2017 年 4 月 7 日。 在此日期之后，你将无法再购买新的 Office 365 E4 订阅，现有的 E4 订阅在到期后将不会自动续订。

当 E4 订阅结束时，它们将会被取消。 为了确保客户服务连续性，你应该将 E4 订阅快过期的客户过渡到下列支持的 SKU 选项。 建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。 

> [!NOTE]  
>  Office 365 企业版 E4 商业版和政府版 Sku 均已停用。
 
在订阅的详细信息页面上，E4 订阅状态已从“[日期] 自动续订”更改为“[日期] 过期”。 

如果你使用 API（CREST 或合作伙伴中心），则可以通过评估订阅的结束日期以及“自动更新 = False”属性来发现快到期的订阅。 

2017 年 4 月 7 日，E4 订阅将设置为“自动更新 = False”。 你可以随时将客户移到新计划中。 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 企业版 E4 版本替换计划

你可以选择保持与 E4 相同的功能，或者让你的客户利用 Office 365 和 Skype for Business Online 中的较新特性和功能。 定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。 可以分别在 Office 365 企业版 E3 或 Office 365 企业版 E5 的以下选项中替换 Secure Product Enterprise E3 或 Secure Productive Enterprise E5。

- 选项 1：Office 365 企业版 E5

- 选项 2：Office 365 企业版 E3 + Skype for Business 云 PBX

- 选项 3：Office 365 企业版 E3 + Skype for Business Plus CAL（价格和功能与 E4 相同）

- 选项 4：Office 365 企业版 E3


| 功能 | 选项 1 | 方法 2 | 选项 3 | 选项 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| 获取 Office 365 企业版 E4 中包含的所有功能？ | 是 | 是 | 是 | 是 |
| 在 Office 365 中管理电话号码？ | 是 | 是 | 是 | 是 |
| 在本地和 Office 365（混合部署）中管理电话号码？ | 是 | 是 | 是 | 是 |
| 选项用于添加 PSTN 语音通话套餐？ | 是 | 是 | 是 | 是 |
| PSTN 会议？ | 是 | 是 | 是 | 是 |
| 用于协作、分析和保证安全的高级工具？ | 是 | 是 | 是 | 是 |
| 交互式报告、仪表板和数据可视化？ | 是 | 是 | 是 | 是 | 
| 更好地控制数据安全性并符合内置的隐私、透明度和改进型用户控件的要求？ | 是 | 是 | 是 | 是 | 

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

Microsoft 不断向我们的合作伙伴提供新产品和服务。 在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。 将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：

-   购买新订阅
-   重新分配当前用户许可证
-   取消旧订阅

按照以下步骤将客户的 Office 365 企业版 E4 订阅迁移到上表中的其中一个选项。

### <a name="step-1---purchase-the-new-subscription"></a>步骤 1 - 购买新订阅

1. 从 "**合作伙伴中心**" 菜单中，选择 "**客户**"，选择要移动的客户，然后选择 "**添加订阅**"。

2. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。

   你的客户现在应具有新订阅和新订阅，旧的 Office 365 企业版 E4 订阅和新的 "目标" 订阅，例如，选项 1-Office 365 企业版 E5。

### <a name="step-2---reassign-the-customers-users-licenses"></a>第 2 步 - 重新分配客户的用户许可证

1. 从 "**合作伙伴中心**" 菜单中，选择 "**客户**"，选择你想要移动的客户，然后选择 "**用户和许可证**"。 此时将打开客户的 "用户和许可证" 页。

2. 若要重新分配用户许可证，请选择要重新分配的用户，然后选择**管理许可证**。

3. 在**管理许可证**页面上，清除 **Office 365 企业版 E4** 许可证复选框，然后选择客户要迁移到的订阅的新服务计划。

4. 选择“提交”。 确认页面列出了新的许可证分配。

5. 对其他任何需要重新分配许可证的客户用户继续执行相同的步骤。

在将用户许可证移动至新服务后，可安全取消最高“客户”级别的已停用订阅。

### <a name="step-3---cancel-the-old-subscription"></a>步骤 3 - 取消旧订阅

1. 从 "**合作伙伴中心**" 菜单中，选择 "**客户**"。 选择你想要移动的客户，并选择你想要取消的订阅。

2. 在订阅详细信息页面中，将订阅状态设置为**已暂停**。

3. 选择“提交”。

旧订阅已暂停，新订阅将激活。 暂停的订阅在 120 天后将自动取消预配。 不会向客户收取旧订阅的任何额外成本。



 



