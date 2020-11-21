---
title: Azure Marketplace 合作伙伴集成
description: 了解与 Azure 环境集成的 Azure Marketplace 解决方案，并获得 Microsoft 合作伙伴提供的部署指南链接。
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: b31486000e59f3d85ee30019ecea000252b297a8
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006899"
---
# <a name="azure-marketplace-partner-integrations"></a><span data-ttu-id="a3470-103">Azure Marketplace 合作伙伴集成</span><span class="sxs-lookup"><span data-stu-id="a3470-103">Azure Marketplace partner integrations</span></span>

<span data-ttu-id="a3470-104">了解如何将合作伙伴解决方案集成到 Azure 环境中。</span><span class="sxs-lookup"><span data-stu-id="a3470-104">Learn how to integrate partner solutions into your Azure environment.</span></span> <span data-ttu-id="a3470-105">本文概述每个解决方案并链接到详细的部署指南。</span><span class="sxs-lookup"><span data-stu-id="a3470-105">This article gives an overview of each solution and links to detailed deployment guides.</span></span> <span data-ttu-id="a3470-106">解决方案按字母顺序列出。</span><span class="sxs-lookup"><span data-stu-id="a3470-106">Solutions are listed in alphabetical order.</span></span> 

## <a name="apache-kafka-on-confluent-cloud"></a><span data-ttu-id="a3470-107">Confluent 云上的 Apache Kafka</span><span class="sxs-lookup"><span data-stu-id="a3470-107">Apache Kafka on Confluent Cloud</span></span>

![Confluent 云](./media/partners/confluent-cloud.png)

<span data-ttu-id="a3470-109">除了你的云应用程序外，Azure 还允许你与 Confluent Cloud 集成。</span><span class="sxs-lookup"><span data-stu-id="a3470-109">Azure lets you integrate with Confluent Cloud in addition to your cloud applications.</span></span> <span data-ttu-id="a3470-110">Confluent 客户经常在 Azure 门户和 Confluent 云之间导航。</span><span class="sxs-lookup"><span data-stu-id="a3470-110">Confluent customers often navigate between the Azure portal and Confluent Cloud.</span></span> <span data-ttu-id="a3470-111">例如，当用户在 Azure Marketplace 中购买 Confluent 云产品/服务后，他们应该使用 Confluent 云设置帐户。</span><span class="sxs-lookup"><span data-stu-id="a3470-111">For example, once a user purchases a Confluent Cloud offer in Azure Marketplace, they are then expected to set up an account with Confluent Cloud.</span></span> <span data-ttu-id="a3470-112">此过程增加了复杂性和时间，并要求用户管理两个门户之间的配置和资源。</span><span class="sxs-lookup"><span data-stu-id="a3470-112">This process adds complexity and time, and requires users to manage configuration and resources between the two portals.</span></span> <span data-ttu-id="a3470-113">为了降低跨平台管理的负担，Microsoft 与 Confluent Cloud 建立了合作，并构建了从 Azure 到 Confluent 云的集成设置层。</span><span class="sxs-lookup"><span data-stu-id="a3470-113">To reduce the burden of managing across platforms, Microsoft, in partnership with Confluent Cloud, built an integrated provisioning layer from Azure to Confluent Cloud.</span></span> <span data-ttu-id="a3470-114">此解决方案在 Azure Marketplace 中提供，并提供在 Azure 上使用 Confluent 云产品的无缝体验</span><span class="sxs-lookup"><span data-stu-id="a3470-114">The solution is available in Azure Marketplace and  provides a seamless experience for using the Confluent Cloud offering on Azure</span></span>

<span data-ttu-id="a3470-115">该解决方案使用 Azure 中启用的资源提供程序来预配 Confluent 云资源。</span><span class="sxs-lookup"><span data-stu-id="a3470-115">The solution uses a resource provider enabled in Azure to provision Confluent Cloud resources.</span></span> <span data-ttu-id="a3470-116">这允许用户通过 Azure 门户、Azure CLI 和 Azure Sdk 访问实时事件流。</span><span class="sxs-lookup"><span data-stu-id="a3470-116">This allows users to access real-time event streaming via the Azure portal, Azure CLI, and Azure SDKs.</span></span> <span data-ttu-id="a3470-117">Confluent Cloud 拥有并运行 SaaS 应用程序，该应用程序包括环境、群集、主题、API 密钥和托管连接器。</span><span class="sxs-lookup"><span data-stu-id="a3470-117">Confluent Cloud owns and runs the SaaS application, which includes environments, clusters, topics, API keys, and managed connectors.</span></span>

<span data-ttu-id="a3470-118">与 Confluent Cloud 的深度集成支持以下功能：</span><span class="sxs-lookup"><span data-stu-id="a3470-118">The deep integration with Confluent Cloud enables the following capabilities:</span></span>

