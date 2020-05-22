---
title: 迁移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将限定的 Dynamics 365 商业版产品/服务迁移到更新的版本，使其过期。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 产品/服务续订优惠，全新 Dynamics 365 Sku
ms.openlocfilehash: d49966db4a2c9de50b0723abf9ccd0fe589a442a
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795970"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="7bbf7-104">将 Dynamics 365 商业版产品/服务迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="7bbf7-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="7bbf7-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="7bbf7-105">**Applies to**</span></span>

- <span data-ttu-id="7bbf7-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="7bbf7-106">Partner Center</span></span>

<span data-ttu-id="7bbf7-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="7bbf7-107">**Appropriate roles**</span></span>
- <span data-ttu-id="7bbf7-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7bbf7-108">Global admin</span></span>
- <span data-ttu-id="7bbf7-109">用户管理员</span><span class="sxs-lookup"><span data-stu-id="7bbf7-109">User admin</span></span>
- <span data-ttu-id="7bbf7-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="7bbf7-110">Admin agent</span></span>
- <span data-ttu-id="7bbf7-111">销售代理</span><span class="sxs-lookup"><span data-stu-id="7bbf7-111">Sales agent</span></span>

<span data-ttu-id="7bbf7-112">2019年1月1日生效，具有 Dynamics 365 Business Edition 订阅的客户不再能够续订这些旧产品/服务。现有订阅将不会在过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="7bbf7-113">在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="7bbf7-114">若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="7bbf7-115">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="7bbf7-116">如果使用 API （CREST 或合作者中心），可以通过评估订阅的结束日期以及自动续订 = False 属性来找到过期订阅。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="7bbf7-117">相关订阅将在2019年1月1日设置为自动续订 = False。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="7bbf7-118">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="7bbf7-119">要停用的 Dynamics 365 业务版本</span><span class="sxs-lookup"><span data-stu-id="7bbf7-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="7bbf7-120">Dynamics 365 for Finance and Operations Business Edition</span><span class="sxs-lookup"><span data-stu-id="7bbf7-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="7bbf7-121">适用于团队成员的 Dynamics 365，商业版</span><span class="sxs-lookup"><span data-stu-id="7bbf7-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="7bbf7-122">Dynamics Business Central-Dynamics 365 Business Edition 新产品/服务</span><span class="sxs-lookup"><span data-stu-id="7bbf7-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="7bbf7-123">利用全新的 Dynamics Business Central 产品/服务，你的客户可以连接其财务、销售、服务和操作，以优化业务流程、改善客户交互，并做出更好的决策。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="7bbf7-124">Dynamics 365 Business Central 是基于云的，并且仅可通过云解决方案提供商（CSP）计划合作伙伴获得。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="7bbf7-125">Dynamics 365 Business Edition 客户有资格在2020年6月30日之前获得新的业务中心产品/服务的折扣过渡价格。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="7bbf7-126">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="7bbf7-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="7bbf7-127">将客户从停用的 Sku 转移到新的 Sku 需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7bbf7-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="7bbf7-128">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="7bbf7-128">Purchase the new subscription</span></span>
- <span data-ttu-id="7bbf7-129">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="7bbf7-129">Reassign current user licenses</span></span>
- <span data-ttu-id="7bbf7-130">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="7bbf7-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="7bbf7-131">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="7bbf7-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="7bbf7-132">从左侧导航栏中选择 "**客户**"，并选择要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="7bbf7-133">选择 "**添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="7bbf7-134">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="7bbf7-135">你的客户现在将具有旧订阅和新订阅。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="7bbf7-136">下一步是向客户的用户重新分配许可证。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="7bbf7-137">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7bbf7-138">选择 "**用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="7bbf7-139">若要为用户重新分配许可证，请选择该用户，然后选择 "**管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="7bbf7-140">在 "**管理许可证**" 页上，清除 "基本（合格产品/服务）许可证的 Dynamics 365 for Sales/Customer Engagement 计划" 复选框，并为客户要移到的订阅选择新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="7bbf7-141">选择“提交”  。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-141">Select **Submit**.</span></span> <span data-ttu-id="7bbf7-142">你将对需要新许可证的每个用户执行此操作。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="7bbf7-143">将许可证转移到新订阅后，可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="7bbf7-144">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7bbf7-145">在 "订阅详细信息" 页上，将旧订阅设置为 "**挂起**"，然后选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="7bbf7-146">旧订阅现已暂停，新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="7bbf7-147">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="7bbf7-148">你的客户不会对旧订阅产生额外的费用。</span><span class="sxs-lookup"><span data-stu-id="7bbf7-148">Your customer will incur no additional costs for the old subscription.</span></span>
