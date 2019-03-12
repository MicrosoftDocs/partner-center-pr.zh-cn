---
title: 将 Dynamics 365 和 Customer Engagement 计划从 Basic （限定产品/服务） 迁移到较新版本 |合作伙伴中心
ms.topic: article
ms.date: 12/12/2018
description: 为销售的 Dynamics 365 Customer Engagement 计划从 Basic （限定提供） 的订阅不能再续订 /。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 产品/服务，续订产品/服务，新的 Dynamics 365 Sku
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586940"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="ef5a5-104">将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="ef5a5-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="ef5a5-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="ef5a5-105">**Applies to**</span></span>

-  <span data-ttu-id="ef5a5-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="ef5a5-106">Partner Center</span></span>

<span data-ttu-id="ef5a5-107">有效 2019 年 1 月 1 日，客户与销售的 Dynamics 365 Customer Engagement 计划从 Basic （限定提供） 的订阅无法再续订这些旧的产品/服务; /过期时，将不自动续订现有订阅。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="ef5a5-108">在订阅的详细信息页上，订阅状态将从"自动续订于 [date]"更改为"过期日期 [date]"。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="ef5a5-109">若要为客户确保连续性，应转换那些与受支持的选项，下面列出的即将过期订阅。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="ef5a5-110">建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ef5a5-111">如果使用 API （CREST 或合作伙伴中心），可以找到通过计算结束日期以及自动订阅的过期订阅续订 = False 属性。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="ef5a5-112">相关的订阅将设置为自动续订在 2019 年 1 月 1 日 = False。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="ef5a5-113">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="ef5a5-114">Dynamics 365 提供了即将停用</span><span class="sxs-lookup"><span data-stu-id="ef5a5-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="ef5a5-115">Dynamics 365 for 销售 Enterprise Edition CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-116">Dynamics 365 for 教职员工版的销售 Enterprise Edition CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ef5a5-117">Dynamics 365 for 面向学生的销售 Enterprise Edition CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ef5a5-118">Dynamics 365 for 销售企业版 （政府定价） CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-119">Dynamics 365 适用于销售的 Enterprise Edition 来自 SA 的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-120">Dynamics 365 适用于销售的 Enterprise Edition 来自 SA 的 CRM Basic 教职员工版 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ef5a5-121">Dynamics 365 适用于销售的 Enterprise Edition 来自 SA 的 CRM Basic 学生版 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ef5a5-122">Dynamics 365 的销售企业版 （政府定价） 来自 SA 的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-123">Dynamics 365 的销售企业版外接程序的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-124">Dynamics 365 的销售企业版外接程序的 CRM Basic 教职员工版 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ef5a5-125">Dynamics 365 的销售企业版外接程序适用于面向学生的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ef5a5-126">Dynamics 365 的销售企业版 （政府定价） 外接程序的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-127">Dynamics 365 客户参与计划企业版 CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-128">Dynamics 365 客户参与计划企业版 （政府定价） CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-129">Dynamics 365 客户参与计划企业版 CRMOL Basic （限定产品/服务） 学生版</span><span class="sxs-lookup"><span data-stu-id="ef5a5-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ef5a5-130">Dynamics 365 客户参与计划企业版 CRMOL Basic （限定产品/服务） 教职员工版</span><span class="sxs-lookup"><span data-stu-id="ef5a5-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ef5a5-131">来自 SA 的 CRM Basic （限定产品/服务） 的 Dynamics 365 客户参与计划企业版</span><span class="sxs-lookup"><span data-stu-id="ef5a5-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-132">Dynamics 365 客户参与计划企业版 （政府定价） 来自 SA 的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-133">从面向学生的 CRM Basic （限定产品/服务） 的 SA 的 Dynamics 365 客户参与计划企业版</span><span class="sxs-lookup"><span data-stu-id="ef5a5-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ef5a5-134">来自 SA 的 CRM Basic 教职员工版 （限定产品/服务） 的 Dynamics 365 客户参与计划企业版</span><span class="sxs-lookup"><span data-stu-id="ef5a5-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ef5a5-135">Dynamics 365 客户参与计划企业版外接程序的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-136">Dynamics 365 客户参与计划企业版 （政府定价） 的外接程序 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-137">Dynamics 365 客户参与计划企业版外接程序适用于面向学生的 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ef5a5-138">Dynamics 365 客户参与计划企业版外接程序的 CRM Basic 教职员工版 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="ef5a5-139">为销售的 Dynamics 365 Customer Engagement 计划从 Basic （限定提供） 替换计划 /</span><span class="sxs-lookup"><span data-stu-id="ef5a5-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="ef5a5-140">**已停用的产品/服务**</span><span class="sxs-lookup"><span data-stu-id="ef5a5-140">**Retired offers**</span></span>   

- <span data-ttu-id="ef5a5-141">从 CRM Basic 或 CRMOL Basic （限定产品/服务） 销售的 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ef5a5-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ef5a5-142">Dynamics 365 客户参与计划从 CRM Basic 或 CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="ef5a5-143">**替换选项**</span><span class="sxs-lookup"><span data-stu-id="ef5a5-143">**Replacement options**</span></span>
- <span data-ttu-id="ef5a5-144">Dynamics 365 for Sales 专业版 （新）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ef5a5-145">Dynamics 365 for Sales 专业版 （新）</span><span class="sxs-lookup"><span data-stu-id="ef5a5-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ef5a5-146">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="ef5a5-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="ef5a5-147">Dynamics 365 客户参与计划或</span><span class="sxs-lookup"><span data-stu-id="ef5a5-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="ef5a5-148">Dynamics 365 团队成员</span><span class="sxs-lookup"><span data-stu-id="ef5a5-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ef5a5-149">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="ef5a5-149">Transition customers to new product plans</span></span>

<span data-ttu-id="ef5a5-150">将客户从已停用 Sku 移动到较新的需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="ef5a5-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="ef5a5-151">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="ef5a5-151">Purchase the new subscription</span></span>
- <span data-ttu-id="ef5a5-152">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="ef5a5-152">Reassign current user licenses</span></span>
- <span data-ttu-id="ef5a5-153">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="ef5a5-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="ef5a5-154">为您的客户购买新的计划</span><span class="sxs-lookup"><span data-stu-id="ef5a5-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="ef5a5-155">选择**客户**从左侧导航栏，然后选择你想要将移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="ef5a5-156">选择**添加订阅**。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="ef5a5-157">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="ef5a5-158">您的客户现在将在旧订阅并新建一个。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="ef5a5-159">下一步是重新分配给客户的用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="ef5a5-160">选择**客户**从左侧导航栏，然后选择客户正在移动。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ef5a5-161">选择**用户和许可证**。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="ef5a5-162">若要重新分配给用户的许可证，选择用户，然后选择**管理许可证**。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="ef5a5-163">上**管理许可证**页上，清除销售 Dynamics 365 / Basic （限定产品/服务） 中的客户参与计划许可证复选框，然后选择订阅客户移动到新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="ef5a5-164">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-164">Select **Submit**.</span></span> <span data-ttu-id="ef5a5-165">将为每个用户都需要新许可证来执行此操作。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="ef5a5-166">一旦您已将的许可证移到新的订阅可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="ef5a5-167">选择**客户**从左侧导航栏，然后选择客户正在移动。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ef5a5-168">在订阅详细信息页上，将旧的订阅设置为**Suspended** ，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="ef5a5-169">旧订阅现在已挂起，但新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="ef5a5-170">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ef5a5-171">您的客户将产生在旧订阅无额外成本。</span><span class="sxs-lookup"><span data-stu-id="ef5a5-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



