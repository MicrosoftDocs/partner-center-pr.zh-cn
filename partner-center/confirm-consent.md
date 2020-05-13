---
title: 确认客户接受 Microsoft 客户协议
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何确认客户接受 Microsoft 客户协议。 为客户订购 Microsoft 产品和服务时，可能需要这样做。
author: LauraBrenner
ms.author: labrenne
keywords: 客户, 同意, MCA, Microsoft 客户协议, 客户协议模板
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d45f04c8ee1a8d8715f5c6484598ecaca83b1f1
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908152"
---
# <a name="overview-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>概述：确认客户接受 Microsoft 客户协议

**适用于**
-  合作伙伴中心

**相应的角色**

- 管理员代理
- 销售代理

> [!NOTE]
> 目前，协议资源仅受 Microsoft 公有云中合作伙伴中心的支持。 它不适用于：
> * 由世纪互联运营的合作伙伴中心
> * 德国 Microsoft 云合作伙伴中心
> * Microsoft Cloud for US Government 合作伙伴中心

>[!NOTE]
>从 2020 年 1 月 31 日起，所有客户（无论是现有客户还是新客户）都必须签署新的 Microsoft 客户协议。 若要了解详细信息，请参阅[确认客户接受 Microsoft 客户协议](confirm-customer-agreement.md)。

作为合作伙伴，你需要在为客户订购 Microsoft 产品和服务之前确认该客户接受了 Microsoft 客户协议。 为了更好地帮助合作伙伴满足合规性要求，Microsoft 要求合作伙伴通过提供有关接受协议人员的以下详细信息来确认接受协议：

- 名字

- 姓氏

- 电子邮件地址

- 电话号码（可选）

- 接受日期

直接计费合作伙伴和间接提供商在通过合作伙伴中心或合作伙伴中心 API 进行交易时必须确认客户接受了 Microsoft 客户协议。 “确认”为必选项。 

如果没有为给定客户提供确认：

-    你将无法为此客户创建新订单。

-    你将无法为此客户更改现有基于席位的订阅的席位计数。

可以通过合作伙伴中心或合作伙伴中心 API 确认客户接受。 若要通过合作伙伴中心 API 执行此操作，请参阅以下主题： 

-   [获取客户同意的确认](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [获取协议元数据](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [确认客户同意](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


这适用于生产环境和沙盒环境。

## <a name="confirming-customer-acceptance-in-partner-center"></a>在合作伙伴中心中确认客户已接受协议

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>确认新客户接受了协议

在合作伙伴中心中创建新客户租户时，可使用下面的过程来确认客户接受了协议。 请注意，只有管理员代理或销售代理才能执行此操作。

1. 依次选择“客户”、“新客户”、“帐户信息”。   
2. 输入“公司”和“主要联系人”的信息。  

![公司信息](images/mca/mca1.png)

3. 在“Microsoft 客户协议”下，选择“客户已接受最新的 Microsoft 客户协议”。  
4. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。
5. 输入提供接受的用户的详细信息。

![添加接受日期](images/mca/MCA3.png)

默认情况下，将显示主要联系人用户信息。 如果此信息不正确，请选择“更新”，然后输入接受协议的人员的“名字”、“姓氏”、“电子邮件地址”和*“电话号码”（可选）。     

6. 选择“下一步”  ，继续执行创建客户租户的其余步骤。

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>确认现有客户接受了协议

必须是管理员代理或销售代理才能执行此操作。

1. 选择“客户”  ，然后找到并选择要查看的客户。
2. 选择“帐户信息”。 
3. 在“Microsoft 客户协议”下，选择“更新”。  

![更新](images/mca/mca4.png)

4. 输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    
5. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。
6. 选择“保存并继续”。 

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>在为现有客户创建新订单时确认客户接受了协议

如果为之前未确认过是否接受了协议的现有客户创建新订单，你将收到完成确认的提示。 请使用下面的过程执行此操作。

1. 输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    
2. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。
3. 选择“保存并继续”。 

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>为现有客户检索客户接受了协议的确认

可以使用下面的过程为之前提供过确认的现有客户检索客户接受了协议的确认。 必须是管理员代理或销售代理才能执行此操作。

1. 选择“客户”  ，然后找到并选择要查看的客户。
2. 选择“帐户信息”。 
3. 在“Microsoft 客户协议”下，可以看到是否已为此客户提供过确认。 
