---
title: Azure 计划 - 管理订阅和资源
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解合作伙伴如何使用不同基于角色的访问控制 (RBAC) 选项来获得对客户 Azure 资源的操作控制和管理。
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534924"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a><span data-ttu-id="76518-103">管理 Azure 计划中的订阅和资源</span><span class="sxs-lookup"><span data-stu-id="76518-103">Manage subscriptions and resources under the Azure plan</span></span>

<span data-ttu-id="76518-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="76518-104">**Appropriate roles**</span></span>

- <span data-ttu-id="76518-105">管理员代理</span><span class="sxs-lookup"><span data-stu-id="76518-105">Admin agent</span></span>


<span data-ttu-id="76518-106">本文介绍了 CSP 合作伙伴如何使用不同的基于角色的访问控制 (RBAC) 选项对客户的 Azure 资源进行操作控制和管理。</span><span class="sxs-lookup"><span data-stu-id="76518-106">This article explains how CSP partners can use different role-based access control (RBAC) options to gain operational control and management of a customer's Azure resources.</span></span> <span data-ttu-id="76518-107">将客户过渡到 Azure 计划时，默认你会获得 Azure 中的特权管理员权限（由管理员代表授予的订阅所有者权限）。</span><span class="sxs-lookup"><span data-stu-id="76518-107">When you transition a customer to the Azure plan, you are assigned privileged admin rights in Azure (subscription owner rights through admin on behalf of) by default.</span></span>

 > [!NOTE]
 > <span data-ttu-id="76518-108">客户可以在订阅、资源组或工作负荷级别删除 Azure 订阅的管理员权限。</span><span class="sxs-lookup"><span data-stu-id="76518-108">Admin rights to the Azure subscription can be removed by the customer at a subscription, resource group, or workload level.</span></span> 

 <span data-ttu-id="76518-109">合作伙伴可以使用通过基于角色的访问控制功能 (RBAC) 提供的不同选项，获取对客户在云解决方案提供商中的 Azure 资源的全天候操作控制和管理权限。</span><span class="sxs-lookup"><span data-stu-id="76518-109">Partners can gain 24x7 operational control and management of a customer's Azure resources in CSP by using different options provided through the role-based access control feature (RBAC).</span></span> 

- <span data-ttu-id="76518-110">管理员代表 (AOBO) - 借助 [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)，在合作伙伴租户中具有“管理员代理”角色的任何用户将对你通过云解决方案提供商计划创建的 Azure 订阅拥有 RBAC 所有者访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-110">**Admin on Behalf Of (AOBO)** - With [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), any user with the Admin Agent role in the partner tenant will have RBAC owner access to Azure subscriptions that you create through the CSP program.</span></span>

- <span data-ttu-id="76518-111">**Azure Lighthouse**：使用 AOBO 不能灵活地创建处理不同客户的不同组，或者为组或用户启用不同的角色。</span><span class="sxs-lookup"><span data-stu-id="76518-111">**Azure Lighthouse**: AOBO doesn't allow the flexibility to create distinct groups that work with different customers, or to enable different roles for groups or users.</span></span> <span data-ttu-id="76518-112">使用 Azure Lighthouse 可将不同的组分配到不同的客户或角色。</span><span class="sxs-lookup"><span data-stu-id="76518-112">Using Azure Lighthouse, you can assign different groups to different customers or roles.</span></span> <span data-ttu-id="76518-113">由于用户将通过 Azure 委托的资源管理获取适当的访问级别，因此你可以减少具有“管理员代理”角色的用户数量（因此拥有完全 AOBO 访问权限）。</span><span class="sxs-lookup"><span data-stu-id="76518-113">Because users will have the appropriate level of access through Azure delegated resource management, you can reduce the number of users who have the Admin Agent role (and thus have full AOBO access).</span></span> <span data-ttu-id="76518-114">这有助于通过限制对客户资源的不必要访问权限来提高安全性。</span><span class="sxs-lookup"><span data-stu-id="76518-114">This helps improve security by limiting unnecessary access to your customers' resources.</span></span> <span data-ttu-id="76518-115">此外，它还可以让你更灵活地大规模管理多个客户。</span><span class="sxs-lookup"><span data-stu-id="76518-115">It also gives you more flexibility to manage multiple customers at scale.</span></span> <span data-ttu-id="76518-116">有关详细信息，请参阅 [Azure Lighthouse 和云解决方案提供商计划](/azure/lighthouse/concepts/cloud-solution-provider)。</span><span class="sxs-lookup"><span data-stu-id="76518-116">For more information, read [Azure Lighthouse and the Cloud Solution Provider program](/azure/lighthouse/concepts/cloud-solution-provider).</span></span>

