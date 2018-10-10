---
title: 将 Dynamics AX 订阅迁移到 Dynamics 365 | 合作伙伴中心
description: Microsoft 引入了 Dynamics 365，这是下一代智能业务应用程序，可使组织成长、发展和转型，满足客户需求并抓住新机遇。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: f5e03825226171b8002b260e1b00a59a5eb53ebb
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489783"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a><span data-ttu-id="e33c9-103">将 Dynamics AX 订阅迁移到 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e33c9-103">Migrate Dynamics AX subscriptions to Dynamics 365</span></span>

**<span data-ttu-id="e33c9-104">适用于</span><span class="sxs-lookup"><span data-stu-id="e33c9-104">Applies to</span></span>**

-  <span data-ttu-id="e33c9-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="e33c9-105">Partner Center</span></span>

<span data-ttu-id="e33c9-106">Microsoft 引入了 Dynamics 365，这是下一代智能业务应用程序，可使组织成长、发展和转型，满足客户需求并抓住新机遇。</span><span class="sxs-lookup"><span data-stu-id="e33c9-106">Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.</span></span> <span data-ttu-id="e33c9-107">作为新产品的一部分，Microsoft 在 2016 年 11 月 1 日为客户引进了新 Microsoft Dynamics 订阅计划，该计划与当前计划类似但不相同。</span><span class="sxs-lookup"><span data-stu-id="e33c9-107">As part of the new product, Microsoft introduced new Microsoft Dynamics subscription plans for customers on November 1st, 2016, that are similar but not identical to your current plans.</span></span>

<span data-ttu-id="e33c9-108">本文档中的说明介绍了间接提供商如何将客户的现有 Microsoft Dynamics AX 订阅和 Microsoft Dymanics CRM Online 订阅转换为 Microsoft Dynamics 365。</span><span class="sxs-lookup"><span data-stu-id="e33c9-108">The instructions in this document describe how indirect providers can switch customers’ existing Microsoft Dynamics AX subscriptions and Microsoft Dymanics CRM Online subscriptions to Microsoft Dynamics 365.</span></span> <span data-ttu-id="e33c9-109">这些说明也适用于其他更新到新版本的 Microsoft 产品，需要提供商将客户订阅迁移到新 SKU。</span><span class="sxs-lookup"><span data-stu-id="e33c9-109">The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.</span></span>

<span data-ttu-id="e33c9-110">Microsoft Dynamics CRM Online 和 AX 计划已停用。</span><span class="sxs-lookup"><span data-stu-id="e33c9-110">The Microsoft Dynamics CRM Online and AX plans are retired.</span></span>  <span data-ttu-id="e33c9-111">2017 年 7 月 1 日生效，你可以不再续订这些旧计划，此外，现有 E4 订阅在到期时将不会自动续订。</span><span class="sxs-lookup"><span data-stu-id="e33c9-111">Effective July 1, 2017, you can no longer renew into the legacy plans, also existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="e33c9-112">当 CRM Online 和 AX 订阅结束时，它们将会被取消。</span><span class="sxs-lookup"><span data-stu-id="e33c9-112">When CRM Online and AX subscriptions end, they will be canceled.</span></span> <span data-ttu-id="e33c9-113">为确保客户服务连续性，将具有即将到期订阅的客户过渡到下列支持的 SKU 选项。</span><span class="sxs-lookup"><span data-stu-id="e33c9-113">To ensure continuity for customers, plan to transition customers with expiring subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="e33c9-114">建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。</span><span class="sxs-lookup"><span data-stu-id="e33c9-114">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span> 

<span data-ttu-id="e33c9-115">在订阅详细信息页面上，即将到期的订阅的状态会从“[日期] 自动续订”更改为“[日期] 过期”。</span><span class="sxs-lookup"><span data-stu-id="e33c9-115">On the subscription's detail page, you will see that for these expiring subscriptions, the subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="e33c9-116">如果你使用 API（CREST 或合作伙伴中心），则可以通过评估订阅的结束日期以及“自动续订 = False”属性来发现即将到期的订阅。2017 年 7 月 1 日，这些订阅已被设置为“自动续订 = False”。</span><span class="sxs-lookup"><span data-stu-id="e33c9-116">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.The subscriptions were set to auto renew=False on July 1, 2017.</span></span> <span data-ttu-id="e33c9-117">你可以随时将客户移到新计划中。</span><span class="sxs-lookup"><span data-stu-id="e33c9-117">You can move customers to a new plan at any time.</span></span> 

