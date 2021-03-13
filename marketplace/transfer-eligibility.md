---
title: 转让资格–在帐单帐户、Azure Marketplace 之间传输订阅的准则
description: 在 Azure 门户中的计费帐户之间传输订阅之前的商业检查准则。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412550"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="340f4-103">传输计费帐户之间的订阅的资格</span><span class="sxs-lookup"><span data-stu-id="340f4-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="340f4-104">可以在 Azure 门户的 "计费" 部分中将订阅从一个计费帐户 [转移](/azure/cost-management-billing/understand/subscription-transfer) 到另一个。</span><span class="sxs-lookup"><span data-stu-id="340f4-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="340f4-105">在传输之前，会扫描订阅以获取第三方产品。</span><span class="sxs-lookup"><span data-stu-id="340f4-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="340f4-106">仅当清除 *所有* 产品进行传输时才允许传输 (请参阅下面的 [条件](#criteria-for-transfer-approval-or-denial)) 。</span><span class="sxs-lookup"><span data-stu-id="340f4-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="340f4-107">系统将为未能清除的应用生成相关的错误消息，以帮助你确定后续步骤。</span><span class="sxs-lookup"><span data-stu-id="340f4-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="340f4-108">本文不适用于 SaaS 产品，因为 SaaS 资源附加到租户，而不是订阅。</span><span class="sxs-lookup"><span data-stu-id="340f4-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="340f4-109">SaaS 资源可从一个计费帐户转移到另一个计费帐户，但这是根据资源和 Azure 支持作为支持请求来完成的。</span><span class="sxs-lookup"><span data-stu-id="340f4-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="340f4-110">传输批准或拒绝的条件</span><span class="sxs-lookup"><span data-stu-id="340f4-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="340f4-111">如果任何第三方应用满足以下任一条件，则无法传输订阅：</span><span class="sxs-lookup"><span data-stu-id="340f4-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="340f4-112">目标帐户是商业的，应用可以选择退出，通过合作伙伴进行销售。</span><span class="sxs-lookup"><span data-stu-id="340f4-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="340f4-113">对于所选的合作伙伴，此应用将处于选中状态，并且目标帐户不在允许列表中。</span><span class="sxs-lookup"><span data-stu-id="340f4-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="340f4-114">产品/服务是过去对于所选订阅的预览提议，或者是专用产品/服务，并且订阅不再处于允许列表中。</span><span class="sxs-lookup"><span data-stu-id="340f4-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="340f4-115">新的计费帐户所在的区域与产品/服务的销售区域不同，该产品/服务不会出售到该区域。</span><span class="sxs-lookup"><span data-stu-id="340f4-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="340f4-116">在从订阅中删除资源之前，阻止的传输将一直有效，之后可以再次尝试传输。</span><span class="sxs-lookup"><span data-stu-id="340f4-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="340f4-117">后续步骤</span><span class="sxs-lookup"><span data-stu-id="340f4-117">Next steps</span></span>

[<span data-ttu-id="340f4-118">获取 Microsoft AppSource 和 Azure Marketplace 的支持</span><span class="sxs-lookup"><span data-stu-id="340f4-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

