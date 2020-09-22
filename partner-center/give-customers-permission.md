---
title: 让客户在 CSP 中购买自己的服务
description: 了解 CSP 计划合作伙伴如何允许客户购买其自己的服务（如 Azure 保留），以用于为合作伙伴中心购买的订阅。
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19f86ec5353abc21e14a3a8ac2ef17dd17924cfe
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000461"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="9373e-103">向客户授予合作伙伴中心的权限，以购买自己的产品或服务</span><span class="sxs-lookup"><span data-stu-id="9373e-103">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="9373e-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="9373e-104">**Applies to**</span></span>

- <span data-ttu-id="9373e-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="9373e-105">Partner Center</span></span>
- <span data-ttu-id="9373e-106">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="9373e-106">Partners in the CSP program</span></span>

<span data-ttu-id="9373e-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="9373e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="9373e-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="9373e-108">Admin agent</span></span>
- <span data-ttu-id="9373e-109">销售代理</span><span class="sxs-lookup"><span data-stu-id="9373e-109">Sales agent</span></span>

<span data-ttu-id="9373e-110">本文介绍云解决方案提供商中的合作伙伴 (CSP) 计划如何向客户提供购买一些自己的服务或资源的权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-110">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="9373e-111">CSP 计划中的合作伙伴通常使用合作伙伴中心及其商业市场为客户购买解决方案和服务。</span><span class="sxs-lookup"><span data-stu-id="9373e-111">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="9373e-112">然后，合作伙伴允许一些客户直接从 Azure 门户预配这些服务。</span><span class="sxs-lookup"><span data-stu-id="9373e-112">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="9373e-113">下面是一个示例。</span><span class="sxs-lookup"><span data-stu-id="9373e-113">Here's an example.</span></span> <span data-ttu-id="9373e-114">假设你为合作伙伴中心的客户购买 Azure 计划订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-114">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="9373e-115">然后，你决定将其他资源或服务代表客户添加到该订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-115">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="9373e-116">在这种情况下，你可以向客户的订阅添加 Azure 保留 (例如，将预留的虚拟机实例添加) 。</span><span class="sxs-lookup"><span data-stu-id="9373e-116">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="9373e-117">然后，你可以允许客户在 Azure 门户中进一步预配 Azure 预订资源。</span><span class="sxs-lookup"><span data-stu-id="9373e-117">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="9373e-118">现在，通过 " **客户权限** " 功能，你可以向客户提供 Azure 资源的更多自助服务选项。</span><span class="sxs-lookup"><span data-stu-id="9373e-118">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="9373e-119">通过为客户启用权限，你可以让客户购买自己的资源， (例如购买自己的 Azure 预订) 。</span><span class="sxs-lookup"><span data-stu-id="9373e-119">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="9373e-120">合作伙伴中心的客户权限概述</span><span class="sxs-lookup"><span data-stu-id="9373e-120">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="9373e-121">使用 "客户 **帐户** " 页打开 (或关闭) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-121">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="9373e-122">目前，此功能支持：</span><span class="sxs-lookup"><span data-stu-id="9373e-122">Currently, this feature supports:</span></span>

