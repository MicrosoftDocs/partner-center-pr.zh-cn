---
title: 让客户在 CSP 中购买自己的服务
description: 了解 CSP 计划合作伙伴如何让客户购买自己的服务（例如 Azure 预留）来购买在 合作伙伴中心。
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150754"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="29ff0-103">授予客户合作伙伴中心购买自己的产品或服务的权限</span><span class="sxs-lookup"><span data-stu-id="29ff0-103">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="29ff0-104">**适当的角色**：管理员代理|销售代理</span><span class="sxs-lookup"><span data-stu-id="29ff0-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="29ff0-105">本文介绍云解决方案提供商云解决方案提供商 (合作伙伴) 如何授予客户购买自己的一些服务或资源的权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-105">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="29ff0-106">CSP 计划的合作伙伴通常使用 合作伙伴中心及其商业市场为客户购买解决方案和服务。</span><span class="sxs-lookup"><span data-stu-id="29ff0-106">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="29ff0-107">然后，合作伙伴允许某些客户直接从客户Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="29ff0-107">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="29ff0-108">下面是一个示例。</span><span class="sxs-lookup"><span data-stu-id="29ff0-108">Here's an example.</span></span> <span data-ttu-id="29ff0-109">假设你为 合作伙伴中心 中的客户购买 Azure 计划合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="29ff0-109">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="29ff0-110">然后，你决定代表客户将其他资源或服务添加到该订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-110">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="29ff0-111">在这种情况下，可以将 Azure 预留添加到客户的订阅 (例如，将虚拟机预留实例添加到) 。</span><span class="sxs-lookup"><span data-stu-id="29ff0-111">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="29ff0-112">然后，可以允许客户在门户中进一步预配 Azure 预留Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="29ff0-112">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="29ff0-113">现在，使用 **"客户权限** "功能，可以为客户提供更多 Azure 资源的自助服务选项。</span><span class="sxs-lookup"><span data-stu-id="29ff0-113">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="29ff0-114">通过为客户启用权限，可以让客户购买自己的资源，例如 (购买自己的 Azure 预留) 。</span><span class="sxs-lookup"><span data-stu-id="29ff0-114">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="29ff0-115">客户权限概述合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="29ff0-115">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="29ff0-116">使用" **客户帐户** "页可以启用 (或关闭) 权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-116">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="29ff0-117">目前，此功能支持：</span><span class="sxs-lookup"><span data-stu-id="29ff0-117">Currently, this feature supports:</span></span>

