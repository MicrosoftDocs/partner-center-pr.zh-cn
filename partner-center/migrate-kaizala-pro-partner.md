---
title: 将 Kaizala Pro 订阅迁移到 Microsoft 365
description: 了解如何将 Kaizala Pro 订阅迁移到 Microsoft 365 或 Office 365 版本。 阅读本文，了解有关如何转换客户的详细信息。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172398"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="72c9d-104">将 Kaizala Pro 独立订阅迁移到 Microsoft 365 或 Office 365 版本</span><span class="sxs-lookup"><span data-stu-id="72c9d-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="72c9d-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="72c9d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="72c9d-106">销售代理</span><span class="sxs-lookup"><span data-stu-id="72c9d-106">Sales agent</span></span>

<span data-ttu-id="72c9d-107">2020年7月1日生效，Microsoft 正在结束 Kaizala Pro 独立服务的销售。</span><span class="sxs-lookup"><span data-stu-id="72c9d-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="72c9d-108">在此日期后，客户将无法再购买新的 Kaizala Pro 订阅，现有的 Kaizala Pro 订阅将不会在过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="72c9d-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="72c9d-109">若要确保客户的连续性，应将 Kaizala Pro 独立订阅过期的客户转换为受支持的 SKU 选项，如下所示。</span><span class="sxs-lookup"><span data-stu-id="72c9d-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="72c9d-110">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="72c9d-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="72c9d-111">如果使用 API ("CREST" 或 "合作伙伴中心") ，则可以通过评估订阅的结束日期以及将 "自动续订" 属性设置为 "false：" 来发现过期订阅 `auto renew = False` 。</span><span class="sxs-lookup"><span data-stu-id="72c9d-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="72c9d-112">E4 订阅将 `auto renew=False` 在2020年7月1日设置为。</span><span class="sxs-lookup"><span data-stu-id="72c9d-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="72c9d-113">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="72c9d-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="72c9d-114">Kaizala Pro 独立更换计划</span><span class="sxs-lookup"><span data-stu-id="72c9d-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="72c9d-115">使用新计划，你的客户可以在 Microsoft 365 中利用新的特性和功能。</span><span class="sxs-lookup"><span data-stu-id="72c9d-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="72c9d-116">定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。</span><span class="sxs-lookup"><span data-stu-id="72c9d-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="72c9d-117">[**适用于企业的 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)，包括：</span><span class="sxs-lookup"><span data-stu-id="72c9d-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="72c9d-118">Microsoft 365 商业基本版</span><span class="sxs-lookup"><span data-stu-id="72c9d-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="72c9d-119">Microsoft 365 商业标准版</span><span class="sxs-lookup"><span data-stu-id="72c9d-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="72c9d-120">Microsoft 365 商业高级版</span><span class="sxs-lookup"><span data-stu-id="72c9d-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="72c9d-121">[**Microsoft 365 前端**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)，包括：</span><span class="sxs-lookup"><span data-stu-id="72c9d-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="72c9d-122">Microsoft 365 F3（以前为 Microsoft 365 F1）和 Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="72c9d-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="72c9d-123">[**适用于企业的 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)，包括：</span><span class="sxs-lookup"><span data-stu-id="72c9d-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="72c9d-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="72c9d-124">Office 365 E1</span></span>
   - <span data-ttu-id="72c9d-125">Microsoft 365 E3 和 Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="72c9d-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="72c9d-126">Microsoft 365 E5 和 Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="72c9d-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="72c9d-127">[**Microsoft 365 教育**](https://www.microsoft.com/education/buy-license/microsoft365)，包括：</span><span class="sxs-lookup"><span data-stu-id="72c9d-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="72c9d-128">Microsoft 365 A1 和 Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="72c9d-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="72c9d-129">Microsoft 365 A3 和 Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="72c9d-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="72c9d-130">Microsoft 365 A5 和 Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="72c9d-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="72c9d-131">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="72c9d-131">Transition customers to new product plans</span></span>

<span data-ttu-id="72c9d-132">Microsoft 不断向我们的合作伙伴提供新产品和服务。</span><span class="sxs-lookup"><span data-stu-id="72c9d-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="72c9d-133">在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。</span><span class="sxs-lookup"><span data-stu-id="72c9d-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="72c9d-134">将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="72c9d-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="72c9d-135">A.</span><span class="sxs-lookup"><span data-stu-id="72c9d-135">A.</span></span> <span data-ttu-id="72c9d-136">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="72c9d-136">Purchase the new subscription</span></span>

<span data-ttu-id="72c9d-137">B.</span><span class="sxs-lookup"><span data-stu-id="72c9d-137">B.</span></span> <span data-ttu-id="72c9d-138">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="72c9d-138">Reassign current user licenses</span></span>

<span data-ttu-id="72c9d-139">C.</span><span class="sxs-lookup"><span data-stu-id="72c9d-139">C.</span></span> <span data-ttu-id="72c9d-140">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="72c9d-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="72c9d-141">将你的客户迁移至新计划</span><span class="sxs-lookup"><span data-stu-id="72c9d-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="72c9d-142">A.</span><span class="sxs-lookup"><span data-stu-id="72c9d-142">A.</span></span> <span data-ttu-id="72c9d-143">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="72c9d-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="72c9d-144">若要购买新的订阅，请从 " **合作伙伴中心** " 菜单中选择 " **客户**"，选择要移动的客户，然后选择 " **添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="72c9d-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="72c9d-145">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。</span><span class="sxs-lookup"><span data-stu-id="72c9d-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="72c9d-146">你的客户现在应具有新订阅和新订阅，旧的 Kaizala Pro 独立订阅和新的 "目标" 订阅，例如，选项 1-Office 365 企业版 F1。</span><span class="sxs-lookup"><span data-stu-id="72c9d-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="72c9d-147">B.</span><span class="sxs-lookup"><span data-stu-id="72c9d-147">B.</span></span> <span data-ttu-id="72c9d-148">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="72c9d-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="72c9d-149">若要重新分配客户的用户许可证，请在 " **合作伙伴中心** " 菜单中选择 " **客户**"，选择要移动的客户，然后选择 " **用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="72c9d-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="72c9d-150">此时将打开客户的 "用户和许可证" 页。</span><span class="sxs-lookup"><span data-stu-id="72c9d-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="72c9d-151">若要重新分配用户许可证，请选择要重新分配的用户，然后选择 " **管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="72c9d-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="72c9d-152">在 " **管理许可证** " 页上，清除 "Kaizala Pro 独立许可" 复选框，并为客户要移到的订阅选择新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="72c9d-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="72c9d-153">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="72c9d-153">Select **Submit**.</span></span> <span data-ttu-id="72c9d-154">确认页面列出了新的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="72c9d-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="72c9d-155">继续对需要许可证分配的其他用户执行相同过程。</span><span class="sxs-lookup"><span data-stu-id="72c9d-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="72c9d-156">C.</span><span class="sxs-lookup"><span data-stu-id="72c9d-156">C.</span></span> <span data-ttu-id="72c9d-157">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="72c9d-157">Cancel old subscription</span></span>

<span data-ttu-id="72c9d-158">在将用户许可证移动至新服务后，可安全取消该客户级别的已停用订阅。</span><span class="sxs-lookup"><span data-stu-id="72c9d-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="72c9d-159">从 " **合作伙伴中心** " 菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="72c9d-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="72c9d-160">选择要取消其订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="72c9d-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="72c9d-161">在订阅详细信息页面中，将订阅设置为 **已暂停**。</span><span class="sxs-lookup"><span data-stu-id="72c9d-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="72c9d-162">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="72c9d-162">Select **Submit**.</span></span>

<span data-ttu-id="72c9d-163">旧订阅已暂停，新订阅将激活。</span><span class="sxs-lookup"><span data-stu-id="72c9d-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="72c9d-164">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="72c9d-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="72c9d-165">不会向客户收取旧订阅的任何额外成本。</span><span class="sxs-lookup"><span data-stu-id="72c9d-165">The customer incurs no additional costs for the old subscription.</span></span>
