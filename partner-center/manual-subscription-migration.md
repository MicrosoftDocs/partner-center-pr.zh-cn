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
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151638"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="5228b-103">将 Dynamics 365 和客户参与度计划从基本（限定产品/服务）迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="5228b-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="5228b-104">**适当的角色**：全局管理员 |用户管理管理员 |管理代理 |销售代理</span><span class="sxs-lookup"><span data-stu-id="5228b-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="5228b-105">从2019年1月1日起生效，对于来自基本 (合格产品/服务的销售/客户参与计划的365客户，) 订阅不能再续订这些旧产品/服务。现有订阅将不会在过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="5228b-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="5228b-106">在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。</span><span class="sxs-lookup"><span data-stu-id="5228b-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="5228b-107">若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。</span><span class="sxs-lookup"><span data-stu-id="5228b-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="5228b-108">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="5228b-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="5228b-109">如果 ("CREST" 或 "合作伙伴中心") 使用 API，则可以通过使用 "自动续订 = False" 属性来评估订阅的结束日期，找到过期订阅。</span><span class="sxs-lookup"><span data-stu-id="5228b-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="5228b-110">相关订阅将在2019年1月1日设置为自动续订 = False。</span><span class="sxs-lookup"><span data-stu-id="5228b-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="5228b-111">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="5228b-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="5228b-112">Dynamics 365 产品/服务已停用</span><span class="sxs-lookup"><span data-stu-id="5228b-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="5228b-113">Dynamics 365 for Sales Enterprise Edition CRMOL 基本 (合格提议) </span><span class="sxs-lookup"><span data-stu-id="5228b-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-114">适用于 Sales Enterprise Edition 的 Dynamics 365 CRMOL Basic (限定提议) 教职员</span><span class="sxs-lookup"><span data-stu-id="5228b-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5228b-115">适用于 Sales Enterprise Edition 的 Dynamics 365 CRMOL Basic (合格提议) 学生</span><span class="sxs-lookup"><span data-stu-id="5228b-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5228b-116">Dynamics 365 for Sales Enterprise Edition (政府定价) CRMOL 基本 (合格产品/服务) </span><span class="sxs-lookup"><span data-stu-id="5228b-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-117">来自 SA for CRM Basic (合格的产品/服务的 Dynamics 365 for Sales Enterprise Edition) </span><span class="sxs-lookup"><span data-stu-id="5228b-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-118">用于 CRM Basic (合格产品/) 服务的 SA 的 Dynamics 365 for Sales Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="5228b-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5228b-119">适用于适用于 CRM 的 SA 的 Dynamics 365 for Sales Enterprise Edition (合格的产品/服务) 学生</span><span class="sxs-lookup"><span data-stu-id="5228b-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5228b-120">适用于 Sales Enterprise Edition 的 Dynamics 365 (政府定价) ，适用于 CRM 基本 (合格产品/服务) </span><span class="sxs-lookup"><span data-stu-id="5228b-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (符合条件的产品/) </span><span class="sxs-lookup"><span data-stu-id="5228b-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (符合条件的产品/) 教职员工</span><span class="sxs-lookup"><span data-stu-id="5228b-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5228b-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (符合条件的产品/) 学生版</span><span class="sxs-lookup"><span data-stu-id="5228b-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5228b-124">DYNAMICs 365 for Sales Enterprise Edition (政府定价) Add-On CRM Basic (符合条件的产品/) </span><span class="sxs-lookup"><span data-stu-id="5228b-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-125">Dynamics 365 客户参与计划Enterprise Edition CRMOL Basic (符合条件的套餐) </span><span class="sxs-lookup"><span data-stu-id="5228b-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-126">Dynamics 365 客户参与计划Enterprise Edition (政府定价) CRMOL Basic (符合条件的套餐) </span><span class="sxs-lookup"><span data-stu-id="5228b-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-127">Dynamics 365 客户参与计划 Enterprise Edition CRMOL Basic (学生) 符合条件的产品/服务</span><span class="sxs-lookup"><span data-stu-id="5228b-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5228b-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for 教职员工</span><span class="sxs-lookup"><span data-stu-id="5228b-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5228b-129">Dynamics 365 客户参与计划 Enterprise Edition SA for CRM Basic (符合条件的产品/服务) </span><span class="sxs-lookup"><span data-stu-id="5228b-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-130">Dynamics 365 客户参与计划Enterprise Edition (政府定价) 来自 SA for CRM Basic (符合条件的套餐) </span><span class="sxs-lookup"><span data-stu-id="5228b-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="5228b-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5228b-132">Dynamics 365 客户参与计划 Enterprise Edition SA for CRM Basic (符合条件的产品/服务) 教职员工</span><span class="sxs-lookup"><span data-stu-id="5228b-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="5228b-133">Dynamics 365 客户参与计划Enterprise Edition Add-On CRM Basic (符合条件的套餐) </span><span class="sxs-lookup"><span data-stu-id="5228b-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-134">Dynamics 365 客户参与计划Enterprise Edition (CRM Basic) Add-On符合条件的产品/服务 (政府定价) </span><span class="sxs-lookup"><span data-stu-id="5228b-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="5228b-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="5228b-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="5228b-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="5228b-137">Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offers) 替换计划</span><span class="sxs-lookup"><span data-stu-id="5228b-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="5228b-138">**已停用的优惠**</span><span class="sxs-lookup"><span data-stu-id="5228b-138">**Retired offers**</span></span>   

