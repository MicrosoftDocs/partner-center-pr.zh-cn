---
title: 云解决方案提供商区域授权租户合并 | 合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
description: 使用这些说明合并不同国家/地区的租户。
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: 迁移客户, 预配, 租户帐户, 合并租户
ms.localizationpriority: medium
ms.openlocfilehash: 183b5f518a57fdaf27badce5927a2ea09a5ec89c
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587550"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="61338-104">云解决方案提供商区域授权租户合并</span><span class="sxs-lookup"><span data-stu-id="61338-104">CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="61338-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="61338-105">**Applies to**</span></span>

-  <span data-ttu-id="61338-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="61338-106">Partner Center</span></span>
-  <span data-ttu-id="61338-107">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="61338-107">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="61338-108">\[有些信息与预发布产品的商业发布之前可能有大幅度修改。</span><span class="sxs-lookup"><span data-stu-id="61338-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="61338-109">Microsoft 不做任何明示或暗示的担保，此处提供的信息。\]</span><span class="sxs-lookup"><span data-stu-id="61338-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="61338-110">使用这些说明合并不同国家/地区的租户。</span><span class="sxs-lookup"><span data-stu-id="61338-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="61338-111">**注意** 必须注意在过渡帐户中为客户预配的所有订阅和席位计数。</span><span class="sxs-lookup"><span data-stu-id="61338-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="61338-112">作为迁移过程的一部分，你将使用新中心云解决方案提供商帐户下的相同席位计数重新预配这些相同的订阅。</span><span class="sxs-lookup"><span data-stu-id="61338-112">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="61338-113">使用导出列表功能，帮助创建移动至集中租户的客户列表。</span><span class="sxs-lookup"><span data-stu-id="61338-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="61338-114">合作伙伴选择合并租户。</span><span class="sxs-lookup"><span data-stu-id="61338-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="61338-115">合并完成后，合作伙伴无法还原为之前的状态。</span><span class="sxs-lookup"><span data-stu-id="61338-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="61338-116">请注意，可能还要求客户进行操作。</span><span class="sxs-lookup"><span data-stu-id="61338-116">Note that customer action may also be required.</span></span>



## <a name="prepare-for-migration"></a><span data-ttu-id="61338-117">准备迁移</span><span class="sxs-lookup"><span data-stu-id="61338-117">Prepare for migration</span></span>


-   <span data-ttu-id="61338-118">登录到您**合作伙伴中心**与**转换**（现有） 帐户 （将转换的一个） 和 take 记下的所有客户并为这些客户的所有服务预配。</span><span class="sxs-lookup"><span data-stu-id="61338-118">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![区域客户列表](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="61338-120">迁移客户帐户</span><span class="sxs-lookup"><span data-stu-id="61338-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="61338-121">登录到您**合作伙伴中心**与**转换**（新） 帐户 （正在转换到的一个） 并导航到 Customers 列表从**客户**。</span><span class="sxs-lookup"><span data-stu-id="61338-121">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="61338-122">选择客户。</span><span class="sxs-lookup"><span data-stu-id="61338-122">Select Customers.</span></span>

3.  <span data-ttu-id="61338-123">单击**请求经销商关系**。</span><span class="sxs-lookup"><span data-stu-id="61338-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="61338-124">系统将显示向客户显示的默认电子邮件消息。</span><span class="sxs-lookup"><span data-stu-id="61338-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="61338-125">此消息包含带有新建合作伙伴中心帐户独有的 org ID 的 URL。</span><span class="sxs-lookup"><span data-stu-id="61338-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="61338-126">**客户的操作：** 请确保每个你想要迁移 active 客户访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="61338-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="61338-127">打开 URL 时，系统将提示客户登录 Office 365 门户。</span><span class="sxs-lookup"><span data-stu-id="61338-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="61338-128">客户使用访问 Azure 和 Office 365 管理员门户所用的同一 Org ID 登录。</span><span class="sxs-lookup"><span data-stu-id="61338-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="61338-129">登录后，系统将提示客户帐户的全局管理员提交协议，以将委派的管理员权限提供给新云解决方案提供商帐户。</span><span class="sxs-lookup"><span data-stu-id="61338-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="61338-130">如果全局管理员同意，客户选中复选框，并同意授权建立这种关系。</span><span class="sxs-lookup"><span data-stu-id="61338-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="61338-131">提交协议后，客户将逐一显示在合作伙伴的客户列表中。</span><span class="sxs-lookup"><span data-stu-id="61338-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="61338-132">迁移 Office 365 和非 Azure 且基于使用情况的订阅</span><span class="sxs-lookup"><span data-stu-id="61338-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="61338-133">客户签署协议后，可在“集中合作伙伴租户”下重新创建他们的订阅。</span><span class="sxs-lookup"><span data-stu-id="61338-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="61338-134">从**合作伙伴中心**选择**客户**。</span><span class="sxs-lookup"><span data-stu-id="61338-134">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="61338-135">打开要迁移的客户的公司名称。</span><span class="sxs-lookup"><span data-stu-id="61338-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="61338-136">单击**添加订阅**。</span><span class="sxs-lookup"><span data-stu-id="61338-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="61338-137">在目录中添加正确的订阅和席位计数。</span><span class="sxs-lookup"><span data-stu-id="61338-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="61338-138">验证在“过渡源”合作伙伴帐户中提供的信息。</span><span class="sxs-lookup"><span data-stu-id="61338-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

![客户列表](images/regionalcustomer2.png)

6.  <span data-ttu-id="61338-140">单击“提交”。</span><span class="sxs-lookup"><span data-stu-id="61338-140">Click **Submit.**</span></span>

<span data-ttu-id="61338-141">此时，服务将提供给“过渡目标”合作伙伴帐户中的客户。</span><span class="sxs-lookup"><span data-stu-id="61338-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="61338-142">重复这些步骤，迁移所有其他客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="61338-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="61338-143">确保“过渡源”合作伙伴帐户下的所有客户订阅已重新预配在“过渡目标”合作伙伴帐户下。</span><span class="sxs-lookup"><span data-stu-id="61338-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="61338-144">**注意** 在合作伙伴中心中的“过渡目标”合作伙伴租户帐户下过渡和设置订阅的同一天，合作伙伴必须暂停合作伙伴中心中的“过渡源”合作伙伴租户帐户上的订阅，以便确保不会重复计费。</span><span class="sxs-lookup"><span data-stu-id="61338-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="61338-145">由于未正确设置要禁用的“过渡源”订阅而引起的计费重叠，支持请求将因为信用问题而被拒。</span><span class="sxs-lookup"><span data-stu-id="61338-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="61338-146">禁用“过渡源”合作伙伴帐户下的 Office 365 订阅</span><span class="sxs-lookup"><span data-stu-id="61338-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="61338-147">禁用“过渡源”合作伙伴帐户下的云解决方案提供商订阅将阻止以后的任何计费。</span><span class="sxs-lookup"><span data-stu-id="61338-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="61338-148">无需手动禁用 Azure 订阅，因为 Azure 订阅在迁移过程中将自动禁用。</span><span class="sxs-lookup"><span data-stu-id="61338-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="61338-149">登录到**合作伙伴中心**与**转换从**CSP 帐户并导航到的客户列表。</span><span class="sxs-lookup"><span data-stu-id="61338-149">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="61338-150">打开要禁用订阅的客户，然后选择第一个要禁用的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="61338-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="61338-151">将订阅设置为“已暂停”，然后单击“提交”。</span><span class="sxs-lookup"><span data-stu-id="61338-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

 >[!**注意**]<span data-ttu-id="61338-152"> 正在暂停订阅可确保不会发生双计费。</span><span class="sxs-lookup"><span data-stu-id="61338-152"> Suspending the subscription ensures double billing does not occur.</span></span>



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  <span data-ttu-id="61338-153">为该客户下的所有订阅重复这些步骤。</span><span class="sxs-lookup"><span data-stu-id="61338-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="61338-154">验证所有订阅是否显示“已暂停”。</span><span class="sxs-lookup"><span data-stu-id="61338-154">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="61338-155">选择列表上的下一个客户，然后重复禁用所有订阅的过程。</span><span class="sxs-lookup"><span data-stu-id="61338-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="61338-156">迁移 Azure 基于使用情况的订阅</span><span class="sxs-lookup"><span data-stu-id="61338-156">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="61338-157">请注意，对于 Office 365 云解决方案提供商订阅，无需手动迁移 Azure 基于使用情况的云解决方案提供商订阅。</span><span class="sxs-lookup"><span data-stu-id="61338-157">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="61338-158">Microsoft Azure 支持可将 Azure 订阅、所有部署的服务或资源从“过渡源”云解决方案提供商经销商帐户迁移到“过渡目标”云解决方案提供商经销商帐户。</span><span class="sxs-lookup"><span data-stu-id="61338-158">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="61338-159">在此过渡期间，客户服务不会中断。</span><span class="sxs-lookup"><span data-stu-id="61338-159">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="61338-160">确保需要迁移 Azure 订阅的客户帐户已接受与新“过渡目标”云解决方案提供商帐户关联的协议。</span><span class="sxs-lookup"><span data-stu-id="61338-160">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="61338-161">合作伙伴通知 Microsoft 哪些具有 Azure 订阅的客户帐户已准备好迁移，并提供这些客户的公司名称。</span><span class="sxs-lookup"><span data-stu-id="61338-161">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="61338-162">Microsoft 迁移 Azure 基于使用情况的订阅，并通知合作伙伴迁移完成的时间。</span><span class="sxs-lookup"><span data-stu-id="61338-162">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="61338-163">合作伙伴确认“过渡源”云解决方案提供商经销商帐户下的 Azure 订阅现在在客户订阅部分下的“合作伙伴中心”中显示“已暂停”。</span><span class="sxs-lookup"><span data-stu-id="61338-163">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="61338-164">合作伙伴确认“过渡目标”云解决方案提供商经销商帐户下的 Azure 订阅现在在客户订阅部分下的“合作伙伴中心”中显示为“活动”。</span><span class="sxs-lookup"><span data-stu-id="61338-164">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

>[!**注意**]<span data-ttu-id="61338-165"> 禁用在客户订阅不会更改客户列表中的客户的外观。</span><span class="sxs-lookup"><span data-stu-id="61338-165"> Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="61338-166">目前不可选择从列表中删除客户。</span><span class="sxs-lookup"><span data-stu-id="61338-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="61338-167">合作伙伴应避免在以后从“过渡源”帐户中将订阅重新添加到这些客户。</span><span class="sxs-lookup"><span data-stu-id="61338-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>



6.  <span data-ttu-id="61338-168">为所有客户下的所有订阅重复这些步骤，阻止在以后向“过渡源”帐户收费。</span><span class="sxs-lookup"><span data-stu-id="61338-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="61338-169">合作伙伴将收到带有取消日期和计费周期最后一天之间未使用天数的信用的最终发票。</span><span class="sxs-lookup"><span data-stu-id="61338-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="61338-170">最终计费周期后不会再生成任何发票。</span><span class="sxs-lookup"><span data-stu-id="61338-170">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="61338-171">注释</span><span class="sxs-lookup"><span data-stu-id="61338-171">Notes</span></span>

-   <span data-ttu-id="61338-172">禁用“过渡源”云解决方案提供商帐户中的订阅不会影响最终客户的服务，前提是在禁用前，该服务已在“过渡目标”云解决方案提供商帐户中预配。</span><span class="sxs-lookup"><span data-stu-id="61338-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="61338-173">订阅无法由客户使用，并且在暂停或取消时不会产生费用。</span><span class="sxs-lookup"><span data-stu-id="61338-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="61338-174">当前无法将客户从“客户”列表中完全删除。</span><span class="sxs-lookup"><span data-stu-id="61338-174">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="61338-175">**注意** 在合作伙伴中心中的“过渡目标”合作伙伴租户帐户下过渡和设置订阅的同一天，合作伙伴必须暂停合作伙伴中心中的“过渡源”合作伙伴租户帐户上的订阅，以便确保不会重复计费。</span><span class="sxs-lookup"><span data-stu-id="61338-175">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="61338-176">由于未正确设置要暂停的“过渡源”订阅而引起的计费重叠，Microsoft 不会支持有信用问题的请求。</span><span class="sxs-lookup"><span data-stu-id="61338-176">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>



### <a name="simplify-migration-using-export"></a><span data-ttu-id="61338-177">使用“导出”简化迁移</span><span class="sxs-lookup"><span data-stu-id="61338-177">Simplify migration using Export</span></span>

<span data-ttu-id="61338-178">使用“导出函数”，捕获要在新合并的结构中使用的订阅：</span><span class="sxs-lookup"><span data-stu-id="61338-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="61338-179">单击**客户**在合作伙伴中心以查看现有结构中的客户列表。</span><span class="sxs-lookup"><span data-stu-id="61338-179">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="61338-180">打开所需的客户名称。</span><span class="sxs-lookup"><span data-stu-id="61338-180">Open the desired customer name.</span></span>

3.  <span data-ttu-id="61338-181">在“订阅”页上，单击“导出订阅”，将订阅的详细信息导出到 Excel 文件。</span><span class="sxs-lookup"><span data-stu-id="61338-181">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="61338-182">使用此列表在新合并的租户中重新创建订阅。</span><span class="sxs-lookup"><span data-stu-id="61338-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="61338-183">API 注册</span><span class="sxs-lookup"><span data-stu-id="61338-183">API registration</span></span>

<span data-ttu-id="61338-184">有关 API 注册的详细信息，[请参阅此页](https://go.microsoft.com/fwlink/?linkid=847990)。</span><span class="sxs-lookup"><span data-stu-id="61338-184">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>








