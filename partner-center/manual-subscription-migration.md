---
title: 迁移合格的 Dynamics 365 订阅
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在现有订阅过期之前从合格的基本 Dynamics 365 订阅迁移到新的订阅。
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436846"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="94c03-103">将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="94c03-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="94c03-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="94c03-104">**Applies to**</span></span>

-  <span data-ttu-id="94c03-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="94c03-105">Partner Center</span></span>

<span data-ttu-id="94c03-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="94c03-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="94c03-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="94c03-107">Global admin</span></span>
-   <span data-ttu-id="94c03-108">用户管理员</span><span class="sxs-lookup"><span data-stu-id="94c03-108">User admin</span></span>
-   <span data-ttu-id="94c03-109">管理员代理</span><span class="sxs-lookup"><span data-stu-id="94c03-109">Admin agent</span></span>
-   <span data-ttu-id="94c03-110">销售代理</span><span class="sxs-lookup"><span data-stu-id="94c03-110">Sales agent</span></span>

<span data-ttu-id="94c03-111">从2019年1月1日起生效，对于基本（合格的产品/服务）订阅，具有 Dynamics 365 的客户将无法再续订这些旧产品/服务。现有订阅将不会在过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="94c03-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="94c03-112">在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。</span><span class="sxs-lookup"><span data-stu-id="94c03-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="94c03-113">若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。</span><span class="sxs-lookup"><span data-stu-id="94c03-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="94c03-114">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="94c03-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="94c03-115">如果使用 API （CREST 或合作者中心），可以通过评估订阅的结束日期以及自动续订 = False 属性来找到过期订阅。</span><span class="sxs-lookup"><span data-stu-id="94c03-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="94c03-116">相关订阅将在2019年1月1日设置为自动续订 = False。</span><span class="sxs-lookup"><span data-stu-id="94c03-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="94c03-117">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="94c03-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="94c03-118">Dynamics 365 产品/服务已停用</span><span class="sxs-lookup"><span data-stu-id="94c03-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="94c03-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格提议）</span><span class="sxs-lookup"><span data-stu-id="94c03-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格产品）</span><span class="sxs-lookup"><span data-stu-id="94c03-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="94c03-121">适用于 Sales Enterprise Edition 的 Dynamics 365 CRMOL Basic （合格产品）</span><span class="sxs-lookup"><span data-stu-id="94c03-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="94c03-122">Dynamics 365 for Sales Enterprise Edition （政府定价） CRMOL 基本（合格产品）</span><span class="sxs-lookup"><span data-stu-id="94c03-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-123">适用于 CRM Basic 的 SA 的 Dynamics 365 for Sales Enterprise Edition （合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-124">适用于教职员工的 SA for CRM Basic （合格产品/服务）的 Sales Enterprise Edition Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="94c03-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="94c03-125">适用于学生的 SA for CRM Basic （合格产品/服务）的 Sales Enterprise Edition Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="94c03-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="94c03-126">适用于 CRM Basic 的 SA 的 Dynamics 365 for Sales Enterprise Edition （政府定价）（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-127">适用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-128">适用于教职员工的 Dynamics 365 for Sales Enterprise Edition 外接程序</span><span class="sxs-lookup"><span data-stu-id="94c03-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="94c03-129">适用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 外接程序（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="94c03-130">适用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定价）外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-131">Dynamics 365 客户参与计划企业版 CRMOL 基本（合格产品）</span><span class="sxs-lookup"><span data-stu-id="94c03-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-132">Dynamics 365 客户参与计划企业版（政府定价） CRMOL 基本（合格产品）</span><span class="sxs-lookup"><span data-stu-id="94c03-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-133">Dynamics 365 客户参与计划企业版 CRMOL 基本（合格提议）学生版</span><span class="sxs-lookup"><span data-stu-id="94c03-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="94c03-134">Dynamics 365 客户参与计划企业版 CRMOL 基本（合格提议）</span><span class="sxs-lookup"><span data-stu-id="94c03-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="94c03-135">Dynamics 365 客户参与计划适用于 CRM Basic 的 SA 的企业版（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-136">适用于 CRM Basic 的来自 SA 的 Dynamics 365 Customer Engagement 计划 Enterprise Edition （政府定价）（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-137">Dynamics 365 客户参与计划适用于 CRM 的 SA 的企业版基本版（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="94c03-138">Dynamics 365 客户参与计划针对教职员工的 SA for CRM Basic （合格产品/服务）的企业版</span><span class="sxs-lookup"><span data-stu-id="94c03-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="94c03-139">适用于 CRM Basic 的 Dynamics 365 客户参与计划企业版外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-140">适用于 CRM Basic 的 Dynamics 365 客户参与计划企业版（政府定价）外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-141">Dynamics 365 客户参与计划适用于 CRM 基本版（合格产品/服务）的企业版外接程序</span><span class="sxs-lookup"><span data-stu-id="94c03-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="94c03-142">Dynamics 365 客户参与计划适用于 CRM 基本版（合格产品/服务）的企业版外接程序</span><span class="sxs-lookup"><span data-stu-id="94c03-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="94c03-143">基本（合格产品/服务）更换计划的 Dynamics 365 for Sales/Customer Engagement 计划</span><span class="sxs-lookup"><span data-stu-id="94c03-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="94c03-144">**停用的产品**</span><span class="sxs-lookup"><span data-stu-id="94c03-144">**Retired offers**</span></span>   