- <span data-ttu-id="5228b-139">CRM Basic 或 CRMOL Basic 中的 Dynamics 365 for Sales (符合条件的产品/服务) </span><span class="sxs-lookup"><span data-stu-id="5228b-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="5228b-140">CRM Basic 或 CRMOL Basic 中的 Dynamics 365 客户参与计划 (符合条件的套餐) </span><span class="sxs-lookup"><span data-stu-id="5228b-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="5228b-141">**替换选项**</span><span class="sxs-lookup"><span data-stu-id="5228b-141">**Replacement options**</span></span>
- <span data-ttu-id="5228b-142">Dynamics 365 for Sales Professional (NEW) </span><span class="sxs-lookup"><span data-stu-id="5228b-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="5228b-143">Dynamics 365 for Sales Professional (NEW) </span><span class="sxs-lookup"><span data-stu-id="5228b-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="5228b-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="5228b-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="5228b-145">Dynamics 365 客户参与计划或</span><span class="sxs-lookup"><span data-stu-id="5228b-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="5228b-146">Dynamics 365 团队成员</span><span class="sxs-lookup"><span data-stu-id="5228b-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5228b-147">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="5228b-147">Transition customers to new product plans</span></span>

<span data-ttu-id="5228b-148">将客户从已停用的 SKUS 迁移到较新的 SKUS 需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="5228b-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="5228b-149">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="5228b-149">Purchase the new subscription</span></span>
- <span data-ttu-id="5228b-150">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="5228b-150">Reassign current user licenses</span></span>
- <span data-ttu-id="5228b-151">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="5228b-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="5228b-152">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="5228b-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="5228b-153">从 **左侧** 导航中选择"客户"，然后选择要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="5228b-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="5228b-154">选择"**添加订阅"。**</span><span class="sxs-lookup"><span data-stu-id="5228b-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="5228b-155">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。</span><span class="sxs-lookup"><span data-stu-id="5228b-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="5228b-156">现在，你的客户将同时拥有旧订阅和新订阅。</span><span class="sxs-lookup"><span data-stu-id="5228b-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="5228b-157">下一步是为客户的用户重新分配许可证。</span><span class="sxs-lookup"><span data-stu-id="5228b-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="5228b-158">从 **左侧** 导航中选择"客户"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="5228b-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="5228b-159">选择 **"用户和许可证"。**</span><span class="sxs-lookup"><span data-stu-id="5228b-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="5228b-160">若要向用户重新分配许可证，请选择该用户，然后选择"**管理许可证"。**</span><span class="sxs-lookup"><span data-stu-id="5228b-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="5228b-161">在"管理许可证"页上，清除"基本 (合格产品/服务) 许可证"复选框中的"Dynamics 365 for Sales/Customer Engagement 计划"复选框，并选择客户要移动到的订阅的新服务计划。</span><span class="sxs-lookup"><span data-stu-id="5228b-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="5228b-162">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="5228b-162">Select **Submit**.</span></span> <span data-ttu-id="5228b-163">你将为需要新许可证的每个用户执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5228b-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="5228b-164">将许可证移到新订阅后，可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="5228b-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="5228b-165">从 **左侧** 导航中选择"客户"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="5228b-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="5228b-166">在订阅详细信息页上，将旧订阅设置为"已挂起 **"，** 然后选择"提交 **"。**</span><span class="sxs-lookup"><span data-stu-id="5228b-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="5228b-167">旧订阅现已暂停，新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="5228b-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="5228b-168">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="5228b-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="5228b-169">对于旧订阅，客户不会产生额外的费用。</span><span class="sxs-lookup"><span data-stu-id="5228b-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



