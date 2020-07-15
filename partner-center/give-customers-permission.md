---
title: 让客户在 CSP 中购买自己的服务
description: 了解 CSP 计划合作伙伴如何允许客户购买其自己的服务（如 Azure 保留），以用于为合作伙伴中心购买的订阅。
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
Keywords: 订阅，自助服务购买，自助服务 RI，启用 RI，禁用 RI，自助服务，客户购买，客户权限，客户采购预订实例，客户购买 Azure 保留，启用自助服务，关闭自助服务
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 62447e284ce35b414594031c590110cedc5a59ab
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377451"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="8d837-104">向客户授予合作伙伴中心的权限，以购买自己的产品或服务</span><span class="sxs-lookup"><span data-stu-id="8d837-104">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="8d837-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="8d837-105">**Applies to**</span></span>

- <span data-ttu-id="8d837-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8d837-106">Partner Center</span></span>
- <span data-ttu-id="8d837-107">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="8d837-107">Partners in the CSP program</span></span>

<span data-ttu-id="8d837-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="8d837-108">**Appropriate roles**</span></span>

- <span data-ttu-id="8d837-109">管理员代理</span><span class="sxs-lookup"><span data-stu-id="8d837-109">Admin agent</span></span>
- <span data-ttu-id="8d837-110">销售代理</span><span class="sxs-lookup"><span data-stu-id="8d837-110">Sales agent</span></span>

<span data-ttu-id="8d837-111">本文介绍了云解决方案提供商（CSP）计划中的合作伙伴如何向客户提供购买一些自己的服务或资源的权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-111">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="8d837-112">CSP 计划中的合作伙伴通常使用合作伙伴中心及其商业市场为客户购买解决方案和服务。</span><span class="sxs-lookup"><span data-stu-id="8d837-112">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="8d837-113">然后，合作伙伴允许一些客户直接从 Azure 门户预配这些服务。</span><span class="sxs-lookup"><span data-stu-id="8d837-113">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="8d837-114">下面是一个示例。</span><span class="sxs-lookup"><span data-stu-id="8d837-114">Here's an example.</span></span> <span data-ttu-id="8d837-115">假设你为合作伙伴中心的客户购买 Azure 计划订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-115">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="8d837-116">然后，你决定将其他资源或服务代表客户添加到该订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-116">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="8d837-117">在这种情况下，你可以向客户的订阅添加 Azure 保留项（例如，添加预留的虚拟机实例）。</span><span class="sxs-lookup"><span data-stu-id="8d837-117">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="8d837-118">然后，你可以允许客户在 Azure 门户中进一步预配 Azure 预订资源。</span><span class="sxs-lookup"><span data-stu-id="8d837-118">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="8d837-119">现在，通过 "**客户权限**" 功能，你可以向客户提供 Azure 资源的更多自助服务选项。</span><span class="sxs-lookup"><span data-stu-id="8d837-119">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="8d837-120">通过为客户启用权限，你可以让客户购买自己的资源（例如，购买自己的 Azure 预订）。</span><span class="sxs-lookup"><span data-stu-id="8d837-120">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="8d837-121">合作伙伴中心的客户权限概述</span><span class="sxs-lookup"><span data-stu-id="8d837-121">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="8d837-122">使用 "客户**帐户**" 页可以打开（或关闭）客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-122">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="8d837-123">目前，此功能支持：</span><span class="sxs-lookup"><span data-stu-id="8d837-123">Currently, this feature supports:</span></span>

