---
title: 创建客户关联
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 创建与申报 (CPOR) 型号的客户关联。 有助于管理 Microsoft 365 & Dynamics 365 客户的销售、使用情况、奖励。
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489945"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>针对 Microsoft 365 和 Dynamics 365，通过声明的记录 (CPOR) 模型的客户关联


**适当的角色**：激励管理员

2019年10月1日，Microsoft 开始使用 "CPOR 的申报合作伙伴" ("") 模型来管理与 Microsoft 365 和 Dynamics 365 客户之间的关联，和 Dynamics 客户与在线服务咨询) 相关， ("

>[!Important]
> 客户关联 (CPOR) 声明仅适用于在线服务咨询 (OSA) 销售、在线服务使用 (OSU) Microsoft 365 和 OSU-Business 应用程序奖励计划。 如果要为其他程序（如云解决方案提供商 (CSP) 、托管经销商、托管或 Surface）提交合作声明，请参阅此处所述的合作声明过程。 <br><br>提交声明时，Microsoft 将对其进行验证。 此时，我们可能会要求你提供详细信息。 我们还将通知客户你的关联请求。 客户需要5个工作日来选择退出。如果未选择退出，则与此特定租户和工作负荷的关联将为官方。 此时，你将可以访问客户的使用情况数据。 

你将需要以下信息来完成声明：

- **MPN id** (构成声明的实体 Microsoft 合作伙伴网络 id) 

- 客户的 **域名** (有关详细信息，请参阅 [查找租户 ID、域名、用户对象 ID](find-ids-and-domain-names.md)) 

- 客户的 **目录 id** 或 **租户 id** (有关详细信息，请参阅 [查找租户 ID、域名、用户对象 ID](find-ids-and-domain-names.md)) 

- **解决方案区域**，如 Business Applications 或 Microsoft 365

- 已执行的 **活动** 和要进行的声明的类型，例如售前、使用情况或收入关联

- 你的客户的 **联系人姓名**、标题和电子邮件地址

- 对于 Dynamics 365，还需要提供客户的 **技术联系人** 姓名、职务和电子邮件地址

- 自己公司的 **联系人姓名** 和电子邮件地址

- 你将为此声明创建 **名称**

- **产品 ()** 或 () 你所申报的工作负荷

- **(PoE) 的执行证明**，如客户签署的工作声明。 你还可以下载要使用的 PoE 模板。

- 仅适用于申报收入关联的合作伙伴： **Dynamics 解决方案卖方名称**、 **客户名称** 和 **ISV 产品/解决方案的名称**。 

还应了解以下要点：

- 如果现有 Microsoft 365 客户，则需要使用此过程重新关联要继续获得 OSU 激励的客户。

- 如果现有与 Dynamics 365 或 Power BI 客户的关联，则这些关联将保持有效，直到其订阅过期。

- 一个客户可以具有多个合作伙伴，但每个工作负荷 (适用于 OSA-Sell 和 OSU-Business 应用程序的 OSU-Microsoft 365) 或订阅 (，) 只能与一个合作伙伴关联。

## <a name="create-a-customer-association"></a>创建客户关联

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。

2. 选择 " **激励** " 选项卡，选择 " **概述**"，然后选择 " **客户关联**"。

3. 在 "客户关联" 页的顶部，选择 " **+ 客户关联**"。

4. 选择要与客户关联的合作伙伴位置的 MPN ID，然后添加客户的域名和目录 ID。 [查找此](find-ids-and-domain-names.md)

5. 选择“继续”。

6. 选择 **解决方案区域** 和 **活动**。 

   >[!Note]
   >
   >如果选择 "Business Applications"，请选择 " **使用情况" 和/或 "提前销售**" 或 " **收入关联**"，然后选择 " **继续**"。 
   <br><br>如果选择“收入关联”，系统将提示你输入与下面所列信息稍有不同的信息。

7. 在 " **关联客户** " 页上输入相应信息，然后选择 " **创建声明**"。

8. 选择与此客户关联关联的产品 () ，然后选择 " **继续**"。

9. 填写客户联系信息和你公司的联系信息。 所有字段都是必填字段。 

   >[!NOTE]
   >如果你的产品是 Dynamics 365，并且你选择的产品有多个订阅用于此特定客户，则还需要输入订阅 ID。

10. 提供你的 PoE。 可以将其拖到框中，浏览找到自己的支持性文档，或通过选择“下载模板”来使用模板。 

11. 根据需要添加并保存注释，然后选择“提交声明”。 我们将向客户发送一封电子邮件，请求批准客户关联。

   >[!NOTE]
   >提交客户关联后，不能对其进行编辑。

客户关联的状态显示在“状态”字段中。

选择“历史记录”查看客户关联的历史记录。

## <a name="next-steps"></a>后续步骤

- [管理客户关联](incentives-manage-customer-associations.md)