- <span data-ttu-id="76518-117">**目录用户、来宾用户或 [服务主体](/azure/active-directory/develop/app-objects-and-service-principals)** ：可以通过将用户添加到客户目录，或者添加来宾用户并分配特定的 RBAC 角色，来委托对 CSP 订阅的精细访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-117">**Directory or Guest Users or [Service Principals](/azure/active-directory/develop/app-objects-and-service-principals)**: You can delegate granular access to CSP subscriptions by adding users in the customer directory or adding guest users and assigning specific RBAC roles.</span></span>

<span data-ttu-id="76518-118">Microsoft 建议为用户分配最低的权限，使他们能够履行自己的职责即可，这是一种安全做法。</span><span class="sxs-lookup"><span data-stu-id="76518-118">Microsoft recommends that users have the minimum permissions they need to perform their work as a security practice.</span></span> <span data-ttu-id="76518-119">请参阅 [Azure Active Directory Privileged Identity Management 资源](/azure/active-directory/privileged-identity-management/pim-configure)。</span><span class="sxs-lookup"><span data-stu-id="76518-119">See [Azure Active Directory Privileged Identity Management resources](/azure/active-directory/privileged-identity-management/pim-configure).</span></span>

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a><span data-ttu-id="76518-120">将合作伙伴 ID (MPN ID) 链接到用于管理客户 Azure 资源的凭据</span><span class="sxs-lookup"><span data-stu-id="76518-120">Link your partner ID (MPN ID)to your credentials for managing customer's Azure resources</span></span>

<span data-ttu-id="76518-121">下表显示了用于将合作伙伴 ID 关联到各种 RBAC 访问选项的方法。</span><span class="sxs-lookup"><span data-stu-id="76518-121">The following table shows the methods used to associate your partner ID with various RBAC access options.</span></span>