- <span data-ttu-id="29ff0-118">**Azure 预留：** 启用此权限后，客户可以购买自己为特定 Azure 订阅购买的 Azure 预留。</span><span class="sxs-lookup"><span data-stu-id="29ff0-118">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="29ff0-119">在启用客户权限之前，请注意以下要点：</span><span class="sxs-lookup"><span data-stu-id="29ff0-119">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="29ff0-120">默认情况下，客户权限在 (中) 自动合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="29ff0-120">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="29ff0-121">你必须在合作伙伴中心为你分配 "管理员代理" 角色，然后才能打开 (或关闭客户的) 权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-121">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="29ff0-122">分配有 "销售代理" 或 "技术支持" 代理角色的合作伙伴具有只读访问权限，并且不能打开或关闭客户权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-122">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="29ff0-123">您可以打开 (为您选择的任何客户启用) 权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-123">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="29ff0-124">你可以使用合作伙伴中心仪表板或 [合作伙伴中心 api](/partner-center/develop/manage-customers)打开 (或关闭) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-124">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="29ff0-125">开启 (为特定客户启用) 权限后，你将负责为该客户所进行的任何后续购买付费。</span><span class="sxs-lookup"><span data-stu-id="29ff0-125">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="29ff0-126">如果客户想要交换、取消或续订已 (的购买，或者他们想要更改预订) 的初始范围，他们将不能这样做。</span><span class="sxs-lookup"><span data-stu-id="29ff0-126">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="29ff0-127">他们需要询问你，作为合作伙伴，帮助他们交换、取消和续订购买，或在以后对预订范围做出更改。</span><span class="sxs-lookup"><span data-stu-id="29ff0-127">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="29ff0-128">为特定客户启用权限后，你将 **不** 会收到客户对你的任何以后购买的通知。</span><span class="sxs-lookup"><span data-stu-id="29ff0-128">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="29ff0-129">以后购买的客户将显示在合作伙伴中心，以及你所做的任何购买。</span><span class="sxs-lookup"><span data-stu-id="29ff0-129">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="29ff0-130">您可以在客户的 **订单历史记录** 页、其 **预订** 页或 [**活动日志**](activity-logs.md)中找到这些购买内容。</span><span class="sxs-lookup"><span data-stu-id="29ff0-130">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="29ff0-131">有关客户将支付的价格以及如何帮助客户管理其购买的信息，请参阅 [帮助客户管理他们购买的预订](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-131">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="29ff0-132">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="29ff0-132">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="29ff0-133">Azure 预订是以折扣价购买 Azure 服务的一种绝佳方式。</span><span class="sxs-lookup"><span data-stu-id="29ff0-133">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="29ff0-134">若要详细了解 Azure 保留项的优点，请参阅 [什么是 Azure 保留？](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="29ff0-134">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="29ff0-135">现在，你可以选择代表你的客户购买 Azure 预订，因为你可能已经做了。</span><span class="sxs-lookup"><span data-stu-id="29ff0-135">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="29ff0-136">或者，你可以授予客户购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-136">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="29ff0-137">向客户授予购买自己的 Azure 预订的权限后，可帮助他们管理他们购买的任何预订。</span><span class="sxs-lookup"><span data-stu-id="29ff0-137">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="29ff0-138">有关详细信息，请参阅帮助 [客户管理他们购买的预留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-138">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="29ff0-139">使客户能够购买自己的 Azure 预留</span><span class="sxs-lookup"><span data-stu-id="29ff0-139">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="29ff0-140">验证客户是否拥有你代表他们购买的现有 Azure 计划或 Azure 全局订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-140">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="29ff0-141">验证是否为客户分配了 **此订阅的** "所有者"角色。</span><span class="sxs-lookup"><span data-stu-id="29ff0-141">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="29ff0-142">启用客户权限 (开启此功能 **)** 购买自己的 Azure 预留。</span><span class="sxs-lookup"><span data-stu-id="29ff0-142">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="29ff0-143">每个步骤如下所示。</span><span class="sxs-lookup"><span data-stu-id="29ff0-143">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="29ff0-144">验证客户是否具有现有的 Azure 订阅</span><span class="sxs-lookup"><span data-stu-id="29ff0-144">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="29ff0-145">在授予客户购买自己的 Azure 预留项的权限之前，必须验证客户是否具有现有的 Azure 计划或 Azure 全球订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-145">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="29ff0-146">如果客户在订阅中未显示当前 Azure 合作伙伴中心，则必须在启用其客户权限之前为这些用户购买订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-146">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="29ff0-147">若要了解客户是否已有 Azure 订阅，请登录到 合作伙伴中心 仪表板，然后选择 **"CSP"，** 然后选择"**客户"。**</span><span class="sxs-lookup"><span data-stu-id="29ff0-147">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="29ff0-148">从列表中选择特定客户。</span><span class="sxs-lookup"><span data-stu-id="29ff0-148">Select the specific customer from the list.</span></span> <span data-ttu-id="29ff0-149">然后选择 **"订阅** "，然后查找 Azure 计划或 Azure Global 的任何基于使用情况的订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-149">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="29ff0-150">如果客户没有现有的 Azure 订阅，可以购买其订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-150">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="29ff0-151">请参阅 [购买 Azure 计划](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-151">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="29ff0-152">验证客户在 Azure 中是否分配了正确的角色</span><span class="sxs-lookup"><span data-stu-id="29ff0-152">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="29ff0-153">验证客户是否具有现有的 Azure 订阅后，还需要验证是否为与客户关联的密钥用户分配了该 Azure 订阅的正确所有者角色。 </span><span class="sxs-lookup"><span data-stu-id="29ff0-153">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="29ff0-154">这是基于角色的访问 (RBAC) 客户需要为购买的 Azure 订阅购买 Azure 预留。</span><span class="sxs-lookup"><span data-stu-id="29ff0-154">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="29ff0-155">某些合作伙伴可能已经将"所有者"角色分配给想要主动管理和预配自己的 Azure 资源的客户。</span><span class="sxs-lookup"><span data-stu-id="29ff0-155">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="29ff0-156">如果已 **为客户分配"** 所有者"状态来管理之前为其购买的订阅，可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="29ff0-156">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="29ff0-157">如果尚未为某个客户分配 " **所有者** " 角色，则他们将收到一个错误，Azure 门户阻止他们购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="29ff0-157">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="29ff0-158">若要验证是否已为客户分配 Azure 订阅的 **所有者** 角色，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="29ff0-158">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="29ff0-159">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-159">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="29ff0-160">依次选择 " **CSP**"、" **客户** " 和 "特定客户"。</span><span class="sxs-lookup"><span data-stu-id="29ff0-160">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="29ff0-161">选择该客户的 **订阅** ，并找到特定的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="29ff0-161">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="29ff0-162">选择该客户的订阅旁边的 " **管理** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="29ff0-162">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="29ff0-163">这样做会打开 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-163">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="29ff0-164">若要将 **所有者** 角色分配给特定用户，请按照以下步骤将 [用户分配为管理员](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-164">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="29ff0-165">启用或禁用客户权限以购买自己的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="29ff0-165">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="29ff0-166">验证客户是否有现有的 Azure 订阅，并为用户分配了该订阅的 **所有者** 角色后，便可以打开 (启用) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-166">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="29ff0-167">你还可以使用这些步骤关闭 (禁用) 客户权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-167">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="29ff0-168">你可以使用合作伙伴中心仪表板或 [合作伙伴中心 api](/partner-center/develop/manage-customers)启用或禁用客户权限。</span><span class="sxs-lookup"><span data-stu-id="29ff0-168">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="29ff0-169">若要打开 (或关闭合作伙伴中心) 客户权限：</span><span class="sxs-lookup"><span data-stu-id="29ff0-169">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="29ff0-170">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-170">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="29ff0-171">从左侧导航菜单中，依次选择 " **CSP**"、" **客户**"。</span><span class="sxs-lookup"><span data-stu-id="29ff0-171">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="29ff0-172">此时将显示客户列表。</span><span class="sxs-lookup"><span data-stu-id="29ff0-172">A customer list appears.</span></span>

3. <span data-ttu-id="29ff0-173">选择特定的客户名称。</span><span class="sxs-lookup"><span data-stu-id="29ff0-173">Select a specific customer name.</span></span>

4. <span data-ttu-id="29ff0-174">从 "客户" 菜单中选择 " **帐户** "。</span><span class="sxs-lookup"><span data-stu-id="29ff0-174">Select **Account** from the customer menu.</span></span> <span data-ttu-id="29ff0-175">此时会显示 "客户 **帐户** " 页。</span><span class="sxs-lookup"><span data-stu-id="29ff0-175">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="29ff0-176">查找页面底部的 " **客户权限** " 区域。</span><span class="sxs-lookup"><span data-stu-id="29ff0-176">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="客户权限帐户页。" border="true":::

6. <span data-ttu-id="29ff0-178">在 " **Azure 保留**" 下，找到 " **允许客户购买** " 选项。</span><span class="sxs-lookup"><span data-stu-id="29ff0-178">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="29ff0-179">若要启用客户权限，请将此选项旁的开关移到 " **开** " 位置。</span><span class="sxs-lookup"><span data-stu-id="29ff0-179">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="29ff0-180">若要关闭客户权限，请将开关移到 " **关闭** " 位置。</span><span class="sxs-lookup"><span data-stu-id="29ff0-180">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="29ff0-181">若要了解当你打开客户的权限来购买自己的 Azure 预订时，还会发生什么情况，请参阅 [合作伙伴中心的客户权限概述](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-181">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="29ff0-182">打开 (或关闭) 客户权限时，活动日志会记录每个操作。</span><span class="sxs-lookup"><span data-stu-id="29ff0-182">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="29ff0-183">从 "合作伙伴中心" 仪表板) 顶部选择齿轮图标时， (可以访问此日志。</span><span class="sxs-lookup"><span data-stu-id="29ff0-183">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="29ff0-184">当你打开或关闭客户权限时，该操作将在活动日志中显示为 " **创建客户购买权限** " 或 " **删除客户购买权限** "。</span><span class="sxs-lookup"><span data-stu-id="29ff0-184">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="29ff0-185">帮助客户管理他们购买的预订</span><span class="sxs-lookup"><span data-stu-id="29ff0-185">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="29ff0-186">一旦你向客户提供购买其自己的 Azure 预订的权限，你就可以帮助他们更好地管理他们购买的任何资源。</span><span class="sxs-lookup"><span data-stu-id="29ff0-186">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="29ff0-187">客户可以直接从 [Azure 门户](https://portal.azure.com/)管理 Azure 预订的许多方面。</span><span class="sxs-lookup"><span data-stu-id="29ff0-187">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="29ff0-188">他们将需要你的帮助来管理他们在 CSP 订阅中购买的 Azure 保留部分的其他方面。</span><span class="sxs-lookup"><span data-stu-id="29ff0-188">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="29ff0-189">帮助客户更详细地了解如何管理 Azure 预订的这些方面：</span><span class="sxs-lookup"><span data-stu-id="29ff0-189">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="29ff0-190">价格客户将支付 Azure 预订费用</span><span class="sxs-lookup"><span data-stu-id="29ff0-190">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="29ff0-191">客户如何优化 Azure 预订的使用</span><span class="sxs-lookup"><span data-stu-id="29ff0-191">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="29ff0-192">当客户购买具有共享作用域的预留时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="29ff0-192">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="29ff0-193">如果客户想要更改、取消和续订预订，或更改其作用域，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="29ff0-193">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="29ff0-194">**价格客户将为其预留付费。**</span><span class="sxs-lookup"><span data-stu-id="29ff0-194">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="29ff0-195">你的客户将根据你先前为 CSP 合作伙伴计费帐户购买的订阅购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="29ff0-195">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="29ff0-196">客户根据此订阅购买的任何 Azure 预订的价格也由您设置。</span><span class="sxs-lookup"><span data-stu-id="29ff0-196">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="29ff0-197">此价格可能与客户在 Azure 门户中看到的 Web 直接价格不同。</span><span class="sxs-lookup"><span data-stu-id="29ff0-197">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="29ff0-198">**客户如何优化预订的使用。**</span><span class="sxs-lookup"><span data-stu-id="29ff0-198">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="29ff0-199">一些客户可能会从详细了解如何优化预留的使用或在购买期间分配预留的初始范围中获益。</span><span class="sxs-lookup"><span data-stu-id="29ff0-199">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="29ff0-200">有关详细信息，请让客户阅读 [管理 Azure 资源的预留](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。</span><span class="sxs-lookup"><span data-stu-id="29ff0-200">For more information, ask customers to read [Manage reservations for Azure resources](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="29ff0-201">**客户购买具有共享范围的预留时会发生什么情况？**</span><span class="sxs-lookup"><span data-stu-id="29ff0-201">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="29ff0-202">当客户基于以前的 CSP 订阅购买预留并将共享范围分配给该预留时，CSP 提供的任何折扣将应用于 CSP 合作伙伴为客户购买的所有订阅的匹配使用情况。</span><span class="sxs-lookup"><span data-stu-id="29ff0-202">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="29ff0-203">**如果客户想要交换、取消或续订已购买的购买，或更改预留的初始范围，应该怎么办？**</span><span class="sxs-lookup"><span data-stu-id="29ff0-203">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="29ff0-204">客户需要请求其合作伙伴帮助他们更改预留的初始范围。</span><span class="sxs-lookup"><span data-stu-id="29ff0-204">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="29ff0-205">他们还需要合作伙伴的帮助来交换、取消或续订预留。</span><span class="sxs-lookup"><span data-stu-id="29ff0-205">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="29ff0-206">他们无法根据 CSP 合作伙伴为它们购买的订阅，使用预留自行执行这些任务。</span><span class="sxs-lookup"><span data-stu-id="29ff0-206">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="29ff0-207">后续步骤</span><span class="sxs-lookup"><span data-stu-id="29ff0-207">Next steps</span></span>

- [<span data-ttu-id="29ff0-208">代表客户购买 Azure 预留</span><span class="sxs-lookup"><span data-stu-id="29ff0-208">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="29ff0-209">合作伙伴中心 - 销售 Microsoft 预留</span><span class="sxs-lookup"><span data-stu-id="29ff0-209">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="29ff0-210">代表客户管理 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="29ff0-210">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)