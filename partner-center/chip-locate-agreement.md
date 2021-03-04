---
title: 查找桌面计数和费用级别
ms.topic: how-to
ms.date: 02/18/2021
description: 了解如何使用渠道奖励平台 (芯片) 查找协议的桌面计数和费用级别信息。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756109"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>找到协议的桌面设备计数和费用级别

**相应的角色**

- 主要联系人或计划管理员

你可以登录到 [explore.ms](https://www.explore.ms/) 以查看协议，或下载提供有关桌面计数和费用级别的协议详细信息的文件。

## <a name="to-locate-the-information"></a>查找信息

### <a name="method-1--explorems"></a>方法1– Explore.ms

1. 在 Internet Explorer 中打开 [explore.ms](https://www.explore.ms/) 。 

>[!Note]
>不能在 Google Chrome 或 Microsoft Edge 中执行此功能。

2. 使用工作/学校帐户或 live ID 登录。  

3. 在 " **报表** " 字段中，选择 " **协议**"。

4. 在生成的页上，在 **搜索** 字段中输入协议号，然后选择 " **选择列**"。

5. 在弹出窗口中，从 "可用列" 列表中选择 " **协议桌面计数** "，然后选择向右箭头以添加该列。 选择“确定”。

6. 选择 " **搜索"。**

7. 在随后出现的屏幕中，滚动搜索结果以查找 " **协议桌面计数** " 列。 

8. 使用 "桌面计数" 根据下面的费率表确定费用级别。  

| 费用级别 | 桌面计数 |
| ------ | :-----------: |
|  A | 0–2399    |
|  B | 2400–5999    |
|  C | 6000–14999    |
|  D | 15000 +   |

>[!NOTE]
>企业激励级别基于桌面或用户计数 ( (PS PS PS) 注册中的更高) 。 对于没有与自然关联的桌面或用户计数的注册，Microsoft 基于附带的 EA 的桌面计数或用户计数应用桌面计数。 <br><br>如果没有随附的 EA，则费用级别基于注册的定价级别。 还可以在 [www.explore.ms](https://www.explore.ms/)上查看该交易的定价级别。 <br><br>如果现有的 EA/EAS 上有多个池和/或定价级别，Microsoft 将按分配的最高定价/池级别支付奖励，将级别 A 指定为最低，级别为最高级别。

#### <a name="pool-and-pricing-levels"></a>池和定价级别

使用上述步骤在 explore.ms 中搜索协议编号后，选择协议编号。 这会将你转到 "协议详细信息" 页面，该页面将显示 " **协议摘要** " 和 " **产品/服务**"。 "产品/服务" 部分包含定价级别。

## <a name="method-2---chip"></a>方法 2-芯片

1. 登录到芯片，并选择 LSP 奖励。

2. 从 "**合作伙伴付款摘要**" 页中，选择要查看的报表月份，然后从 "**导出到 Excel**" 下的下拉列表中选择 "**计算详细信息**"：

:::image type="content" source="images/chip/chiplocate.png" alt-text="查找程序详细信息":::

3. 导出将开始，你可以打开文件或将其保存/保存到目标。

4. 当报表处于打开状态时，导航到左下角的 " **DetailReport-FlatFile** " 选项卡：

:::image type="content" source="images/chip/flatfile.png" alt-text="平面文件下载":::

你现在可以在第 J 列中搜索所需的协议编号，并在列 R 中找到分配的桌面计数，并将其标记 Agreement_DesktopCount。 你还可以在 "AI" 标记为 "层" 的列中确认此协议的费用级别。

## <a name="next-steps"></a>后续步骤

- [排查芯片访问问题](chip-access-trouble.md)
