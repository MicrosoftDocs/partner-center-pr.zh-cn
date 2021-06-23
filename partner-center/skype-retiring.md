---
title: 迁移 Skype for Business 订阅
description: 了解如何以及何时将已过期 Skype for business Online 计划1订阅的特定客户迁移到新的 Office 365 版本。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: a8de5b824a24b07607b5365848ec1027ca0d08e8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551531"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="eff18-103">将 Skype for Business Online Plan 1 订阅迁移到更新的 Office 365 版本</span><span class="sxs-lookup"><span data-stu-id="eff18-103">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="eff18-104">**适当的角色**：销售代理</span><span class="sxs-lookup"><span data-stu-id="eff18-104">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="eff18-105">Skype for Business Online 计划1将停用，在2018年8月1日生效。</span><span class="sxs-lookup"><span data-stu-id="eff18-105">The Skype for Business Online Plan 1 will be retired, effective August 1, 2018.</span></span> <span data-ttu-id="eff18-106">该日期之后，客户将无法再购买新的 Skype for Business Plan 1 订阅，现有订阅在过期后不会自动续订且不会提供订阅选项。</span><span class="sxs-lookup"><span data-stu-id="eff18-106">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="eff18-107">在订阅的详细信息页面上，Skype for Business Online Plan 1 订阅状态已从“[日期] 自动续订”更改为“[日期] 过期”。</span><span class="sxs-lookup"><span data-stu-id="eff18-107">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="eff18-108">为了确保客户服务连续性，你应该将 Skype for Business Online Plan 1 订阅快过期的客户过渡到下列支持的 SKU 选项。</span><span class="sxs-lookup"><span data-stu-id="eff18-108">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="eff18-109">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="eff18-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="eff18-110">Skype for Business Online Plan 1 商业和政府 SKU 均已停用。</span><span class="sxs-lookup"><span data-stu-id="eff18-110">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="eff18-111">如果使用 API (Commerce REST (CREST) 或合作伙伴中心) ，则通过评估订阅的结束日期以及自动续订 = False 属性，查找过期订阅。</span><span class="sxs-lookup"><span data-stu-id="eff18-111">If you use the API (either Commerce REST (CREST) or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="eff18-112">Skype for Business Online Plan 1 订阅将在 2018 年 9 月 1 设置为自动续订=False。</span><span class="sxs-lookup"><span data-stu-id="eff18-112">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="eff18-113">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="eff18-113">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="eff18-114">Skype for Business Online Plan 1 替换计划</span><span class="sxs-lookup"><span data-stu-id="eff18-114">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="eff18-115">使用新计划，你的客户可以利用 Office 365 中的更新功能。</span><span class="sxs-lookup"><span data-stu-id="eff18-115">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="eff18-116">定价详细信息位于合作伙伴中心内的价目表及产品/服务列表矩阵中。</span><span class="sxs-lookup"><span data-stu-id="eff18-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="eff18-117">选项 1：Office 365 企业版 F1</span><span class="sxs-lookup"><span data-stu-id="eff18-117">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="eff18-118">选项 2：Microsoft 365 企业版 F1</span><span class="sxs-lookup"><span data-stu-id="eff18-118">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="eff18-119">选项 3：其他 Office 365 计划</span><span class="sxs-lookup"><span data-stu-id="eff18-119">Option 3: Other Office 365 plans</span></span>

|<span data-ttu-id="eff18-120">**功能**</span><span class="sxs-lookup"><span data-stu-id="eff18-120">**Feature**</span></span>    |<span data-ttu-id="eff18-121">**选项 1**</span><span class="sxs-lookup"><span data-stu-id="eff18-121">**Option 1**</span></span>   |<span data-ttu-id="eff18-122">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="eff18-122">**Option 2**</span></span>   |<span data-ttu-id="eff18-123">**选项3**</span><span class="sxs-lookup"><span data-stu-id="eff18-123">**Option 3**</span></span>   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="eff18-124">获取 Skype for Business Online Plan 1 所含的所有功能</span><span class="sxs-lookup"><span data-stu-id="eff18-124">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="eff18-125">是</span><span class="sxs-lookup"><span data-stu-id="eff18-125">Yes</span></span>   |<span data-ttu-id="eff18-126">是</span><span class="sxs-lookup"><span data-stu-id="eff18-126">Yes</span></span>   |<span data-ttu-id="eff18-127">是</span><span class="sxs-lookup"><span data-stu-id="eff18-127">Yes</span></span>   |
|<span data-ttu-id="eff18-128">IM 和状态</span><span class="sxs-lookup"><span data-stu-id="eff18-128">IM and presence</span></span> |<span data-ttu-id="eff18-129">是</span><span class="sxs-lookup"><span data-stu-id="eff18-129">Yes</span></span>   |<span data-ttu-id="eff18-130">是</span><span class="sxs-lookup"><span data-stu-id="eff18-130">Yes</span></span>   |<span data-ttu-id="eff18-131">是</span><span class="sxs-lookup"><span data-stu-id="eff18-131">Yes</span></span>   |
|<span data-ttu-id="eff18-132">通过 IP 的对等音频和视频</span><span class="sxs-lookup"><span data-stu-id="eff18-132">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="eff18-133">是</span><span class="sxs-lookup"><span data-stu-id="eff18-133">Yes</span></span>   |<span data-ttu-id="eff18-134">是</span><span class="sxs-lookup"><span data-stu-id="eff18-134">Yes</span></span>   |<span data-ttu-id="eff18-135">是</span><span class="sxs-lookup"><span data-stu-id="eff18-135">Yes</span></span>   
|<span data-ttu-id="eff18-136">以通过身份验证的用户身份加入会议</span><span class="sxs-lookup"><span data-stu-id="eff18-136">Join meetings as an authenticated user</span></span>| <span data-ttu-id="eff18-137">是</span><span class="sxs-lookup"><span data-stu-id="eff18-137">Yes</span></span>   |<span data-ttu-id="eff18-138">是</span><span class="sxs-lookup"><span data-stu-id="eff18-138">Yes</span></span>   |<span data-ttu-id="eff18-139">是</span><span class="sxs-lookup"><span data-stu-id="eff18-139">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="eff18-140">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="eff18-140">Transition customers to new product plans</span></span>

<span data-ttu-id="eff18-141">Microsoft 不断向我们的合作伙伴提供新产品和服务。</span><span class="sxs-lookup"><span data-stu-id="eff18-141">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="eff18-142">在这些情况下，你可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。</span><span class="sxs-lookup"><span data-stu-id="eff18-142">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="eff18-143">将客户从停用的 SKU 中迁移到新 SKU 需要按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="eff18-143">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="eff18-144">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="eff18-144">Purchase the new subscription</span></span>
- <span data-ttu-id="eff18-145">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="eff18-145">Reassign current user licenses</span></span>
- <span data-ttu-id="eff18-146">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="eff18-146">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="eff18-147">将你的客户迁移至新计划</span><span class="sxs-lookup"><span data-stu-id="eff18-147">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="eff18-148">若要购买新的订阅，请从 " **合作伙伴中心" 菜单** 中选择 " **客户**"，选择要移动的客户，然后选择 " **添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="eff18-148">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="eff18-149">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。</span><span class="sxs-lookup"><span data-stu-id="eff18-149">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="eff18-150">你的客户现在应具有新订阅和新订阅，旧的 Skype for Business Online 计划1订阅和新的 "目标" 订阅，例如，选项 1-Office 365 企业 F1。</span><span class="sxs-lookup"><span data-stu-id="eff18-150">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="eff18-151">若要重新分配客户的用户许可证，请在 " **合作伙伴中心** " 菜单中选择 " **客户**"，选择要移动的客户，然后选择 " **用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="eff18-151">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="eff18-152">此时将打开客户的 "用户和许可证" 页。</span><span class="sxs-lookup"><span data-stu-id="eff18-152">The customer's Users and Licenses page opens.</span></span>

4. <span data-ttu-id="eff18-153">若要重新分配用户许可证，请选择要重新分配的用户，然后选择 **管理许可证**。</span><span class="sxs-lookup"><span data-stu-id="eff18-153">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="eff18-154">在 **管理许可证** 页面上，清除 Skype for Business Online Plan 1 许可证复选框，然后选择客户要迁移到的订阅的新服务计划。</span><span class="sxs-lookup"><span data-stu-id="eff18-154">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="eff18-155">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="eff18-155">Select **Submit**.</span></span> <span data-ttu-id="eff18-156">确认页面列出了新的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="eff18-156">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="eff18-157">继续对需要许可证分配的其他用户执行相同过程。</span><span class="sxs-lookup"><span data-stu-id="eff18-157">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="eff18-158">在将用户许可证移动至新服务后，可安全取消该客户级别的已停用订阅。</span><span class="sxs-lookup"><span data-stu-id="eff18-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="eff18-159">从 " **合作伙伴中心** " 菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="eff18-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="eff18-160">选择要取消其订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="eff18-160">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="eff18-161">在订阅详细信息页面中，将订阅设置为 **已暂停**。</span><span class="sxs-lookup"><span data-stu-id="eff18-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="eff18-162">选择 " **提交"。**</span><span class="sxs-lookup"><span data-stu-id="eff18-162">Select **Submit.**</span></span>

<span data-ttu-id="eff18-163">旧订阅已暂停，新订阅将激活。</span><span class="sxs-lookup"><span data-stu-id="eff18-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="eff18-164">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="eff18-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="eff18-165">不会向客户收取旧订阅的任何额外成本。</span><span class="sxs-lookup"><span data-stu-id="eff18-165">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eff18-166">后续步骤</span><span class="sxs-lookup"><span data-stu-id="eff18-166">Next steps</span></span>

- [<span data-ttu-id="eff18-167">顾问：创建并发送试用版邀请，以便客户端尝试使用 Office 365</span><span class="sxs-lookup"><span data-stu-id="eff18-167">Advisors: Create and send a trial invitation for clients to try Office 365</span></span>](advisors-create-a-trial-invitation.md)
- [<span data-ttu-id="eff18-168">顾问：通过 Office 365 试用邀请和购买优惠构建客户群</span><span class="sxs-lookup"><span data-stu-id="eff18-168">Advisors: Build your client base with Office 365 trial invitations and purchase offers</span></span>](advisors-build-your-business.md)
- [<span data-ttu-id="eff18-169">顾问：创建购买提议</span><span class="sxs-lookup"><span data-stu-id="eff18-169">Advisors: Create a purchase offer</span></span>](advisor-create-a-purchase-offer.md)
