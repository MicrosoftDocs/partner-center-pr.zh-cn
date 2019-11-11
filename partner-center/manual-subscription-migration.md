---
title: 将 Dynamics 365 和 Customer Engagement 计划从基本（合格的产品/服务）迁移到更新的版本 |合作伙伴中心
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 不能再续订 Dynamics 365 for Sales/Customer Engagement 计划（基本（合格产品））订阅。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 产品/服务续订优惠，全新 Dynamics 365 Sku
ms.openlocfilehash: 354846973227fd292514454dd6f648934e5156ef
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653311"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="7b51e-104">将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="7b51e-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="7b51e-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="7b51e-105">**Applies to**</span></span>

-  <span data-ttu-id="7b51e-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="7b51e-106">Partner Center</span></span>

<span data-ttu-id="7b51e-107">从2019年1月1日起生效，对于基本（合格的产品/服务）订阅，具有 Dynamics 365 的客户将无法再续订这些旧产品/服务。现有订阅将不会在过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="7b51e-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="7b51e-108">在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。</span><span class="sxs-lookup"><span data-stu-id="7b51e-108">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="7b51e-109">若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。</span><span class="sxs-lookup"><span data-stu-id="7b51e-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="7b51e-110">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="7b51e-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="7b51e-111">如果使用 API （CREST 或合作者中心），可以通过评估订阅的结束日期以及自动续订 = False 属性来找到过期订阅。</span><span class="sxs-lookup"><span data-stu-id="7b51e-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="7b51e-112">相关订阅将在2019年1月1日设置为自动续订 = False。</span><span class="sxs-lookup"><span data-stu-id="7b51e-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="7b51e-113">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="7b51e-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="7b51e-114">Dynamics 365 产品/服务已停用</span><span class="sxs-lookup"><span data-stu-id="7b51e-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="7b51e-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格提议）</span><span class="sxs-lookup"><span data-stu-id="7b51e-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格产品）</span><span class="sxs-lookup"><span data-stu-id="7b51e-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7b51e-117">适用于 Sales Enterprise Edition 的 Dynamics 365 CRMOL Basic （合格产品）</span><span class="sxs-lookup"><span data-stu-id="7b51e-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7b51e-118">Dynamics 365 for Sales Enterprise Edition （政府定价） CRMOL 基本（合格产品）</span><span class="sxs-lookup"><span data-stu-id="7b51e-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-119">适用于 CRM Basic 的 SA 的 Dynamics 365 for Sales Enterprise Edition （合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-120">适用于教职员工的 SA for CRM Basic （合格产品/服务）的 Sales Enterprise Edition Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="7b51e-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7b51e-121">适用于学生的 SA for CRM Basic （合格产品/服务）的 Sales Enterprise Edition Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="7b51e-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7b51e-122">适用于 CRM Basic 的 SA 的 Dynamics 365 for Sales Enterprise Edition （政府定价）（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-123">适用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-124">适用于教职员工的 Dynamics 365 for Sales Enterprise Edition 外接程序</span><span class="sxs-lookup"><span data-stu-id="7b51e-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7b51e-125">适用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 外接程序（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7b51e-126">适用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定价）外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-127">Dynamics 365 客户参与计划企业版 CRMOL 基本（合格产品）</span><span class="sxs-lookup"><span data-stu-id="7b51e-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-128">Dynamics 365 客户参与计划企业版（政府定价） CRMOL 基本（合格产品）</span><span class="sxs-lookup"><span data-stu-id="7b51e-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-129">Dynamics 365 客户参与计划企业版 CRMOL 基本（合格提议）学生版</span><span class="sxs-lookup"><span data-stu-id="7b51e-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7b51e-130">Dynamics 365 客户参与计划企业版 CRMOL 基本（合格提议）</span><span class="sxs-lookup"><span data-stu-id="7b51e-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7b51e-131">Dynamics 365 客户参与计划适用于 CRM Basic 的 SA 的企业版（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-132">适用于 CRM Basic 的来自 SA 的 Dynamics 365 Customer Engagement 计划 Enterprise Edition （政府定价）（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-133">Dynamics 365 客户参与计划适用于 CRM 的 SA 的企业版基本版（合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7b51e-134">Dynamics 365 客户参与计划针对教职员工的 SA for CRM Basic （合格产品/服务）的企业版</span><span class="sxs-lookup"><span data-stu-id="7b51e-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7b51e-135">适用于 CRM Basic 的 Dynamics 365 客户参与计划企业版外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-136">适用于 CRM Basic 的 Dynamics 365 客户参与计划企业版（政府定价）外接程序（合格的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-137">Dynamics 365 客户参与计划适用于 CRM 基本版（合格产品/服务）的企业版外接程序</span><span class="sxs-lookup"><span data-stu-id="7b51e-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7b51e-138">Dynamics 365 客户参与计划适用于 CRM 基本版（合格产品/服务）的企业版外接程序</span><span class="sxs-lookup"><span data-stu-id="7b51e-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="7b51e-139">基本（合格产品/服务）更换计划的 Dynamics 365 for Sales/Customer Engagement 计划</span><span class="sxs-lookup"><span data-stu-id="7b51e-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="7b51e-140">**停用的产品**</span><span class="sxs-lookup"><span data-stu-id="7b51e-140">**Retired offers**</span></span>   

