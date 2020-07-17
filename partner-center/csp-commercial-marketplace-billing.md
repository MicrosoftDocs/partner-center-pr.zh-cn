---
title: 商业应用商店产品的帐单
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何针对从合作伙伴中心内的商业市场为客户购买的 ISV SaaS 产品或订阅付费。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7625488266aab3eb8d1797a99847eaec56ced36f
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435136"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>适用于合作伙伴中心的商业 marketplace 产品和订阅的帐单

**适用于**

- 合作伙伴中心
- 云解决方案提供商计划中的合作伙伴

**相应的角色**

- 全局管理员
- 计费管理员

作为 CSP 计划中的合作伙伴，你可以使用合作伙伴中心从商业应用商店中的 ISV 出版商那里购买基于许可证的 SaaS 产品。 完成此操作后，你可以访问这些类型采购的帐单。 计费周期从日历月的第一天开始，到日历月的最后一天结束。 发票在下个月的第8天可用。

你可以通过合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/)或使用[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/)访问发票。

CSP 计划中的合作伙伴需要为客户购买的 ISV 商用 marketplace 解决方案收费，当他们从合作伙伴中心或从 Azure 门户购买这些产品（使用客户以前的 CSP 购买的 Azure 租户）。

>[!NOTE]
>如果客户使用其自己的 Azure AD 租户（不是从 CSP 计划中的合作伙伴购买的租户），则客户还可以选择直接从（[Microsoft AppSource](https://appsource.microsoft.com/)或[Azure Marketplace](https://azuremarketplace.microsoft.com/)）购买自己的 ISV SaaS 解决方案。 如果他们这样做，他们将直接从 Microsoft 接收自己的帐单。 同样，如果 CSP 计划中的合作伙伴向客户销售 Azure 订阅或新的 Azure 计划，并向客户（或间接经销商）授予对该租户的[基于角色的访问权限](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)（向除**读者**以外的客户分配任何角色），则该客户（或间接经销商）还可以购买商业 marketplace 产品/服务，而不需要事先批准或通知 CSP 合作伙伴。 在这种情况下，Microsoft 不会直接在 CSP 计划中向合作伙伴通知客户的购买情况。 但是，Microsoft 提供了一个可选的[Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)机制，可用于设置有关 Azure 订阅上的活动的警报或通知。

## <a name="access-billing-information-for-commercial-marketplace-products"></a>访问商业 marketplace 产品的计费信息

当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。 若要访问商业 marketplace 产品购买的最新发票和对帐文件，请执行以下操作：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/)。

2. 在“合作伙伴中心”菜单中，选择“计费”。 

    你将在帐单页的顶部看到两个选项卡：**定期**、**定期和一次性购买**。 每个选项卡允许您访问不同 marketplace 产品的发票和对帐（侦测）文件：

    - "**定期**" 选项卡：显示与 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、PowerBI Pro 和 Microsoft Azure 相关的订阅的发票和对帐文件。

    - **定期和一次性购买**选项卡：显示 azure 计划、azure 预订、软件和商业应用商店产品的发票和对帐文件。
  
3. 选择 "**定期购买" 和 "一次性购买**" 选项卡。如果为客户购买了不同货币的订阅，则会看到每个货币的选项卡。 你可以执行以下操作： om 此页：

    - 若要查看最新的发票和协调文件，请选择 "**发票**" 或 "**对帐文件**"。 （如果需要，还可以使用[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/)访问最新的发票和侦测文件数据。

    - 若要查看以前的发票和侦测文件，请展开下面的 "**帐单历史记录**" 行。

    - 若要根据最新的帐户活动，随时查看估计的帐户余额或帐单，请在 "**估计**" 标题下选择一个链接。  

    >[!NOTE]
    > 当我们在每月的第8天发布帐单时，它将包含税金以及任何其他适用的费用和信用额度。 这意味着最终的应付金额可能不同于计费期间的显示内容。

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>有关商业 marketplace 产品的发票和侦测文件的详细信息

