---
title: 将 Office 365 E4 订阅迁移到较新的 Office 365 版本 |合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
description: Microsoft Office 365 企业版 E4 版本自 2017 年 4 月 7 日起已停用。 了解如何将你的客户订阅迁移到较新版本的 Office 365。
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 1dc3957d6abe4069f3868d49e92a458d20e7fbec
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796100"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="4a31f-104">将 Office 365 E4 订阅迁移到较新的 Office 365 版本</span><span class="sxs-lookup"><span data-stu-id="4a31f-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

**<span data-ttu-id="4a31f-105">适用于</span><span class="sxs-lookup"><span data-stu-id="4a31f-105">Applies to</span></span>**

-  <span data-ttu-id="4a31f-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="4a31f-106">Partner Center</span></span>

<span data-ttu-id="4a31f-107">Office 365 企业版 E4 计划已停用，停用的生效日期为 2017 年 4 月 7 日。</span><span class="sxs-lookup"><span data-stu-id="4a31f-107">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="4a31f-108">在此日期之后，你将无法再购买新的 Office 365 E4 订阅，现有的 E4 订阅在到期后将不会自动续订。</span><span class="sxs-lookup"><span data-stu-id="4a31f-108">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="4a31f-109">当 E4 订阅结束时，它们将会被取消。</span><span class="sxs-lookup"><span data-stu-id="4a31f-109">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="4a31f-110">为了确保客户服务连续性，你应该将 E4 订阅快过期的客户过渡到下列支持的 SKU 选项。</span><span class="sxs-lookup"><span data-stu-id="4a31f-110">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="4a31f-111">建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。</span><span class="sxs-lookup"><span data-stu-id="4a31f-111">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="4a31f-112">Office 365 企业版 E4 商业和政府 Sku 均已停用。</span><span class="sxs-lookup"><span data-stu-id="4a31f-112">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="4a31f-113">在订阅的详细信息页面上，E4 订阅状态已从“[日期] 自动续订”更改为“[日期] 过期”。</span><span class="sxs-lookup"><span data-stu-id="4a31f-113">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="4a31f-114">如果你使用 API（CREST 或合作伙伴中心），则可以通过评估订阅的结束日期以及“自动更新 = False”属性来发现快到期的订阅。</span><span class="sxs-lookup"><span data-stu-id="4a31f-114">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="4a31f-115">2017 年 4 月 7 日，E4 订阅将设置为“自动更新 = False”。</span><span class="sxs-lookup"><span data-stu-id="4a31f-115">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="4a31f-116">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="4a31f-116">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="4a31f-117">Office 365 企业版 E4 版本替换计划</span><span class="sxs-lookup"><span data-stu-id="4a31f-117">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="4a31f-118">你可以选择保持与 E4 相同的功能，或者让你的客户利用 Office 365 和 Skype for Business Online 中的较新特性和功能。</span><span class="sxs-lookup"><span data-stu-id="4a31f-118">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="4a31f-119">定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。</span><span class="sxs-lookup"><span data-stu-id="4a31f-119">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="4a31f-120">可以分别在 Office 365 企业版 E3 或 Office 365 企业版 E5 的以下选项中替换 Secure Product Enterprise E3 或 Secure Productive Enterprise E5。</span><span class="sxs-lookup"><span data-stu-id="4a31f-120">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="4a31f-121">选项 1：Office 365 企业版 E5</span><span class="sxs-lookup"><span data-stu-id="4a31f-121">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="4a31f-122">选项 2：Office 365 企业版 E3 + Skype for Business 云 PBX</span><span class="sxs-lookup"><span data-stu-id="4a31f-122">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="4a31f-123">选项 3：Office 365 企业版 E3 + Skype for Business Plus CAL（价格和功能与 E4 相同）</span><span class="sxs-lookup"><span data-stu-id="4a31f-123">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="4a31f-124">选项 4：Office 365 企业版 E3</span><span class="sxs-lookup"><span data-stu-id="4a31f-124">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="4a31f-125">功能</span><span class="sxs-lookup"><span data-stu-id="4a31f-125">Feature</span></span> | <span data-ttu-id="4a31f-126">选项 1</span><span class="sxs-lookup"><span data-stu-id="4a31f-126">Option 1</span></span> | <span data-ttu-id="4a31f-127">选项 2</span><span class="sxs-lookup"><span data-stu-id="4a31f-127">Option 2</span></span> | <span data-ttu-id="4a31f-128">选项 3</span><span class="sxs-lookup"><span data-stu-id="4a31f-128">Option 3</span></span> | <span data-ttu-id="4a31f-129">选项 4</span><span class="sxs-lookup"><span data-stu-id="4a31f-129">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="4a31f-130">获取 Office 365 企业版 E4 中包含的所有功能？</span><span class="sxs-lookup"><span data-stu-id="4a31f-130">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="4a31f-131">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-131">Yes</span></span> | <span data-ttu-id="4a31f-132">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-132">Yes</span></span> | <span data-ttu-id="4a31f-133">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-133">Yes</span></span> | <span data-ttu-id="4a31f-134">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-134">No</span></span> |
| <span data-ttu-id="4a31f-135">在 Office 365 中管理电话号码？</span><span class="sxs-lookup"><span data-stu-id="4a31f-135">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="4a31f-136">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-136">Yes</span></span> | <span data-ttu-id="4a31f-137">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-137">Yes</span></span> | <span data-ttu-id="4a31f-138">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-138">No</span></span> | <span data-ttu-id="4a31f-139">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-139">No</span></span> |
| <span data-ttu-id="4a31f-140">在本地和 Office 365（混合部署）中管理电话号码？</span><span class="sxs-lookup"><span data-stu-id="4a31f-140">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="4a31f-141">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-141">Yes</span></span> | <span data-ttu-id="4a31f-142">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-142">Yes</span></span> | <span data-ttu-id="4a31f-143">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-143">No</span></span> | <span data-ttu-id="4a31f-144">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-144">No</span></span> |
| <span data-ttu-id="4a31f-145">选项用于添加 PSTN 语音通话套餐？</span><span class="sxs-lookup"><span data-stu-id="4a31f-145">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="4a31f-146">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-146">Yes</span></span> | <span data-ttu-id="4a31f-147">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-147">Yes</span></span> | <span data-ttu-id="4a31f-148">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-148">No</span></span> | <span data-ttu-id="4a31f-149">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-149">No</span></span> |
| <span data-ttu-id="4a31f-150">PSTN 会议？</span><span class="sxs-lookup"><span data-stu-id="4a31f-150">PSTN Conferencing?</span></span> | <span data-ttu-id="4a31f-151">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-151">Yes</span></span> | <span data-ttu-id="4a31f-152">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-152">No</span></span> | <span data-ttu-id="4a31f-153">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-153">No</span></span> | <span data-ttu-id="4a31f-154">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-154">No</span></span> |
| <span data-ttu-id="4a31f-155">用于协作、分析和保证安全的高级工具？</span><span class="sxs-lookup"><span data-stu-id="4a31f-155">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="4a31f-156">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-156">Yes</span></span> | <span data-ttu-id="4a31f-157">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-157">No</span></span> | <span data-ttu-id="4a31f-158">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-158">No</span></span> | <span data-ttu-id="4a31f-159">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-159">No</span></span> |
| <span data-ttu-id="4a31f-160">交互式报告、仪表板和数据可视化？</span><span class="sxs-lookup"><span data-stu-id="4a31f-160">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="4a31f-161">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-161">Yes</span></span> | <span data-ttu-id="4a31f-162">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-162">No</span></span> | <span data-ttu-id="4a31f-163">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-163">No</span></span> | <span data-ttu-id="4a31f-164">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-164">No</span></span> | 
| <span data-ttu-id="4a31f-165">更好地控制数据安全性并符合内置的隐私、透明度和改进型用户控件的要求？</span><span class="sxs-lookup"><span data-stu-id="4a31f-165">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="4a31f-166">是</span><span class="sxs-lookup"><span data-stu-id="4a31f-166">Yes</span></span> | <span data-ttu-id="4a31f-167">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-167">No</span></span> | <span data-ttu-id="4a31f-168">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-168">No</span></span> | <span data-ttu-id="4a31f-169">否</span><span class="sxs-lookup"><span data-stu-id="4a31f-169">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="4a31f-170">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="4a31f-170">Transition customers to new product plans</span></span>

