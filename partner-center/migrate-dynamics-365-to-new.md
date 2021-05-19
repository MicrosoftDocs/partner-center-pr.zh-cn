---
title: 迁移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在符合条件的 Dynamics 365 Business Edition 产品/服务过期之前将其迁移到较新版本。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151519"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="89405-103">将 Dynamics 365 商业版产品/服务迁移到较新版本</span><span class="sxs-lookup"><span data-stu-id="89405-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="89405-104">**适当的角色**：全局管理员|用户管理管理员|管理代理|销售代理</span><span class="sxs-lookup"><span data-stu-id="89405-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="89405-105">自 2019 年 1 月 1 日起，具有 Dynamics 365 Business Edition 订阅的客户无法再续订这些旧版产品/服务;现有订阅过期时不会自动续订。</span><span class="sxs-lookup"><span data-stu-id="89405-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="89405-106">在订阅的详细信息页上，订阅状态从"[日期]自动续订"更改为"[date]过期"。</span><span class="sxs-lookup"><span data-stu-id="89405-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="89405-107">为了确保客户的连续性，应该将即将过期的订阅转换为下面列出的受支持选项。</span><span class="sxs-lookup"><span data-stu-id="89405-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="89405-108">我们建议在订阅的每年结束日期之前将客户移动到新订阅，以避免客户发生任何服务中断。</span><span class="sxs-lookup"><span data-stu-id="89405-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="89405-109">如果使用 CREST (或 合作伙伴中心) API，则可以通过评估订阅的结束日期以及自动续订 = False 属性来查找即将过期的订阅。</span><span class="sxs-lookup"><span data-stu-id="89405-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="89405-110">有关订阅将在 2019 年 1 月 1 日设置为 auto renew=False。</span><span class="sxs-lookup"><span data-stu-id="89405-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="89405-111">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="89405-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="89405-112">即将停用的 Dynamics 365 商业版</span><span class="sxs-lookup"><span data-stu-id="89405-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="89405-113">Dynamics 365 for Finance and Operations Business Edition</span><span class="sxs-lookup"><span data-stu-id="89405-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="89405-114">适用于团队成员的 Dynamics 365，商业版</span><span class="sxs-lookup"><span data-stu-id="89405-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="89405-115">Dynamics Business Central - Dynamics 365 Business Edition 新产品/服务</span><span class="sxs-lookup"><span data-stu-id="89405-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="89405-116">借助新的 Dynamics Business Central 产品/服务，客户可以连接其财务、销售、服务和操作，以简化业务流程、改善客户交互并做出更好的决策。</span><span class="sxs-lookup"><span data-stu-id="89405-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="89405-117">Dynamics 365 Business Central 基于云的，仅通过云解决方案云解决方案提供商 (CSP) 合作伙伴提供。</span><span class="sxs-lookup"><span data-stu-id="89405-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="89405-118">在 2020 年 6 月 30 日之前，Dynamics 365 Business Edition 客户有资格享受新的 Business Central 产品/服务的折扣转换定价。</span><span class="sxs-lookup"><span data-stu-id="89405-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="89405-119">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="89405-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="89405-120">将客户从已停用的 SKUS 迁移到较新的 SKUS 需要按以下顺序执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="89405-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="89405-121">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="89405-121">Purchase the new subscription</span></span>
- <span data-ttu-id="89405-122">重新分配当前用户许可证</span><span class="sxs-lookup"><span data-stu-id="89405-122">Reassign current user licenses</span></span>
- <span data-ttu-id="89405-123">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="89405-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="89405-124">为客户购买新计划</span><span class="sxs-lookup"><span data-stu-id="89405-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="89405-125">从 **左侧** 导航中选择"客户"，然后选择要移动到新订阅的客户。</span><span class="sxs-lookup"><span data-stu-id="89405-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="89405-126">选择"**添加订阅"。**</span><span class="sxs-lookup"><span data-stu-id="89405-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="89405-127">从目录中选择要购买的订阅（在此情况下是以上选项之一）、输入许可证数，然后选择 **提交**。</span><span class="sxs-lookup"><span data-stu-id="89405-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="89405-128">你的客户现在将具有旧订阅和新订阅。</span><span class="sxs-lookup"><span data-stu-id="89405-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="89405-129">下一步是向客户的用户重新分配许可证。</span><span class="sxs-lookup"><span data-stu-id="89405-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="89405-130">从左侧导航栏中选择 " **客户** "，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="89405-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="89405-131">选择 " **用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="89405-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="89405-132">若要为用户重新分配许可证，请选择该用户，然后选择 " **管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="89405-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="89405-133">在 " **管理许可证** " 页上，清除 "基本 (合格产品/服务) 许可证" 复选框中的 "Dynamics 365 for Sales/Customer Engagement 计划"，然后为客户要移到的订阅选择新的服务计划。</span><span class="sxs-lookup"><span data-stu-id="89405-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="89405-134">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="89405-134">Select **Submit**.</span></span> <span data-ttu-id="89405-135">你将对需要新许可证的每个用户执行此操作。</span><span class="sxs-lookup"><span data-stu-id="89405-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="89405-136">将许可证移至新订阅后，可以取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="89405-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="89405-137">从左侧导航栏中选择 " **客户** "，然后选择要移动的客户。</span><span class="sxs-lookup"><span data-stu-id="89405-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="89405-138">在 "订阅详细信息" 页上，将旧订阅设置为 " **挂起** "，然后选择 " **提交**"。</span><span class="sxs-lookup"><span data-stu-id="89405-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="89405-139">旧订阅现已暂停，新订阅处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="89405-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="89405-140">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="89405-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="89405-141">你的客户不会对旧订阅产生额外的费用。</span><span class="sxs-lookup"><span data-stu-id="89405-141">Your customer will incur no additional costs for the old subscription.</span></span>