- <span data-ttu-id="8d837-124">**Azure 保留：** 如果启用此权限，则客户可以为你为其购买的特定 Azure 订阅购买自己的 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="8d837-124">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="8d837-125">在打开客户权限之前，请注意以下重要事项：</span><span class="sxs-lookup"><span data-stu-id="8d837-125">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="8d837-126">默认情况下，会在合作伙伴中心中自动禁用（关闭）客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-126">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="8d837-127">在为客户打开（或关闭）权限之前，必须在合作伙伴中心为你分配 "管理员代理" 角色。</span><span class="sxs-lookup"><span data-stu-id="8d837-127">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="8d837-128">分配有 "销售代理" 或 "技术支持" 代理角色的合作伙伴具有只读访问权限，并且不能打开或关闭客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-128">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="8d837-129">你可以为所选的任何客户打开（启用）权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-129">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="8d837-130">你可以使用合作伙伴中心仪表板或[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/manage-customers)打开（或关闭）客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-130">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="8d837-131">为特定客户启用（启用）权限后，你将负责为该客户所进行的任何后续购买付费。</span><span class="sxs-lookup"><span data-stu-id="8d837-131">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="8d837-132">如果客户想要交换、取消或续订已进行的购买（或者他们想要更改预订的初始范围），他们将无法自行完成此操作。</span><span class="sxs-lookup"><span data-stu-id="8d837-132">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="8d837-133">他们需要询问你，作为合作伙伴，帮助他们交换、取消和续订购买，或在以后对预订范围做出更改。</span><span class="sxs-lookup"><span data-stu-id="8d837-133">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="8d837-134">为特定客户启用权限后，你将**不**会收到客户对你的任何以后购买的通知。</span><span class="sxs-lookup"><span data-stu-id="8d837-134">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="8d837-135">以后购买的客户将显示在合作伙伴中心，以及你所做的任何购买。</span><span class="sxs-lookup"><span data-stu-id="8d837-135">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="8d837-136">您可以在客户的**订单历史记录**页、其**预订**页或[**活动日志**](activity-logs.md)中找到这些购买内容。</span><span class="sxs-lookup"><span data-stu-id="8d837-136">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="8d837-137">有关客户将支付的价格以及如何帮助客户管理其购买的信息，请参阅[帮助客户管理他们购买的预订](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="8d837-137">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="8d837-138">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="8d837-138">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="8d837-139">Azure 预订是以折扣价购买 Azure 服务的一种绝佳方式。</span><span class="sxs-lookup"><span data-stu-id="8d837-139">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="8d837-140">若要详细了解 Azure 保留项的优点，请参阅[什么是 Azure 保留？](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="8d837-140">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="8d837-141">现在，你可以选择代表你的客户购买 Azure 预订，因为你可能已经做了。</span><span class="sxs-lookup"><span data-stu-id="8d837-141">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="8d837-142">或者，你可以授予客户购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-142">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="8d837-143">向客户授予购买自己的 Azure 预订的权限后，可帮助他们管理他们购买的任何预订。</span><span class="sxs-lookup"><span data-stu-id="8d837-143">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="8d837-144">有关详细信息，请参阅[帮助客户管理他们购买的预订](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="8d837-144">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="8d837-145">让客户购买自己的 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="8d837-145">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="8d837-146">验证客户是否有代表你购买的现有 Azure 计划或 Azure 全局订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-146">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="8d837-147">验证是否已为客户分配此订阅的**所有者**角色。</span><span class="sxs-lookup"><span data-stu-id="8d837-147">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="8d837-148">启用客户权限（启用**此功能）** 以购买自己的 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="8d837-148">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="8d837-149">每个步骤如下所示。</span><span class="sxs-lookup"><span data-stu-id="8d837-149">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="8d837-150">验证客户是否有现有的 Azure 订阅</span><span class="sxs-lookup"><span data-stu-id="8d837-150">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="8d837-151">在向客户提供购买其自己的 Azure 预订的权限之前，必须确保客户具有现有的 Azure 计划或 Azure 全局订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-151">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="8d837-152">如果客户在合作伙伴中心未显示当前的 Azure 订阅，则必须先为订阅购买订阅，然后才能打开其客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-152">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="8d837-153">若要查看客户是否已有 Azure 订阅，请登录到合作伙伴中心仪表板，然后选择 " **CSP**后跟**客户**"。</span><span class="sxs-lookup"><span data-stu-id="8d837-153">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="8d837-154">从列表中选择特定的客户。</span><span class="sxs-lookup"><span data-stu-id="8d837-154">Select the specific customer from the list.</span></span> <span data-ttu-id="8d837-155">然后，选择 "**订阅**"，并查找适用于 azure 计划或 azure Global 的任何基于使用情况的订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-155">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="8d837-156">如果客户没有现有的 Azure 订阅，你可以购买订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-156">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="8d837-157">请参阅[购买 Azure 计划](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="8d837-157">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="8d837-158">验证是否在 Azure 中为客户分配了正确的角色</span><span class="sxs-lookup"><span data-stu-id="8d837-158">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="8d837-159">验证客户是否有现有 Azure 订阅后，还需要验证与客户关联的密钥用户是否已被分配了正确的 Azure 订阅**所有者**角色。</span><span class="sxs-lookup"><span data-stu-id="8d837-159">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="8d837-160">这是基于角色的访问（RBAC），客户需要为你购买的 Azure 订阅购买 Azure 保留项。</span><span class="sxs-lookup"><span data-stu-id="8d837-160">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="8d837-161">某些合作伙伴可能已将 "**所有者**" 角色分配给想要主动管理和预配自己的 Azure 资源的客户。</span><span class="sxs-lookup"><span data-stu-id="8d837-161">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="8d837-162">如果已为客户分配了 "**所有者**状态" 以管理为其购买的以前的订阅，则可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="8d837-162">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="8d837-163">如果尚未为某个客户分配 "**所有者**" 角色，则他们将收到一个错误，Azure 门户阻止他们购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="8d837-163">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="8d837-164">若要验证是否已为客户分配 Azure 订阅的**所有者**角色，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="8d837-164">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="8d837-165">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="8d837-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8d837-166">依次选择 " **CSP**"、"**客户**" 和 "特定客户"。</span><span class="sxs-lookup"><span data-stu-id="8d837-166">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="8d837-167">选择该客户的**订阅**，并找到特定的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="8d837-167">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="8d837-168">选择该客户的订阅旁边的 "**管理**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="8d837-168">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="8d837-169">这样做会打开[Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="8d837-169">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="8d837-170">若要将**所有者**角色分配给特定用户，请按照以下步骤将[用户分配为管理员](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。</span><span class="sxs-lookup"><span data-stu-id="8d837-170">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="8d837-171">启用或禁用客户权限以购买自己的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="8d837-171">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="8d837-172">验证客户是否有现有的 Azure 订阅，并为用户分配了该订阅的**所有者**角色后，便可以打开（启用）客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-172">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="8d837-173">你还可以使用这些步骤来关闭（禁用）客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-173">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="8d837-174">你可以使用合作伙伴中心仪表板或[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/manage-customers)启用或禁用客户权限。</span><span class="sxs-lookup"><span data-stu-id="8d837-174">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="8d837-175">若要在合作伙伴中心打开（或关闭）客户权限：</span><span class="sxs-lookup"><span data-stu-id="8d837-175">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="8d837-176">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="8d837-176">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8d837-177">从左侧导航菜单中，依次选择 " **CSP**"、"**客户**"。</span><span class="sxs-lookup"><span data-stu-id="8d837-177">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="8d837-178">此时将显示客户列表。</span><span class="sxs-lookup"><span data-stu-id="8d837-178">A customer list appears.</span></span>

3. <span data-ttu-id="8d837-179">选择特定的客户名称。</span><span class="sxs-lookup"><span data-stu-id="8d837-179">Select a specific customer name.</span></span>

4. <span data-ttu-id="8d837-180">从 "客户" 菜单中选择 "**帐户**"。</span><span class="sxs-lookup"><span data-stu-id="8d837-180">Select **Account** from the customer menu.</span></span> <span data-ttu-id="8d837-181">此时会显示 "客户**帐户**" 页。</span><span class="sxs-lookup"><span data-stu-id="8d837-181">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="8d837-182">查找页面底部的 "**客户权限**" 区域。</span><span class="sxs-lookup"><span data-stu-id="8d837-182">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="客户权限帐户页。" border="true":::

6. <span data-ttu-id="8d837-184">在 " **Azure 保留**" 下，找到 "**允许客户购买**" 选项。</span><span class="sxs-lookup"><span data-stu-id="8d837-184">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="8d837-185">若要启用客户权限，请将此选项旁的开关移到 "**开**" 位置。</span><span class="sxs-lookup"><span data-stu-id="8d837-185">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="8d837-186">若要关闭客户权限，请将开关移到 "**关闭**" 位置。</span><span class="sxs-lookup"><span data-stu-id="8d837-186">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="8d837-187">若要了解当你打开客户的权限来购买自己的 Azure 预订时，还会发生什么情况，请参阅[合作伙伴中心的客户权限概述](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="8d837-187">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="8d837-188">当你打开（或关闭）客户权限时，活动日志将记录每个操作。</span><span class="sxs-lookup"><span data-stu-id="8d837-188">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="8d837-189">（如果从 "合作伙伴中心" 仪表板顶部选择齿轮图标，则可以访问此日志）。</span><span class="sxs-lookup"><span data-stu-id="8d837-189">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="8d837-190">当你打开或关闭客户权限时，该操作将在活动日志中显示为 "**创建客户购买权限**" 或 "**删除客户购买权限**"。</span><span class="sxs-lookup"><span data-stu-id="8d837-190">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="8d837-191">帮助客户管理他们购买的预订</span><span class="sxs-lookup"><span data-stu-id="8d837-191">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="8d837-192">一旦你向客户提供购买其自己的 Azure 预订的权限，你就可以帮助他们更好地管理他们购买的任何资源。</span><span class="sxs-lookup"><span data-stu-id="8d837-192">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="8d837-193">客户可以直接从[Azure 门户](https://portal.azure.com/)管理 Azure 预订的许多方面。</span><span class="sxs-lookup"><span data-stu-id="8d837-193">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="8d837-194">他们将需要你的帮助来管理他们在 CSP 订阅中购买的 Azure 保留部分的其他方面。</span><span class="sxs-lookup"><span data-stu-id="8d837-194">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="8d837-195">帮助客户更详细地了解如何管理 Azure 预订的这些方面：</span><span class="sxs-lookup"><span data-stu-id="8d837-195">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="8d837-196">价格客户将支付 Azure 预订费用</span><span class="sxs-lookup"><span data-stu-id="8d837-196">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="8d837-197">客户如何优化 Azure 预订的使用</span><span class="sxs-lookup"><span data-stu-id="8d837-197">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="8d837-198">当客户购买具有共享作用域的预留时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="8d837-198">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="8d837-199">如果客户想要更改、取消和续订预订，或更改其作用域，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="8d837-199">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="8d837-200">**价格客户将为其预留付费。**</span><span class="sxs-lookup"><span data-stu-id="8d837-200">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="8d837-201">你的客户将根据你先前为 CSP 合作伙伴计费帐户购买的订阅购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="8d837-201">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="8d837-202">客户根据此订阅购买的任何 Azure 预订的价格也由您设置。</span><span class="sxs-lookup"><span data-stu-id="8d837-202">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="8d837-203">此价格可能与客户在 Azure 门户中看到的 Web 直接价格不同。</span><span class="sxs-lookup"><span data-stu-id="8d837-203">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="8d837-204">**客户如何优化预订的使用。**</span><span class="sxs-lookup"><span data-stu-id="8d837-204">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="8d837-205">一些客户可以从了解有关如何优化预订使用情况的详细信息，或者如何在购买过程中分配预订的初始范围。</span><span class="sxs-lookup"><span data-stu-id="8d837-205">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="8d837-206">有关详细信息，请客户阅读[Azure 资源的管理预订](https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。</span><span class="sxs-lookup"><span data-stu-id="8d837-206">For more information, ask customers to read [Manage reservations for Azure resources](https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="8d837-207">**当客户购买具有共享作用域的预订时，会发生什么情况？**</span><span class="sxs-lookup"><span data-stu-id="8d837-207">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="8d837-208">当客户基于之前的 CSP 订阅购买保留并为该预订分配共享范围时，CSP 提供的任何折扣将应用于 CSP 合作伙伴为该客户购买的所有订阅的匹配使用情况。</span><span class="sxs-lookup"><span data-stu-id="8d837-208">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="8d837-209">**如果客户想要交换、取消或续订已进行的购买，或更改保留的初始范围，应执行哪些操作？**</span><span class="sxs-lookup"><span data-stu-id="8d837-209">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="8d837-210">客户需要咨询合作伙伴来帮助他们更改保留的初始范围。</span><span class="sxs-lookup"><span data-stu-id="8d837-210">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="8d837-211">他们还需要合作伙伴的帮助来交换、取消或续订预订。</span><span class="sxs-lookup"><span data-stu-id="8d837-211">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="8d837-212">它们不能根据为 CSP 合作伙伴购买的订阅，使用预订来执行这些任务。</span><span class="sxs-lookup"><span data-stu-id="8d837-212">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8d837-213">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8d837-213">Next steps</span></span>

- [<span data-ttu-id="8d837-214">代表你的客户购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="8d837-214">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="8d837-215">合作伙伴中心-销售 Microsoft 预订</span><span class="sxs-lookup"><span data-stu-id="8d837-215">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="8d837-216">代表客户管理 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="8d837-216">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
