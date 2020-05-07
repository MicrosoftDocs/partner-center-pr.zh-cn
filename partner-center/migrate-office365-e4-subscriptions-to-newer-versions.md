---
title: 将 Office 365 E4 订阅迁移到较新的 Office 365 版本 |合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 企业版 E4 版本自 2017 年 4 月 7 日起已停用。 了解如何将你的客户订阅迁移到较新版本的 Office 365。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 02d383172595e09a4ab0bf9c6db34862fcc17204
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798873"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="4c385-104">将 Office 365 E4 订阅迁移到较新的 Office 365 版本</span><span class="sxs-lookup"><span data-stu-id="4c385-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="4c385-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="4c385-105">**Applies to**</span></span>

-  <span data-ttu-id="4c385-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="4c385-106">Partner Center</span></span>

<span data-ttu-id="4c385-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="4c385-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="4c385-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4c385-108">Global admin</span></span>
-   <span data-ttu-id="4c385-109">用户管理员</span><span class="sxs-lookup"><span data-stu-id="4c385-109">User admin</span></span>
-   <span data-ttu-id="4c385-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="4c385-110">Admin agent</span></span>
-   <span data-ttu-id="4c385-111">销售代理</span><span class="sxs-lookup"><span data-stu-id="4c385-111">Sales agent</span></span>