**<span data-ttu-id="e33c9-118">Microsoft Dynamics AX 授权更改</span><span class="sxs-lookup"><span data-stu-id="e33c9-118">Microsoft Dynamics AX licensing changes</span></span>**

<span data-ttu-id="e33c9-119">Microsoft Dynamics AX 产品线于 2016 年 11 月 1 日停用。</span><span class="sxs-lookup"><span data-stu-id="e33c9-119">The Microsoft Dynamics AX product line was retired, effective November 1st, 2016.</span></span> <span data-ttu-id="e33c9-120">若要了解关于 Dynamics 365 的新授权选项的更多信息，请参阅[授权指南](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)。</span><span class="sxs-lookup"><span data-stu-id="e33c9-120">To learn more about the new licensing options for Dynamics 365, review the [Licensing Guide](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).</span></span>

 <span data-ttu-id="e33c9-121">请参考下表，了解关于许可证映射的详细信息：</span><span class="sxs-lookup"><span data-stu-id="e33c9-121">Refer to the following table for details on license mapping:</span></span>

|**<span data-ttu-id="e33c9-122">已停用的 SKU</span><span class="sxs-lookup"><span data-stu-id="e33c9-122">Retired SKU</span></span>**   |**<span data-ttu-id="e33c9-123">Dynamics 365 SKU</span><span class="sxs-lookup"><span data-stu-id="e33c9-123">Dynamics 365 SKU</span></span>**   |
|-------------------|:----------------------|
|<span data-ttu-id="e33c9-124">企业版 SKU</span><span class="sxs-lookup"><span data-stu-id="e33c9-124">Enterprise SKU</span></span>|<span data-ttu-id="e33c9-125">针对 Unified Operations 或 Microsoft Dynamics 365 计划的 Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e33c9-125">Microsoft Dynamics 365 for Unified Operations or Microsoft Dynamics 365 Plan</span></span> |
|<span data-ttu-id="e33c9-126">任务</span><span class="sxs-lookup"><span data-stu-id="e33c9-126">Task</span></span>|<span data-ttu-id="e33c9-127">Microsoft Dynamics 365 for Activity</span><span class="sxs-lookup"><span data-stu-id="e33c9-127">Microsoft Dynamics 365 for Activity</span></span>
|<span data-ttu-id="e33c9-128">任务/自助服务</span><span class="sxs-lookup"><span data-stu-id="e33c9-128">Task/self service</span></span>|<span data-ttu-id="e33c9-129">Microsoft Dynamics 365 for Team Members</span><span class="sxs-lookup"><span data-stu-id="e33c9-129">Microsoft Dynamics 365 for Team Members</span></span>|
|<span data-ttu-id="e33c9-130">设备</span><span class="sxs-lookup"><span data-stu-id="e33c9-130">Device</span></span>|<span data-ttu-id="e33c9-131">Microsoft Dynamics 365 for Operations Device</span><span class="sxs-lookup"><span data-stu-id="e33c9-131">Microsoft Dynamics 365 for Operations Device</span></span>|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a><span data-ttu-id="e33c9-132">Microsoft Dynamics CRM Online 授权更改</span><span class="sxs-lookup"><span data-stu-id="e33c9-132">Microsoft Dynamics CRM Online licensing changes</span></span> 

**<span data-ttu-id="e33c9-133">Microsoft Dynamics CRM Online</span><span class="sxs-lookup"><span data-stu-id="e33c9-133">Microsoft Dynamics CRM Online</span></span>**

