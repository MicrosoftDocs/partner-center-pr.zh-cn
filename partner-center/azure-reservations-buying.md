---
title: 为客户Microsoft Azure预留
description: 了解如何代表客户在 合作伙伴中心 购买或购买 Azure 预留。 还列出了 Azure 预留不可用的市场。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149530"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>在Microsoft Azure中代表客户购买合作伙伴中心

**适当的角色**：管理员代理|全局管理员|支持人员代理|销售代理|用户管理管理员

本文介绍如何代表客户在 合作伙伴中心 购买或购买 Azure 预留。 它还标识 Azure 预留不可用的市场。
 
> [!NOTE]
> 本文仅适用于云解决方案提供商计划云解决方案提供商 () 合作伙伴。 使用其他类型的订阅（例如 (即用即付、个人、Microsoft 客户协议 或 企业协议 订阅) 应改为阅读 [此 Azure](/azure/cost-management-billing/reservations)预留文档。

## <a name="before-you-begin"></a>准备阶段

在代表客户购买 Azure 预留之前，请查看以下重要信息。  (是否希望客户能够从之前购买的 Azure 订阅购买自己的 Azure 预留？ 请参阅 [授予客户购买自己的 Azure 预留](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)的权限 .) 

- 如果客户签署新订阅，Microsoft 客户协议 (确认客户接受 Microsoft 客户协议) ，[](confirm-customer-agreement.md)则必须在 Azure 计划下购买 Azure 预留。 有关详细信息，请阅读购买 [Azure 计划](purchase-azure-plan.md)。

- 客户必须已经拥有有效的 Azure 订阅，然后你才能代表他们购买预订
  
- 软件订阅成本（例如 SQL 数据库或 SUSE Linux 软件）不包括在 Azure 预留价格中

- Microsoft 的商业定价不包括税款，除非你的位置是巴西。 如果你的位置是巴西，则商业价格包括相应的税款

- 销售和支持人员代理需要显式访问 Azure 订阅，以便他们可以代表客户在 Azure 门户中购买或管理订阅，以及提出支持请求，包括进行兑换和退款  

- 如果你是间接提供商，并且通过 Azure 门户 购买 Azure 预留，则记录合作伙伴 (间接经销商) 继承自你选择Azure CSP订阅。

- 无法在购买后更改 Azure 预订的记录合作伙伴。 您可以取消现有预订，并使用新的记录合作伙伴购买新预订。

- 如果客户需要将 Azure 订阅从直接方式或 EA 转移至云解决方案提供商计划，预订不会转移。

## <a name="azure-reservations-unavailable-markets"></a>不可使用 Azure 预留的市场

> [!IMPORTANT]
> Azure 预留在以下市场中不可用：  
>  
> **不可用市场（按字母顺序）**
>
> |A 到 Gi   | Gr 到 Pal  | Pap 到 Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | 奥兰岛     | 格陵兰     | 巴布亚新几内亚     |
> | 美属萨摩亚     | 格林纳达     | 皮特凯恩群岛     |
> | 安道尔     | 瓜德罗普岛     | 留尼汪     |
> | 安圭拉岛     | 关岛     | 萨巴   |
> | 南极洲     | 格恩西岛     | 圣巴泰勒米岛   |
> | 安提瓜和巴布达       | 几内亚     | 圣卢西亚   |
> | 阿鲁巴岛       | 几内亚比绍     | 法属圣马丁   |
> | 阿塞拜疆       | 圭亚那     | 圣皮埃尔和密克隆岛   |
> | 贝宁     | 海地       | 圣文森特和格林纳丁斯     |
> | 不丹     | 赫德岛和麦克唐纳群岛       | 萨摩亚     |
> | 博内尔     | 曼岛     | 圣马力诺     |
> | 布韦岛     | 扬马延岛     | 圣多美和普林西比   |
> | 英属印度洋领地       | 泽西     | 塞舌尔   |
> | 英属维尔京群岛     | 基里巴斯       | 塞拉利昂   |
> | 布基纳法索     | 科索沃     | 圣尤斯特歇斯     |
> | 布隆迪     | 老挝     | 荷属圣马丁     |
> | 柬埔寨     | 莱索托     | 所罗门群岛     |
> | 中非共和国     | 利比里亚     | 索马里     |
> | 乍得     | 马达加斯加     | 南乔治亚岛和南桑威奇群岛     |
> | 中国     | 马拉维     | 南苏丹     |
> | 圣延岛     | 马尔代夫     | 圣赫勒拿-阿森松-特里斯坦达库尼亚     |
> | 科科斯群岛     | 马里     | 苏里南     |
> | 科摩罗     | 马绍尔群岛     | 斯瓦尔巴岛     |
> | 刚果     | 马提尼克     | 斯威士兰     |
> | 刚果（民主共和国）     | 毛里塔尼亚     | 东帝汶   |
> | 库克群岛     | 马约特     | 多哥   |
> | 吉布提     | 密克罗尼西亚     | 托克劳   |
> | 多米尼加     | 蒙特塞拉特     | 汤加   |
> | 赤道几内亚     | 莫桑比克     | 特克斯和凯科斯群岛   |
> | 厄立特里亚     | 缅甸     | 图瓦卢   |
> | 福克兰群岛     | 瑙鲁     | 美国本土外小岛屿   |
> | 法属圭亚那     | 新喀里多尼亚     | 瓦努阿图   |
> | 法属玻里尼西亚     | 尼日尔     | 梵蒂冈   |
> | 法属南部领地     | 纽埃     | 瓦利斯和富图纳   |
> | 加蓬     | 诺福克岛     | 也门   |
> | 冈比亚     | 北马里亚纳群岛     |    |
> | 直布罗陀     | 帕劳       |    |