|<span data-ttu-id="76518-122">**类别**</span><span class="sxs-lookup"><span data-stu-id="76518-122">**Category**</span></span>   |<span data-ttu-id="76518-123">**方案**</span><span class="sxs-lookup"><span data-stu-id="76518-123">**Scenario**</span></span>   |<span data-ttu-id="76518-124">**MPN ID 关联**</span><span class="sxs-lookup"><span data-stu-id="76518-124">**MPN ID association**</span></span>|
|-----------------|:------------------------|:------------------|
|<span data-ttu-id="76518-125">AOBO</span><span class="sxs-lookup"><span data-stu-id="76518-125">AOBO</span></span>   |<span data-ttu-id="76518-126">CSP 直接合作伙伴或间接提供商为客户创建订阅，并使用 AOBO 将 CSP 直接伙伴或间接提供商指定为该订阅的默认所有者；CSP 直接合作伙伴或间接提供商使用 AOBO 向间接经销商授予对该订阅的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-126">CSP direct partner or indirect provider creates the subscription for the customer making the CSP direct partner or indirect provider default owner of the subscription using AOBO.; CSP direct partner or indirect provider give indirect reseller access to the subscription using AOBO.</span></span>|<span data-ttu-id="76518-127">自动（无需合作伙伴的干预）</span><span class="sxs-lookup"><span data-stu-id="76518-127">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="76518-128">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="76518-128">Azure Lighthouse</span></span>|<span data-ttu-id="76518-129">合作伙伴[在市场中创建新的托管服务套餐](/azure/lighthouse/concepts/managed-services-offers)。</span><span class="sxs-lookup"><span data-stu-id="76518-129">Partner creates a new [Managed Services offer in Marketplace](/azure/lighthouse/concepts/managed-services-offers).</span></span> <span data-ttu-id="76518-130">此套餐在 CSP 订阅中接受，合作伙伴获取对该 CSP 订阅的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-130">This offer is accepted on the CSP subscription and partner gets access to the CSP subscription.</span></span>|<span data-ttu-id="76518-131">自动（无需合作伙伴的干预）</span><span class="sxs-lookup"><span data-stu-id="76518-131">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="76518-132">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="76518-132">Azure Lighthouse</span></span>|<span data-ttu-id="76518-133">合作伙伴在 Azure 订阅中部署 [ARM 模板](/azure/lighthouse/how-to/onboard-customer)</span><span class="sxs-lookup"><span data-stu-id="76518-133">Partner deploys [ARM template](/azure/lighthouse/how-to/onboard-customer) in Azure subscription</span></span>|<span data-ttu-id="76518-134">合作伙伴需要将 MPN ID 关联到合作伙伴租户中的用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="76518-134">Partner needs to associate the MPN ID to the user or service principal in the partner tenant.</span></span> <span data-ttu-id="76518-135">有关详细信息，请参阅[链接合作伙伴 ID](/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="76518-135">For more information - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).</span></span>|
|<span data-ttu-id="76518-136">目录或来宾用户</span><span class="sxs-lookup"><span data-stu-id="76518-136">Directory or guest user</span></span>|<span data-ttu-id="76518-137">合作伙伴在客户目录中创建新的用户或服务主体，并向用户授予对 CSP 订阅的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-137">Partner creates a new user or service principal in the customer directory and gives access to the CSP subscription to the user.</span></span> <span data-ttu-id="76518-138">合作伙伴在客户目录中创建新的用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="76518-138">Partner creates a new user or service principal in the customer directory.</span></span> <span data-ttu-id="76518-139">伙伴将用户添加到某个组，并向该组授予对 CSP 订阅的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-139">Partner adds the user to a group and gives access to the CSP subscription to the group.</span></span>|<span data-ttu-id="76518-140">合作伙伴需要将 MPN ID 关联到客户租户中的用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="76518-140">Partner needs to associate the MPN ID to the user or service principal in the customer tenant.</span></span> <span data-ttu-id="76518-141">有关详细信息，请参阅[链接合作伙伴 ID](/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="76518-141">For more information - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).</span></span>|

## <a name="confirm-that-you-have-admin-access"></a><span data-ttu-id="76518-142">确认你拥有管理员访问权限</span><span class="sxs-lookup"><span data-stu-id="76518-142">Confirm that you have admin access</span></span>

<span data-ttu-id="76518-143">你需要拥有管理员访问权限才能管理客户的服务和接收赚取的返点。</span><span class="sxs-lookup"><span data-stu-id="76518-143">You require admin access to manage your customer's services and to received earned credits.</span></span> <span data-ttu-id="76518-144">有关赚取的返点的详细信息，请阅读[合作伙伴赚取的返点](partner-earned-credit.md)</span><span class="sxs-lookup"><span data-stu-id="76518-144">Read [Partner earned credits](partner-earned-credit.md) for detailed information on earned credits.</span></span> <span data-ttu-id="76518-145">可通过两种方式来确认你是否拥有管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-145">You have two ways to make sure you know that you have admin access.</span></span>

- <span data-ttu-id="76518-146">查看每日使用情况文件 - 可以通过查看每日使用情况文件中的单价和有效单价，并确认当前是否应用了某种折扣，来确定你是否拥有管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-146">Review the daily usage file - This can be determined by reviewing the unit price and effective unit price within the daily usage file and confirming if a discount is being applied.</span></span> <span data-ttu-id="76518-147">如果收到了折扣，则你是管理员。</span><span class="sxs-lookup"><span data-stu-id="76518-147">If you are receiving the discount you are the admin.</span></span>

