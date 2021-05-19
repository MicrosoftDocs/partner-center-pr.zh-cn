---
title: 概述 - CSP 市场
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何销售来自独立软件供应商和市场中 ISV (SaaS) 产品/服务 (客户订阅) 软件即服务。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7c18f69a62e8f8d126a0756911d2fbcdfdb85d8d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147864"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>合作伙伴中心内的商业市场概述

**相应的角色**：全局管理员

作为 云解决方案提供商 (CSP) 计划的合作伙伴，可以捆绑和销售 Microsoft 产品以及由独立软件供应商第三方 ISV (发布的) 。 通过能够这样捆绑解决方案，可以更好地为最终客户提供服务，并发展 CSP 服务业务。

作为 CSP 计划的合作伙伴，可以使用 合作伙伴中心 Microsoft 商业市场购买许多 ISV 解决方案。 这为你提供了几个主要优势：

- 访问针对 Microsoft 技术和环境优化的软件解决方案的目录。
- 简化了采购周期和采购周期。
- 单个与 合作伙伴中心 API 集成。  (这种集成可以进一步访问 ISV 解决方案目录，降低运营和工程成本，并通过单个提供程序简化多个供应商订阅和计费的管理) 
- 简化了客户的 Azure 租户中的部署和预配 (基于虚拟机的解决方案) 。
- 减少直接 ISV 购买或采购、Microsoft 解决方案配置和集成的潜在挑战，以及管理或合并来自多个供应商的定期发票需求。

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>商业市场中的 CSP 产品/服务概述

如果你是 CSP 计划的合作伙伴，你可能希望针对 ISV 产品/服务执行许多商业市场活动。 请参阅下表，详细了解每个活动。

|**如果你想要**  |**读取**   |
|:------------------------------------|:------------------|
|了解如何查看或搜索可用产品/服务、定价、产品详细信息或发布者联系信息 | [发现产品/服务](csp-commercial-marketplace-discover.md) | 
|了解如何购买和部署产品/服务   | [购买产品/服务](csp-commercial-marketplace-purchase.md)   | 
|了解如何取消或续订订阅，或者添加或删除许可证  | [管理套餐](csp-commercial-marketplace-manage.md) |
|了解计费如何适用于商业 marketplace 购买 | [了解帐单](csp-commercial-marketplace-billing.md) |
|了解谁负责 ISV 购买哪些类型的支持 | [了解支持](csp-commercial-marketplace-support.md) |
|了解有关商业应用商店中 CSP 合作伙伴和 Isv 的合同和责任 | [了解合同](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> 本概述介绍了 CSP 计划中的合作伙伴如何使用合作伙伴中心的某些商业 marketplace 功能。 与 CSP 计划中的合作伙伴相比，ISV 发布者具有不同的 marketplace 角色。 它们还在合作伙伴中心提供不同的商业 Marketplace 功能。 若要了解有关 ISV 发布者角色的详细信息，请参阅 [Azure 商业市场概述](/azure/marketplace/partner-center-portal/commercial-marketplace-overview)。

## <a name="where-to-complete-commercial-marketplace-activities"></a>完成商业市场活动的位置

作为 CSP 计划中的合作伙伴，你可以直接从合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard) 或使用 [合作伙伴中心 api](/partner-center/develop/)完成多个适用于 ISV SaaS 产品/服务的商业市场活动。 但是，若要完成其他 marketplace 活动，你可能需要执行以下操作：

- [Microsoft Azure 管理门户](https://portal.azure.com/)

    或

- 第三方 ISV 发布者的系统或网站

在其中，你可以从你选择的产品/服务的类型着手完成活动。 CSP 计划中的合作伙伴当前可以通过第三方 ISV 发布者来处理两种类型的产品/服务：

1. 基于许可证的 SaaS 产品  
2. 基于使用情况的提供 (包括基于虚拟机、容器或 Azure 应用程序的提供) 

请参阅 [计费基础知识](billing-basics.md) ，详细了解基于许可证的产品/服务和基于使用情况的产品/服务的计费方式有所不同。  

若要了解在何处完成基于许可证或基于使用情况的 ISV 产品/服务的特定市场活动，请参阅下表。

|**对于 ISV 提供的基于许可证或按流量计费的 SaaS 产品/服务**  |**使用**  |
|:------------------------------------|:------------------|
|发现或搜索可用产品/服务  | 合作伙伴中心仪表板或合作伙伴中心 API  |
|购买产品/服务  | 合作伙伴中心仪表板或合作伙伴中心 API  |
|在客户的 AAD 租户 (帐户设置、软件管理或部署中部署购买的产品/服务)   | ISV 发布者的系统或网站  |
|取消/续订套餐订阅或添加/删除许可证 | 合作伙伴中心仪表板或合作伙伴中心 API  |
|创建用户或管理权限  | ISV 发布者的系统或网站  |

|**对于 ISV 提供的基于使用情况的优惠**  |**使用**  |
|:------------------------------------|:------------------|
|发现或搜索可用产品/服务  | 合作伙伴中心仪表板、合作伙伴中心 API 或Azure 门户  |
|购买产品/服务  | Azure 门户  |
|在客户的 AAD 租户 (帐户设置、软件管理或部署中部署购买的产品/服务)   | Azure 门户  |
|取消/续订套餐订阅或添加/删除许可证 | Azure 门户  |
|创建用户或管理权限  | Azure 门户  |

## <a name="next-steps"></a>后续步骤

- [发现或查看商业市场产品/服务](csp-commercial-marketplace-discover.md)
- [购买商业市场优惠](csp-commercial-marketplace-purchase.md)
