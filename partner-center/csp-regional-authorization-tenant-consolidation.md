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
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147575"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="b613d-104">云解决方案提供商区域授权租户合并说明</span><span class="sxs-lookup"><span data-stu-id="b613d-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="b613d-105">**适用** 于：合作伙伴中心 |适用于美国政府的 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="b613d-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b613d-106">**适当的角色**：全局管理员 |管理代理</span><span class="sxs-lookup"><span data-stu-id="b613d-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="b613d-107">\[某些信息与预发布的产品相关，这些信息可能会在正式发布之前进行重大修改。</span><span class="sxs-lookup"><span data-stu-id="b613d-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="b613d-108">对于此处提供的信息，Microsoft 不作任何明示或暗示的担保。\]</span><span class="sxs-lookup"><span data-stu-id="b613d-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="b613d-109">你可以整合业务的租户。</span><span class="sxs-lookup"><span data-stu-id="b613d-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="b613d-110">使用这些说明合并不同国家/地区的租户。</span><span class="sxs-lookup"><span data-stu-id="b613d-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="b613d-111">您必须知道要从中转换的帐户中每个客户的所有预配订阅和许可证计数。</span><span class="sxs-lookup"><span data-stu-id="b613d-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="b613d-112">在迁移过程中，将重新预配在新的中心 CSP 帐户下具有相同许可证计数的相同订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="b613d-113">使用导出列表功能，帮助创建移动至集中租户的客户列表。</span><span class="sxs-lookup"><span data-stu-id="b613d-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="b613d-114">合并完成后，将无法还原到以前的租户状态。</span><span class="sxs-lookup"><span data-stu-id="b613d-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="b613d-115">还可能需要客户操作。</span><span class="sxs-lookup"><span data-stu-id="b613d-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="b613d-116">准备迁移</span><span class="sxs-lookup"><span data-stu-id="b613d-116">Prepare for migration</span></span>

- <span data-ttu-id="b613d-117">使用过渡帐户登录到 **合作伙伴中心**  (你 **将转换为** 新帐户) ，并查看为这些客户预配的所有客户和所有服务。</span><span class="sxs-lookup"><span data-stu-id="b613d-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="b613d-118">从此帐户中注销。</span><span class="sxs-lookup"><span data-stu-id="b613d-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="b613d-119">迁移客户帐户</span><span class="sxs-lookup"><span data-stu-id="b613d-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="b613d-120">通过 **转换** (新的) 帐户 (要将客户过渡到) 中的帐户登录到 **合作伙伴中心**。</span><span class="sxs-lookup"><span data-stu-id="b613d-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="b613d-121">选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="b613d-121">Select **Customers**.</span></span>

3. <span data-ttu-id="b613d-122">选择 " **请求分销商关系**"。</span><span class="sxs-lookup"><span data-stu-id="b613d-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="b613d-123">系统会显示一个要发送给客户的默认电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b613d-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="b613d-124">此消息包含带有新建合作伙伴中心帐户独有的 org ID 的 URL。</span><span class="sxs-lookup"><span data-stu-id="b613d-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="b613d-125">**客户操作：** 确保想要迁移的所有活动客户均访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="b613d-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="b613d-126">打开 URL 时，系统将提示客户登录 Office 365 门户。</span><span class="sxs-lookup"><span data-stu-id="b613d-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="b613d-127">客户使用访问 Azure 和 Office 365 管理员门户所用的同一 Org ID 登录。</span><span class="sxs-lookup"><span data-stu-id="b613d-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="b613d-128">登录后，系统会提示 **客户帐户** 的全局管理员提交一个协议，该协议向新的 CSP 帐户授予委派的管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b613d-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="b613d-129">如果全局管理员同意，客户选中复选框，并同意授权建立这种关系。</span><span class="sxs-lookup"><span data-stu-id="b613d-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="b613d-130">客户每次提交协议后，会在合作伙伴的客户列表中显示。</span><span class="sxs-lookup"><span data-stu-id="b613d-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="b613d-131">迁移 Office 365 和非 Azure 且基于使用情况的订阅</span><span class="sxs-lookup"><span data-stu-id="b613d-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="b613d-132">客户签署协议后，可在“集中合作伙伴租户”下重新创建他们的订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="b613d-133">从 " **合作伙伴中心**"，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="b613d-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="b613d-134">打开要迁移的客户的公司名称。</span><span class="sxs-lookup"><span data-stu-id="b613d-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="b613d-135">选择“添加订阅”。</span><span class="sxs-lookup"><span data-stu-id="b613d-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="b613d-136">从目录中添加正确的订阅和许可证计数。</span><span class="sxs-lookup"><span data-stu-id="b613d-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="b613d-137">验证从合作伙伴帐户 **转换** 中提供的信息。</span><span class="sxs-lookup"><span data-stu-id="b613d-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="客户列表":::

