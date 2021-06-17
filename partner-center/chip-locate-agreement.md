---
title: 查找桌面计数和费用级别
ms.topic: how-to
ms.date: 02/18/2021
description: 了解如何使用 CHIP (渠道奖励) 查找协议的桌面计数和费用级别信息。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276926"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>找到协议的桌面设备计数和费用级别

**适当的角色**：主要联系人或计划管理员

可以登录到 explore.ms[](https://www.explore.ms/)查看协议，或下载提供桌面计数和费用级别的协议详细信息的文件。

## <a name="to-locate-the-information"></a>查找信息

### <a name="method-1--explorems"></a>方法 1 – Explore.ms

1. 在 [explore.ms](https://www.explore.ms/) 中Internet Explorer。 

>[!Note]
>无法在 Google Chrome 或 Microsoft Edge 中执行Microsoft Edge。

2. 使用工作/学校帐户或实时 ID 登录。  

3. 在"**报表"** 字段中，选择"**协议"。**

4. 在生成的页上，在"搜索"字段中输入协议 **编号**，然后选择"**选择/排序列"。**

5. 在弹出窗口中，从可用列列表中选择" **协议** 桌面计数"，然后选择右箭头以添加列。 选择“确定”。

6. 选择" **搜索"。**

7. 在生成的屏幕中，滚动浏览结果以查找"协议 **桌面计数"** 列。 

8. 使用桌面计数根据下面的费率表确定费用级别。  

| 费用级别 | 桌面计数 |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>企业激励级别基于桌面或用户计数 (在商业和) 部门或 PS (注册中) 较高者。 对于没有自然关联桌面或用户计数的注册，Microsoft 根据随附 EA 的桌面计数或用户计数应用桌面计数。 <br><br>如果没有随附的 EA，则费用级别基于注册的定价级别。 还可以在上查看交易定价[www.explore.ms。](https://www.explore.ms/) <br><br>如果现有 EA/EAS 上有多个池和/或定价级别，Microsoft 将在分配的最高定价/池级别支付奖励，级别 A 为最低，级别 D 为最高。

#### <a name="pool-and-pricing-levels"></a>池和定价级别

使用上述步骤在 explore.ms 中搜索协议编号后，选择协议编号。 这会将你打开协议详细信息页，其中会显示"协议摘要"**和**"**产品/服务"。** 产品/服务部分包含定价级别。

## <a name="method-2---chip"></a>方法 2 - CHIP

1. 登录到 CHIP 并选择"LSP 奖励"。

2. 在"**合作伙伴付款摘要"** 页中，选择要查看的报告月份，然后从"导出到Excel"下的下拉列表中选择"计算 **详细信息"：**

:::image type="content" source="images/chip/chiplocate.png" alt-text="找到程序详细信息。":::

3. 导出将启动，你可以打开该文件，也可以将 文件另存为目标。

4. 当报表打开时，导航到最左下角 **的 DetailReport-FlatFile** 选项卡：

:::image type="content" source="images/chip/flatfile.png" alt-text="平面文件下载。":::

现在可以在列 J 中搜索要查找的协议编号。可以在列 R 中查找分配的桌面计数，该计数Agreement_DesktopCount。 还可以在标记为"层"的"AI"列中确认此协议的费用级别。

## <a name="next-steps"></a>后续步骤

- [排查 CHIP 访问问题](chip-access-trouble.md)
