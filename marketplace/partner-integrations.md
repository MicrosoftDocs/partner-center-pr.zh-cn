---
title: Azure Marketplace 合作伙伴集成
description: 了解与 Azure 环境集成的 Azure Marketplace 解决方案，并获得 Microsoft 合作伙伴提供的部署指南链接。
ms.service: partner-services
ms.topic: conceptual
author: dsindona
ms.author: dsindona
ms.date: 11/16/2020
ms.openlocfilehash: 7c97936e7764361c21503eca174433029707cf69
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691643"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace 合作伙伴集成

了解如何将合作伙伴解决方案集成到 Azure 环境中。 本文概述每个解决方案并链接到详细的部署指南。 解决方案按字母顺序列出。 

## <a name="apache-kafka-on-confluent-cloud"></a>Confluent 云上的 Apache Kafka

![Confluent 云](./media/partners/confluent-cloud.png)

除了你的云应用程序外，Azure 还允许你与 Confluent Cloud 集成。 Confluent 客户经常在 Azure 门户和 Confluent 云之间导航。 例如，当用户在 Azure Marketplace 中购买 Confluent 云产品/服务后，他们应该使用 Confluent 云设置帐户。 此过程增加了复杂性和时间，并要求用户管理两个门户之间的配置和资源。 为了降低跨平台管理的负担，Microsoft 与 Confluent Cloud 建立了合作，并构建了从 Azure 到 Confluent 云的集成设置层。 此解决方案在 Azure Marketplace 中提供，并提供在 Azure 上使用 Confluent 云产品的无缝体验

该解决方案使用 Azure 中启用的资源提供程序来预配 Confluent 云资源。 这允许用户通过 Azure 门户、Azure CLI 和 Azure Sdk 访问实时事件流。 Confluent Cloud 拥有并运行 SaaS 应用程序，该应用程序包括环境、群集、主题、API 密钥和托管连接器。

与 Confluent Cloud 的深度集成支持以下功能：

- 使用完全托管的基础结构，从 Azure 门户预配新的 Confluent 云组织资源。
- 通过 Azure Active Directory 简化从 Azure 到 Confluent Cloud 的单一登录。Confluent 云门户无需单独进行身份验证。
- 通过 Azure 订阅开票获取 Confluent 云消耗费用的统一计费。
- 从 Azure 门户管理 Confluent 云资源，并在 " **所有资源** " 页中跟踪 Azure 资源。

[Confluent 云部署指南](https://docs.confluent.io/current/cloud/marketplace/index.html)

有关与 Azure 上的 Confluent 相关的问题，请参阅 [https://support.confluent.io](https://support.confluent.io) 。 如果你是第一次用户，请在登录到 Confluent 支持门户之前重置密码。 如果你没有帐户使用 Confluent，请向发送电子邮件 [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。

## <a name="datadog"></a>Datadog

![DataDog 徽标](./media/partners/datadog.png)

Datadog 为 Azure 用户提供可观察性和安全工具，以了解在混合环境和多云环境中应用程序的运行状况和性能。 但是，通常需要在 Azure 门户和 Datadog 之间导航才能配置所需的集成。 为了简化跨门户的配置和资源管理，Microsoft 使用 Datadog 在 Azure 上创建集成 Datadog 解决方案。 此解决方案可通过 Azure Marketplace 提供，为 Azure 客户提供使用 Datadog 的云监视解决方案的无缝体验。

请参阅 [Azure Monitor 文档](/azure/azure-monitor/platform/partners#datadog) ，了解有关此解决方案的详细信息并注册公开预览版。

## <a name="next-steps"></a>后续步骤

- [Azure Marketplace 在线商店](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn：创建 Azure 帐户](/learn/modules/create-an-azure-account/)
