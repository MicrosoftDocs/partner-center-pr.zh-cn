---
title: 将 Dynamics 365 和客户参与度计划从基本 （限定产品/服务） 迁移到较新版本 |合作伙伴中心
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / 从 （限定产品/服务） 的基本订阅的客户参与度计划不再续订。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968267"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="20b93-103">将 Dynamics 365 和客户参与度计划从基本 （限定产品/服务） 迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="20b93-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="20b93-104">适用范围</span><span class="sxs-lookup"><span data-stu-id="20b93-104">Applies to</span></span>**

-  <span data-ttu-id="20b93-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="20b93-105">Partner Center</span></span>

<span data-ttu-id="20b93-106">Dynamics 365 for Sales 的有效于 2019 年 1 月 1 日，客户 / 从 （限定产品/服务） 的基本订阅的客户参与度计划可以不再续订这些旧的产品/服务。当它们到期时，现有订阅将不会自动续订。</span><span class="sxs-lookup"><span data-stu-id="20b93-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="20b93-107">订阅的详细信息页面上的订阅状态将从"自动续订 [日期]"更改为"[日期] 过期"。</span><span class="sxs-lookup"><span data-stu-id="20b93-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="20b93-108">若要确保客户服务连续性，你应该过渡那些到支持的选项，下面列出的订阅快过期。</span><span class="sxs-lookup"><span data-stu-id="20b93-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="20b93-109">建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。</span><span class="sxs-lookup"><span data-stu-id="20b93-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="20b93-110">如果你使用 API （CREST 或合作伙伴中心），你可以找到通过评估以及自动订阅的结束日期即将到期订阅续订 = False 属性。</span><span class="sxs-lookup"><span data-stu-id="20b93-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="20b93-111">问题的订阅将设置为自动续订 = False 于 2019 年 1 月 1 日。</span><span class="sxs-lookup"><span data-stu-id="20b93-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="20b93-112">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="20b93-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="20b93-113">Dynamics 365 产品/服务被停用</span><span class="sxs-lookup"><span data-stu-id="20b93-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="20b93-114">Dynamics 365 销售企业版 CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-115">Dynamics 365 销售企业版 CRMOL 基本 （限定产品/服务） （教职员工）</span><span class="sxs-lookup"><span data-stu-id="20b93-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="20b93-116">Dynamics 365 的学生的销售企业版 CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="20b93-117">Dynamics 365 销售企业版 （政府定价） CRMOL 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-118">Dynamics 365 销售企业版从 SA CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-119">Dynamics 365 销售企业版从 SA CRM 基本 （限定产品/服务） （教职员工）</span><span class="sxs-lookup"><span data-stu-id="20b93-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="20b93-120">Dynamics 365 销售企业版 SA CRM 基本 （限定产品/服务） 的学生从</span><span class="sxs-lookup"><span data-stu-id="20b93-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="20b93-121">Dynamics 365 销售企业版 （定价政府） 从 SA CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-122">Dynamics 365 销售企业版加载项 CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-123">Dynamics 365 销售企业版加载项 （教职员工） CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="20b93-124">Dynamics 365 销售企业版加载项 （学生） CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="20b93-125">Dynamics 365 销售企业版 （政府定价） 加载项 CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-126">Dynamics 365 客户参与度计划企业版 CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-127">Dynamics 365 客户参与度计划企业版 （政府定价） CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-128">Dynamics 365 客户参与度计划企业版 CRMOL Basic （限定产品/服务） (学生）</span><span class="sxs-lookup"><span data-stu-id="20b93-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="20b93-129">Dynamics 365 客户参与度计划企业版 CRMOL Basic （限定产品/服务） (教职员工）</span><span class="sxs-lookup"><span data-stu-id="20b93-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="20b93-130">从 CRM 基本 （限定产品/服务） 的 SA Dynamics 365 客户参与度计划企业版</span><span class="sxs-lookup"><span data-stu-id="20b93-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-131">Dynamics 365 客户参与度计划企业版 （定价政府） 从 SA CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-132">从 CRM 基本 （限定产品/服务） 的学生的 SA Dynamics 365 客户参与度计划企业版</span><span class="sxs-lookup"><span data-stu-id="20b93-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="20b93-133">从教职员工有关 CRM 基本 （限定产品/服务） 的 SA Dynamics 365 客户参与度计划企业版</span><span class="sxs-lookup"><span data-stu-id="20b93-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="20b93-134">Dynamics 365 客户参与度计划企业版的加载项 CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-135">Dynamics 365 客户参与度计划企业版 （政府定价） 加载项 CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-136">Dynamics 365 客户参与度计划企业版加载项 (学生） CRM Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="20b93-137">Dynamics 365 客户参与度计划企业版的加载项 （教职员工） CRM 基本 （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="20b93-138">Dynamics 365 for Sales / 客户参与度计划从 （限定产品/服务） 的基本替换计划</span><span class="sxs-lookup"><span data-stu-id="20b93-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="20b93-139">已停用产品/服务</span><span class="sxs-lookup"><span data-stu-id="20b93-139">Retired offers</span></span>**   

- <span data-ttu-id="20b93-140">Dynamics 365 for Sales 从 CRM 基本或 CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="20b93-141">Dynamics 365 客户参与度计划从 CRM 基本或 CRMOL Basic （限定产品/服务）</span><span class="sxs-lookup"><span data-stu-id="20b93-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="20b93-142">替换选项</span><span class="sxs-lookup"><span data-stu-id="20b93-142">Replacement options</span></span>**
- <span data-ttu-id="20b93-143">Dynamics 365 的销售专业版 （新增）</span><span class="sxs-lookup"><span data-stu-id="20b93-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="20b93-144">Dynamics 365 的销售专业版 （新增）</span><span class="sxs-lookup"><span data-stu-id="20b93-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="20b93-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="20b93-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="20b93-146">Dynamics 365 客户参与度计划或</span><span class="sxs-lookup"><span data-stu-id="20b93-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="20b93-147">Dynamics 365 团队成员</span><span class="sxs-lookup"><span data-stu-id="20b93-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="20b93-148">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="20b93-148">Transition customers to new product plans</span></span>

<span data-ttu-id="20b93-149">从已停用的 Sku 的客户移动到较新的需要按此顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="20b93-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="20b93-150">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="20b93-150">Purchase the new subscription</span></span>
- <span data-ttu-id="20b93-151">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="20b93-151">Reassign current user licenses</span></span>
- <span data-ttu-id="20b93-152">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="20b93-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="20b93-153">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="20b93-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="20b93-154">从左侧导航中选择**客户**，然后选择你想要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="20b93-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="20b93-155">选择**添加订阅**。</span><span class="sxs-lookup"><span data-stu-id="20b93-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="20b93-156">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="20b93-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="20b93-157">你的客户现在将具有旧订阅和新。</span><span class="sxs-lookup"><span data-stu-id="20b93-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="20b93-158">下一步是许可证重新分配到客户的用户。</span><span class="sxs-lookup"><span data-stu-id="20b93-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="20b93-159">从左侧导航中选择**客户**，然后选择你要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="20b93-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="20b93-160">选择**用户和许可证**。</span><span class="sxs-lookup"><span data-stu-id="20b93-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="20b93-161">若要重新分配用户许可证，选择用户，然后选择**管理许可证**。</span><span class="sxs-lookup"><span data-stu-id="20b93-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="20b93-162">在**管理许可证**页上，清除 Dynamics 365 for Sales/从基本 （限定产品/服务） 的客户参与度计划许可证复选框，然后选择客户要迁移到的订阅的新服务计划。</span><span class="sxs-lookup"><span data-stu-id="20b93-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="20b93-163">选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="20b93-163">Select **Submit**.</span></span> <span data-ttu-id="20b93-164">将每个用户都需要新许可证来执行此操作。</span><span class="sxs-lookup"><span data-stu-id="20b93-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="20b93-165">你已移许可证的新订阅后您可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="20b93-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="20b93-166">从左侧导航中选择**客户**，然后选择你要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="20b93-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="20b93-167">在订阅详细信息页上，设置为**已暂停**的旧订阅，并选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="20b93-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="20b93-168">旧订阅现在暂停，并且新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="20b93-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="20b93-169">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="20b93-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="20b93-170">你的客户将产生的旧订阅任何额外成本。</span><span class="sxs-lookup"><span data-stu-id="20b93-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