<span data-ttu-id="4a31f-171">Microsoft 不断向我们的合作伙伴提供新产品和服务。</span><span class="sxs-lookup"><span data-stu-id="4a31f-171">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="4a31f-172">在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。</span><span class="sxs-lookup"><span data-stu-id="4a31f-172">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="4a31f-173">将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="4a31f-173">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="4a31f-174">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="4a31f-174">Purchase the new subscription</span></span>
-   <span data-ttu-id="4a31f-175">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="4a31f-175">Reassign current user licenses</span></span>
-   <span data-ttu-id="4a31f-176">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="4a31f-176">Cancel the old subscription</span></span>

<span data-ttu-id="4a31f-177">按照以下步骤将客户的 Office 365 企业版 E4 订阅迁移到上表中的其中一个选项。</span><span class="sxs-lookup"><span data-stu-id="4a31f-177">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="4a31f-178">步骤 1 - 购买新订阅</span><span class="sxs-lookup"><span data-stu-id="4a31f-178">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="4a31f-179">从**合作伙伴中心**菜单中，选择**客户**、 选择你想要移动的客户，然后选择**添加订阅**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-179">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="4a31f-180">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-180">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="4a31f-181">你的客户现在应该具有旧订阅和新订阅，即旧的 Office 365 企业版 E4 订阅和新的“目标”订阅，例如“选项 1 - Office 365 企业版 E5”。</span><span class="sxs-lookup"><span data-stu-id="4a31f-181">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new ‘target’ subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="4a31f-182">第 2 步 - 重新分配客户的用户许可证</span><span class="sxs-lookup"><span data-stu-id="4a31f-182">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="4a31f-183">从**合作伙伴中心**菜单中，选择**客户**、 选择你想要移动的客户，然后选择**用户和许可证**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-183">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="4a31f-184">将打开客户的“用户和许可证”页。</span><span class="sxs-lookup"><span data-stu-id="4a31f-184">The customer’s Users and Licenses page opens.</span></span>