- <span data-ttu-id="76518-148">创建 Azure Monitor 警报 - 可以创建 Azure Monitor 活动日志[警报](/azure/azure-monitor/platform/alerts-activity-log)，如果从 CSP 订阅中删除了你的 RBAC 访问权限，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="76518-148">Create an Azure monitor alert - You can create an Azure Monitor activity log [alert](/azure/azure-monitor/platform/alerts-activity-log) to be notified of  when your RBAC access is removed from CSP subscription.</span></span>

### <a name="create-an-azure-monitor-alert"></a><span data-ttu-id="76518-149">创建 Azure Monitor 警报</span><span class="sxs-lookup"><span data-stu-id="76518-149">Create an Azure monitor alert</span></span>

1. <span data-ttu-id="76518-150">创建警报</span><span class="sxs-lookup"><span data-stu-id="76518-150">Create alert.</span></span>

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure 警报":::

2. <span data-ttu-id="76518-152">选择希望警报执行的操作类型。例如，如果指定电子邮件，则发生任何角色分配删除操作时，你会收到一封通知电子邮件。</span><span class="sxs-lookup"><span data-stu-id="76518-152">Select the type of action you want the alert to take.For example, if you specify that you want an email, you will receive an email notifying you if any role assignment deletion occurs.</span></span>

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="配置警报":::

### <a name="aobo-removal"></a><span data-ttu-id="76518-154">AOBO 删除</span><span class="sxs-lookup"><span data-stu-id="76518-154">AOBO removal</span></span>

<span data-ttu-id="76518-155">客户可以在 Azure 门户上的“访问控制”中管理对其订阅的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-155">Customers can manage access to their subscriptions by going to **Access Control** on the Azure portal.</span></span> <span data-ttu-id="76518-156">在“角色分配”选项卡中，选择“删除访问权限”即可。 </span><span class="sxs-lookup"><span data-stu-id="76518-156">From the **Role assignments** tab, they select **Remove access**.</span></span> <span data-ttu-id="76518-157">如果发生这种情况，你可以：</span><span class="sxs-lookup"><span data-stu-id="76518-157">If this happens, you can:</span></span>

- <span data-ttu-id="76518-158">与客户沟通，看看是否可以恢复管理访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-158">Talk with your customer to see if admin access can be reinstated.</span></span>

- <span data-ttu-id="76518-159">使用通过[基于角色的访问控制 (RBAC)](/azure/role-based-access-control/overview) 提供的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-159">Use the access provided through [role-based access control (RBAC)](/azure/role-based-access-control/overview).</span></span>

- <span data-ttu-id="76518-160">使用通过 [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) 提供的访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-160">Use access provided through [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).</span></span>

<span data-ttu-id="76518-161">基于角色的访问权限不同于管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="76518-161">Role-based access differs from admin access.</span></span> <span data-ttu-id="76518-162">角色精确界定你可以和不可以执行的操作。</span><span class="sxs-lookup"><span data-stu-id="76518-162">Roles delimit precisely what you can and can't do.</span></span> <span data-ttu-id="76518-163">管理员访问权限更广泛。</span><span class="sxs-lookup"><span data-stu-id="76518-163">Admin access is broader.</span></span>

<span data-ttu-id="76518-164">若要查看有资格赚取 PEC 的角色，请阅读[可赚取返点的合作伙伴的角色和权限](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)。</span><span class="sxs-lookup"><span data-stu-id="76518-164">To see the roles eligible to earn PEC, read [Roles and permissions for the partner earned credit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).</span></span>

## <a name="next-steps"></a><span data-ttu-id="76518-165">后续步骤</span><span class="sxs-lookup"><span data-stu-id="76518-165">Next steps</span></span>

- [<span data-ttu-id="76518-166">撤销和恢复 Azure CSP 订阅的管理员权限</span><span class="sxs-lookup"><span data-stu-id="76518-166">Revoking and reinstating admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)

- [<span data-ttu-id="76518-167">合作伙伴赚取的返点 - 概述</span><span class="sxs-lookup"><span data-stu-id="76518-167">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- [<span data-ttu-id="76518-168">合作伙伴赚取的托管服务返点</span><span class="sxs-lookup"><span data-stu-id="76518-168">Partner earned credit for managed services</span></span>](partner-earned-credit-explanation.md)