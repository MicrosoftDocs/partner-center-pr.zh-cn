---
title: 合作伙伴赚取的托管服务返点
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何计算和支付 Microsoft 合作伙伴赚取的托管服务返点 (PEC)，以及如何确保你有资格赚取它们。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3ceb2ded6e52083ad0d74a411026558fbce2f642
ms.sourcegitcommit: 883c332a10f51b41b72c2f3fe08bb9593b569d28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2020
ms.locfileid: "91852582"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="b0102-103">合作伙伴赚取的返点的计算与支付方式</span><span class="sxs-lookup"><span data-stu-id="b0102-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="b0102-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="b0102-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b0102-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b0102-105">Global admin</span></span>
- <span data-ttu-id="b0102-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="b0102-106">User admin</span></span>
- <span data-ttu-id="b0102-107">管理员代理</span><span class="sxs-lookup"><span data-stu-id="b0102-107">Admin agent</span></span>
- <span data-ttu-id="b0102-108">计费管理员</span><span class="sxs-lookup"><span data-stu-id="b0102-108">Billing admin</span></span>
- <span data-ttu-id="b0102-109">销售代理</span><span class="sxs-lookup"><span data-stu-id="b0102-109">Sales agent</span></span>

<span data-ttu-id="b0102-110">合作伙伴赚取的托管服务返点 (PEC) 是对合作伙伴为客户的部分或整个 Azure 环境提供全天候 IT 运营控制和管理所做努力给予的认可和奖励。</span><span class="sxs-lookup"><span data-stu-id="b0102-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="b0102-111">默认情况下，在云解决方案提供商中，合作伙伴对客户订阅拥有必要的访问权限，以便能够对订阅中的资源进行全天候的运营管理和控制。</span><span class="sxs-lookup"><span data-stu-id="b0102-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="b0102-112">下一部分将会介绍客户为交易合作伙伴预配访问权限的其他方法。</span><span class="sxs-lookup"><span data-stu-id="b0102-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="b0102-113">每月发票金额是合作伙伴赚取的返点净额。</span><span class="sxs-lookup"><span data-stu-id="b0102-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="b0102-114">合作伙伴可以在其每月对帐文件中查看 PEC 详细信息。</span><span class="sxs-lookup"><span data-stu-id="b0102-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="b0102-115">有关客户可为交易合作伙伴预配访问权限的其他方法，请参阅[管理 Azure 计划中的订阅和资源](azure-plan-manage.md)。</span><span class="sxs-lookup"><span data-stu-id="b0102-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="b0102-116">另请参阅[恢复 Azure CSP 订阅的管理员权限](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="b0102-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="b0102-117">重要的资格和计算信息</span><span class="sxs-lookup"><span data-stu-id="b0102-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="b0102-118">合作伙伴应已签署有效的 MPN 协议并具有有效的 RBAC 角色，才能赚取 Azure 资产管理工作的返点。</span><span class="sxs-lookup"><span data-stu-id="b0102-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="b0102-119">对于间接提供商及其间接经销商，如果间接提供商或/和间接经销商为云解决方案提供商中的客户 Azure 资源提供全天候运营控制和管理，则间接提供商有资格赚取 PEC。</span><span class="sxs-lookup"><span data-stu-id="b0102-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="b0102-120">PEC 与云解决方案提供商中由合作伙伴管理的客户 Azure 资产的计费（可收费）消耗量相关联。</span><span class="sxs-lookup"><span data-stu-id="b0102-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="b0102-121">PEC 仅适用于 CSP 中由 Microsoft 计费的合作伙伴（间接提供商和直接计费合作伙伴）。</span><span class="sxs-lookup"><span data-stu-id="b0102-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="b0102-122">符合条件的服务：合作伙伴赚取的返点适用于 Azure 计划消费定价（合作伙伴可从 [Azure 计划定价](https://partner.microsoft.com/commerce/sales)页将其导出）中列出的服务。</span><span class="sxs-lookup"><span data-stu-id="b0102-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="b0102-123">合作伙伴赚取的赠金不适用于在 Azure 计划消费定价表的“标记”列中被标识为“第三方”的第三方产品、Azure 计划预留项、市场定价表中的产品以及 [Azure 现成虚拟机](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/) 。</span><span class="sxs-lookup"><span data-stu-id="b0102-123">Partner earned credit is not applicable to third-party products identified as **Third Party** in the **Tags column** of the Azure plan consumption price list, Azure Plan reservations, products in the Marketplace price list and [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/).</span></span>

- <span data-ttu-id="b0102-124">PEC 每日计算，可在每日使用情况文件和每月发票对帐文件中查看。</span><span class="sxs-lookup"><span data-stu-id="b0102-124">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="b0102-125">合作伙伴（间接提供商或间接经销商）必须拥有全天 (24x7) 的访问权限，才可确保赚取 PEC。</span><span class="sxs-lookup"><span data-stu-id="b0102-125">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="b0102-126">PEC 根据所管理的 Azure 资产每日计算一次。</span><span class="sxs-lookup"><span data-stu-id="b0102-126">PEC is calculated on daily basis on the managed Azure assets.</span></span> <span data-ttu-id="b0102-127">给定计费周期（月份）的 PEC 不超过 15%。</span><span class="sxs-lookup"><span data-stu-id="b0102-127">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="b0102-128">如果合作伙伴针对所有符合条件的资源（访问范围）保留持久性特权访问一整月（范围跨度），他们将获得完整 15% 的 PEC。</span><span class="sxs-lookup"><span data-stu-id="b0102-128">Partners retaining persistent privileged access through the month(span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="b0102-129">范围和跨度变小将导致当月 PEC 比率变低。</span><span class="sxs-lookup"><span data-stu-id="b0102-129">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="b0102-130">无论是否应用了 PEC，针对 Azure 资产，每天都会显示按每日计费的使用量文件。</span><span class="sxs-lookup"><span data-stu-id="b0102-130">Daily rated usage file shows on daily basis on an Azure asset whether PEC is applied or not.</span></span> <span data-ttu-id="b0102-131">合作伙伴还可注册接收警报，以检测持久性特权访问是否有变化。</span><span class="sxs-lookup"><span data-stu-id="b0102-131">Partners can also enroll in alerts to detect if there are changes to persistent privileged access.</span></span>

- <span data-ttu-id="b0102-132">可赚取 PEC 的最低级别为 Azure 资源级别。</span><span class="sxs-lookup"><span data-stu-id="b0102-132">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="b0102-133">如果合作伙伴在订阅或资源组级别拥有有效的访问权限，则他们可以赚取该角色直到更高一级实体的资源的 PEC。</span><span class="sxs-lookup"><span data-stu-id="b0102-133">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="b0102-134">[Azure 成本管理](/azure/cost-management-billing/costs/get-started-partners)中也提供了 PEC 详细信息</span><span class="sxs-lookup"><span data-stu-id="b0102-134">PEC details will also be available on [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="b0102-135">Azure 成本管理</span><span class="sxs-lookup"><span data-stu-id="b0102-135">Azure Cost Management</span></span>

<span data-ttu-id="b0102-136">使用成本分析的 Azure 成本管理 (ACM) 能够让你以合作伙伴的身份查看已享有 PEC 权益的费用。</span><span class="sxs-lookup"><span data-stu-id="b0102-136">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="b0102-137">在 [Azure 门户](https://portal.azure.com)中，登录到合作伙伴租户，并选择“成本管理”+“计费”。</span><span class="sxs-lookup"><span data-stu-id="b0102-137">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="b0102-138">选择“成本管理”</span><span class="sxs-lookup"><span data-stu-id="b0102-138">Select **Cost management**</span></span>

3. <span data-ttu-id="b0102-139">选择“成本分析”</span><span class="sxs-lookup"><span data-stu-id="b0102-139">Select **Cost Analysis**</span></span>

   <span data-ttu-id="b0102-140">成本分析视图将显示计费帐户的成本，即以你支付给 Microsoft 的价格购买和使用的所有服务的成本。</span><span class="sxs-lookup"><span data-stu-id="b0102-140">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="b0102-141">在数据透视图的下拉菜单中选择 PartnerEarnedCreditApplied，以查看应用了 PEC 的成本。</span><span class="sxs-lookup"><span data-stu-id="b0102-141">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="b0102-142">如果 PartnerEarnedCreditApplied 属性为 True，则表示关联的成本享有合作伙伴赚取的返点的权益。</span><span class="sxs-lookup"><span data-stu-id="b0102-142">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="b0102-143">如果 PartnerEarnedCreditApplied 属性为 False，则表示关联的成本不满足所需的返点条件，或者购买的服务不符合合作伙伴赚取的返点条件。</span><span class="sxs-lookup"><span data-stu-id="b0102-143">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="b0102-144">通常情况下，服务的使用情况在 8-24 小时后才会出现在“成本管理”中，PEC 额度自访问时间起 48 小时内显示在“Azure 成本管理”中。</span><span class="sxs-lookup"><span data-stu-id="b0102-144">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="b0102-145">还可以使用“分组依据和添加”筛选器功能按 PartnerEarnedCreditApplied 属性进行分组和筛选，从而深入分析享有 PEC 权益的成本以及没有应用 PEC 的成本 。</span><span class="sxs-lookup"><span data-stu-id="b0102-145">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b0102-146">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b0102-146">Next steps</span></span>

- [<span data-ttu-id="b0102-147">合作伙伴赚取的返点 - 概述</span><span class="sxs-lookup"><span data-stu-id="b0102-147">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="b0102-148">在可通过合作伙伴中心仪表板访问（需要登录）的价目表中，提供了合作伙伴赚取的返点的计算方式的详细示例。</span><span class="sxs-lookup"><span data-stu-id="b0102-148">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="b0102-149">转移到 Azure 计划 - 入门</span><span class="sxs-lookup"><span data-stu-id="b0102-149">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="b0102-150">管理 Azure 计划中的订阅和资源</span><span class="sxs-lookup"><span data-stu-id="b0102-150">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="b0102-151">撤销或恢复 Azure CSP 订阅的管理员权限</span><span class="sxs-lookup"><span data-stu-id="b0102-151">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