2. <span data-ttu-id="4a31f-185">若要重新分配用户许可证，请选择要重新分配的用户，然后选择**管理许可证**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-185">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="4a31f-186">在**管理许可证**页面上，清除 **Office 365 企业版 E4** 许可证复选框，然后选择客户要迁移到的订阅的新服务计划。</span><span class="sxs-lookup"><span data-stu-id="4a31f-186">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="4a31f-187">选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-187">Select **Submit**.</span></span> <span data-ttu-id="4a31f-188">确认页面列出了新的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="4a31f-188">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="4a31f-189">对其他任何需要重新分配许可证的客户用户继续执行相同的步骤。</span><span class="sxs-lookup"><span data-stu-id="4a31f-189">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="4a31f-190">在将用户许可证移动至新服务后，可安全取消最高“客户”级别的已停用订阅。</span><span class="sxs-lookup"><span data-stu-id="4a31f-190">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="4a31f-191">步骤 3 - 取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="4a31f-191">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="4a31f-192">从**合作伙伴中心**菜单中，选择**客户**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-192">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4a31f-193">选择你想要移动的客户，并选择你想要取消的订阅。</span><span class="sxs-lookup"><span data-stu-id="4a31f-193">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="4a31f-194">在订阅详细信息页面中，将订阅状态设置为**已暂停**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-194">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="4a31f-195">选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="4a31f-195">Select **Submit**.</span></span>

<span data-ttu-id="4a31f-196">旧订阅已暂停，新订阅将激活。</span><span class="sxs-lookup"><span data-stu-id="4a31f-196">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="4a31f-197">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="4a31f-197">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="4a31f-198">不会向客户收取旧订阅的任何额外成本。</span><span class="sxs-lookup"><span data-stu-id="4a31f-198">The customer incurs no additional costs for the old subscription.</span></span>



 