本部分提供了有关为第三方 ISV 发布者购买的商业 marketplace SaaS 订阅的发票和对帐文件的详细信息。

当你从 "合作伙伴中心" 菜单中的 "**计费**" 选项中选择 "**定期购买" 和 "一次性购买**" 时，你将获得对与 Microsoft （第一方）和 ISV （第三方）购买相关的费用的发票和协调文件的访问权限。 这些购买可能会与相关联：

- SaaS 订阅（来自 Microsoft 或 ISV 发布者）

- Azure 计划

- Azure 预留项

- 其他基于订阅的软件（来自 Microsoft 或 ISV 发布者）

这些购买的示例可能包括 SUSE Linux 软件（软件订阅）或 Azure ISV SaaS 产品订阅。

>[!NOTE]
> 有关如何读取发票和侦测文件的详细信息，请参阅[帐单概述](billing.md)。

### <a name="tips-on-reading-your-invoice"></a>阅读发票提示

从第三方 ISV 发布商处购买基于许可证的 SaaS 产品时，你只会看到发票上的许可费用收费。 即使 ISV 的 SaaS 产品使用（或使用）底层 Azure 基础结构资源，也是如此。 这是因为，对 isv 的 SaaS 产品的客户的 Azure 基础结构用量收费直接向 ISV 收费。 （Isv 会在其自己的 Azure 使用情况-每日级别的发票对帐文件中看到关联的 Azure 消耗收费。）

你的发票将包含多个页面：

- **发票第1页：** 包含 CSP 计划合作伙伴的计费详细信息的摘要概述。 这包括计费周期的费用摘要、发票编号、支付条款（净60天）以及通过线路或支票支付的帐单支付方法。

- **发票的第2页（以及所有后续页面）：** 从商业性 marketplace 购买第一方 Microsoft 购买和第三方 ISV （基于许可证）的费用。 可以通过每个产品名称下的**发布者**行标识基于 ISV 许可证的购买。 关联的对帐文件为特定发票费用提供更多计费详细信息。

- **发票的最后一页：** 如果你使用 ISV 提供的基于许可证的 marketplace 产品收费，此最后一页将显示有关 ISV 发布者的姓名和地址的详细信息。

### <a name="tips-on-reading-your-reconciliation-file"></a>有关读取对帐文件的提示

**定期和一次性采购**对帐文件包含多个列，其中包含映射到发票中的费用的其他详细信息。 **PublisherName**列显示购买是来自 Microsoft 还是第三方 ISV 发布者。

对帐文件的某些费用可能会显示为 $0。 这可能是由于 ISV "免费试用版" 产品/服务（通常为30或60天）或自带许可提供。

对于免费试用版 ISV，请提供：

- 免费试用期涵盖了在此期间 ISV 基于许可证的 SaaS 产品的成本。 对于关联的 Azure 基础结构使用该 SaaS 产品，还不会向你收费。  但是，如果使用基于使用情况的 ISV 产品/服务，则免费试用版不包括基础 Azure 基础结构的使用成本。 在这种情况下，Azure 基础结构使用费用将显示在单独的 Azure 对帐文件中。

- 当你为客户购买并部署 ISV 的免费试用版产品时，客户将自动注册到 ISV 发布者的免费试用版。 免费试用期将在 ISV 发布者定义的时间段后自动结束。 该时间段结束后，将向客户收费。 这意味着，对等认证的产品可能会显示两行：一个跟踪试用期的行和一个跟踪付费产品/服务的行（在试用期结束之前，将显示成本为 $0）。 试用期结束后，显示付费产品/服务的行将开始显示费用。 

有关每个列代表的内容的详细信息，请参阅[使用对帐文件](use-the-reconciliation-files.md)。 另请参阅[合作伙伴中心的计费类型](billing-different-types.md)

## <a name="next-steps"></a>后续步骤

- [为客户管理商业 marketplace 产品](csp-commercial-marketplace-manage.md)
- [了解对商业 marketplace 产品的支持](csp-commercial-marketplace-support.md)