- <span data-ttu-id="9373e-123">**Azure 保留：** 如果启用此权限，则客户可以为你为其购买的特定 Azure 订阅购买自己的 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="9373e-123">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="9373e-124">在打开客户权限之前，请注意以下重要事项：</span><span class="sxs-lookup"><span data-stu-id="9373e-124">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="9373e-125">默认情况下， (关闭合作伙伴中心) ，将自动禁用客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-125">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="9373e-126">你必须在合作伙伴中心为你分配 "管理员代理" 角色，然后才能打开 (或关闭客户的) 权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-126">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="9373e-127">分配有 "销售代理" 或 "技术支持" 代理角色的合作伙伴具有只读访问权限，并且不能打开或关闭客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-127">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="9373e-128">您可以打开 (为您选择的任何客户启用) 权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-128">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="9373e-129">你可以使用合作伙伴中心仪表板或 [合作伙伴中心 api](/partner-center/develop/manage-customers)打开 (或关闭) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-129">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="9373e-130">开启 (为特定客户启用) 权限后，你将负责为该客户所进行的任何后续购买付费。</span><span class="sxs-lookup"><span data-stu-id="9373e-130">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="9373e-131">如果客户想要交换、取消或续订已 (的购买，或者他们想要更改预订) 的初始范围，他们将不能这样做。</span><span class="sxs-lookup"><span data-stu-id="9373e-131">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="9373e-132">他们需要询问你，作为合作伙伴，帮助他们交换、取消和续订购买，或在以后对预订范围做出更改。</span><span class="sxs-lookup"><span data-stu-id="9373e-132">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="9373e-133">为特定客户启用权限后，你将 **不** 会收到客户对你的任何以后购买的通知。</span><span class="sxs-lookup"><span data-stu-id="9373e-133">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="9373e-134">以后购买的客户将显示在合作伙伴中心，以及你所做的任何购买。</span><span class="sxs-lookup"><span data-stu-id="9373e-134">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="9373e-135">您可以在客户的 **订单历史记录** 页、其 **预订** 页或 [**活动日志**](activity-logs.md)中找到这些购买内容。</span><span class="sxs-lookup"><span data-stu-id="9373e-135">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="9373e-136">有关客户将支付的价格以及如何帮助客户管理其购买的信息，请参阅 [帮助客户管理他们购买的预订](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="9373e-136">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="9373e-137">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="9373e-137">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="9373e-138">Azure 预订是以折扣价购买 Azure 服务的一种绝佳方式。</span><span class="sxs-lookup"><span data-stu-id="9373e-138">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="9373e-139">若要详细了解 Azure 保留项的优点，请参阅 [什么是 Azure 保留？](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="9373e-139">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="9373e-140">现在，你可以选择代表你的客户购买 Azure 预订，因为你可能已经做了。</span><span class="sxs-lookup"><span data-stu-id="9373e-140">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="9373e-141">或者，你可以授予客户购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-141">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="9373e-142">向客户授予购买自己的 Azure 预订的权限后，可帮助他们管理他们购买的任何预订。</span><span class="sxs-lookup"><span data-stu-id="9373e-142">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="9373e-143">有关详细信息，请参阅 [帮助客户管理他们购买的预订](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="9373e-143">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="9373e-144">让客户购买自己的 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="9373e-144">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="9373e-145">验证客户是否有代表你购买的现有 Azure 计划或 Azure 全局订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-145">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="9373e-146">验证是否已为客户分配此订阅的 **所有者** 角色。</span><span class="sxs-lookup"><span data-stu-id="9373e-146">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="9373e-147">启用客户权限 (**在) 上** 启用此功能，以购买自己的 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="9373e-147">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="9373e-148">每个步骤如下所示。</span><span class="sxs-lookup"><span data-stu-id="9373e-148">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="9373e-149">验证客户是否有现有的 Azure 订阅</span><span class="sxs-lookup"><span data-stu-id="9373e-149">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="9373e-150">在向客户提供购买其自己的 Azure 预订的权限之前，必须确保客户具有现有的 Azure 计划或 Azure 全局订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-150">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="9373e-151">如果客户在合作伙伴中心未显示当前的 Azure 订阅，则必须先为订阅购买订阅，然后才能打开其客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-151">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="9373e-152">若要查看客户是否已有 Azure 订阅，请登录到合作伙伴中心仪表板，然后选择 " **CSP** 后跟 **客户**"。</span><span class="sxs-lookup"><span data-stu-id="9373e-152">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="9373e-153">从列表中选择特定的客户。</span><span class="sxs-lookup"><span data-stu-id="9373e-153">Select the specific customer from the list.</span></span> <span data-ttu-id="9373e-154">然后，选择 " **订阅** "，并查找适用于 azure 计划或 azure Global 的任何基于使用情况的订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-154">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="9373e-155">如果客户没有现有的 Azure 订阅，你可以购买订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-155">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="9373e-156">请参阅 [购买 Azure 计划](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="9373e-156">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="9373e-157">验证是否在 Azure 中为客户分配了正确的角色</span><span class="sxs-lookup"><span data-stu-id="9373e-157">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="9373e-158">验证客户是否有现有 Azure 订阅后，还需要验证与客户关联的密钥用户是否已被分配了正确的 Azure 订阅 **所有者** 角色。</span><span class="sxs-lookup"><span data-stu-id="9373e-158">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="9373e-159">这是基于角色的访问 (RBAC) 客户需要为你购买的 Azure 订阅购买 Azure 保留项。</span><span class="sxs-lookup"><span data-stu-id="9373e-159">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="9373e-160">某些合作伙伴可能已将 " **所有者** " 角色分配给想要主动管理和预配自己的 Azure 资源的客户。</span><span class="sxs-lookup"><span data-stu-id="9373e-160">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="9373e-161">如果已为客户分配了 " **所有者** 状态" 以管理为其购买的以前的订阅，则可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="9373e-161">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="9373e-162">如果尚未为某个客户分配 " **所有者** " 角色，则他们将收到一个错误，Azure 门户阻止他们购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="9373e-162">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="9373e-163">若要验证是否已为客户分配 Azure 订阅的 **所有者** 角色，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="9373e-163">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="9373e-164">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="9373e-164">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9373e-165">依次选择 " **CSP**"、" **客户** " 和 "特定客户"。</span><span class="sxs-lookup"><span data-stu-id="9373e-165">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="9373e-166">选择该客户的 **订阅** ，并找到特定的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="9373e-166">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="9373e-167">选择该客户的订阅旁边的 " **管理** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="9373e-167">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="9373e-168">这样做会打开 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="9373e-168">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="9373e-169">若要将 **所有者** 角色分配给特定用户，请按照以下步骤将 [用户分配为管理员](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。</span><span class="sxs-lookup"><span data-stu-id="9373e-169">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="9373e-170">启用或禁用客户权限以购买自己的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="9373e-170">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="9373e-171">验证客户是否有现有的 Azure 订阅，并为用户分配了该订阅的 **所有者** 角色后，便可以打开 (启用) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-171">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="9373e-172">你还可以使用这些步骤关闭 (禁用) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-172">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="9373e-173">你可以使用合作伙伴中心仪表板或 [合作伙伴中心 api](/partner-center/develop/manage-customers)启用或禁用客户权限。</span><span class="sxs-lookup"><span data-stu-id="9373e-173">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="9373e-174">若要打开 (或关闭合作伙伴中心) 客户权限：</span><span class="sxs-lookup"><span data-stu-id="9373e-174">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="9373e-175">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="9373e-175">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9373e-176">从左侧导航菜单中，依次选择 " **CSP**"、" **客户**"。</span><span class="sxs-lookup"><span data-stu-id="9373e-176">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="9373e-177">此时将显示客户列表。</span><span class="sxs-lookup"><span data-stu-id="9373e-177">A customer list appears.</span></span>

3. <span data-ttu-id="9373e-178">选择特定的客户名称。</span><span class="sxs-lookup"><span data-stu-id="9373e-178">Select a specific customer name.</span></span>

4. <span data-ttu-id="9373e-179">从 "客户" 菜单中选择 " **帐户** "。</span><span class="sxs-lookup"><span data-stu-id="9373e-179">Select **Account** from the customer menu.</span></span> <span data-ttu-id="9373e-180">此时会显示 "客户 **帐户** " 页。</span><span class="sxs-lookup"><span data-stu-id="9373e-180">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="9373e-181">查找页面底部的 " **客户权限** " 区域。</span><span class="sxs-lookup"><span data-stu-id="9373e-181">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="客户权限帐户页。" border="true":::

6. <span data-ttu-id="9373e-183">在 " **Azure 保留**" 下，找到 " **允许客户购买** " 选项。</span><span class="sxs-lookup"><span data-stu-id="9373e-183">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="9373e-184">若要启用客户权限，请将此选项旁的开关移到 " **开** " 位置。</span><span class="sxs-lookup"><span data-stu-id="9373e-184">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="9373e-185">若要关闭客户权限，请将开关移到 " **关闭** " 位置。</span><span class="sxs-lookup"><span data-stu-id="9373e-185">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="9373e-186">若要了解当你打开客户的权限来购买自己的 Azure 预订时，还会发生什么情况，请参阅 [合作伙伴中心的客户权限概述](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="9373e-186">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="9373e-187">打开 (或关闭) 客户权限时，活动日志会记录每个操作。</span><span class="sxs-lookup"><span data-stu-id="9373e-187">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="9373e-188">从 "合作伙伴中心" 仪表板) 顶部选择齿轮图标时， (可以访问此日志。</span><span class="sxs-lookup"><span data-stu-id="9373e-188">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="9373e-189">当你打开或关闭客户权限时，该操作将在活动日志中显示为 " **创建客户购买权限** " 或 " **删除客户购买权限** "。</span><span class="sxs-lookup"><span data-stu-id="9373e-189">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="9373e-190">帮助客户管理他们购买的预订</span><span class="sxs-lookup"><span data-stu-id="9373e-190">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="9373e-191">一旦你向客户提供购买其自己的 Azure 预订的权限，你就可以帮助他们更好地管理他们购买的任何资源。</span><span class="sxs-lookup"><span data-stu-id="9373e-191">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="9373e-192">客户可以直接从 [Azure 门户](https://portal.azure.com/)管理 Azure 预订的许多方面。</span><span class="sxs-lookup"><span data-stu-id="9373e-192">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="9373e-193">他们将需要你的帮助来管理他们在 CSP 订阅中购买的 Azure 保留部分的其他方面。</span><span class="sxs-lookup"><span data-stu-id="9373e-193">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="9373e-194">帮助客户更详细地了解如何管理 Azure 预订的这些方面：</span><span class="sxs-lookup"><span data-stu-id="9373e-194">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="9373e-195">价格客户将支付 Azure 预订费用</span><span class="sxs-lookup"><span data-stu-id="9373e-195">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="9373e-196">客户如何优化 Azure 预订的使用</span><span class="sxs-lookup"><span data-stu-id="9373e-196">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="9373e-197">当客户购买具有共享作用域的预留时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="9373e-197">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="9373e-198">如果客户想要更改、取消和续订预订，或更改其作用域，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="9373e-198">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="9373e-199">**价格客户将为其预留付费。**</span><span class="sxs-lookup"><span data-stu-id="9373e-199">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="9373e-200">你的客户将根据你先前为 CSP 合作伙伴计费帐户购买的订阅购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="9373e-200">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="9373e-201">客户根据此订阅购买的任何 Azure 预订的价格也由您设置。</span><span class="sxs-lookup"><span data-stu-id="9373e-201">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="9373e-202">此价格可能与客户在 Azure 门户中看到的 Web 直接价格不同。</span><span class="sxs-lookup"><span data-stu-id="9373e-202">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="9373e-203">**客户如何优化预订的使用。**</span><span class="sxs-lookup"><span data-stu-id="9373e-203">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="9373e-204">一些客户可以从了解有关如何优化预订使用情况的详细信息，或者如何在购买过程中分配预订的初始范围。</span><span class="sxs-lookup"><span data-stu-id="9373e-204">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="9373e-205">有关详细信息，请客户阅读 [Azure 资源的管理预订](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。</span><span class="sxs-lookup"><span data-stu-id="9373e-205">For more information, ask customers to read [Manage reservations for Azure resources](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="9373e-206">**当客户购买具有共享作用域的预订时，会发生什么情况？**</span><span class="sxs-lookup"><span data-stu-id="9373e-206">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="9373e-207">当客户基于之前的 CSP 订阅购买保留并为该预订分配共享范围时，CSP 提供的任何折扣将应用于 CSP 合作伙伴为该客户购买的所有订阅的匹配使用情况。</span><span class="sxs-lookup"><span data-stu-id="9373e-207">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="9373e-208">**如果客户想要交换、取消或续订已进行的购买，或更改保留的初始范围，应执行哪些操作？**</span><span class="sxs-lookup"><span data-stu-id="9373e-208">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="9373e-209">客户需要咨询合作伙伴来帮助他们更改保留的初始范围。</span><span class="sxs-lookup"><span data-stu-id="9373e-209">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="9373e-210">他们还需要合作伙伴的帮助来交换、取消或续订预订。</span><span class="sxs-lookup"><span data-stu-id="9373e-210">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="9373e-211">它们不能根据为 CSP 合作伙伴购买的订阅，使用预订来执行这些任务。</span><span class="sxs-lookup"><span data-stu-id="9373e-211">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9373e-212">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9373e-212">Next steps</span></span>

- [<span data-ttu-id="9373e-213">代表你的客户购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="9373e-213">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="9373e-214">合作伙伴中心-销售 Microsoft 预订</span><span class="sxs-lookup"><span data-stu-id="9373e-214">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="9373e-215">代表客户管理 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="9373e-215">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)