6. <span data-ttu-id="b613d-139">选择" **提交"。**</span><span class="sxs-lookup"><span data-stu-id="b613d-139">Select **Submit.**</span></span>

   <span data-ttu-id="b613d-140">现在，服务从"转换到合作伙伴" **帐户提供给** 客户。</span><span class="sxs-lookup"><span data-stu-id="b613d-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="b613d-141">重复这些步骤，迁移所有其他客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="b613d-142">在继续下一部分之前，请确保在"转换到合作伙伴帐户"下重新预配"从合作伙伴帐户转换"下 **存在** 的所有客户订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="b613d-143">合作伙伴必须在 合作伙伴中心 中暂停从合作伙伴租户帐户转换的订阅，这些订阅在 合作伙伴中心 中的"转换到合作伙伴租户"帐户下进行转换和设置时，以确保不会发生双重计费。</span><span class="sxs-lookup"><span data-stu-id="b613d-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="b613d-144">由于未正确禁用"从订阅转换"而发生的计费重叠，因此将拒绝对额度 **的支持** 请求。</span><span class="sxs-lookup"><span data-stu-id="b613d-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="b613d-145">禁用“过渡源”合作伙伴帐户下的 Office 365 订阅</span><span class="sxs-lookup"><span data-stu-id="b613d-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="b613d-146">在"从合作伙伴帐户转换"下禁用 CSP 订阅会停止任何将来的计费。</span><span class="sxs-lookup"><span data-stu-id="b613d-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="b613d-147">不必手动禁用 Azure 订阅，因为在迁移过程中会自动禁用 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="b613d-148">使用"从 **CSP** **合作伙伴中心"登录到** 客户帐户并导航到客户列表。</span><span class="sxs-lookup"><span data-stu-id="b613d-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="b613d-149">打开要禁用订阅的客户，然后选择第一个要禁用的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="b613d-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="b613d-150">将订阅设置为"**挂起"，** 然后选择"提交 **"。**</span><span class="sxs-lookup"><span data-stu-id="b613d-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="b613d-151">暂停订阅可确保不会进行双重计费。</span><span class="sxs-lookup"><span data-stu-id="b613d-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="b613d-152">订阅在 **订阅列表中** 显示"挂起"。</span><span class="sxs-lookup"><span data-stu-id="b613d-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="b613d-153">为该客户下的所有订阅重复这些步骤。</span><span class="sxs-lookup"><span data-stu-id="b613d-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="b613d-154">验证是否所有显示 **已挂起。**</span><span class="sxs-lookup"><span data-stu-id="b613d-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="b613d-155">选择列表上的下一个客户，然后重复禁用所有订阅的过程。</span><span class="sxs-lookup"><span data-stu-id="b613d-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="b613d-156">迁移 Azure 基于使用情况的订阅</span><span class="sxs-lookup"><span data-stu-id="b613d-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="b613d-157">与 Office 365 CSP 订阅不同，Azure 不需要手动迁移基于使用情况的 CSP 订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="b613d-158">Microsoft Azure支持部门将 Azure 订阅以及所有已部署的服务或资源从"从 **CSP** 经销商帐户转换"迁移到 **CSP** 经销商帐户。</span><span class="sxs-lookup"><span data-stu-id="b613d-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="b613d-159">在此过渡期间，客户服务不会中断。</span><span class="sxs-lookup"><span data-stu-id="b613d-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="b613d-160">确保将迁移 Azure 订阅的客户帐户已接受协议，以与新的 **转换到** CSP 帐户相关联。</span><span class="sxs-lookup"><span data-stu-id="b613d-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="b613d-161">你将通知 Microsoft 哪些客户帐户已准备好进行迁移，并提供这些客户的公司名称。</span><span class="sxs-lookup"><span data-stu-id="b613d-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="b613d-162">Microsoft 迁移基于 Azure 使用情况的订阅，并在迁移完成后通知你。</span><span class="sxs-lookup"><span data-stu-id="b613d-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="b613d-163">需要确认当前在 "客户订阅" 部分下的 "合作伙伴 **中心" 下** 将 Azure 订阅标记为 "已 **挂起** "。</span><span class="sxs-lookup"><span data-stu-id="b613d-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="b613d-164">确认 **转换为** CSP 分销商帐户下的 Azure 订阅现在在 "客户订阅" 部分下的 "合作伙伴中心" 中显示 " **活动** " 状态。</span><span class="sxs-lookup"><span data-stu-id="b613d-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="b613d-165">禁用客户的订阅后，不会在 "客户" 列表中更改客户的外观。</span><span class="sxs-lookup"><span data-stu-id="b613d-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="b613d-166">目前不可选择从列表中删除客户。</span><span class="sxs-lookup"><span data-stu-id="b613d-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="b613d-167">合作伙伴应避免向这些客户添加从将来 **过渡** 到这些客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="b613d-168">为所有客户下的所有订阅重复这些步骤，以停止 **从** 帐户 () 的将来的收费。</span><span class="sxs-lookup"><span data-stu-id="b613d-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="b613d-169">合作伙伴将收到带有取消日期和计费周期最后一天之间未使用天数的信用的最终发票。</span><span class="sxs-lookup"><span data-stu-id="b613d-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="b613d-170">最终计费周期后不会再生成任何发票。</span><span class="sxs-lookup"><span data-stu-id="b613d-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="b613d-171">其他信息</span><span class="sxs-lookup"><span data-stu-id="b613d-171">Additional information</span></span>