- <span data-ttu-id="7b51e-141">CRM Basic 或 CRMOL Basic 中的销售额的 Dynamics 365 （合格产品/服务）</span><span class="sxs-lookup"><span data-stu-id="7b51e-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7b51e-142">CRM Basic 或 CRMOL Basic 中的 Dynamics 365 客户参与计划（合格提议）</span><span class="sxs-lookup"><span data-stu-id="7b51e-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="7b51e-143">**替换选项**</span><span class="sxs-lookup"><span data-stu-id="7b51e-143">**Replacement options**</span></span>
- <span data-ttu-id="7b51e-144">针对销售专业人员的 Dynamics 365 （新）</span><span class="sxs-lookup"><span data-stu-id="7b51e-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="7b51e-145">针对销售专业人员的 Dynamics 365 （新）</span><span class="sxs-lookup"><span data-stu-id="7b51e-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="7b51e-146">适用于客户服务的 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="7b51e-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="7b51e-147">Dynamics 365 客户参与计划或</span><span class="sxs-lookup"><span data-stu-id="7b51e-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="7b51e-148">Dynamics 365 团队成员</span><span class="sxs-lookup"><span data-stu-id="7b51e-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="7b51e-149">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="7b51e-149">Transition customers to new product plans</span></span>

<span data-ttu-id="7b51e-150">将客户从停用的 Sku 转移到新的 Sku 需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7b51e-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="7b51e-151">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="7b51e-151">Purchase the new subscription</span></span>
- <span data-ttu-id="7b51e-152">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="7b51e-152">Reassign current user licenses</span></span>
- <span data-ttu-id="7b51e-153">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="7b51e-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="7b51e-154">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="7b51e-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="7b51e-155">从左侧导航栏中选择 "**客户**"，并选择要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="7b51e-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="7b51e-156">选择 "**添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="7b51e-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="7b51e-157">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="7b51e-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="7b51e-158">你的客户现在将具有旧订阅和新订阅。</span><span class="sxs-lookup"><span data-stu-id="7b51e-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="7b51e-159">下一步是向客户的用户重新分配许可证。</span><span class="sxs-lookup"><span data-stu-id="7b51e-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="7b51e-160">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="7b51e-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7b51e-161">选择**用户和许可证**。</span><span class="sxs-lookup"><span data-stu-id="7b51e-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="7b51e-162">若要为用户重新分配许可证，请选择该用户，然后选择 "**管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="7b51e-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="7b51e-163">在 "**管理许可证**" 页上，清除 "基本（合格产品/服务）许可证的 Dynamics 365 for Sales/Customer Engagement 计划" 复选框，并为客户要移到的订阅选择新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="7b51e-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="7b51e-164">选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="7b51e-164">Select **Submit**.</span></span> <span data-ttu-id="7b51e-165">你将对需要新许可证的每个用户执行此操作。</span><span class="sxs-lookup"><span data-stu-id="7b51e-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="7b51e-166">将许可证转移到新订阅后，可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="7b51e-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="7b51e-167">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="7b51e-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7b51e-168">在 "订阅详细信息" 页上，将旧订阅设置为 "**挂起**"，然后选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="7b51e-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="7b51e-169">旧订阅现已暂停，新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="7b51e-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="7b51e-170">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="7b51e-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="7b51e-171">你的客户不会对旧订阅产生额外的费用。</span><span class="sxs-lookup"><span data-stu-id="7b51e-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



