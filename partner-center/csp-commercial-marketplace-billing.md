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
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148017"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>适用于合作伙伴中心的商业 marketplace 产品和订阅的帐单


**适当的角色**：全局管理员 |计费管理员

作为 CSP 计划中的合作伙伴，你可以使用合作伙伴中心从商业应用商店中的 ISV 出版商那里购买基于许可证的 SaaS 产品。 完成此操作后，你可以访问这些类型采购的帐单。 计费周期从日历月的第一天开始，到日历月的最后一天结束。 发票在下个月的第8天可用。

你可以通过合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/) 或使用 [合作伙伴中心 api](/partner-center/develop/)访问发票。

CSP 计划中的合作伙伴需要为客户购买的 ISV 商用 marketplace 解决方案收费，当他们从合作伙伴中心或从 Azure 门户 (使用客户以前购买的 Azure 租户) 购买这些产品。

>[!NOTE]
>如果客户使用他们自己的 Azure AD 租户 (不是从 CSP 计划中的合作伙伴那里购买的) ，则客户还可以选择直接从 ([Microsoft AppSource](https://appsource.microsoft.com/) 或 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) 购买自己的 ISV SaaS 解决方案。 如果他们这样做，他们将直接从 Microsoft 接收自己的帐单。 同样，如果 CSP 计划中的合作伙伴向客户销售 Azure 订阅或新的 Azure 计划，并授予客户 (或间接分销商) 对该租户的 [基于角色的访问权限](/azure/role-based-access-control/built-in-roles) (向客户分配除 **读者**) 以外的任何角色，则该客户 (或间接经销商) 还可以购买商业 marketplace 产品/服务，而不需要事先批准或通知 CSP 合作伙伴。 在这种情况下，Microsoft 不会直接在 CSP 计划中向合作伙伴通知客户的购买情况。 但是，Microsoft 确实 [提供了](/azure/azure-monitor/platform/alerts-activity-log) Azure Monitor，可用于设置有关 Azure 订阅上的活动的警报或通知。

## <a name="access-billing-information-for-commercial-marketplace-products"></a>访问商业市场产品的计费信息

当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。 访问商业市场产品购买的最新发票和对帐文件：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/)。

2. 在“合作伙伴中心”菜单中，选择“计费”。 

    "计费"页顶部有两个选项卡："定期"和"定期"和 **"一次性购买"。** 通过每个选项卡，可以访问发票 (对帐) 不同市场产品的对帐文件：

    - **"** 定期"选项卡：显示与 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、Power BI Pro 和 Microsoft Azure 相关的订阅的发票和对帐文件。

    - **定期和一次性购买** 选项卡：显示 Azure 计划、Azure 预留、软件和商业市场产品的发票和对帐文件。
  
3. 选择" **定期和一次性购买"** 选项卡。如果以其他货币为客户购买了订阅，则会看到每种货币的选项卡。 可以从此页面执行一些操作：

    - 若要查看最新的发票和对帐文件，请选择"**发票或****对帐文件"。**  (如果需要，还可使用 API 访问最新的发票 [和合作伙伴中心数据](/partner-center/develop/)。

    - 若要查看较早的发票和对帐文件，请展开下面的 **"计费历史记录"** 行。

    - 若要随时根据最新的帐户活动检查估计的帐户余额或帐单，请在"估计"标题下 **选择一个** 链接。  

    >[!NOTE]
    > 当我们在当月的第 8 天发布帐单时，它将包括税款以及任何其他适用的费用与额度。 这意味着最终到期金额可能与计费周期内看到的金额不同。

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>详细了解商业市场产品的发票和重新确认文件

本部分提供了有关为第三方 ISV 发布者购买的商业 marketplace SaaS 订阅的发票和对帐文件的详细信息。

当你从 "合作伙伴中心" 菜单中的 "**计费**" 选项中选择 "**定期购买" 和 "一次性购买**" 时，你将获得对发票和协调文件的访问权限，以获取与 Microsoft (第一方) 和 ISV (第三方) 购买相关的费用。 这些购买可能会与相关联：

- Microsoft 或 ISV 发布者 (的 SaaS 订阅) 

- Azure 计划

- Azure 预留项

- 来自 Microsoft 或 ISV 发布者的其他基于订阅的软件 () 

这些购买的示例可能包括 SUSE Linux 软件 (软件订阅) 或 Azure ISV SaaS 产品订阅。

>[!NOTE]
> 有关如何读取发票和侦测文件的详细信息，请参阅 [帐单概述](billing.md)。

### <a name="tips-on-reading-your-invoice"></a>阅读发票提示

从第三方 ISV 发布商处购买基于许可证的 SaaS 产品时，你只会看到发票上的许可费用收费。 即使 ISV 的 SaaS 产品使用 (或使用) 底层 Azure 基础结构资源，也是如此。 这是因为，对 isv 的 SaaS 产品的客户的 Azure 基础结构用量收费直接向 ISV 收费。  (Isv 会在其自己的 Azure 使用情况的每日评级发票对帐文件中看到关联的 Azure 消耗费用。 ) 

你的发票将包含多个页面：

- **发票第1页：** 包含 CSP 计划合作伙伴的计费详细信息的摘要概述。 这包括计费周期的费用摘要、发票编号、 (Net 60 days) 的付款条款，以及通过线路或支票支付的帐单支付方法。

- **第2页 () 发票的所有后续页面：** 第一方 Microsoft 购买和第三方 ISV (基于许可证的) 从商业应用商店购买的详细信息。 可以通过发布者行在每个产品名称下标识基于 ISV许可证的购买。 关联的对帐文件提供特定发票费用的更多计费详细信息。

- **发票的最后一页：** 如果从 ISV 对基于许可证的市场产品收费，此最终页面将显示有关 ISV 发布者名称和地址的更多详细信息。

### <a name="tips-on-reading-your-reconciliation-file"></a>有关读取对帐文件的提示

定期 **和一次性购买** 对帐文件包含多个列，其中包含映射到发票中费用的其他详细信息。 **PublisherName** 列显示购买内容是 Microsoft 还是第三方 ISV 发布者。

对帐文件中可能会出现一些费用，费用为 0 美元。 这可能是由于 ISV"免费试用"产品/服务 (30 或 60 天) 自带许可产品/服务。

对于免费试用版 ISV 产品/服务：

- 免费试用期涵盖在此期间 ISV 基于许可证的 SaaS 产品的成本。 对于该 SaaS 产品的关联 Azure 基础结构使用，也不需要付费。  但是，如果使用的是基于使用情况的 ISV 产品/服务，则免费试用版不包括基础 Azure 基础结构使用的成本。 在这种情况下，Azure 基础结构使用费用将显示在单独的 Azure 对帐文件中。

- 为客户购买和部署符合 ISV 免费试用版资格的产品时，ISV 发布者会自动将客户注册到免费试用版中。 免费试用期在 ISV 发布者定义的期限之后自动结束。 在期限结束后，将收取客户费用。 这意味着，对帐文件可能会显示符合试用条件的产品的两行：一行跟踪试用期，另一行跟踪付费产品/服务 (在试用期结束后显示费用为 0 美元) 。 试用结束后，显示付费产品/服务行将开始显示费用。 

有关每个列代表的内容的详细信息，请参阅 [使用对帐文件](use-the-reconciliation-files.md)。 另请参阅 [合作伙伴中心的计费类型](./billing-basics.md)

## <a name="next-steps"></a>后续步骤

- [为客户管理商业 marketplace 产品](csp-commercial-marketplace-manage.md)
- [了解对商业 marketplace 产品的支持](csp-commercial-marketplace-support.md)