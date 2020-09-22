---
title: 云解决方案提供商区域授权租户合并
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用这些说明合并不同国家/地区的租户。 这包括迁移客户帐户和客户订阅的步骤。
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 232eae10927d8ac38b4cce0842fbb8e4278f8d03
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000371"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="0e77e-104">云解决方案提供商区域授权租户合并说明</span><span class="sxs-lookup"><span data-stu-id="0e77e-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="0e77e-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="0e77e-105">**Applies to**</span></span>

-  <span data-ttu-id="0e77e-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="0e77e-106">Partner Center</span></span>
-  <span data-ttu-id="0e77e-107">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="0e77e-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="0e77e-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="0e77e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="0e77e-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0e77e-109">Global admin</span></span>
- <span data-ttu-id="0e77e-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="0e77e-110">Admin agent</span></span>

<span data-ttu-id="0e77e-111">\[某些信息与预发布的产品相关，这些信息可能会在正式发布之前进行重大修改。</span><span class="sxs-lookup"><span data-stu-id="0e77e-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="0e77e-112">Microsoft 对此处提供的信息不提供任何明示或暗示的保证。\]</span><span class="sxs-lookup"><span data-stu-id="0e77e-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="0e77e-113">你可以整合业务的租户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="0e77e-114">使用这些说明合并不同国家/地区的租户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="0e77e-115">您必须知道要从中转换的帐户中每个客户的所有预配订阅和许可证计数。</span><span class="sxs-lookup"><span data-stu-id="0e77e-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="0e77e-116">在迁移过程中，将重新预配在新的中心 CSP 帐户下具有相同许可证计数的相同订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="0e77e-117">使用导出列表功能，帮助创建移动至集中租户的客户列表。</span><span class="sxs-lookup"><span data-stu-id="0e77e-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="0e77e-118">合并完成后，将无法还原到以前的租户状态。</span><span class="sxs-lookup"><span data-stu-id="0e77e-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="0e77e-119">还可能需要客户操作。</span><span class="sxs-lookup"><span data-stu-id="0e77e-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="0e77e-120">准备迁移</span><span class="sxs-lookup"><span data-stu-id="0e77e-120">Prepare for migration</span></span>

- <span data-ttu-id="0e77e-121">使用过渡帐户登录到 **合作伙伴中心**  (你 **将转换为** 新帐户) ，并查看为这些客户预配的所有客户和所有服务。</span><span class="sxs-lookup"><span data-stu-id="0e77e-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="0e77e-122">从此帐户中注销。</span><span class="sxs-lookup"><span data-stu-id="0e77e-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="0e77e-123">迁移客户帐户</span><span class="sxs-lookup"><span data-stu-id="0e77e-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="0e77e-124">通过**转换** (新的) 帐户 (要将客户过渡到) 中的帐户登录到**合作伙伴中心**。</span><span class="sxs-lookup"><span data-stu-id="0e77e-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="0e77e-125">选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="0e77e-125">Select **Customers**.</span></span>

3. <span data-ttu-id="0e77e-126">单击 " **请求分销商关系**"。</span><span class="sxs-lookup"><span data-stu-id="0e77e-126">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="0e77e-127">系统会显示一个要发送给客户的默认电子邮件。</span><span class="sxs-lookup"><span data-stu-id="0e77e-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="0e77e-128">此消息包含带有新建合作伙伴中心帐户独有的 org ID 的 URL。</span><span class="sxs-lookup"><span data-stu-id="0e77e-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="0e77e-129">**客户操作：** 确保想要迁移的所有活动客户均访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="0e77e-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="0e77e-130">打开 URL 时，系统将提示客户登录 Office 365 门户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="0e77e-131">客户使用访问 Azure 和 Office 365 管理员门户所用的同一 Org ID 登录。</span><span class="sxs-lookup"><span data-stu-id="0e77e-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="0e77e-132">登录后，系统会提示 **客户帐户** 的全局管理员提交一个协议，该协议向新的 CSP 帐户授予委派的管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0e77e-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="0e77e-133">如果全局管理员同意，客户选中复选框，并同意授权建立这种关系。</span><span class="sxs-lookup"><span data-stu-id="0e77e-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="0e77e-134">客户每次提交协议后，会在合作伙伴的客户列表中显示。</span><span class="sxs-lookup"><span data-stu-id="0e77e-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="0e77e-135">迁移 Office 365 和非 Azure 且基于使用情况的订阅</span><span class="sxs-lookup"><span data-stu-id="0e77e-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="0e77e-136">客户签署协议后，可在“集中合作伙伴租户”下重新创建他们的订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="0e77e-137">从 **合作伙伴中心** 选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="0e77e-137">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="0e77e-138">打开要迁移的客户的公司名称。</span><span class="sxs-lookup"><span data-stu-id="0e77e-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="0e77e-139">选择“添加订阅”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="0e77e-139">Select **Add subscription**.</span></span>

5. <span data-ttu-id="0e77e-140">从目录中添加正确的订阅和许可证计数。</span><span class="sxs-lookup"><span data-stu-id="0e77e-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="0e77e-141">验证从合作伙伴帐户 **转换** 中提供的信息。</span><span class="sxs-lookup"><span data-stu-id="0e77e-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="客户列表":::

6. <span data-ttu-id="0e77e-143">单击 " **提交"。**</span><span class="sxs-lookup"><span data-stu-id="0e77e-143">Click **Submit.**</span></span>

   <span data-ttu-id="0e77e-144">现在，服务将提供给客户，从 **过渡到** 合作伙伴帐户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="0e77e-145">重复这些步骤，迁移所有其他客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="0e77e-146">在继续下一节之前，请确保在 "**过渡到**合作伙伴帐户" 下重新设置了 "从合作伙伴帐户**转换**" 下的所有客户订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="0e77e-147">合作伙伴必须在合作伙伴中心的合作伙伴租户帐户 **之间** 暂停订阅，这一天在合作伙伴中心转换 **为** 合作伙伴租户帐户时，会将这些订阅转换并设置为，以确保不会发生双重计费。</span><span class="sxs-lookup"><span data-stu-id="0e77e-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="0e77e-148">由于不能正确禁用 **从订阅转换** 而产生的任何费用重叠，因此会拒绝支持请求。</span><span class="sxs-lookup"><span data-stu-id="0e77e-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="0e77e-149">禁用“过渡源”合作伙伴帐户下的 Office 365 订阅</span><span class="sxs-lookup"><span data-stu-id="0e77e-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="0e77e-150">在从合作伙伴帐户转换时禁用 CSP 订阅会停止任何将来 **的** 帐单。</span><span class="sxs-lookup"><span data-stu-id="0e77e-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="0e77e-151">你不必手动禁用 Azure 订阅，因为在迁移过程中会自动禁用 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="0e77e-152">通过从 CSP 帐户**转换**并导航到 customer 列表，登录到**合作伙伴中心**。</span><span class="sxs-lookup"><span data-stu-id="0e77e-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="0e77e-153">打开要禁用订阅的客户，然后选择第一个要禁用的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="0e77e-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="0e77e-154">将 "订阅" 设置为 " **挂起**"，然后单击 " **提交**"。</span><span class="sxs-lookup"><span data-stu-id="0e77e-154">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="0e77e-155">挂起订阅可确保不会进行双重计费。</span><span class="sxs-lookup"><span data-stu-id="0e77e-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="0e77e-156">订阅显示 "订阅" 列表中的 " **挂起** "。</span><span class="sxs-lookup"><span data-stu-id="0e77e-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="0e77e-157">为该客户下的所有订阅重复这些步骤。</span><span class="sxs-lookup"><span data-stu-id="0e77e-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="0e77e-158">验证所有 "显示已 **挂起"。**</span><span class="sxs-lookup"><span data-stu-id="0e77e-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="0e77e-159">选择列表上的下一个客户，然后重复禁用所有订阅的过程。</span><span class="sxs-lookup"><span data-stu-id="0e77e-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="0e77e-160">迁移 Azure 基于使用情况的订阅</span><span class="sxs-lookup"><span data-stu-id="0e77e-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="0e77e-161">与 Office 365 CSP 订阅不同，Azure，基于使用情况的 CSP 订阅不需要手动迁移。</span><span class="sxs-lookup"><span data-stu-id="0e77e-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="0e77e-162">Microsoft Azure 支持会将 Azure 订阅和所有已部署的服务或资源从 CSP 经销商帐户 **转换** 为 **转换为** csp 分销商帐户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="0e77e-163">在此过渡期间，客户服务不会中断。</span><span class="sxs-lookup"><span data-stu-id="0e77e-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="0e77e-164">确保将迁移 Azure 订阅的客户帐户接受与新的 " **转换为** CSP" 帐户关联的协议。</span><span class="sxs-lookup"><span data-stu-id="0e77e-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="0e77e-165">你将通知 Microsoft 哪些客户帐户已准备好进行迁移，并提供这些客户的公司名称。</span><span class="sxs-lookup"><span data-stu-id="0e77e-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="0e77e-166">Microsoft 迁移基于 Azure 使用情况的订阅，并在迁移完成后通知你。</span><span class="sxs-lookup"><span data-stu-id="0e77e-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="0e77e-167">需要确认当前在 "客户订阅" 部分下的 "合作伙伴 **中心" 下** 将 Azure 订阅标记为 "已 **挂起** "。</span><span class="sxs-lookup"><span data-stu-id="0e77e-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="0e77e-168">确认 **转换为** CSP 分销商帐户下的 Azure 订阅现在在 "客户订阅" 部分下的 "合作伙伴中心" 中显示 " **活动** " 状态。</span><span class="sxs-lookup"><span data-stu-id="0e77e-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="0e77e-169">禁用客户的订阅后，不会在 "客户" 列表中更改客户的外观。</span><span class="sxs-lookup"><span data-stu-id="0e77e-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="0e77e-170">目前不可选择从列表中删除客户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="0e77e-171">合作伙伴应避免向这些客户添加从将来 **过渡** 到这些客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="0e77e-172">为所有客户下的所有订阅重复这些步骤，以停止 **从** 帐户 () 的将来的收费。</span><span class="sxs-lookup"><span data-stu-id="0e77e-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="0e77e-173">合作伙伴将收到带有取消日期和计费周期最后一天之间未使用天数的信用的最终发票。</span><span class="sxs-lookup"><span data-stu-id="0e77e-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="0e77e-174">最终计费周期后不会再生成任何发票。</span><span class="sxs-lookup"><span data-stu-id="0e77e-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="0e77e-175">其他信息</span><span class="sxs-lookup"><span data-stu-id="0e77e-175">Additional information</span></span>

- <span data-ttu-id="0e77e-176">如果在禁用订阅之前从 "**转换为**csp" 帐户预配了服务，则通过从 CSP 帐户**转换**禁用订阅不会影响最终客户的服务。</span><span class="sxs-lookup"><span data-stu-id="0e77e-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="0e77e-177">订阅不能由客户使用，并且在挂起或取消时不会产生费用。</span><span class="sxs-lookup"><span data-stu-id="0e77e-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="0e77e-178">目前没有办法完全从 **客户** 列表中删除客户。</span><span class="sxs-lookup"><span data-stu-id="0e77e-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="0e77e-179">合作伙伴必须在伙伴中心中暂停从合作伙伴租户帐户 **过渡** 到的订阅，这一天的订阅将转换为，并在 **转换为** 帐户下设置，以确保不会发生双重计费。</span><span class="sxs-lookup"><span data-stu-id="0e77e-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="0e77e-180">Microsoft 将不支持信用额度请求，因为不能正确地将 " **从订阅转换** " 设置为 "已挂起"。</span><span class="sxs-lookup"><span data-stu-id="0e77e-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="0e77e-181">使用“导出”简化迁移</span><span class="sxs-lookup"><span data-stu-id="0e77e-181">Simplify migration using Export</span></span>

<span data-ttu-id="0e77e-182">使用 **Export 函数**，可以捕获需要在新的合并结构中使用的订阅：</span><span class="sxs-lookup"><span data-stu-id="0e77e-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="0e77e-183">单击 "合作伙伴中心" 上的 " **客户** "，以查看客户列表。</span><span class="sxs-lookup"><span data-stu-id="0e77e-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="0e77e-184">打开所需的客户名称。</span><span class="sxs-lookup"><span data-stu-id="0e77e-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="0e77e-185">在 " **订阅** " 页上，单击 " **导出订阅** "，将订阅的详细信息导出到 Excel 文件中。</span><span class="sxs-lookup"><span data-stu-id="0e77e-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="0e77e-186">使用此列表在新合并的租户中重新创建订阅。</span><span class="sxs-lookup"><span data-stu-id="0e77e-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="0e77e-187">API 注册</span><span class="sxs-lookup"><span data-stu-id="0e77e-187">API registration</span></span>

<span data-ttu-id="0e77e-188">有关 API 注册的详细信息，请参阅 [在合作伙伴中心设置 api 访问权限](/partner-center/develop/set-up-api-access-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="0e77e-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="0e77e-189">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0e77e-189">Next steps</span></span>

- [<span data-ttu-id="0e77e-190">合作伙伴中心内针对经销商合作伙伴的客户帐户设置和管理</span><span class="sxs-lookup"><span data-stu-id="0e77e-190">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)