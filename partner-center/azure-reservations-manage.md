---
title: 管理客户的 Azure 保留
description: 了解如何管理客户的 Azure 保留，包括如何取消预订、交换预订或请求退款。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: fba1427978e61b739c8ffb14374a44331ef51d27
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "89366871"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>为客户管理、取消、交换或退款 Microsoft Azure 预订

**适用于**

- 合作伙伴中心
- Microsoft Azure 门户 
- 云解决方案提供商计划中的合作伙伴

**相应的角色**

- 管理员代理
- 全局管理员
- 支持人员代理
- 销售代理
- “用户管理”管理员

> [!NOTE]
> 本文仅适用于云解决方案提供商 (CSP) 计划中的合作伙伴。 使用其他订阅类型的客户 (例如，即用即付、个人、Microsoft 客户协议或企业协议订阅) 应改为阅读 [此 Azure 保留文档](https://docs.microsoft.com/azure/cost-management-billing/reservations)。

若要在购买后管理客户的 Azure 预订，请选择要在合作伙伴中心管理的客户和预订，然后在 Azure 门户中对预订进行更改。

1. 若要开始，请从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要管理其预留的客户。 

2. 在客户的详细信息页面菜单上，选择 " **Azure 保留** "，然后选择要管理的特定预订。  

3. 在 " **操作**" 下，选择 " **管理** " 以前往 Azure 门户中的客户预订记录。 在预订详细信息页面上，执行以下步骤来完成任务。  

    | **Select**   | **收件人**    |
    |:-----------------------------|:-----------------|
    | **概述**   | 查看客户预订的详细信息，包括到期日期、范围和利用率数据。 **注意** 选择**退款**可以创建一个按比例退款的支持请求。 选择**兑换**可以创建一个兑换未使用部分的预订期限的支持请求。  
    | ** (IAM) 的访问控制 **   | 管理对客户预订信息的访问。|
    | **配置**   | 更改保留的作用域和/或与之关联的 Azure 订阅。    |
    | **属性**   | 查看预订的属性并将其复制到剪贴板中保留 ID 和预留订单 ID。 **注意** 当你代表客户请求支持时，支持人员可能会要求你提供预订 ID 和预订订单 ID。    |
    | **新建支持请求**    | 请求 Microsoft 支持人员提供帮助。   |
 
## <a name="cancel-or-exchange-a-reservation"></a>取消或兑换预订

如果客户的业务需求发生了变化，则他们可能需要取消预订，并获得退款或交换预订的按比例支付的退款金额，以用于新预订的价格。

在这两种情况下，Microsoft 将为你退款，这样你就可以通过客户管理生成的财务交易。 Microsoft 不会直接与客户联系，就计费、取消或退款。

### <a name="how-cancellations-work"></a>如何取消

客户可随时请求取消预留 (每年 $50000 的退款金额) 。 取消预订后，客户可以返回 Azure 预订的剩余月份数，以提前终止费。 剩余的按比例余额减去提前终止费，以使你的帐户获得退款。 

请参阅下面的 "取消详细信息和费用"。


|**取消日期**<br>  (天)    |**使用情况**    |**额度**  |**提前终止**<br> 费用    |**退款 cap** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5个或更少                         | 否          | 100%       | 否                              | $50000 USD   |
|5个或更少                         | 是         | 按比例  | 否                              | $50000 USD   |
|超过5个                        | 否          | 按比例  | 12%                             | $50000 USD   |
|超过5个                        | 是         | 按比例  | 12%                             | $50000 USD   |

### <a name="how-exchanges-work"></a>如何兑换 

如果客户想要购买不同于他们最初购买的预订，则他们可以请求交换。 交换预订可能是取消预订的极具吸引力的替代方法，因为它允许客户使用按比例支付的退款量来支付新预订的价格。 

按比例退款金额将贷记到你的帐户，以便为客户提供 exchange。

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>代表客户请求退款或兑换

若要为代表客户的退款或 exchange 提供支持请求，请选择 "合作伙伴中心" 中的 "客户和预订"，然后在 Azure 门户中创建支持请求。 

>[!NOTE]
>Microsoft 支持代理可能会要求你提供预订 ID 和预订订单 ID。 你可以在 Azure 门户的保留 **属性** 页上找到此信息。

1. 若要开始，请从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要退款的客户。 

2. 在客户的详细信息页上，选择 " **Azure 预订** "，然后选择客户希望获得退款的特定预订。  

3. 在 " **操作**" 下，选择 " **退款** " 以前往 Azure 门户中的客户预订记录，并启动支持请求。  

4. 在**新建支持请求**页上，请按照以下步骤来请求退款。 执行每个步骤后选择**下一步**。 

   |**步骤**                    |**选择**    |
   |:---------------------------|:-----------------|
   |**1基础知识**                |问题类型：计费。  |
   |**2 问题**               |问题类型：预订管理。 类别：兑换和退款。 |
   |**3 联系人信息**   |选择首选项并输入所需的信息。 

5. 完成后，选择“创建”****。

## <a name="azure-reservations-resources"></a>Azure 预订资源

|**有关以下方面的信息**   |**阅读此文**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [销售 Microsoft Azure 预留实例](azure-reservations.md) |
|在合作伙伴中心为客户购买 Azure 保留   | [购买 Azure 预订](azure-reservations-buying.md) |
|确定正确的虚拟机大小，然后确认客户虚拟机使用情况   | [针对最大 Azure 预订利用率确定虚拟机大小](azure-usage.md)   |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)   |
|为客户提供从为他们购买的订阅购买自己的 Azure 预订的权限。 | [授予客户购买自己的 Azure 预订的权限](give-customers-permission.md)   |

