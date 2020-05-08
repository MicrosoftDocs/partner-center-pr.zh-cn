---
title: 购买商业市场优惠
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 计划合作伙伴如何使用合作伙伴中心市场从独立软件供应商（Isv）购买 SaaS 产品/服务。
author: LauraBrenner
ms.author: labrenne
keywords: 订阅，marketplace，商业市场，第三方，ISV，SaaS 产品/服务，云解决方案提供商计划，购买产品/服务，购买订阅
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c740ae823670644cb1f81c0a667d1fb48fc873ae
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908083"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>在合作伙伴中心为客户购买商业 marketplace 产品

**适用于**

- 合作伙伴中心
- 云解决方案提供商计划中的合作伙伴

**相应的角色**

- 全局管理员
- 管理员代理

作为云解决方案提供商（CSP）计划的合作伙伴，你可以使用商业市场为你的客户购买订阅，使其能够使用独立软件供应商（Isv）提供的某些软件即服务（SaaS）产品。 

通过向客户提供 ISV SaaS 订阅，你可以帮助区分你的业务。 你还可以让客户访问满足其特定业务需求的软件捆绑。 你可以像管理 Microsoft 产品的许可证和订阅一样，管理 ISV 发布者提供的这些 marketplace SaaS 产品的许可证和订阅。

你可以购买**基于许可证的**SaaS 订阅或**基于使用情况的**订阅。 若要详细了解基于许可证和基于使用情况的计费之间的差异，请参阅[计费基础知识](billing-basics.md)。

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>在合作伙伴中心购买基于许可证的 SaaS 订阅

你使用为 Microsoft 产品购买订阅时所用的同一过程为 ISV 发布者提供的基于许可证的 SaaS 产品购买订阅。

若要在合作伙伴中心购买基于许可证的 SaaS 订阅，请参阅[创建、暂停或取消客户订阅](create-a-new-subscription.md#create-a-new-subscription)。

也可使用[合作伙伴中心 API](https://docs.microsoft.com/partner-center/develop/) 为客户创建商业市场订阅。 （有关使用合作伙伴中心 Api 的详细信息，请参阅[为商业 marketplace 产品创建订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。）

>[!IMPORTANT]
> 作为 CSP 计划中的合作伙伴，只能从合作伙伴中心内的 ISV 发布者购买**基于许可证的**SaaS 订阅。 这意味着你可以购买 ISV 发布者提供的任何**基于许可证**的 SaaS 产品/服务，包括你有权访问的[独家产品/服务](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)。 若要购买或管理其他商业市场，请参阅 Isv 提供的产品/服务（例如**基于使用情况**、按流量计费或基于消耗的产品/服务，包括 Azure 应用程序、容器或 vm），你必须使用[Azure 门户](https://portal.azure.com/)。 有关详细信息，请参阅以下主题。

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>在 Azure 门户中购买基于使用情况的订阅

与第三方 ISV 发布者的基于许可证的 SaaS 订阅不同，基于使用情况的订阅首先要求客户拥有 Azure 订阅。 针对商业市场的计费，基于使用情况的资源属于客户的 Azure 订阅。 一旦你的客户拥有 Azure 订阅，CSP 计划中的合作伙伴便可按照以下步骤为其购买商业 marketplace 订阅：

1. 登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard)，然后从左侧菜单中选择 "**客户**"。

2. 选择特定客户，然后选择 "**订阅**"。  

3. 在 "**基于使用情况的订阅**" 下，选择 "**所有资源**"。 这会转到 Azure 管理门户。

4. 在 Azure 管理门户中，从左侧菜单中选择 "**创建资源**"。

5. 选择 "Azure Marketplace" 列表顶部的 "**查看全部**"。

6. 若要缩小列表范围，请在 Marketplace 列表顶部使用筛选器。 例如，你可以从 "**发布者**" 下拉列表中选择 " **microsoft** " 或 "**合作伙伴**"，以仅查看 microsoft 提供的或来自 ISV 发布者的产品/服务。

7. 选择特定产品/服务，然后选择 "**创建**"。

## <a name="next-steps"></a>后续步骤

- [管理商业 marketplace 产品/服务](csp-commercial-marketplace-purchase.md)