---
title: 添加 Azure 合作伙伴共享服务
description: 使用Azure 合作伙伴共享服务购买 Azure 订阅供自己使用，并使用统一方法来购买、跟踪和管理 Azure。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551599"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>添加Azure 合作伙伴共享服务，以便合作伙伴可以购买 Azure 订阅供自己使用

**适当的角色**：全局管理员|管理代理|销售代理

Azure 合作伙伴共享服务 (APSS) 是 云解决方案提供商 (CSP) 计划中的合作伙伴的新产品/服务类型，使合作伙伴能够购买 Azure 订阅供自己使用。  该服务除了可以合并 Azure 许可和 Microsoft 经销协议之外，还可以为合作伙伴使用统一的方法购买、跟踪和管理 Azure 创造机会。 借助 APSS，合作伙伴现在可以像在 Microsoft 企业协议 和 Web Direct 程序中一样灵活地在 CSP 中使用 Azure 订阅，打开以下方案：构建开发和测试环境、部署内部工作负载，以及托管共享服务或多租户应用程序。  

## <a name="create-the-shared-services-tenant"></a>创建共享服务租户

1. 转到"**设置帐户**  >  **设置""**  >  **共享服务"。**

   :::image type="content" source="images/sharedservices2.png" alt-text="共享服务>帐户设置":::

2. 如果还没有共享服务租户，请选择"**创建共享服务"。**

   :::image type="content" source="images/sharedservices3.png" alt-text="创建共享服务。":::

3. 这将创建共享服务租户并购买 Azure 云解决方案提供商共享服务订阅，以用于共享的资源和内部工作负载。

   :::image type="content" source="images/sharedservices5.png" alt-text="创建租户并购买订阅。":::

## <a name="about-the-azure--internalshared-services-offer"></a>关于“Azure - 内部/共享服务”

- Azure - 内部/共享服务订阅是 CSP 中的一种新的 Azure 产品/服务类型，合作伙伴中心合作伙伴获取的 Azure 套餐类型。

- Azure 合作伙伴共享服务订阅符合条件，并可用于购买 IS。

- “Azure - 内部/共享服务”服务只能应用于共享服务租户。

- 订阅的主要用途Azure - 内部/共享服务，以便可以将 Azure 用于自己的开发目的。 用于预配此产品/服务的共享租户不能用于 Office 365 或 Dynamics 许可证等其他服务。

- 你可以像取消任何其他订阅一样取消该订阅。 转到设置"**查看**  >  **所有设置共享**  >  **服务"。** 选择“Azure - 内部/共享服务”订阅，并将其取消。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>访问 Azure 合作伙伴共享服务使用详细信息

你将在云解决方案提供商帐单和对帐文件中找到 Azure 使用信息。 它将包括在帐单内的 Microsoft Azure 行项中。 针对为此服务创建的租户记录的对帐文件中将提供详细使用信息。

## <a name="azure-partner-shared-services-pricing"></a>Azure 合作伙伴共享服务定价

若要查看 APSS 的新定价文件，请转到"**销售** 定价和产品/服务"并选择当前  >  月份价目表。 在接下来的几周内，还将发布特定费率卡 API。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>市场产品/Azure 合作伙伴共享服务

从 2019 年 3 月 1 日开始，APSS 不再支持市场产品/服务。

|**市场支持**   |**2019 年 3 月 1 日之前支持的 APSS**|**2019 年 3 月 1 日之后**|
|---------------------------|:----------------------------|:-------------------|
|使用 BYOL (和免费) 自带许可证   | 是   | 否|
|其他第三方市场产品/服务   | 否   |否|

使用 APSS 部署 BYOL 或免费服务的合作伙伴不会受到影响;但是，在 2019 年 3 月 1 日之后，他们将无法购买新的 BYOL 或免费服务。

若要利用可用的市场产品/服务的完整目录， (BYOL 和免费服务) ，我们建议 CSP 合作伙伴使用 Web 直接 Azure 订阅部署共享服务。  建议以前从市场部署第三方 BYOL 和免费服务资源并想要继续使用这些资源并部署更多第三方产品/服务的 CSP 合作伙伴将 APSS 订阅迁移到 Web 直接迁移 [现有 Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)订阅。

计划在 2019 年 3 月 1 日之后继续使用 APSS 订阅并想要部署新的第三方 [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) 服务或免费服务的合作伙伴可以按照 ISV 的说明将其部署到其 APSS 订阅。

## <a name="next-steps"></a>后续步骤

- [通过云解决方案提供商销售软件订阅](csp-software-subscriptions.md)