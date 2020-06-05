---
title: 添加 Azure 合作伙伴共享服务
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Azure 合作伙伴共享服务来购买 Azure 订阅，供自己使用，并提供一种统一的方法来购买、跟踪和管理 Azure。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, 共享服务, 租户
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 62989c58284de46834f02abc01041c454e725a81
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425946"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>添加 Azure 合作伙伴共享服务，以便合作伙伴可以购买 Azure 订阅供自己使用

**适用于**

- 合作伙伴中心

Azure 合作伙伴共享服务是面向云解决方案提供商计划合作伙伴的新服务类型，可以让合作伙伴购买供自己使用的 Azure 订阅。  该服务除了可以合并 Azure 许可和 Microsoft 经销协议之外，还可以为合作伙伴使用统一的方法购买、跟踪和管理 Azure 创造机会。 使用 Azure 合作伙伴共享服务，合作伙伴现在可以灵活地使用 CSP 中的 Azure 订阅，就像在 Microsoft 企业协议和 Web 直接程序中一样，打开方案，例如：生成开发和测试环境、部署内部工作负荷，以及托管共享服务或多租户应用程序。  

## <a name="create-the-shared-services-tenant"></a>创建共享服务租户

1. 请参阅 "**设置**" "  >  **查看所有设置**" "  >  **共享服务**"。

   ![**帐户设置** > **共享服务**](images/sharedservices2.png)

2. 如果你还没有共享服务租户，请单击**创建共享服务**。

   ![创建共享服务](images/sharedservices3.png)

3. 这将创建共享服务租户并购买 Azure 云解决方案提供商共享服务订阅，以用于共享的资源和内部工作负载。

   ![创建租户和购买订阅](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>关于“Azure - 内部/共享服务”

- Azure-内部/共享服务订阅是一个新的 Azure 产品/服务类型，可通过合作伙伴为其自己使用 Azure 的合作伙伴访问 CSP。 

- Azure-内部/共享服务产品/服务不适用于折扣和奖励。

- “Azure - 内部/共享服务”服务只能应用于共享服务租户。

- Azure-内部/共享服务订阅的主要用途是，以便可以将 Azure 用于自己的开发目的。 用于预配此服务的共享租户无法用于其他服务，如 Office 365 或 Dynamics 席位。 

- 你可以像取消任何其他订阅一样取消该订阅。 请参阅 "**设置**" "  >  **查看所有设置**" "  >  **共享服务**"。 选择“Azure - 内部/共享服务”订阅，并将其取消。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>访问 Azure 合作伙伴共享服务使用详细信息

你将在云解决方案提供商帐单和对帐文件中找到 Azure 使用信息。 它将包括在帐单内的 Microsoft Azure 行项中。 针对为此服务创建的租户记录的对帐文件中将提供详细使用信息。 

## <a name="azure-partner-shared-services-pricing"></a>Azure 合作伙伴共享服务定价

若要查看 Azure 合作伙伴共享服务的新定价文件，请前往**销售**  >  **定价和产品**/服务，并选择当月的价格列表。 在接下来的几周内，还将发布特定费率卡 API。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace 产品和 Azure 合作伙伴共享服务

从2019年3月1日起，Azure 合作伙伴共享服务（应用）不再支持 Marketplace 产品/服务。

|**Marketplace 支持**   |**2019年3月1日之前支持应用**|**2019年3月1日之后**|
|---------------------------|:----------------------------|:-------------------|
|自带许可（BYOL）和免费服务   | 是   | No|
|其他第三方 marketplace 产品   | 否   |否|

使用应用部署了 BYOL 或免费服务的合作伙伴将不受影响;但2019年3月1日之后，他们将无法购买新的 BYOL 或免费服务。

若要充分利用 Marketplace 产品/服务的完整目录（不只是 BYOL 和免费服务），建议使用 web 直接 Azure 订阅来部署共享服务。  我们鼓励现有的 CSP 合作伙伴从 Marketplace 部署第三方 BYOL 和免费服务资源，并希望继续使用它们并部署更多第三方产品/服务，以将应用订阅迁移到 web 直接[迁移现有的 Azure 订阅](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)。

如果合作伙伴计划在2019年3月1日之后继续使用应用订阅，并且想要部署新的第三方[BYOL 服务](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)或免费服务，则可以按照 isv 提供的说明将它们部署到其应用订阅。