<span data-ttu-id="4c385-112">Office 365 企业版 E4 计划已停用，停用的生效日期为 2017 年 4 月 7 日。</span><span class="sxs-lookup"><span data-stu-id="4c385-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="4c385-113">在此日期之后，你将无法再购买新的 Office 365 E4 订阅，现有的 E4 订阅在到期后将不会自动续订。</span><span class="sxs-lookup"><span data-stu-id="4c385-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="4c385-114">当 E4 订阅结束时，它们将会被取消。</span><span class="sxs-lookup"><span data-stu-id="4c385-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="4c385-115">为了确保客户服务连续性，你应该将 E4 订阅快过期的客户过渡到下列支持的 SKU 选项。</span><span class="sxs-lookup"><span data-stu-id="4c385-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="4c385-116">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="4c385-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="4c385-117">Office 365 企业版 E4 商业版和政府版 Sku 均已停用。</span><span class="sxs-lookup"><span data-stu-id="4c385-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="4c385-118">在订阅的详细信息页面上，E4 订阅状态已从“[日期] 自动续订”更改为“[日期] 过期”。</span><span class="sxs-lookup"><span data-stu-id="4c385-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="4c385-119">如果你使用 API（CREST 或合作伙伴中心），则可以通过评估订阅的结束日期以及“自动更新 = False”属性来发现快到期的订阅。</span><span class="sxs-lookup"><span data-stu-id="4c385-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="4c385-120">2017 年 4 月 7 日，E4 订阅将设置为“自动更新 = False”。</span><span class="sxs-lookup"><span data-stu-id="4c385-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="4c385-121">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="4c385-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="4c385-122">Office 365 企业版 E4 版本替换计划</span><span class="sxs-lookup"><span data-stu-id="4c385-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="4c385-123">你可以选择保持与 E4 相同的功能，或者让你的客户利用 Office 365 和 Skype for Business Online 中的较新特性和功能。</span><span class="sxs-lookup"><span data-stu-id="4c385-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="4c385-124">定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。</span><span class="sxs-lookup"><span data-stu-id="4c385-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="4c385-125">可以分别在 Office 365 企业版 E3 或 Office 365 企业版 E5 的以下选项中替换 Secure Product Enterprise E3 或 Secure Productive Enterprise E5。</span><span class="sxs-lookup"><span data-stu-id="4c385-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="4c385-126">选项 1：Office 365 企业版 E5</span><span class="sxs-lookup"><span data-stu-id="4c385-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="4c385-127">选项 2：Office 365 企业版 E3 + Skype for Business 云 PBX</span><span class="sxs-lookup"><span data-stu-id="4c385-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="4c385-128">选项 3：Office 365 企业版 E3 + Skype for Business Plus CAL（价格和功能与 E4 相同）</span><span class="sxs-lookup"><span data-stu-id="4c385-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="4c385-129">选项 4：Office 365 企业版 E3</span><span class="sxs-lookup"><span data-stu-id="4c385-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="4c385-130">Feature</span><span class="sxs-lookup"><span data-stu-id="4c385-130">Feature</span></span> | <span data-ttu-id="4c385-131">选项 1</span><span class="sxs-lookup"><span data-stu-id="4c385-131">Option 1</span></span> | <span data-ttu-id="4c385-132">方法 2</span><span class="sxs-lookup"><span data-stu-id="4c385-132">Option 2</span></span> | <span data-ttu-id="4c385-133">选项 3</span><span class="sxs-lookup"><span data-stu-id="4c385-133">Option 3</span></span> | <span data-ttu-id="4c385-134">选项 4</span><span class="sxs-lookup"><span data-stu-id="4c385-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="4c385-135">获取 Office 365 企业版 E4 中包含的所有功能？</span><span class="sxs-lookup"><span data-stu-id="4c385-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="4c385-136">是</span><span class="sxs-lookup"><span data-stu-id="4c385-136">Yes</span></span> | <span data-ttu-id="4c385-137">是</span><span class="sxs-lookup"><span data-stu-id="4c385-137">Yes</span></span> | <span data-ttu-id="4c385-138">是</span><span class="sxs-lookup"><span data-stu-id="4c385-138">Yes</span></span> | <span data-ttu-id="4c385-139">否</span><span class="sxs-lookup"><span data-stu-id="4c385-139">No</span></span> |
| <span data-ttu-id="4c385-140">在 Office 365 中管理电话号码？</span><span class="sxs-lookup"><span data-stu-id="4c385-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="4c385-141">是</span><span class="sxs-lookup"><span data-stu-id="4c385-141">Yes</span></span> | <span data-ttu-id="4c385-142">是</span><span class="sxs-lookup"><span data-stu-id="4c385-142">Yes</span></span> | <span data-ttu-id="4c385-143">否</span><span class="sxs-lookup"><span data-stu-id="4c385-143">No</span></span> | <span data-ttu-id="4c385-144">否</span><span class="sxs-lookup"><span data-stu-id="4c385-144">No</span></span> |
| <span data-ttu-id="4c385-145">在本地和 Office 365（混合部署）中管理电话号码？</span><span class="sxs-lookup"><span data-stu-id="4c385-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="4c385-146">是</span><span class="sxs-lookup"><span data-stu-id="4c385-146">Yes</span></span> | <span data-ttu-id="4c385-147">是</span><span class="sxs-lookup"><span data-stu-id="4c385-147">Yes</span></span> | <span data-ttu-id="4c385-148">否</span><span class="sxs-lookup"><span data-stu-id="4c385-148">No</span></span> | <span data-ttu-id="4c385-149">否</span><span class="sxs-lookup"><span data-stu-id="4c385-149">No</span></span> |
| <span data-ttu-id="4c385-150">选项用于添加 PSTN 语音通话套餐？</span><span class="sxs-lookup"><span data-stu-id="4c385-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="4c385-151">是</span><span class="sxs-lookup"><span data-stu-id="4c385-151">Yes</span></span> | <span data-ttu-id="4c385-152">是</span><span class="sxs-lookup"><span data-stu-id="4c385-152">Yes</span></span> | <span data-ttu-id="4c385-153">否</span><span class="sxs-lookup"><span data-stu-id="4c385-153">No</span></span> | <span data-ttu-id="4c385-154">否</span><span class="sxs-lookup"><span data-stu-id="4c385-154">No</span></span> |
| <span data-ttu-id="4c385-155">PSTN 会议？</span><span class="sxs-lookup"><span data-stu-id="4c385-155">PSTN Conferencing?</span></span> | <span data-ttu-id="4c385-156">是</span><span class="sxs-lookup"><span data-stu-id="4c385-156">Yes</span></span> | <span data-ttu-id="4c385-157">否</span><span class="sxs-lookup"><span data-stu-id="4c385-157">No</span></span> | <span data-ttu-id="4c385-158">否</span><span class="sxs-lookup"><span data-stu-id="4c385-158">No</span></span> | <span data-ttu-id="4c385-159">否</span><span class="sxs-lookup"><span data-stu-id="4c385-159">No</span></span> |
| <span data-ttu-id="4c385-160">用于协作、分析和保证安全的高级工具？</span><span class="sxs-lookup"><span data-stu-id="4c385-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="4c385-161">是</span><span class="sxs-lookup"><span data-stu-id="4c385-161">Yes</span></span> | <span data-ttu-id="4c385-162">否</span><span class="sxs-lookup"><span data-stu-id="4c385-162">No</span></span> | <span data-ttu-id="4c385-163">否</span><span class="sxs-lookup"><span data-stu-id="4c385-163">No</span></span> | <span data-ttu-id="4c385-164">否</span><span class="sxs-lookup"><span data-stu-id="4c385-164">No</span></span> |
| <span data-ttu-id="4c385-165">交互式报告、仪表板和数据可视化？</span><span class="sxs-lookup"><span data-stu-id="4c385-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="4c385-166">是</span><span class="sxs-lookup"><span data-stu-id="4c385-166">Yes</span></span> | <span data-ttu-id="4c385-167">否</span><span class="sxs-lookup"><span data-stu-id="4c385-167">No</span></span> | <span data-ttu-id="4c385-168">否</span><span class="sxs-lookup"><span data-stu-id="4c385-168">No</span></span> | <span data-ttu-id="4c385-169">否</span><span class="sxs-lookup"><span data-stu-id="4c385-169">No</span></span> | 
| <span data-ttu-id="4c385-170">更好地控制数据安全性并符合内置的隐私、透明度和改进型用户控件的要求？</span><span class="sxs-lookup"><span data-stu-id="4c385-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="4c385-171">是</span><span class="sxs-lookup"><span data-stu-id="4c385-171">Yes</span></span> | <span data-ttu-id="4c385-172">否</span><span class="sxs-lookup"><span data-stu-id="4c385-172">No</span></span> | <span data-ttu-id="4c385-173">否</span><span class="sxs-lookup"><span data-stu-id="4c385-173">No</span></span> | <span data-ttu-id="4c385-174">否</span><span class="sxs-lookup"><span data-stu-id="4c385-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="4c385-175">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="4c385-175">Transition customers to new product plans</span></span>

