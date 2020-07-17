---
title: 迁移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将限定的 Dynamics 365 商业版产品/服务迁移到更新的版本，使其过期。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436826"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="1a88c-103">将 Dynamics 365 商业版产品/服务迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="1a88c-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="1a88c-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="1a88c-104">**Applies to**</span></span>

- <span data-ttu-id="1a88c-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1a88c-105">Partner Center</span></span>

<span data-ttu-id="1a88c-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="1a88c-106">**Appropriate roles**</span></span>
- <span data-ttu-id="1a88c-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1a88c-107">Global admin</span></span>
- <span data-ttu-id="1a88c-108">用户管理员</span><span class="sxs-lookup"><span data-stu-id="1a88c-108">User admin</span></span>
- <span data-ttu-id="1a88c-109">管理员代理</span><span class="sxs-lookup"><span data-stu-id="1a88c-109">Admin agent</span></span>
- <span data-ttu-id="1a88c-110">销售代理</span><span class="sxs-lookup"><span data-stu-id="1a88c-110">Sales agent</span></span>

<span data-ttu-id="1a88c-111">2019年1月1日生效，具有 Dynamics 365 Business Edition 订阅的客户不再能够续订这些旧产品/服务。现有订阅将不会在过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="1a88c-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="1a88c-112">在订阅的详细信息页上，订阅状态将更改为 "在 [date] 上自动续订时过期时间为 [日期]"。</span><span class="sxs-lookup"><span data-stu-id="1a88c-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="1a88c-113">若要确保客户的连续性，应将具有过期订阅的人员转换为受支持的选项，如下所示。</span><span class="sxs-lookup"><span data-stu-id="1a88c-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="1a88c-114">建议将客户移动到订阅的每年结束日期之前的新订阅，以避免客户发生服务中断。</span><span class="sxs-lookup"><span data-stu-id="1a88c-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="1a88c-115">如果使用 API （CREST 或合作者中心），可以通过评估订阅的结束日期以及自动续订 = False 属性来找到过期订阅。</span><span class="sxs-lookup"><span data-stu-id="1a88c-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="1a88c-116">相关订阅将在2019年1月1日设置为自动续订 = False。</span><span class="sxs-lookup"><span data-stu-id="1a88c-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="1a88c-117">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="1a88c-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="1a88c-118">要停用的 Dynamics 365 业务版本</span><span class="sxs-lookup"><span data-stu-id="1a88c-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="1a88c-119">Dynamics 365 for Finance and Operations Business Edition</span><span class="sxs-lookup"><span data-stu-id="1a88c-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="1a88c-120">适用于团队成员的 Dynamics 365，商业版</span><span class="sxs-lookup"><span data-stu-id="1a88c-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="1a88c-121">Dynamics Business Central-Dynamics 365 Business Edition 新产品/服务</span><span class="sxs-lookup"><span data-stu-id="1a88c-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="1a88c-122">利用全新的 Dynamics Business Central 产品/服务，你的客户可以连接其财务、销售、服务和操作，以优化业务流程、改善客户交互，并做出更好的决策。</span><span class="sxs-lookup"><span data-stu-id="1a88c-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="1a88c-123">Dynamics 365 Business Central 是基于云的，并且仅可通过云解决方案提供商（CSP）计划合作伙伴获得。</span><span class="sxs-lookup"><span data-stu-id="1a88c-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="1a88c-124">Dynamics 365 Business Edition 客户有资格在2020年6月30日之前获得新的业务中心产品/服务的折扣过渡价格。</span><span class="sxs-lookup"><span data-stu-id="1a88c-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="1a88c-125">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="1a88c-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="1a88c-126">将客户从停用的 Sku 转移到新的 Sku 需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="1a88c-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="1a88c-127">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="1a88c-127">Purchase the new subscription</span></span>
- <span data-ttu-id="1a88c-128">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="1a88c-128">Reassign current user licenses</span></span>
- <span data-ttu-id="1a88c-129">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="1a88c-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="1a88c-130">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="1a88c-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="1a88c-131">从左侧导航栏中选择 "**客户**"，并选择要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="1a88c-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="1a88c-132">选择 "**添加订阅**"。</span><span class="sxs-lookup"><span data-stu-id="1a88c-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="1a88c-133">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="1a88c-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="1a88c-134">你的客户现在将具有旧订阅和新订阅。</span><span class="sxs-lookup"><span data-stu-id="1a88c-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="1a88c-135">下一步是向客户的用户重新分配许可证。</span><span class="sxs-lookup"><span data-stu-id="1a88c-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="1a88c-136">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="1a88c-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="1a88c-137">选择 "**用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="1a88c-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="1a88c-138">若要为用户重新分配许可证，请选择该用户，然后选择 "**管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="1a88c-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="1a88c-139">在 "**管理许可证**" 页上，清除 "基本（合格产品/服务）许可证的 Dynamics 365 for Sales/Customer Engagement 计划" 复选框，并为客户要移到的订阅选择新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="1a88c-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="1a88c-140">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="1a88c-140">Select **Submit**.</span></span> <span data-ttu-id="1a88c-141">你将对需要新许可证的每个用户执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1a88c-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="1a88c-142">将许可证转移到新订阅后，可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="1a88c-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="1a88c-143">从左侧导航栏中选择 "**客户**"，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="1a88c-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="1a88c-144">在 "订阅详细信息" 页上，将旧订阅设置为 "**挂起**"，然后选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="1a88c-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="1a88c-145">旧订阅现已暂停，新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="1a88c-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="1a88c-146">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="1a88c-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="1a88c-147">你的客户不会对旧订阅产生额外的费用。</span><span class="sxs-lookup"><span data-stu-id="1a88c-147">Your customer will incur no additional costs for the old subscription.</span></span>
