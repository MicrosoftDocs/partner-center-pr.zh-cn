---
title: 在 合作伙伴中心
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何为客户销售 Microsoft 发布的产品以及第三方 ISV 发布的 SaaS 产品的订阅。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201402"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>创建、暂停或取消客户订阅

**适用于 ：** 合作伙伴中心 |合作伙伴中心Microsoft Cloud for US Government

**适当的角色**：管理员代理|计费管理员|全局管理员|支持人员代理|销售代理

在合作伙伴中心中创建客户的记录后，你可以向他们销售目录中产品的订阅。 这包括 Microsoft 发布的产品以及软件即服务 (SaaS) 产品，这些产品由第三方独立软件供应商 (ISV) 商业市场[发布。](https://azuremarketplace.microsoft.com/marketplace)

某些套餐仅限每个客户的一个订阅。 若要查看受限制的套餐列表，请访问合作伙伴中心定价和套餐页面。

>[!IMPORTANT]
> 作为 CSP 计划的合作伙伴，可以从云解决方案提供商的 ISV发布者购买基于许可证或按流量计费的 SaaS 合作伙伴中心。 这意味着，你可以购买 ISV 发布者提供给你的任何基于许可证或按流量计费的 **SaaS** 产品/服务 [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)，包括你有权访问的独占产品/服务。  若要从 ISV 购买或管理其他商业市场产品/服务 (例如涉及 Azure 应用程序、容器或 VM) 的基于使用情况的产品/服务，必须转到[Azure 门户。](https://portal.azure.com/)

>[!NOTE]
>所有日期和时间在 合作伙伴中心 UTC 协调世界时标准 () 给定。 这可能与本地时间最多相差 24 小时。

## <a name="create-a-new-subscription"></a>创建新订阅

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择“添加订阅”。 " **联机服务"** 选项卡将显示所有可用的市场 SaaS 产品/服务。

4. 若只要查看特定类型的订阅，请在可用筛选器中进行选择：
   - **发布者**： **选择"Microsoft"** 仅查看来自 Microsoft 的产品/服务 **，或选择** "合作伙伴"查看 ISV 发布的商业市场产品。
   - **计费类型**：选择想要使用的订阅计费类型： **许可证** 或 **使用情况**。 请参阅 [基于许可证的](license-based-billing.md) 计费，了解有助于在每月和按年计费频率之间做出决定的信息。
   - **类别**：选择 **"企业****"、"小型企业"** 或"**试用"。** 若要了解试用版订阅，请参阅[为客户提供 Microsoft 产品试用版](offer-your-customers-trials-of-microsoft-products.md)。

5. 选择要为客户购买的产品订阅。 所看到的产品取决于客户段的类型 (教育、政府等 ) 和应用的筛选器。 Marketplace 上显示的某些产品/服务可能并不总是用于特定客户或特定的 CSP 合作伙伴。 这可能是因为：

   - 该客户已订阅该产品，只允许使用一个

   - 客户的订阅可能已挂起 (在这种情况下，您可以重新激活订阅，而不是购买新订阅。 ) 

   - 对于 ISV SaaS 产品/服务，可能有几个原因无法购买产品/服务： ISV 可能不支持客户的计费国家或地区;ISV 可能已选择不通过 CSP 计划提供产品/服务;或者，ISV 可能已 [仅向特定的 CSP](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 合作伙伴提供产品/服务。 还可以通过合作伙伴中心 (（例如，容器或某些基于使用情况的产品/) 服务）来事务 ISV 产品/服务。  

6. 对于要添加的每个订阅，请在需要时输入 (的许可证数量) 并选择 " **添加到购物车**"。

7. 添加完订阅后，请选择 " **查看** 并查看你的订单"。

8. 查看订单并准备好购买这些订阅后，选择 " **购买**"。

9. 为客户购买订阅后，将发生以下情况：

    - 您可以通过从该客户的 " **订阅** " 页中选择订阅名称来查看或编辑该订阅。 在这里，可以选择附加许可证（如果有）、更改许可证数量，或者暂停订阅。

    **对于 ISV SaaS (基于许可证并按流量计费) 订阅：**
    - 你将收到 ISV 发布者网站的链接。 此链接应有助于你完成客户订阅的部署或帐户设置。
      
    >[!NOTE]
    > 你和你的客户都不会收到一封电子邮件，其中包含为此类型的 ISV 订阅设置/预配的说明。 ) 

    - 如果订阅附带30天的免费试用版，则将自动应用免费试用期。 作为 CSP 计划的合作伙伴，你无法放弃为客户购买的产品/服务的免费试用期。 免费试用期结束后，订阅期限将开始，订阅将转换为付费状态。 然后，订阅将按照相同的计划自动续订。
   
## <a name="update-subscriptions-with-add-ons"></a>更新具有加载项的订阅 

若要购买加载项，客户必须先拥有有效的基本订阅。  无法通过目录购买加载项。

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择要管理的订阅。

4. 在 **"状态** "部分下，是订阅的可用加载项列表。  

5. 更新每个必需加载项的许可证数量。 然后“提交”更改  。

通过直接计费和间接提供商合作伙伴中心购买加载项的能力。
仅根据基本要求和区域可用性显示符合条件的加载项。 有关定价和产品/服务的详细信息，请参阅云经销商产品/服务矩阵。 暂停基本订阅也将暂停任何关联的加载项。

加载项的开始日期与基本订阅保持一致，费用根据费用开始日期和费用结束日期计算，在第一张发票中按比例计费。 有关其他信息，请参阅基于 [许可证的计费](license-based-billing.md)。


## <a name="suspend-or-cancel-a-subscription"></a>暂停或取消订阅

在客户提出申请，或者在未付款或欺诈的情况下，合作伙伴可以暂停或取消订阅。

### <a name="suspend-a-subscription"></a>暂停订阅

当你将订阅状态更改为“已暂停”时，用户将无法登录或访问服务。

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择要管理的订阅。

4. 在“状态”部分，选择“已暂停”   。 然后“提交”更改  。

5. 除非在 90 天内或在 90 天加上帐户开具时间与第一个计费周期之间的天数内（最长 120 天）重新激活订阅，否则所有数据将被删除。

暂停订阅后，你在“暂停”按钮下看到的日期即是在不重新激活订阅的情况下，该订阅的自动过期日期。 

>[!NOTE]
>CSP 订阅没有过期期限 (Web 直接订阅) 在此期间服务仍在运行，但订阅不会产生任何计费费用。 CSP 订阅是活动订阅或挂起 (或完全删除) 。

### <a name="cancel-a-subscription"></a>取消订阅

可以从商业市场 内的第三方 ISV 发布者取消基于许可证合作伙伴中心 [订阅](csp-commercial-marketplace-overview.md)。 只要在取消期内取消，你将收到完全退款。

对于 ISV 产品/服务，按月计费：

- 如果在下单后的 24 小时内取消，将在下一张发票上收到完整额度。

- 如果在下单后的 24 小时后取消，则取消将安排在续订时发生。

对于按年计费的优惠：

- 如果在下单后的 14 天内取消，将在下一张发票上收到完整额度。

- 如果在下单后的 14 天内取消，则取消将安排在续订时发生。

在这些时间段结束后，你将无法再看到取消订阅的选项。

> [!NOTE]
> 使用虚拟机或容器的基于使用情况和计量的第三方 ISV 服务 (，例如) 不适合返回。 基于使用情况的服务可以取消预配为取消方法。 由于在使用后费用会计费，因此这些服务没有资格获得退款。

若要从 ISV 发行商取消基于许可证的 SaaS 订阅，请执行以下操作：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 找到要取消的订阅。

4. 在 " **状态** " 列中，选择 " **取消**"。 然后“提交”更改  。

5. 如果出现一个对话框，请填写所有相关的详细信息，然后选择 " **提交**"。

6. 若要确认取消，请选择 **"是，取消**"。

> [!NOTE]
> 还可以选择使用 Api 取消 Azure Marketplace 订阅。 为此，请参阅 [取消 Azure Marketplace 订阅](/partner-center/develop/cancel-an-azure-marketplace-subscription)。

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>选择是否自动续订商业市场订阅

默认情况下，活动订阅设置为订阅期限过期时自动续订。 对于 [商业 marketplace 产品订阅](csp-commercial-marketplace-overview.md)，你可以选择不自动续订订阅。

若要阻止有效的商业市场订阅自动续订：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 选择“订阅”。 这会列出已为客户购买的任何基于许可证的订阅。

4. 在 " **订阅** " 列中，选择要修改的订阅。

5. 在 "订阅详细信息" 页中，找到 " **状态** " 部分并取消选中 " **自动续订** " 框。

6. 选择“提交”。

## <a name="next-steps"></a>后续步骤

- [为客户购买商业市场产品](csp-commercial-marketplace-purchase.md)

- [为客户管理商业 marketplace 产品](csp-commercial-marketplace-manage.md)

- [商业市场概述](csp-commercial-marketplace-overview.md)