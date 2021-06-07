---
title: Azure Marketplace 中的专用产品/服务
description: 了解 Azure Marketplace 中的专用产品/服务。
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534152"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="6cb12-103">Azure Marketplace 中的私有计划</span><span class="sxs-lookup"><span data-stu-id="6cb12-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="6cb12-104">专用计划是发布者如何向特定客户提供自定义计划。</span><span class="sxs-lookup"><span data-stu-id="6cb12-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="6cb12-105">私人计划仅适用于付费产品/服务，可从 Azure 门户购买并直接安装。</span><span class="sxs-lookup"><span data-stu-id="6cb12-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="6cb12-106">发布者无法创建咨询服务的专用计划、将我作为呼叫操作或任何免费服务 **联系** 的任何服务，不管是否可以从门户安装此服务。</span><span class="sxs-lookup"><span data-stu-id="6cb12-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="6cb12-107">在 Azure 门户中查找专用计划</span><span class="sxs-lookup"><span data-stu-id="6cb12-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="6cb12-108">当合作伙伴发布专用计划时，它仅对 Azure 门户的 **Marketplace** 部分中的合格用户可见。</span><span class="sxs-lookup"><span data-stu-id="6cb12-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="6cb12-109">这些用户由订阅 ID 或租户 ID 定义，具体取决于产品/服务类型。</span><span class="sxs-lookup"><span data-stu-id="6cb12-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="6cb12-110">如果你有资格获得专用计划，可通过两种方式在门户中找到它们。</span><span class="sxs-lookup"><span data-stu-id="6cb12-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="6cb12-111">专用计划是可搜索的，但不能 (按类别) 在 Azure 门户中进行筛选。</span><span class="sxs-lookup"><span data-stu-id="6cb12-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="6cb12-112">在 Azure 门户中，选择 " **+ 创建资源** " 或搜索 "marketplace" 以前往 **marketplace** 页面。</span><span class="sxs-lookup"><span data-stu-id="6cb12-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="6cb12-113">如果你有资格获得专用计划，你会在页面顶部看到 " **你有私有计划可用** " 标题。</span><span class="sxs-lookup"><span data-stu-id="6cb12-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="6cb12-114">选择 "查看" " **产品/服务** " "计划" 以切换到 "专用计划" 页。</span><span class="sxs-lookup"><span data-stu-id="6cb12-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="可用专用计划时显示的横幅。":::

## <a name="review-private-plans"></a><span data-ttu-id="6cb12-116">查看私有计划</span><span class="sxs-lookup"><span data-stu-id="6cb12-116">Review private plans</span></span>

<span data-ttu-id="6cb12-117">私有计划是产品/服务中的多个计划的一部分。</span><span class="sxs-lookup"><span data-stu-id="6cb12-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="6cb12-118">每个服务可以有多个计划，无论是公共的还是私有的，但私有计划显示在公共计划的单独列表下。</span><span class="sxs-lookup"><span data-stu-id="6cb12-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="6cb12-119">你可以在 " **计划** " 选项卡下查看可用的私有计划，并将其标记为有特殊的 **专用** 徽章：</span><span class="sxs-lookup"><span data-stu-id="6cb12-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="标记为私有的计划页。":::

<span data-ttu-id="6cb12-121">如果有多个订阅，将看到所有订阅均可使用的所有私有计划。</span><span class="sxs-lookup"><span data-stu-id="6cb12-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="6cb12-122">选择 " **创建**" 后，会路由到 "资源创建" 页，开始配置资源。</span><span class="sxs-lookup"><span data-stu-id="6cb12-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="6cb12-123">如果选择 " **创建** " 并且有多个订阅，但并不是所有订阅都添加到私有计划中，则默认订阅可能不是可用于此专用计划的订阅。</span><span class="sxs-lookup"><span data-stu-id="6cb12-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="6cb12-124">在这种情况下，请选择正确的订阅。</span><span class="sxs-lookup"><span data-stu-id="6cb12-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="显示了更多可用专用计划的链接。":::

## <a name="next-steps"></a><span data-ttu-id="6cb12-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6cb12-126">Next steps</span></span>

- [<span data-ttu-id="6cb12-127">什么是 Azure 市场？</span><span class="sxs-lookup"><span data-stu-id="6cb12-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