- <span data-ttu-id="b613d-172">如果在禁用订阅之前从 "**转换为** csp" 帐户预配了服务，则通过从 CSP 帐户 **转换** 禁用订阅不会影响最终客户的服务。</span><span class="sxs-lookup"><span data-stu-id="b613d-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="b613d-173">订阅不能由客户使用，并且在挂起或取消时不会产生费用。</span><span class="sxs-lookup"><span data-stu-id="b613d-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="b613d-174">目前没有办法完全从 **客户** 列表中删除客户。</span><span class="sxs-lookup"><span data-stu-id="b613d-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="b613d-175">合作伙伴必须在伙伴中心中暂停从合作伙伴租户帐户 **过渡** 到的订阅，这一天的订阅将转换为，并在 **转换为** 帐户下设置，以确保不会发生双重计费。</span><span class="sxs-lookup"><span data-stu-id="b613d-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="b613d-176">Microsoft 将不支持信用额度请求，因为不能正确地将 " **从订阅转换** " 设置为 "已挂起"。</span><span class="sxs-lookup"><span data-stu-id="b613d-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="b613d-177">使用“导出”简化迁移</span><span class="sxs-lookup"><span data-stu-id="b613d-177">Simplify migration using Export</span></span>

<span data-ttu-id="b613d-178">使用 **Export 函数**，可以捕获需要在新的合并结构中使用的订阅：</span><span class="sxs-lookup"><span data-stu-id="b613d-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="b613d-179">选择"合作伙伴中心"以查看客户列表。</span><span class="sxs-lookup"><span data-stu-id="b613d-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="b613d-180">打开所需的客户名称。</span><span class="sxs-lookup"><span data-stu-id="b613d-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="b613d-181">在 **"订阅"** 页上， **选择"导出** 订阅"，将订阅的详细信息导出到 Excel 文件。</span><span class="sxs-lookup"><span data-stu-id="b613d-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="b613d-182">使用此列表在新合并的租户中重新创建订阅。</span><span class="sxs-lookup"><span data-stu-id="b613d-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="b613d-183">API 注册</span><span class="sxs-lookup"><span data-stu-id="b613d-183">API registration</span></span>

<span data-ttu-id="b613d-184">有关 API 注册详细信息，请参阅[在 中设置 API 合作伙伴中心。](/partner-center/develop/set-up-api-access-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="b613d-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b613d-185">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b613d-185">Next steps</span></span>

- [<span data-ttu-id="b613d-186">云解决方案提供商可以销售 CSP 产品/服务的区域市场和货币</span><span class="sxs-lookup"><span data-stu-id="b613d-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
