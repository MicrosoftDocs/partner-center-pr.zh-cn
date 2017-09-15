---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="18972-103">CSP regional authorization tenant consolidation</span><span class="sxs-lookup"><span data-stu-id="18972-103">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="18972-104">Applies to</span><span class="sxs-lookup"><span data-stu-id="18972-104">Applies to</span></span>**

-  <span data-ttu-id="18972-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="18972-105">Partner Center</span></span>
-  <span data-ttu-id="18972-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="18972-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="18972-107">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="18972-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="18972-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span><span class="sxs-lookup"><span data-stu-id="18972-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="18972-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span><span class="sxs-lookup"><span data-stu-id="18972-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="18972-110">Use these instructions to consolidate tenants for different country/regions.</span><span class="sxs-lookup"><span data-stu-id="18972-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="18972-111">**注意** 必须注意在过渡帐户中为客户预配的所有订阅和席位计数。</span><span class="sxs-lookup"><span data-stu-id="18972-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="18972-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span><span class="sxs-lookup"><span data-stu-id="18972-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="18972-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span><span class="sxs-lookup"><span data-stu-id="18972-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="18972-114">Partners choose to consolidate their tenants.</span><span class="sxs-lookup"><span data-stu-id="18972-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="18972-115">Once consolidation is complete, Partners cannot revert to their previous state.</span><span class="sxs-lookup"><span data-stu-id="18972-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="18972-116">Note that customer action is also be required.</span><span class="sxs-lookup"><span data-stu-id="18972-116">Note that customer action is also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="18972-117">Prepare for migration</span><span class="sxs-lookup"><span data-stu-id="18972-117">Prepare for migration</span></span>


-   <span data-ttu-id="18972-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span><span class="sxs-lookup"><span data-stu-id="18972-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="18972-120">Migrate customer accounts</span><span class="sxs-lookup"><span data-stu-id="18972-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="18972-121">使用过渡（新建）帐户登录 <https://partnercenter.microsoft.com>，然后从“合作伙伴中心”仪表板导航至“客户”列表。</span><span class="sxs-lookup"><span data-stu-id="18972-121">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="18972-122">Select Customer.</span><span class="sxs-lookup"><span data-stu-id="18972-122">Select Customer.</span></span>

3.  <span data-ttu-id="18972-123">单击**请求经销商关系**。</span><span class="sxs-lookup"><span data-stu-id="18972-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="18972-124">You are presented with a default email message to present to your customers.</span><span class="sxs-lookup"><span data-stu-id="18972-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="18972-125">This message contains a URL with the org ID unique to your new Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="18972-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="18972-126">**客户操作：**确保想要迁移的所有活动客户均访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="18972-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="18972-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span><span class="sxs-lookup"><span data-stu-id="18972-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="18972-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span><span class="sxs-lookup"><span data-stu-id="18972-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="18972-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span><span class="sxs-lookup"><span data-stu-id="18972-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="18972-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span><span class="sxs-lookup"><span data-stu-id="18972-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="18972-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span><span class="sxs-lookup"><span data-stu-id="18972-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="18972-132">Migrating Office 365 and non-Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="18972-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="18972-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span><span class="sxs-lookup"><span data-stu-id="18972-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="18972-134">在“合作伙伴中心”仪表板上，单击左侧导航中的**客户**</span><span class="sxs-lookup"><span data-stu-id="18972-134">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="18972-135">Open the company name for the customer you want to migrate.</span><span class="sxs-lookup"><span data-stu-id="18972-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="18972-136">单击**添加订阅**。</span><span class="sxs-lookup"><span data-stu-id="18972-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="18972-137">Add the correct subscriptions and seat counts from the catalog.</span><span class="sxs-lookup"><span data-stu-id="18972-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="18972-138">验证在**过渡源**合作伙伴帐户中提供的信息。</span><span class="sxs-lookup"><span data-stu-id="18972-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  <span data-ttu-id="18972-140">单击**提交**。</span><span class="sxs-lookup"><span data-stu-id="18972-140">Click **Submit.**</span></span>

