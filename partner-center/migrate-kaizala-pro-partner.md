---
title: 将 Kaizala Pro 订阅迁移到 Microsoft 365
description: 了解如何将 Kaizala Pro 订阅迁移到 Microsoft 365 或 Office 365 版本。 有关转换客户的更多详细信息，请阅读此文。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146419"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>将 Kaizala Pro 独立订阅迁移到 Microsoft 365 或 Office 365 版本

**适当角色**：销售代理

从 2020 年 7 月 1 日开始，Microsoft 将结束 Kaizala Pro 独立服务的销售。 在此日期之后，客户将无法再购买新的 Kaizala Pro 订阅，现有的 Kaizala Pro 订阅在过期时不会自动续订。

为了确保客户的连续性，应该将即将到期的 Kaizala Pro 独立订阅的客户转换为下面列出的受支持的 SKU 选项。 我们建议在订阅的每年结束日期之前将客户移动到新订阅，以避免客户发生任何服务中断。

如果使用 CREST 或 (API 合作伙伴中心) ，则可以通过评估订阅的结束日期以及设置为 false 的自动续订属性来发现即将过期的订阅 `auto renew = False` ：。

E4 订阅将于 `auto renew=False` 2020 年 7 月 1 日设置为 。 你可以随时将客户移到新计划中。

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro 独立版替换计划

借助新计划，客户可以利用新版Microsoft 365。 定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。

- [**Microsoft 365企业，**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)包括：  
   - Microsoft 365 商业基本版
   - Microsoft 365 商业标准版
   - Microsoft 365 商业高级版
    
- [**Microsoft 365一线 ，**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)包括：
   - Microsoft 365 F3（以前为 Microsoft 365 F1）和 Office 365 F3
    
- [**Microsoft 365企业版 ，**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)包括： 
   - Office 365 E1
   - Microsoft 365 E3 和 Office 365 E3
   - Microsoft 365 E5 和 Office 365 E5

- [**Microsoft 365教育，**](https://www.microsoft.com/education/buy-license/microsoft365)包括： 
    - Microsoft 365 A1 和 Office 365 A1
    - Microsoft 365 A3 和 Office 365 A3
    - Microsoft 365 A5 和 Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划

Microsoft 不断向我们的合作伙伴提供新产品和服务。 在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。 将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：

A. 购买新订阅

B. 重新分配当前用户许可证

C. 取消旧订阅


## <a name="migrate-your-customers-to-new-plans"></a>将你的客户迁移至新计划

### <a name="a-purchase-the-new-subscription"></a>A. 购买新订阅

1. 若要购买新订阅，请从"合作伙伴中心"菜单中，选择"**客户**"，选择要移动的客户，然后选择"添加 **订阅"。**

2. 从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。

现在，客户应同时拥有新旧订阅、旧的 Kaizala Pro 独立订阅和新"目标"订阅，例如选项 1 - Office 365 企业版 F1。

### <a name="b-reassign-current-user-licenses"></a>B. 重新分配当前用户许可证

1. 若要重新分配客户的用户许可证，请在 " **合作伙伴中心** " 菜单中选择 " **客户**"，选择要移动的客户，然后选择 " **用户和许可证**"。 此时将打开客户的 "用户和许可证" 页。

2. 若要重新分配用户许可证，请选择要重新分配的用户，然后选择 " **管理许可证**"。

3. 在 " **管理许可证** " 页上，清除 "Kaizala Pro 独立许可" 复选框，并为客户要移到的订阅选择新的服务计划。

4.  选择“提交”。 确认页面列出了新的许可证分配。 继续对需要许可证分配的其他用户执行相同过程。

### <a name="c-cancel-old-subscription"></a>C. 取消旧订阅

在将用户许可证移动至新服务后，可安全取消该客户级别的已停用订阅。

1.  从 " **合作伙伴中心** " 菜单中，选择 " **客户**"。 选择要取消其订阅的客户。

2.  在订阅详细信息页面中，将订阅设置为 **已暂停**。

3.  选择“提交”。

旧订阅已暂停，新订阅将激活。 暂停的订阅在 120 天后将自动取消预配。 不会向客户收取旧订阅的任何额外成本。
