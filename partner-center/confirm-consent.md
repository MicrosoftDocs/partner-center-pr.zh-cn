---
title: 确认 Microsoft 云协议客户接受 |合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: 客户、 客户、 同意
ms.localizationpriority: medium
ms.openlocfilehash: baab5e0fb3ac01284b210a2059b006ee2e17f921
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795280"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>确认客户接受 Microsoft 云协议

**适用范围**
-  合作伙伴中心

作为合作伙伴，你需要获取你的客户接受 Microsoft 云协议，然后才可订购 Microsoft 产品和服务使客户。 更好地帮助合作伙伴满足合规性，Microsoft 要求合作伙伴以确认接受通过提供有关接受协议的人员的以下详细信息： 

-   名字

-   姓氏

-   电子邮件地址

-   电话号码

-   接受的日期

若要了解详细信息，请参阅[Microsoft 云协议客户接受确认常见问题](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq)。

## <a name="schedule"></a>计划

**2018 年 8 月 7日日**

-   直接计费的合作伙伴和间接提供商可以确认客户接受 Microsoft 云协议。 确认为*可选*参数。

-   可以通过合作伙伴中心或合作伙伴中心 API 的客户接受确认。

-   客户接受确认仅支持通过 Microsoft 公有云。


**2018 年 11 月 7日日**

-   直接计费的合作伙伴和间接提供商**必须**确认客户接受 Microsoft 云协议。 确认是*必需项*。

-   如果没有为给定客户提供确认：

    -   你将无法创建此客户的新订单。

    -   你将无法更改此客户的现有基于席位的订阅的席位计数。

-   可以通过合作伙伴中心或合作伙伴中心 API 的客户接受确认。

-   客户接受确认仅支持通过 Microsoft 公有云。


## <a name="confirming-customer-acceptance-in-partner-center"></a>确认在合作伙伴中心中的客户接受

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>确认客户接受新客户

使用以下过程来确认客户接受，尽管你在合作伙伴中心中创建一个新的客户租户。 请注意，你必须是管理员代理或销售代理要执行此操作。 
1.  选择**客户**，然后**新客户**。

2.  输入**公司**和**主要联系人**信息。

3.  **Microsoft 云协议**，选择**客户已接受的最新的 Microsoft 云协议**。 

4.  在**协议接受日期**输入相应的日期。 不能将其设置到将来的日期。

5.  输入提供接受的用户的详细信息。 

    默认情况下，显示的主要联系人的用户信息。 如果这不正确，请选择**更新**，然后输入**名字**、**姓氏**、**电子邮件地址**，以及 **电话号码*（可选） 接受协议的人员。

    **注意：** 之前确认客户接受变为必需的你可能会跳过确认不选择**客户已接受的最新的 Microsoft 云协议**，该选项，然后选择**下一步**。

6.  选择**下一步**继续创建客户租户的剩余步骤。

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>确认客户接受为现有客户

你必须是管理员代理或销售代理才能执行此操作。 

1.  选择**客户**，然后找到并选择你想要查看的客户。 

2.  选择**帐户**。

3.  **Microsoft 云协议**，选择**更新**。

4.  输入**名字**、**姓氏**、**电子邮件地址**和**电话号码**（可选） 的用户的接受协议。

5.  在**协议接受日期**输入相应的日期。 不能将其设置到将来的日期。

6.  选择**保存并继续**。

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>确认客户接受时创建的现有客户的新订单

如果你尝试创建为现有客户的前不确认你已新订单，你将收到一条提示，以完成确认。 使用以下过程来执行此操作。 

1.  输入**名字**、**姓氏**、**电子邮件地址**和**电话号码**（可选） 的用户的接受协议。

2.  在**协议接受日期**输入相应的日期。 不能将其设置到将来的日期。

3.  选择**保存并继续**。

**注意：** 确认客户接受变为必需之前，你可以通过选择**取消**跳过确认。

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>检索确认客户接受为现有客户

你可以检索确认客户接受为现有客户具有提供以前使用下面的过程。 你必须是管理员代理或销售代理才能执行此操作。 

1.  选择**客户**，然后找到并选择你想要查看的客户。 

2.  选择**帐户**。

3.  **Microsoft 云协议**，你将看到确认已提供此客户。