<span data-ttu-id="18972-141">此时，服务将提供给**过渡目标**合作伙伴帐户中的客户。</span><span class="sxs-lookup"><span data-stu-id="18972-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="18972-142">Repeat these steps to migrate subscriptions for all additional customers.</span><span class="sxs-lookup"><span data-stu-id="18972-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="18972-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span><span class="sxs-lookup"><span data-stu-id="18972-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="18972-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="18972-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="18972-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span><span class="sxs-lookup"><span data-stu-id="18972-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="18972-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span><span class="sxs-lookup"><span data-stu-id="18972-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="18972-147">禁用**过渡源**合作伙伴帐户下的云解决方案提供商订阅将阻止以后的任何计费。</span><span class="sxs-lookup"><span data-stu-id="18972-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="18972-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span><span class="sxs-lookup"><span data-stu-id="18972-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="18972-149">使用**过渡源**云解决方案提供商帐户登录 <https://partnercenter.microsoft.com>，然后导航至客户列表。</span><span class="sxs-lookup"><span data-stu-id="18972-149">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="18972-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span><span class="sxs-lookup"><span data-stu-id="18972-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="18972-151">将订阅设置为**已暂停**，然后单击**提交**。</span><span class="sxs-lookup"><span data-stu-id="18972-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="18972-152">**注意** 暂停订阅确保不会重复计费。</span><span class="sxs-lookup"><span data-stu-id="18972-152">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="18972-153">该订阅在订阅列表上显示为**已暂停**。</span><span class="sxs-lookup"><span data-stu-id="18972-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="18972-154">Repeat these steps for all subscriptions under the customer.</span><span class="sxs-lookup"><span data-stu-id="18972-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="18972-155">验证所有订阅是否显示**已暂停**。</span><span class="sxs-lookup"><span data-stu-id="18972-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="18972-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span><span class="sxs-lookup"><span data-stu-id="18972-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="18972-157">Migrating Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="18972-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="18972-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span><span class="sxs-lookup"><span data-stu-id="18972-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="18972-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span><span class="sxs-lookup"><span data-stu-id="18972-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="18972-160">There will be no disruption of service to the customer during this transition.</span><span class="sxs-lookup"><span data-stu-id="18972-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="18972-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span><span class="sxs-lookup"><span data-stu-id="18972-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="18972-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span><span class="sxs-lookup"><span data-stu-id="18972-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="18972-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span><span class="sxs-lookup"><span data-stu-id="18972-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="18972-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="18972-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="18972-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="18972-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="18972-166">**注意** 禁用客户下的订阅不会更改客户在“客户”列表中的外观。</span><span class="sxs-lookup"><span data-stu-id="18972-166">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="18972-167">There is currently no option to remove customers from the list.</span><span class="sxs-lookup"><span data-stu-id="18972-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="18972-168">合作伙伴应避免在以后从**过渡源**帐户中将订阅重新添加到这些客户。</span><span class="sxs-lookup"><span data-stu-id="18972-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="18972-169">为所有客户下的所有订阅重复这些步骤，阻止在以后向**过渡源**帐户收费。</span><span class="sxs-lookup"><span data-stu-id="18972-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="18972-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span><span class="sxs-lookup"><span data-stu-id="18972-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="18972-171">No future invoices will generate after that final billing period.</span><span class="sxs-lookup"><span data-stu-id="18972-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="18972-172">Notes</span><span class="sxs-lookup"><span data-stu-id="18972-172">Notes</span></span>

-   <span data-ttu-id="18972-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span><span class="sxs-lookup"><span data-stu-id="18972-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="18972-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span><span class="sxs-lookup"><span data-stu-id="18972-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="18972-175">There is currently no way to remove a customer from the Customers list completely.</span><span class="sxs-lookup"><span data-stu-id="18972-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="18972-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="18972-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="18972-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span><span class="sxs-lookup"><span data-stu-id="18972-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="18972-178">Simplify migration using Export</span><span class="sxs-lookup"><span data-stu-id="18972-178">Simplify migration using Export</span></span>

<span data-ttu-id="18972-179">使用**导出函数**，捕获要在新合并的结构中使用的订阅：</span><span class="sxs-lookup"><span data-stu-id="18972-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="18972-180">单击“仪表板”上的**客户**，查看现有结构中的客户列表。</span><span class="sxs-lookup"><span data-stu-id="18972-180">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="18972-181">Open the desired customer name.</span><span class="sxs-lookup"><span data-stu-id="18972-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="18972-182">在**订阅**页上，单击**导出订阅**，将订阅的详细信息导出到 Excel 文件。</span><span class="sxs-lookup"><span data-stu-id="18972-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="18972-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span><span class="sxs-lookup"><span data-stu-id="18972-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="18972-184">API registration</span><span class="sxs-lookup"><span data-stu-id="18972-184">API registration</span></span>

<span data-ttu-id="18972-185">有关 API 注册的详细信息，[请参阅此页](https://go.microsoft.com/fwlink/?linkid=847990)。</span><span class="sxs-lookup"><span data-stu-id="18972-185">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="18972-186">Partner Center Activity log</span><span class="sxs-lookup"><span data-stu-id="18972-186">Partner Center Activity log</span></span>


<span data-ttu-id="18972-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span><span class="sxs-lookup"><span data-stu-id="18972-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="18972-188">This helps partners track changes on a customer tenant.</span><span class="sxs-lookup"><span data-stu-id="18972-188">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="18972-189">View the Activity log</span><span class="sxs-lookup"><span data-stu-id="18972-189">View the Activity log</span></span>**

1.  <span data-ttu-id="18972-190">在“合作伙伴中心”仪表板上，单击**活动日志**链接。</span><span class="sxs-lookup"><span data-stu-id="18972-190">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="18972-191">在**活动日志**页上，查看对客户帐户进行的更改。</span><span class="sxs-lookup"><span data-stu-id="18972-191">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="18972-192">若要按日期筛选活动日志，请在日志中选择**开始**和**结束**日期，缩小所选记录的范围。</span><span class="sxs-lookup"><span data-stu-id="18972-192">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="18972-193">若要在**活动日志**中按客户筛选，请使用搜索框。</span><span class="sxs-lookup"><span data-stu-id="18972-193">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="18972-194">Export the Activity log</span><span class="sxs-lookup"><span data-stu-id="18972-194">Export the Activity log</span></span>**

-   <span data-ttu-id="18972-195">单击**导出日志**，将活动日志数据导出为 CSV 文件。</span><span class="sxs-lookup"><span data-stu-id="18972-195">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="18972-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span><span class="sxs-lookup"><span data-stu-id="18972-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



