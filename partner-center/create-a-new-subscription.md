---
title: 在合作伙伴中心创建客户订阅
ms.topic: article
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何向 Microsoft 发布的产品以及第三方 Isv 发布的 SaaS 产品销售客户订阅。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3e154fd217af8ca0f5d45c686467e671e5bd9a03
ms.sourcegitcommit: f8e8803b7d9fdf801ba181015a07dc6b570621c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "86949833"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>创建、暂停或取消客户订阅

**适用于**

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心
- 云解决方案提供商合作伙伴

**相应的角色**

- 管理员代理
- 计费管理员
- 全局管理员
- 支持人员代理
- 销售代理

在合作伙伴中心中创建客户的记录后，你可以向他们销售目录中产品的订阅。 这包括 Microsoft 发布的产品以及由第三方独立软件供应商（Isv）发布的软件即服务（SaaS）产品到[商业市场](https://azuremarketplace.microsoft.com/marketplace)。

某些产品/服务仅限每个客户一个订阅。 若要查看受限制的套餐列表，请访问合作伙伴中心定价和套餐页面。

> [!IMPORTANT]
> 作为 CSP 计划中的合作伙伴，只能从合作伙伴中心内的 ISV 发布者购买**基于许可证的**SaaS 订阅。 这意味着你可以购买 ISV 发布者提供的任何**基于许可证**的 SaaS 产品/服务，包括你有权访问的[独家产品/服务](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)。 若要购买或管理其他商业市场，请参阅 Isv 提供的产品/服务（例如**基于使用情况**、按流量计费或基于消耗的产品/服务，包括 azure 应用程序、容器或 vm），你必须使用[azure 管理门户](https://portal.azure.com/)。 有关详细信息，请参阅[购买商业 marketplace 产品](csp-commercial-marketplace-purchase.md)。

## <a name="create-a-new-subscription"></a>创建新订阅

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择“添加订阅”****。 "**联机服务**" 选项卡将显示所有可用的 Marketplace SaaS 产品/服务。

4. 若只要查看特定类型的订阅，请在可用筛选器中进行选择：
   - **发布者**：选择**microsoft**仅查看来自 microsoft 或**合作伙伴**的产品/服务，以查看由 isv 发布的商业 marketplace 产品。
   - **计费类型**：选择要使用的订阅计费类型： "**许可证**" 或 "**使用情况**"。 请参阅[基于许可证的计费](license-based-billing.md)，了解可帮助您决定每月和每年计费频率的信息。
   - **类别**：选择 "**企业**"、"**小企业**" 或 "**试用**"。 若要了解试用版订阅，请参阅[为客户提供 Microsoft 产品试用版](offer-your-customers-trials-of-microsoft-products.md)。

5. 选择要为客户购买的产品订阅。 所看到的产品取决于客户段的类型（教育、政府等）和应用的筛选器。 Marketplace 上显示的某些产品/服务可能并不总是用于特定客户或特定的 CSP 合作伙伴。 这可能是因为：

   - 该客户已订阅该产品，只允许使用一个

   - 客户的订阅可能已挂起（在这种情况下，您可以重新激活订阅，而不是购买新订阅。）

   - 对于 ISV SaaS 产品/服务，可能有几个原因无法购买产品/服务： ISV 可能不支持客户的计费国家或地区;ISV 可能已选择不通过 CSP 计划提供产品/服务;或者，ISV 可能已[仅向特定的 CSP](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)合作伙伴提供产品/服务。 ISV 产品/服务可能也不会通过合作伙伴中心事务（例如，容器或某些基于使用情况的产品/服务）。  

6. 对于要添加的每个订阅，输入许可证数量（如果需要），并选择 "**添加到购物车**"。

7. 添加完订阅后，请选择 "**查看**并查看你的订单"。

8. 查看订单并准备好购买这些订阅后，选择 "**购买**"。

9. 为客户购买订阅后，将发生以下情况：

    - 您可以通过从该客户的 "**订阅**" 页中选择订阅名称来查看或编辑该订阅。 在这里，可以选择附加许可证（如果有）、更改许可证数量，或者暂停订阅。

    **对于 ISV SaaS （基于许可证）订阅：**
    - 你将收到 ISV 发布者网站的链接。 此链接应有助于你完成客户订阅的部署或帐户设置。
      
    >[!NOTE]
    > 你和你的客户都不会收到一封电子邮件，其中包含为此类型的 ISV 订阅设置/预配的说明。）

    - 如果订阅附带30天的免费试用版，则将自动应用免费试用期。 作为 CSP 计划中的合作伙伴，你不能停征你为客户购买的产品/服务的免费试用期。 在免费试用期结束后，订阅期限将开始，订阅将转换为付费状态。 然后，订阅将根据相同的计划自动续订。
   
## <a name="update-subscriptions-with-add-ons"></a>用加载项更新订阅 

若要购买外接程序，客户必须首先具有活动的基本订阅。  不能通过目录购买加载项。

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择要管理的订阅。

4. 在 "**状态**" 部分下，是订阅的可用加载项列表。  

5. 更新每个所需外接程序的许可证数量。 然后“提交”更改  。

通过合作伙伴中心购买加载项的能力仅适用于直接帐单和间接提供商。
仅根据基本要求和区域可用性显示符合条件的加载项。 有关定价和产品/服务的详细信息，请参阅云分销商产品列表。  暂停基本订阅还会挂起任何关联的外接程序。

外接程序的开始日期将与基本订阅进行对齐，并在第一张发票中从 "费用开始日期" 和 "费用结束日期" 计算，按每收费。 有关其他信息，请参阅[基于许可证的计费](license-based-billing.md)。


## <a name="suspend-or-cancel-a-subscription"></a>暂停或取消订阅

在客户提出申请，或者在未付款或欺诈的情况下，合作伙伴可以暂停或取消订阅。

### <a name="suspend-a-subscription"></a>暂停订阅

当你将订阅状态更改为“已暂停”**** 时，用户将无法登录或访问服务。

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择要管理的订阅。

4. 在“状态”部分，选择“已暂停”   。 然后“提交”更改  。

5. 除非在 90 天内或在 90 天加上帐户开具时间与第一个计费周期之间的天数内（最长 120 天）重新激活订阅，否则所有数据将被删除。

暂停订阅后，你在“暂停”**** 按钮下看到的日期即是在不重新激活订阅的情况下，该订阅的自动过期日期。 

### <a name="cancel-a-subscription"></a>取消订阅

你可以选择从合作伙伴中心[商业市场](csp-commercial-marketplace-overview.md)中的第三方 ISV 发布者处取消基于许可证的 SaaS 订阅。 只要你在取消期限内取消，你就会获得全额退款。

对于按月计费的 ISV 产品/服务：

- 如果您在下一次订单后取消了24小时，则您将在下一张发票上收到完全信用额度。

- 如果您在下一次订单后的24小时内取消，则会计划在续订时进行取消。

每年按优惠收费：

- 如果您在订购订单后取消14天，则您将在下一张发票上收到完全信用额度。

- 如果您在下一次订单后取消了14天，则会计划在续订时进行取消。

在这些时间段结束后，你将无法再看到取消订阅的选项。

> [!NOTE]
> 使用基于使用情况和计量的第三方 ISV 服务（例如，使用虚拟机或容器的服务）不适合返回。 基于使用情况的服务可以取消预配为取消方法。 由于在使用后费用会计费，因此这些服务没有资格获得退款。

若要从 ISV 发行商取消基于许可证的 SaaS 订阅，请执行以下操作：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 找到要取消的订阅。

4. 在 "**状态**" 列中，选择 "**取消**"。 然后“提交”更改  。

5. 如果出现一个对话框，请填写所有相关的详细信息，然后选择 "**提交**"。

6. 若要确认取消，请选择 **"是，取消**"。

> [!NOTE]
> 还可以选择使用 Api 取消 Azure Marketplace 订阅。 为此，请参阅[取消 Azure Marketplace 订阅](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)。

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>选择是否自动续订商业市场订阅

默认情况下，活动订阅设置为订阅期限过期时自动续订。 对于[商业 marketplace 产品订阅](csp-commercial-marketplace-overview.md)，你可以选择不自动续订订阅。

若要阻止有效的商业市场订阅自动续订：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择“订阅”。 这会列出已为客户购买的任何基于许可证的订阅。

4. 在 "**订阅**" 列中，选择要修改的订阅。

5. 在 "订阅详细信息" 页中，找到 "**状态**" 部分并取消选中 "**自动续订**" 框。

6. 选择“提交”。

## <a name="next-steps"></a>后续步骤

- [为客户购买商业市场产品](csp-commercial-marketplace-purchase.md)

- [为客户管理商业 marketplace 产品](csp-commercial-marketplace-manage.md)

- [商业市场概述](csp-commercial-marketplace-overview.md)