<span data-ttu-id="4c385-176">Microsoft 不断向我们的合作伙伴提供新产品和服务。</span><span class="sxs-lookup"><span data-stu-id="4c385-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="4c385-177">在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。</span><span class="sxs-lookup"><span data-stu-id="4c385-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="4c385-178">将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="4c385-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="4c385-179">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="4c385-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="4c385-180">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="4c385-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="4c385-181">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="4c385-181">Cancel the old subscription</span></span>

<span data-ttu-id="4c385-182">按照以下步骤将客户的 Office 365 企业版 E4 订阅迁移到上表中的其中一个选项。</span><span class="sxs-lookup"><span data-stu-id="4c385-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="4c385-183">步骤 1 - 购买新订阅</span><span class="sxs-lookup"><span data-stu-id="4c385-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="4c385-184">从 "**合作伙伴中心**" 菜单中，选择 "**客户**"，选择要移动的客户，然后选择 "**添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="4c385-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="4c385-185">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="4c385-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="4c385-186">你的客户现在应具有新订阅和新订阅，旧的 Office 365 企业版 E4 订阅和新的 "目标" 订阅，例如，选项 1-Office 365 企业版 E5。</span><span class="sxs-lookup"><span data-stu-id="4c385-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="4c385-187">第 2 步 - 重新分配客户的用户许可证</span><span class="sxs-lookup"><span data-stu-id="4c385-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="4c385-188">从 "**合作伙伴中心**" 菜单中，选择 "**客户**"，选择你想要移动的客户，然后选择 "**用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="4c385-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="4c385-189">此时将打开客户的 "用户和许可证" 页。</span><span class="sxs-lookup"><span data-stu-id="4c385-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="4c385-190">若要重新分配用户许可证，请选择要重新分配的用户，然后选择 "**管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="4c385-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="4c385-191">在**管理许可证**页面上，清除 **Office 365 企业版 E4** 许可证复选框，然后选择客户要迁移到的订阅的新服务计划。</span><span class="sxs-lookup"><span data-stu-id="4c385-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="4c385-192">选择“提交”。 </span><span class="sxs-lookup"><span data-stu-id="4c385-192">Select **Submit**.</span></span> <span data-ttu-id="4c385-193">确认页面列出了新的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="4c385-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="4c385-194">对其他任何需要重新分配许可证的客户用户继续执行相同的步骤。</span><span class="sxs-lookup"><span data-stu-id="4c385-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="4c385-195">在将用户许可证移动至新服务后，可安全取消最高“客户”级别的已停用订阅。</span><span class="sxs-lookup"><span data-stu-id="4c385-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="4c385-196">步骤 3 - 取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="4c385-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="4c385-197">从 "**合作伙伴中心**" 菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="4c385-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4c385-198">选择你想要移动的客户，并选择你想要取消的订阅。</span><span class="sxs-lookup"><span data-stu-id="4c385-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="4c385-199">在 "订阅详细信息" 页中，将订阅状态设置为 "已**挂起**"。</span><span class="sxs-lookup"><span data-stu-id="4c385-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="4c385-200">选择“提交”。 </span><span class="sxs-lookup"><span data-stu-id="4c385-200">Select **Submit**.</span></span>

<span data-ttu-id="4c385-201">旧订阅已暂停，新订阅将激活。</span><span class="sxs-lookup"><span data-stu-id="4c385-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="4c385-202">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="4c385-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="4c385-203">不会向客户收取旧订阅的任何额外成本。</span><span class="sxs-lookup"><span data-stu-id="4c385-203">The customer incurs no additional costs for the old subscription.</span></span>



 



