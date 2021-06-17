---
title: Azure 市场合作伙伴集成
description: 了解Azure 市场 Azure 环境集成的解决方案，并获取 Microsoft 合作伙伴的部署指南链接。
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276478"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure 市场合作伙伴集成

了解如何将合作伙伴解决方案集成到 Azure 环境中。 本文概述了每个解决方案，并提供了详细的部署指南链接。 解决方案按字母顺序列出。 

## <a name="apache-kafka-on-confluent-cloud"></a>Confluent Cloud 上的 Apache Kafka

![Confluent Cloud。](./media/partners/confluent-cloud.png)

除了云应用程序外，Azure 还允许与 Confluent Cloud 集成。 Confluent 客户经常在 Azure 门户 和 Confluent Cloud 之间导航。 例如，一旦用户在 Azure 市场 购买 Confluent Cloud 产品/服务，他们应设置 Confluent Cloud 帐户。 此过程会增加复杂性和时间，并且要求用户管理两个门户之间的配置和资源。 为了减轻跨平台管理的负担，Microsoft 与 Confluent Cloud 合作，构建了从 Azure 到 Confluent Cloud 的集成预配层。 该解决方案在 Azure 市场中提供，提供在 Azure 上使用 Confluent Cloud 产品/服务无缝体验

该解决方案使用 Azure 中启用的资源提供程序来预配 Confluent Cloud 资源。 这样，用户可以通过 Azure 门户、Azure CLI 和 Azure SDK 访问实时事件流式处理。 Confluent Cloud 拥有并运行 SaaS 应用程序，该应用程序包括环境、群集、主题、API 密钥和托管连接器。

与 Confluent Cloud 深度集成可实现以下功能：

- 使用完全托管的基础结构从 Azure 门户预配新的 Confluent 云组织资源。
- 使用 Azure 门户简化从 Azure 到 Confluent Cloud 的单一Azure Active Directory;无需从 Confluent Cloud 门户单独进行身份验证。
- 通过 Azure 订阅开票获取 Confluent 云使用费的统一计费。
- 从门户管理 Confluent 云Azure 门户，并连同 Azure 资源一起在"所有资源"页中跟踪这些资源。

[Confluent 云部署指南](https://docs.confluent.io/current/cloud/marketplace/index.html)

有关与 Azure 上的 Confluent 相关的问题，请转到 [https://support.confluent.io](https://support.confluent.io) 。 如果你是第一次使用，请重置密码，然后再登录到 Confluent 支持门户。 如果没有 Confluent 帐户，请向 发送电子邮件 [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。

## <a name="datadog"></a>Datadog

![DataDog 徽标。](./media/partners/datadog.png)

Datadog 为 Azure 用户提供可观测性和安全性工具，以跨混合和多云环境了解其应用程序的运行状况和性能。 但是，通常需要在 Azure 门户和 Datadog 之间导航才能配置所需的集成。 为了简化跨门户的配置和资源管理，Microsoft 与 Datadog 合作在 Azure 上创建集成的 Datadog 解决方案。 此解决方案Azure 市场 Datadog 的云监视解决方案，为 Azure 客户提供无缝体验。

请参阅 [Azure Monitor](/azure/azure-monitor/platform/partners#datadog) 文档，详细了解此解决方案并注册公共预览版。

## <a name="next-steps"></a>后续步骤

- [Azure 市场在线商店](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn：创建 Azure 帐户](/learn/modules/create-an-azure-account/)