## <a name="purchase-azure-reservations"></a>购买 Azure 预留项

按照以下步骤在合作伙伴中心购买 Microsoft Azure 预订。  (你希望客户能够从为他们购买的以前的 Azure 订阅购买自己的 Azure 预订吗？ 请参阅 [授予客户购买自己的 Azure 预订的权限](give-customers-permission.md)。 ) 

1. 从 "合作伙伴中心" 菜单中选择 " **客户** "。  

2. 在 " **客户** " 页上，找到想要购买 Azure 预订的客户，然后选择向下箭头以展开客户的行。  

3. 依次选择“添加产品”、“Azure”。 

    a. 从“细分市场”列表中选择该客户的细分市场。

    b. 从 "产品 **类型**" 列表中选择 "**保留**"。

    c. 从“预留项类型”列表中选择客户所需的预留项类型。

4. Azure 预订必须与有效的 Azure 订阅相关联。 从 " **客户订阅** " 列表中选择要向其添加 Azure 预订的客户的订阅。 

   >[!IMPORTANT]
   >如果客户还没有有效的 Azure 订阅，请选择 " **azure** " 立即添加一个。 

5. 使用筛选器查找满足客户要求的虚拟机上的 Azure 保留项。  

6. 找到要购买)  (的预订后，输入客户在 **数量** 中所需的保留实例数，然后选择 " **添加到购物车**"。  

7. 重复步骤5和步骤6，直到将所有必需的项添加到订单中。 选择“查看”以确认订单是否正确无误。  

8. 在 **查看订单** 页面上，可以： 

    - 验证或更改预留实例数量。

    - 选择预订的作用域。 预订的范围可以包含一个订阅或多个订阅（共享范围）。 如果将预留范围限定于单个订阅，则预订折扣仅应用于此订阅。 如果选择 "共享"，则预订折扣将应用到客户的计费上下文内的任何订阅。 

      >[!NOTE] 
      >如果选择将预订的范围限制为单个 Azure 订阅，可能需要增加订阅的 vCPU 配额。 若要增加订阅的 vCPU 配额，需要在 Azure 门户中创建支持请求。 按照 [本主题中](/azure/azure-supportability/resource-manager-core-quotas-request) 的说明创建请求。 

      >[!NOTE]   
      >如果客户位于 Azure 计划下，则 **范围**  将设置为 " **共享**"。 

    - 如果是提供商合作伙伴，请选择要与产品关联的经销商。
    
    - 如果 Azure 预留支持"计费计划"选项，可以从下拉菜单中选择按月计费频率。 
    - 如果 Azure 预留不支持"计费计划"选项，则计费频率默认为一次计费。 

9. 选择 **确认购买** 以购买订购的商品。 订单的详细信息（包括订单编号）将显示在"确认 **"** 页上。 选择“完成”转到“订单历史记录”页。  

10. 若要管理客户在 Azure 门户中的预留，请在"客户"页上找到客户，然后选择向下箭头以展开客户的行。 选择 **Microsoft Azure 管理门户"，** 打开客户在 Azure 门户 中的记录。

## <a name="next-steps"></a>后续步骤

|**有关以下方面的信息**   |**阅读此文**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [销售 Microsoft Azure 预留实例](azure-reservations.md) |
|在门户中管理 Azure 合作伙伴中心 | [在门户中管理 Azure 合作伙伴中心](azure-reservations-manage.md)
|确定正确的虚拟机大小，然后确认客户虚拟机使用情况   |[针对最大 Azure 预订利用率确定虚拟机大小](azure-usage.md)   |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](/partner-center/develop/purchase-azure-reservations)   |
|授予客户购买自己的 Azure 预留的权限  | [为客户提供购买自己的 Azure 预留的权限](give-customers-permission.md)  |