- <span data-ttu-id="a3470-119">使用完全托管的基础结构，从 Azure 门户预配新的 Confluent 云组织资源。</span><span class="sxs-lookup"><span data-stu-id="a3470-119">Provision a new Confluent Cloud organization resource from the Azure portal with fully managed infrastructure.</span></span>
- <span data-ttu-id="a3470-120">通过 Azure Active Directory 简化从 Azure 到 Confluent Cloud 的单一登录。Confluent 云门户无需单独进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="a3470-120">Streamline single sign-on from Azure to Confluent Cloud with Azure Active Directory; no separate authentication needed from the Confluent Cloud portal.</span></span>
- <span data-ttu-id="a3470-121">通过 Azure 订阅开票获取 Confluent 云消耗费用的统一计费。</span><span class="sxs-lookup"><span data-stu-id="a3470-121">Get unified billing of Confluent Cloud consumption charges through Azure subscription invoicing.</span></span>
- <span data-ttu-id="a3470-122">从 Azure 门户管理 Confluent 云资源，并在 " **所有资源** " 页中跟踪 Azure 资源。</span><span class="sxs-lookup"><span data-stu-id="a3470-122">Manage Confluent Cloud resources from the Azure portal, and track them in the **All resources** page, alongside your Azure resources.</span></span>

[<span data-ttu-id="a3470-123">Confluent 云部署指南</span><span class="sxs-lookup"><span data-stu-id="a3470-123">Confluent Cloud deployment guides</span></span>](https://docs.confluent.io/current/cloud/marketplace/index.html)

<span data-ttu-id="a3470-124">有关与 Azure 上的 Confluent 相关的问题，请参阅 [https://support.confluent.io](https://support.confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="a3470-124">For issues related to Confluent on Azure, go to [https://support.confluent.io](https://support.confluent.io).</span></span> <span data-ttu-id="a3470-125">如果你是第一次用户，请在登录到 Confluent 支持门户之前重置密码。</span><span class="sxs-lookup"><span data-stu-id="a3470-125">If you are a first time user, reset your password before you sign in to the Confluent Support Portal.</span></span> <span data-ttu-id="a3470-126">如果你没有帐户使用 Confluent，请向发送电子邮件 [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="a3470-126">If you do not have an account with Confluent, please send an email to [cloud-support@confluent.io](mailto:cloud-support@confluent.io).</span></span>

## <a name="datadog"></a><span data-ttu-id="a3470-127">Datadog</span><span class="sxs-lookup"><span data-stu-id="a3470-127">Datadog</span></span>

![DataDog 徽标](./media/partners/datadog.png)

<span data-ttu-id="a3470-129">Datadog 为 Azure 用户提供可观察性和安全工具，以了解在混合环境和多云环境中应用程序的运行状况和性能。</span><span class="sxs-lookup"><span data-stu-id="a3470-129">Datadog provides observability and security tools for Azure users to understand the health and performance of their applications across hybrid and multi-cloud environments.</span></span> <span data-ttu-id="a3470-130">但是，通常需要在 Azure 门户和 Datadog 之间导航才能配置所需的集成。</span><span class="sxs-lookup"><span data-stu-id="a3470-130">But configuring the necessary integrations often requires navigating between the Azure portal and Datadog.</span></span> <span data-ttu-id="a3470-131">为了简化跨门户的配置和资源管理，Microsoft 使用 Datadog 在 Azure 上创建集成 Datadog 解决方案。</span><span class="sxs-lookup"><span data-stu-id="a3470-131">To simplify configuration and resource management across portals, Microsoft worked with Datadog to create an integrated Datadog solution on Azure.</span></span> <span data-ttu-id="a3470-132">此解决方案可通过 Azure Marketplace 提供，为 Azure 客户提供使用 Datadog 的云监视解决方案的无缝体验。</span><span class="sxs-lookup"><span data-stu-id="a3470-132">Available via the Azure Marketplace, this solution provides a seamless experience for Azure customers to use Datadog’s cloud monitoring solution.</span></span>

<span data-ttu-id="a3470-133">请参阅 [Azure Monitor 文档](/azure/azure-monitor/platform/partners#datadog) ，了解有关此解决方案的详细信息并注册公开预览版。</span><span class="sxs-lookup"><span data-stu-id="a3470-133">See the [Azure Monitor documentation](/azure/azure-monitor/platform/partners#datadog) to learn more about this solution and sign up for the public preview.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a3470-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a3470-134">Next steps</span></span>

- [<span data-ttu-id="a3470-135">Azure Marketplace 在线商店</span><span class="sxs-lookup"><span data-stu-id="a3470-135">Azure Marketplace online store</span></span>](https://azure.microsoft.com/marketplace/)
- [<span data-ttu-id="a3470-136">Microsoft Learn：创建 Azure 帐户</span><span class="sxs-lookup"><span data-stu-id="a3470-136">Microsoft Learn: Create an Azure account</span></span>](/learn/modules/create-an-azure-account/)