<span data-ttu-id="e33c9-134">当前的 Microsoft Dynamics CRM Online 计划于 2016 年 11 月 1 日停用</span><span class="sxs-lookup"><span data-stu-id="e33c9-134">The current Microsoft Dynamics CRM Online plan was retired effective November 1, 2016.</span></span> <span data-ttu-id="e33c9-135">若要了解关于 microsoft Dynaics 365 的新授权选项的更多信息，请参阅[授权指南](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)。</span><span class="sxs-lookup"><span data-stu-id="e33c9-135">To learn more about the new licensing options for microsoft Dynaics 365, review the [licensing guide](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).</span></span> <span data-ttu-id="e33c9-136">若要了解有关新授权选项的详细信息，请参阅[面向 CRM Online 客户的重要信息](https://go.microsoft.com/fwlink/?linkid=831667)。</span><span class="sxs-lookup"><span data-stu-id="e33c9-136">See [Important information for CRM Online customers](https://go.microsoft.com/fwlink/?linkid=831667) to find out more about new licensing options.</span></span>

<span data-ttu-id="e33c9-137">请参考下表，了解关于许可证映射的详细信息：</span><span class="sxs-lookup"><span data-stu-id="e33c9-137">Refer to the following table for details on license mapping:</span></span>

|**<span data-ttu-id="e33c9-138">已停用的 SKU</span><span class="sxs-lookup"><span data-stu-id="e33c9-138">Retired SKU</span></span>**   |**<span data-ttu-id="e33c9-139">Dynamics 365 SKU</span><span class="sxs-lookup"><span data-stu-id="e33c9-139">Dynamics 365 SKU</span></span>**   |
|-------------------|:----------------------|
|<span data-ttu-id="e33c9-140">Enterprise</span><span class="sxs-lookup"><span data-stu-id="e33c9-140">Enterprise</span></span>|<span data-ttu-id="e33c9-141">Dynamics 365 企业客户参与度计划</span><span class="sxs-lookup"><span data-stu-id="e33c9-141">Dynamics 365 Enterprise Customer Engagement Plan</span></span> |
|<span data-ttu-id="e33c9-142">Professional</span><span class="sxs-lookup"><span data-stu-id="e33c9-142">Professional</span></span>|<span data-ttu-id="e33c9-143">Dynamics 365 企业客户参与度计划计划、Dynamics 365 for Sales 或 Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="e33c9-143">Dynamics 365 Enterprise Customer Engagement Plan, Dynamics 365 for Sales, or Dynamics 365 for Customer Service</span></span>|
|<span data-ttu-id="e33c9-144">Basic</span><span class="sxs-lookup"><span data-stu-id="e33c9-144">Basic</span></span>|<span data-ttu-id="e33c9-145">Dynamics 365 for Team Members、Dynamics 365 for Sales、Dynamics 365 for Customer Service 或 Dynamics 365 企业客户参与度计划</span><span class="sxs-lookup"><span data-stu-id="e33c9-145">Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service, or Dynamics 365 Enterprise Customer Engagement Plan</span></span>|
|<span data-ttu-id="e33c9-146">Essential</span><span class="sxs-lookup"><span data-stu-id="e33c9-146">Essential</span></span>|<span data-ttu-id="e33c9-147">Dynamics 365 for Team Members</span><span class="sxs-lookup"><span data-stu-id="e33c9-147">Dynamics 365 for Team Members</span></span>|
|<span data-ttu-id="e33c9-148">现场服务加载项</span><span class="sxs-lookup"><span data-stu-id="e33c9-148">Field service add-on</span></span>|<span data-ttu-id="e33c9-149">Dynamics 365 企业客户参与度计划或 Dynamics 365 for Field Service</span><span class="sxs-lookup"><span data-stu-id="e33c9-149">Dynamics 365 Enterprise Customer Engagement Plan or Dynamics 365 for Field Service</span></span>|
|<span data-ttu-id="e33c9-150">项目服务自动化加载项</span><span class="sxs-lookup"><span data-stu-id="e33c9-150">Project Service Authomation Add-on</span></span>|<span data-ttu-id="e33c9-151">Dynamics 365 企业客户参与度计划或 Dynamics 365 for Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="e33c9-151">Dynamics 365 Customer Engagement Plan or Dynamics 365 for Project Service Automation</span></span>|



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="e33c9-152">将客户过渡到新产品计划</span><span class="sxs-lookup"><span data-stu-id="e33c9-152">Transition customers to new product plans</span></span>


<span data-ttu-id="e33c9-153">Microsoft 不断向经销商和提供商提供新产品和服务。</span><span class="sxs-lookup"><span data-stu-id="e33c9-153">Microsoft continuously offers new products and services to resellers and providers.</span></span> <span data-ttu-id="e33c9-154">在这些情况下，经销商可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。</span><span class="sxs-lookup"><span data-stu-id="e33c9-154">In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="e33c9-155">将客户从旧 SKU 中迁移到新 SKU 需要按照以下顺序操作：</span><span class="sxs-lookup"><span data-stu-id="e33c9-155">Migrating customers from old SKUs to newer ones requires the following sequence:</span></span>

-   <span data-ttu-id="e33c9-156">[购买新订阅](#manual-subscription-migration-purchasenewsubsc)；</span><span class="sxs-lookup"><span data-stu-id="e33c9-156">[Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);</span></span>
-   <span data-ttu-id="e33c9-157">[重新分配当前用户许可证](#manual-subscription-migration-reassignlicenses)；</span><span class="sxs-lookup"><span data-stu-id="e33c9-157">[Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);</span></span>
-   <span data-ttu-id="e33c9-158">[取消旧订阅](#manual-subscription-migration-cancelsubscriptions)。</span><span class="sxs-lookup"><span data-stu-id="e33c9-158">[Cancel the old subscription](#manual-subscription-migration-cancelsubscriptions).</span></span>

<span data-ttu-id="e33c9-159">以下过程将客户从 Microsoft Dynamics AX 或 CRM Online 移动到 Dynamics 365。</span><span class="sxs-lookup"><span data-stu-id="e33c9-159">In the following procedures, you move a customer from Microsoft Dynamics AX or CRM Online to Dynamics 365.</span></span>

<span data-ttu-id="e33c9-160">在该示例中，经销商需要将具有现有 Dynamics AX Enterprise 订阅的客户移至 Dynamics 365 for Operations。</span><span class="sxs-lookup"><span data-stu-id="e33c9-160">In this example, the reseller needs to move a customer with an existing subscription for Dynamics AX Enterprise to Dynamics 365 for Operations.</span></span> <span data-ttu-id="e33c9-161">第一步是购买 Dynamics 365 for Operations。</span><span class="sxs-lookup"><span data-stu-id="e33c9-161">Your first step is to purchase Dynamics 365 for Operations.</span></span>  <span data-ttu-id="e33c9-162">对于将移至 Microsoft Dynamics 365 的 CRM Online 客户，重复这些步骤。</span><span class="sxs-lookup"><span data-stu-id="e33c9-162">Repeat these steps for a CRM Online customer moving to Microsoft Dynamics 365.</span></span>

<a href="" id="purchasenewsubsc"></a>

**<span data-ttu-id="e33c9-163">购买新订阅</span><span class="sxs-lookup"><span data-stu-id="e33c9-163">Purchase the new subscription</span></span>**

1.  <span data-ttu-id="e33c9-164">从**合作伙伴中心**菜单中，选择**客户**、 选择你想要移动的客户，选择**添加订阅**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-164">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.</span></span>
2.  <span data-ttu-id="e33c9-165">选择要从目录中购买的订阅（在此情况下是 Dynamics 365 for Operations 企业版）、输入许可证编号，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-165">Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.</span></span>

    <span data-ttu-id="e33c9-166">此时客户应该具有新旧两个订阅：在此示例中是旧的 Dynamics AX Enterprise 和新的“目标”订阅，即 Dynamics 365 for Operations 企业版。</span><span class="sxs-lookup"><span data-stu-id="e33c9-166">Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.</span></span>

<a href="" id="reassignlicenses"></a><span data-ttu-id="e33c9-167">下一步是将所有现有用户许可证重新分配到新订阅。</span><span class="sxs-lookup"><span data-stu-id="e33c9-167">The next step is to reassign all existing user licenses to the new subscription.</span></span>

**<span data-ttu-id="e33c9-168">重新分配用户许可证</span><span class="sxs-lookup"><span data-stu-id="e33c9-168">Reassign user licenses</span></span>**

1.  <span data-ttu-id="e33c9-169">从**合作伙伴中心**菜单中，选择**客户**，选择你想要移动的客户然后选择**用户和许可证**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-169">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**.</span></span> <span data-ttu-id="e33c9-170">将打开客户的“用户和许可证”页。</span><span class="sxs-lookup"><span data-stu-id="e33c9-170">The customer’s Users and Licenses page opens.</span></span>
2.  <span data-ttu-id="e33c9-171">若要重新分配用户许可证，选择要重新分配的用户，然后选择**管理许可证**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-171">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>
3.  <span data-ttu-id="e33c9-172">在**管理许可证**页上，清除 **Dynamics AX Enterprise** 许可证复选框，然后选择 **Dynamics 365 for Operations** 许可证。</span><span class="sxs-lookup"><span data-stu-id="e33c9-172">On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.</span></span>
4.  <span data-ttu-id="e33c9-173">选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-173">Select **Submit**.</span></span> <span data-ttu-id="e33c9-174">确认页面列出了新的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="e33c9-174">A confirmation page lists the new license assignments.</span></span>
5.  <span data-ttu-id="e33c9-175">对其他任何需要重新分配许可证的客户用户继续执行相同的步骤。</span><span class="sxs-lookup"><span data-stu-id="e33c9-175">Continue the same steps with any other customer users that need license reassignment.</span></span>

<a href="" id="cancelsubscriptions"></a><span data-ttu-id="e33c9-176">在将用户许可证移动至新服务后，可安全取消最高“客户”级别的旧订阅。</span><span class="sxs-lookup"><span data-stu-id="e33c9-176">After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.</span></span>

**<span data-ttu-id="e33c9-177">取消旧订阅</span><span class="sxs-lookup"><span data-stu-id="e33c9-177">Cancel the old subscription</span></span>**

1.  <span data-ttu-id="e33c9-178">从**合作伙伴中心**菜单中，选择**客户**、 选择你想要移动的客户并选择你想要取消的订阅。</span><span class="sxs-lookup"><span data-stu-id="e33c9-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.</span></span>
2.  <span data-ttu-id="e33c9-179">在订阅详细信息页面中，将订阅**状态**设置为**已暂停**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-179">In the subscription details page, set the subscription **Status** to **Suspended**.</span></span>
3.  <span data-ttu-id="e33c9-180">选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="e33c9-180">Select **Submit**.</span></span>

<span data-ttu-id="e33c9-181">旧订阅已暂停，新订阅将激活。</span><span class="sxs-lookup"><span data-stu-id="e33c9-181">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="e33c9-182">暂停的订阅在 120 天后将自动取消预配。</span><span class="sxs-lookup"><span data-stu-id="e33c9-182">The suspended subscription will automatically be de-provisioned after 120 days.</span></span> <span data-ttu-id="e33c9-183">不会向客户收取旧订阅的任何额外成本。</span><span class="sxs-lookup"><span data-stu-id="e33c9-183">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="additional-considerations"></a><span data-ttu-id="e33c9-184">其他注意事项</span><span class="sxs-lookup"><span data-stu-id="e33c9-184">Additional considerations</span></span>


<span data-ttu-id="e33c9-185">如果客户从“开放渠道”移动至“云服务计划”以进一步预配订阅，还需要迁移他们的现有订阅：</span><span class="sxs-lookup"><span data-stu-id="e33c9-185">If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:</span></span>

-   <span data-ttu-id="e33c9-186">如果客户通过“开放渠道”接收旧订阅，可直接移动到新 SKU 上的云解决方案提供商。</span><span class="sxs-lookup"><span data-stu-id="e33c9-186">If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.</span></span>
-   <span data-ttu-id="e33c9-187">如果客户尚未成为你的客户，可向他们发出邀请。</span><span class="sxs-lookup"><span data-stu-id="e33c9-187">If the customer is not yet established as your customer, you can invite them.</span></span> <span data-ttu-id="e33c9-188">有关信息，请参阅[请求与客户建立关系](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx)帮助主题。</span><span class="sxs-lookup"><span data-stu-id="e33c9-188">For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.</span></span>

<span data-ttu-id="e33c9-189">在客户接受你成为他们的间接提供商后，预配步骤与上述步骤大致相同：购买新订阅，然后分配用户许可证。</span><span class="sxs-lookup"><span data-stu-id="e33c9-189">After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses.</span></span> <span data-ttu-id="e33c9-190">唯一的区域是取消旧订阅。</span><span class="sxs-lookup"><span data-stu-id="e33c9-190">The only difference involves cancellation of old subscription(s).</span></span> <span data-ttu-id="e33c9-191">新提供商无法暂停/取消通过其他渠道获取的订阅。</span><span class="sxs-lookup"><span data-stu-id="e33c9-191">A new provider cannot cancel suspend/cancel subscriptions acquired via other channels.</span></span> <span data-ttu-id="e33c9-192">如果客户在其他销售渠道（例如开放渠道）获取了以前的订阅，需要通过该渠道自行取消。</span><span class="sxs-lookup"><span data-stu-id="e33c9-192">If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.</span></span>

 

 