- <span data-ttu-id="94c03-145">CRM Basic 或 CRMOL Basic 中的销售额的 Dynamics 365 （合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="94c03-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="94c03-146">CRM Basic 或 CRMOL Basic 中的 Dynamics 365 客户参与计划（合格提议）</span><span class="sxs-lookup"><span data-stu-id="94c03-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="94c03-147">**替换选项**</span><span class="sxs-lookup"><span data-stu-id="94c03-147">**Replacement options**</span></span>
- <span data-ttu-id="94c03-148">针对销售专业人员的 Dynamics 365 （新）</span><span class="sxs-lookup"><span data-stu-id="94c03-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="94c03-149">针对销售专业人员的 Dynamics 365 （新）</span><span class="sxs-lookup"><span data-stu-id="94c03-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="94c03-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="94c03-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="94c03-151">Dynamics 365 客户参与计划或</span><span class="sxs-lookup"><span data-stu-id="94c03-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="94c03-152">Dynamics 365 团队成员</span><span class="sxs-lookup"><span data-stu-id="94c03-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="94c03-153">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="94c03-153">Transition customers to new product plans</span></span>

<span data-ttu-id="94c03-154">将客户从停用的 Sku 转移到新的 Sku 需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="94c03-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="94c03-155">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="94c03-155">Purchase the new subscription</span></span>
- <span data-ttu-id="94c03-156">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="94c03-156">Reassign current user licenses</span></span>
- <span data-ttu-id="94c03-157">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="94c03-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="94c03-158">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="94c03-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="94c03-159">从左侧导航栏中选择 "**客户**"，并选择要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="94c03-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="94c03-160">选择 "**添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="94c03-160">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="94c03-161">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="94c03-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="94c03-162">你的客户现在将具有旧订阅和新订阅。</span><span class="sxs-lookup"><span data-stu-id="94c03-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="94c03-163">下一步是向客户的用户重新分配许可证。</span><span class="sxs-lookup"><span data-stu-id="94c03-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="94c03-164">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="94c03-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="94c03-165">选择 "**用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="94c03-165">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="94c03-166">若要为用户重新分配许可证，请选择该用户，然后选择 "**管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="94c03-166">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="94c03-167">在 "**管理许可证**" 页上，清除 "基本（合格产品/服务）许可证的 Dynamics 365 for Sales/Customer Engagement 计划" 复选框，并为客户要移到的订阅选择新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="94c03-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="94c03-168">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="94c03-168">Select **Submit**.</span></span> <span data-ttu-id="94c03-169">你将对需要新许可证的每个用户执行此操作。</span><span class="sxs-lookup"><span data-stu-id="94c03-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="94c03-170">将许可证转移到新订阅后，可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="94c03-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="94c03-171">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="94c03-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="94c03-172">在 "订阅详细信息" 页上，将旧订阅设置为 "**挂起**"，然后选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="94c03-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="94c03-173">旧订阅现已暂停，新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="94c03-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="94c03-174">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="94c03-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="94c03-175">你的客户不会对旧订阅产生额外的费用。</span><span class="sxs-lookup"><span data-stu-id="94c03-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



