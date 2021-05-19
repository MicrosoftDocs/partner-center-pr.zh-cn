---
title: 购买商业市场产品/服务
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 计划合作伙伴如何使用 合作伙伴中心 市场从独立软件供应商或 ISV (SaaS 产品/) 。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147847"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>在市场中为客户购买商业市场合作伙伴中心


**适当的角色**：全局管理员|管理员代理

作为 云解决方案提供商 (CSP) 计划的合作伙伴，可以使用商业市场为客户购买由独立软件供应商 (ISV) 提供的某些软件即服务 (SaaS) 产品的订阅。

通过为客户提供 ISV SaaS 订阅，可以帮助区分业务。 还可以让客户访问满足其特定业务需求的软件包。 你可以管理 ISV 发布者的这些市场 SaaS 产品的许可证和订阅，就像管理 Microsoft 产品的许可证和订阅一样。

可以购买基于 **许可证的** SaaS 订阅或 **基于使用情况的** 订阅。 若要详细了解基于许可证的计费与基于使用情况的计费的区别，请参阅 [计费基础知识](billing-basics.md)。

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>在订阅中购买基于许可证和按流量计费的 SaaS 合作伙伴中心

使用购买 Microsoft 产品的订阅时使用的相同过程，为 ISV 发布者提供的基于许可证或按流量计费的 SaaS 产品购买订阅。

若要在 合作伙伴中心 中购买基于许可证或按流量计费的 SaaS 订阅，请参阅创建、挂起或取消 [客户订阅](create-a-new-subscription.md#create-a-new-subscription)。

也可使用[合作伙伴中心 API](/partner-center/develop/) 为客户创建商业市场订阅。  (有关使用 合作伙伴中心 API 的信息，请参阅 [为商业市场](/partner-center/develop/create-subscription-azure-marketplace-products)产品创建订阅 .) 

>[!IMPORTANT]
> 作为 CSP 计划的合作伙伴，可以从云解决方案提供商的 ISV发布者购买基于许可证或按流量计费的 SaaS 合作伙伴中心。 这意味着你可以购买 ISV 发布者提供的任何 **基于许可证** 或 **按流量计费** 的 SaaS 产品/服务，包括你有权访问的 [专有产品/服务](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 。 若要购买或管理其他商用 marketplace，请参阅基于使用情况的产品/服务（包括 Azure 应用程序、容器或 Vm) 的基于使用情况的产品/服务），你必须使用 [Azure 门户](https://portal.azure.com/) (。

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>在 Azure 门户中购买基于使用情况的订阅

与第三方 ISV 发布者的基于许可证的 SaaS 订阅不同，基于使用情况的订阅首先要求客户拥有 Azure 订阅。 针对商业市场的计费，基于使用情况的资源属于客户的 Azure 订阅。 一旦你的客户拥有 Azure 订阅，CSP 计划中的合作伙伴便可按照以下步骤为其购买商业 marketplace 订阅：

1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)，然后从左侧菜单中选择 " **客户** "。

2. 选择特定客户，然后选择 " **订阅**"。  

3. 在 " **基于使用情况的订阅**" 下，选择 " **所有资源**"。 这会转到 Azure 管理门户。

4. 在 Azure 管理门户中，从左侧菜单中选择 " **创建资源** "。

5. 选择 "Azure Marketplace" 列表顶部的 " **查看全部** "。

6. 若要缩小列表范围，请在 Marketplace 列表顶部使用筛选器。 例如，你可以从 "**发布者**" 下拉列表中选择 " **microsoft** " 或 "**合作伙伴**"，以仅查看 microsoft 提供的或来自 ISV 发布者的产品/服务。

7. 选择特定产品/服务，然后选择 " **创建**"。

## <a name="next-steps"></a>后续步骤

- [管理商业 marketplace 产品/服务](csp-commercial-marketplace-purchase.md)