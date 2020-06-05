---
title: 迁移一些 Skype for Business 订阅
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何以及何时将已过期 Skype for business Online 计划1订阅的特定客户迁移到新的 Office 365 版本。
author: LauraBrenner
ms.author: labrenne
keywords: Skype for Business 计划, 停用 Skype, Office 365
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8e3a16450d9ac15785315a1b4b077e1872e1303a
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425956"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>将 Skype for Business Online Plan 1 订阅迁移到更新的 Office 365 版本

**适用于**

- 合作伙伴中心

Skype for Business Online 计划1将停用，在2018年8月1日生效。 该日期之后，客户将无法再购买新的 Skype for Business Plan 1 订阅，现有订阅在过期后不会自动续订且不会提供订阅选项。 在订阅的详细信息页面上，Skype for Business Online Plan 1 订阅状态已从“[日期] 自动续订”更改为“[日期] 过期”。  

为了确保客户服务连续性，你应该将 Skype for Business Online Plan 1 订阅快过期的客户过渡到下列支持的 SKU 选项。 建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。 

>[!NOTE]
>Skype for Business Online Plan 1 商业和政府 SKU 均已停用。

如果你使用 API（CREST 或合作伙伴中心），请通过评估订阅的结束日期以及“自动更新 = False”属性来查找快到期的订阅。 Skype for Business Online Plan 1 订阅将在 2018 年 9 月 1 设置为自动续订=False。 你可以随时将客户移到新计划中。 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype for Business Online Plan 1 替换计划

使用新计划，你的客户可以利用 Office 365 中的更新功能。 定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。 

- 选项 1：Office 365 企业版 F1
- 选项 2：Microsoft 365 企业版 F1
- 选项 3：其他 Office 365 计划

|**功能**    |**选项 1**   |**方法 2**   |**选项3**   |
|:-----------------|:-----------------|:-------------|:------------|
|获取 Skype for Business Online Plan 1 所含的所有功能|是   |是   |是   |
|IM 和状态 |是   |是   |是   |
|通过 IP 的对等音频和视频|是   |是   |是   
|以通过身份验证的用户身份加入会议| 是   |是   |是   |

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

Microsoft 不断向我们的合作伙伴提供新产品和服务。 在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。 将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：

- 购买新订阅
- 重新分配当前用户许可证
- 取消旧订阅

### <a name="migrate-your-customers-to-new-plans"></a>将你的客户迁移至新计划

1. 若要购买新的订阅，请从 "**合作伙伴中心" 菜单**中选择 "**客户**"，选择要移动的客户，然后选择 "**添加订阅**"。

2. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。 

你的客户现在应具有新订阅和新订阅，旧的 Skype for Business Online 计划1订阅和新的 "目标" 订阅，例如，选项 1-Office 365 企业 F1。

3. 若要重新分配客户的用户许可证，请在 "**合作伙伴中心**" 菜单中选择 "**客户**"，选择要移动的客户，然后选择 "**用户和许可证**"。 此时将打开客户的 "用户和许可证" 页。

4. 若要重新分配用户许可证，请选择要重新分配的用户，然后选择**管理许可证**。

5. 在**管理许可证**页面上，清除 Skype for Business Online Plan 1 许可证复选框，然后选择客户要迁移到的订阅的新服务计划。

6. 选择“提交”。 确认页面列出了新的许可证分配。 继续对需要许可证分配的其他用户执行相同过程。

在将用户许可证移动至新服务后，可安全取消该客户级别的已停用订阅。

7. 从 "**合作伙伴中心**" 菜单中，选择 "**客户**"。 选择要取消其订阅的客户。

8. 在订阅详细信息页面中，将订阅设置为**已暂停**。

9. 选择 "**提交"。**

旧订阅已暂停，新订阅将激活。 暂停的订阅在 120 天后将自动取消预配。 不会向客户收取旧订阅的任何额外成本。

