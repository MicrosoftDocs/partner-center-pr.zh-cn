---
title: 如何计算合作伙伴盈余合作伙伴中心
ms.topic: article
ms.date: 09/17/2019
description: 如何计算 Azure 计划的合作伙伴获得的信用额度
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318771"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="9ebc8-103">如何计算合作伙伴获得的信用额度（PEC）</span><span class="sxs-lookup"><span data-stu-id="9ebc8-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="9ebc8-104">在 CSP 中，对部件或其客户的整个 Azure 环境拥有全天候 IT 运营管理的合作伙伴将获得 PEC 奖励。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="9ebc8-105">PEC 作为发票的一部分提供给与 Microsoft 直接计费关系的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="9ebc8-106">该信用额度每天计算，并反映在月度发票中。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="9ebc8-107">默认情况下，在 CSP 中，为合作伙伴授予了对客户订阅所需的访问权限，使其能够对订阅上的资源进行24X7 操作管理和控制。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-107">By default, in CSP, partners are granted the necessary access rights to the customer’s subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="9ebc8-108">下一节介绍了客户可用于预配约束力合作伙伴访问权限的其他方法。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="9ebc8-109">重要的资格和计算要求：</span><span class="sxs-lookup"><span data-stu-id="9ebc8-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="9ebc8-110">合作伙伴应具有有效的 MPN 协议和基于规则的有效帐户 C （RBAC）角色，以接收他们所管理的 azure 资产的获得的信用额度。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="9ebc8-111">了解有关 [有效 RBAC 角色] 的详细信息</span><span class="sxs-lookup"><span data-stu-id="9ebc8-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="9ebc8-112">如果间接提供程序或其间接经销商，或者两者都具有对 CSP 中客户的 Azure 资源的全天候运营控制和管理，则该提供程序适用于 PEC。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer’s Azure resources in CSP.</span></span>

- <span data-ttu-id="9ebc8-113">PEC 与合作伙伴管理的 CSP 中客户的 Azure 场地的计费（收费）消耗相关联。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-113">PEC is associated to billed (chargeable) consumption of customer’s Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="9ebc8-114">PEC 仅适用于由 Microsoft （间接提供商和直接帐单合作伙伴）计费的 CSP 中的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="9ebc8-115">符合条件的服务：合作伙伴获得的信用额度适用于价格列表中提供的所有 Azure 1PP Azure 使用量。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="9ebc8-116">存在例外，包括但不限于3PP 和 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="9ebc8-117">PEC 每日计算一次，可以在每日侦测文件中查看。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="9ebc8-118">合作伙伴（通过其提供商提供的提供商或经销商）必须有整天（24x7）的访问权限，以确保他们获得 PEC。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="9ebc8-119">PEC 向下移动到 Azure 资源级别。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="9ebc8-120">如果合作伙伴在订阅或资源组级别具有有效的访问权限，则具有更高实体的角色的每个资源将获得 PEC。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="9ebc8-121">PEC 将包含在合作伙伴的月度发票中。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="9ebc8-122">发票是收费的。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-122">The invoice is net of charges.</span></span> <span data-ttu-id="9ebc8-123">详细信息显示在 invoice 侦测文件中。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="9ebc8-124">若要了解如何获取管理 Azure 订阅的访问权限，以及如何将 MPN ID 链接到 RBAC 角色，请阅读[Azure 计划下的管理订阅和资源](azure-plan-manage.md)。</span><span class="sxs-lookup"><span data-stu-id="9ebc8-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="9ebc8-125">有关详细信息</span><span class="sxs-lookup"><span data-stu-id="9ebc8-125">For more information</span></span>

- [<span data-ttu-id="9ebc8-126">Azure 计划-计费</span><span class="sxs-lookup"><span data-stu-id="9ebc8-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="9ebc8-127">CSP 中新商业体验的价目表</span><span class="sxs-lookup"><span data-stu-id="9ebc8-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)