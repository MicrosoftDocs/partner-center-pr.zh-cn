---
title: 代表客户管理 Azure 预订 | 合作伙伴中心
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
keywords: azure, 预订, 虚拟机, 管理, 计费, 购买
ms.openlocfilehash: ae27024ba10184b6f704f5ceef9d90af61186321
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2018
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>代表客户管理 Microsoft Azure 预订

**适用范围**

-  合作伙伴仪表板
-  Microsoft Azure 门户
-  云解决方案提供商计划中的合作伙伴

若要在购买后管理客户的 Azure 预订，你需要在合作伙伴仪表板中选择要管理的客户和预订，然后在 Azure 门户中对预订进行更改。 

1. 若要开始，请从你的仪表板菜单中选择**客户**，然后选择你想要管理其预订的客户。 

2. 在客户的详细信息页面上，选择 **Azure 预订**，然后选择你想要管理的特定预订。  

3. 在**操作**下面，选择**管理**以在 Azure 门户中转到客户的预订记录。 在预订详细信息页面上，执行以下步骤来完成任务。  

|**选择**   |**要**    |
|:-----------------------------|:-----------------|
|**概述**   |查看客户预订的详细信息，包括到期日期、范围和使用率数据。 **注意** 选择**退款**可以创建一个按比例退款的支持请求。 选择**兑换**可以创建一个兑换未使用部分的预订期限的支持请求。  
|**访问控制 (IAM)**   |管理客户预订信息的访问权限。|
|**配置**   |更改与预订相关联的预订范围和/或 Azure 订阅。    |
|**属性**   |查看预订的属性并将预订 ID 和预订订单 ID 复制到剪贴板。 **注意** 当你代表客户请求支持时，支持人员可能会要求你提供预订 ID 和预订订单 ID。    |
|**新建支持请求**    |请求 Microsoft 支持人员提供帮助。   |
 
## <a name="cancel-or-exchange-a-reservation"></a>取消或兑换预订 
当客户的业务需求发生变化时，他们可能想要取消预订，或者兑换预订以获得按比例计算的退款金额，用于支付新预订的价格。 

**如何取消**

客户可以随时取消预订（每年最多取消 50,000 美元)。 通过取消，客户可以将剩余数月的 Azure 预订退还给 Microsoft 以获取提前终止费。 按比例计算的余额在扣除手续费后将退还至客户的原始购买帐户。 

**如何兑换** 

通过兑换，客户可以根据预订的剩余时间期限获得按比例计算的退款，并且可以将退款金额用于购买新的预订。   

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>代表客户请求退款或兑换 

若要代表客户提出退款或兑换支持请求，你需要在合作伙伴仪表板中选择客户和预订，然后在 Azure 门户中创建支持请求。 

>[!NOTE]
>Microsoft 支持代理可能会要求你提供预订 ID 和预订订单 ID。 你可以在 Azure 门户中预订的**属性**页面上找到此信息。 

1. 若要开始，请从你的仪表板菜单中选择**客户**，然后选择想要退款的客户。 

2. 在客户的详细信息页面上，选择 **Azure 预订**，然后选择客户想要退款的特定预订。  

3. 在**操作**下面，选择**退款**以在 Azure 门户中转到客户预订记录并自动启动支持请求。  

4. 在**新建支持请求**页上，请按照以下步骤来请求退款。 执行每个步骤后选择**下一步**。 

|**步骤**   |**选择**    |
|:-----------------------------|:-----------------|
|**1 基础知识**   |问题类型：计费。  |
|**2 问题**   |问题类型：预订管理。 类别：兑换和退款。 |
|**3 联系人信息**   |选择首选项并输入所需的信息。 完成后选择**创建**。   |

## <a name="azure-reservations-resources"></a>Azure 预订资源
|**如需以下相关信息**   |**请阅读以下内容**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [销售 Microsoft Azure 虚拟机预留实例](azure-reservations.md) |
|在合作伙伴仪表板中为客户购买 Azure 预订   |[购买 Azure 预订](azure-reservations-buying.md) |
|Azure 预订计费   |[Azure 预订计费](azure-reservations-billing.md)   |
|确定正确的虚拟机大小，然后确认客户虚拟机使用情况   |[针对最大 Azure 预订利用率确定虚拟机大小](azure-usage.md)   |
|在 Azure 门户中购买 Azure 预订 | Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 门户中管理 Azure 预订   |Azure 帮助中的[管理虚拟机预留实例](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)

