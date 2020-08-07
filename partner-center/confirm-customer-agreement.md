---
title: 确认客户接受 Microsoft 客户协议
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何确认客户接受 Microsoft 客户协议。 为客户订购 Microsoft 产品和服务时，云解决方案提供商需要这样做。
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 66be96fe8621089bda8dae546b804320d05fcb25
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527820"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a><span data-ttu-id="d44b6-104">确认客户接受云解决方案提供商合作伙伴计划中的 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-104">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>

<span data-ttu-id="d44b6-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="d44b6-105">**Applies to**</span></span>

- <span data-ttu-id="d44b6-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="d44b6-106">Partner Center</span></span>
- <span data-ttu-id="d44b6-107">Microsoft 365 管理中心</span><span class="sxs-lookup"><span data-stu-id="d44b6-107">Microsoft 365 Admin Center</span></span>

<span data-ttu-id="d44b6-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="d44b6-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d44b6-109">管理员代理</span><span class="sxs-lookup"><span data-stu-id="d44b6-109">Admin agent</span></span>
- <span data-ttu-id="d44b6-110">销售代理</span><span class="sxs-lookup"><span data-stu-id="d44b6-110">Sales agent</span></span>

<span data-ttu-id="d44b6-111">**适当的合作伙伴类型**</span><span class="sxs-lookup"><span data-stu-id="d44b6-111">**Appropriate partner types**</span></span>

- <span data-ttu-id="d44b6-112">间接经销商、直接计费、间接提供商</span><span class="sxs-lookup"><span data-stu-id="d44b6-112">Indirect resellers, Direct bill, Indirect providers</span></span>

<span data-ttu-id="d44b6-113">2019 年 10 月 1 日，Microsoft 推出了针对云解决方案提供商计划的 **Microsoft 客户协议**，替代 Microsoft 云协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-113">On October 1st, 2019, Microsoft introduced the **Microsoft Customer Agreement** to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="d44b6-114">请阅读间接经销商的其他[指南](indirect-reseller-tasks-in-partner-center.md)。</span><span class="sxs-lookup"><span data-stu-id="d44b6-114">Read additional [guidance](indirect-reseller-tasks-in-partner-center.md) for indirect resellers.</span></span> <span data-ttu-id="d44b6-115">为了方便合作伙伴迁移到新协议，在 2020 年 1 月 31 日之前，这两个协议在云解决方案提供商计划中共存。</span><span class="sxs-lookup"><span data-stu-id="d44b6-115">To facilitate partners' migration to the new agreement, both agreements coexisted in the CSP program until January 31st, 2020.</span></span> <span data-ttu-id="d44b6-116">从 2020 年 2 月 1 日开始，Microsoft 客户协议替代了 Microsoft 云协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-116">Starting February 1, 2020, the Microsoft Customer Agreement replaced the Microsoft Cloud Agreement.</span></span>

<span data-ttu-id="d44b6-117">客户有两个选项可用于接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-117">Customers have two options for accepting the Microsoft Customer Agreement.</span></span> 

<span data-ttu-id="d44b6-118">**选项 1**：合作伙伴证明客户已接受 - 合作伙伴可以通过合作伙伴中心 API/SDK 或合作伙伴中心仪表板确认客户接受。</span><span class="sxs-lookup"><span data-stu-id="d44b6-118">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="d44b6-119">**选项 2**：客户直接接受 - 合作伙伴可以通过 URL 邀请客户在 Microsoft 365 管理中心查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-119">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="d44b6-120">访问 Microsoft 客户协议模板</span><span class="sxs-lookup"><span data-stu-id="d44b6-120">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="d44b6-121">可以从[此处](https://aka.ms/customeragreement)手动下载最新版 Microsoft 客户协议模板。</span><span class="sxs-lookup"><span data-stu-id="d44b6-121">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="d44b6-122">Microsoft 客户协议特定于国家/地区。</span><span class="sxs-lookup"><span data-stu-id="d44b6-122">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="d44b6-123">在请求 Microsoft 客户协议模板时，请确保根据客户的位置选择正确的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="d44b6-123">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="d44b6-124">选项 1：在合作伙伴中心中确认客户已接受协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-124">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="d44b6-125">对于新客户和现有客户，合作伙伴可以在合作伙伴中心确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-125">Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="d44b6-126">经销商不能代表其客户进行证明，需通过其间接提供商来完成证明。</span><span class="sxs-lookup"><span data-stu-id="d44b6-126">Resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="d44b6-127">确认新客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-127">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="d44b6-128">在合作伙伴中心创建新客户租户时，请按以下步骤确认客户接受了 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-128">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d44b6-129">必须是管理员代理或销售代理才能执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="d44b6-129">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="d44b6-130">选择“客户”，然后选择“新客户”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-130">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="d44b6-131">在“帐户信息”下，输入公司及其主要联系人的信息。</span><span class="sxs-lookup"><span data-stu-id="d44b6-131">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="d44b6-132">在“Microsoft 协议”下，选中相应的框来证明客户已接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-132">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="d44b6-133">在“协议接受日期”下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="d44b6-133">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d44b6-134">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="d44b6-134">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="d44b6-135">确保显示的主要用户联系人信息正确。</span><span class="sxs-lookup"><span data-stu-id="d44b6-135">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="d44b6-136">如果不正确，请选择“更新”并输入接受该协议的人员的准确信息。</span><span class="sxs-lookup"><span data-stu-id="d44b6-136">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="d44b6-137">选择“下一步”继续创建客户租户。</span><span class="sxs-lookup"><span data-stu-id="d44b6-137">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客户":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="d44b6-139">确认现有客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-139">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="d44b6-140">必须是管理员代理或销售代理才能执行此操作：</span><span class="sxs-lookup"><span data-stu-id="d44b6-140">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="d44b6-141">选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-141">Select **Customers**.</span></span> <span data-ttu-id="d44b6-142">找到并选择客户。</span><span class="sxs-lookup"><span data-stu-id="d44b6-142">Find and select the customer.</span></span>

2. <span data-ttu-id="d44b6-143">选择“帐户信息”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-143">Select **Account info**.</span></span>

3. <span data-ttu-id="d44b6-144">在“Microsoft 客户协议”下选择“更新”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-144">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="d44b6-145">输入已接受协议的人员的**名字**、**姓氏**、**电子邮件地址**和**电话号码**（可选）。</span><span class="sxs-lookup"><span data-stu-id="d44b6-145">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="d44b6-146">在“协议接受日期”下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="d44b6-146">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d44b6-147">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="d44b6-147">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="d44b6-148">选择“保存”，然后继续操作。</span><span class="sxs-lookup"><span data-stu-id="d44b6-148">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="现有客户":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="d44b6-150">检索客户接受协议的确认信息</span><span class="sxs-lookup"><span data-stu-id="d44b6-150">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="d44b6-151">可以按下述步骤检索关于现有客户已接受 Microsoft 客户协议的确认信息。</span><span class="sxs-lookup"><span data-stu-id="d44b6-151">You can retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement using the following steps.</span></span> <span data-ttu-id="d44b6-152">必须是管理员代理或销售代理才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="d44b6-152">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d44b6-153">选择“客户”，然后找到并选择要查看的客户。</span><span class="sxs-lookup"><span data-stu-id="d44b6-153">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="d44b6-154">选择“帐户信息”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-154">Select **Account info**.</span></span>

3. <span data-ttu-id="d44b6-155">在“Microsoft 客户协议”下，查看该客户是否提供过确认。</span><span class="sxs-lookup"><span data-stu-id="d44b6-155">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="d44b6-156">使用合作伙伴中心 API/SDK 确认客户接受协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-156">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="d44b6-157">可以使用合作伙伴中心 API/SDK 确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-157">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d44b6-158">有关 API/SDK 的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d44b6-158">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="d44b6-159">获取 Microsoft 客户协议的协议元数据</span><span class="sxs-lookup"><span data-stu-id="d44b6-159">Get agreement metadata for the Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="d44b6-160">确认客户接受 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-160">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="d44b6-161">获取客户接受 Microsoft 客户协议的确认</span><span class="sxs-lookup"><span data-stu-id="d44b6-161">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="d44b6-162">获取 Microsoft 客户协议模板的下载链接</span><span class="sxs-lookup"><span data-stu-id="d44b6-162">Get a download link for the Microsoft Customer Agreement template</span></span>](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="d44b6-163">选项 2：客户在 Microsoft 365 管理中心接受协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-163">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="d44b6-164">合作伙伴可以通过 URL 邀请新客户和现有客户在 Microsoft 365 管理中心查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-164">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="d44b6-165">接下来的几部分介绍如何执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="d44b6-165">The next few sections show you how to:</span></span>

- <span data-ttu-id="d44b6-166">创建一个新客户，并邀请该客户查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-166">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="d44b6-167">邀请新客户查看并接受经销商关系和协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-167">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="d44b6-168">邀请现有客户查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-168">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="d44b6-169">可以使用[合作伙伴中心 API/SDK](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) 来获取客户直接接受 Microsoft 客户协议的状态。</span><span class="sxs-lookup"><span data-stu-id="d44b6-169">You can use [Partner Center API/SDK](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="d44b6-170">创建一个新客户，并邀请该客户查看并接受协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-170">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="d44b6-171">使用以下步骤在合作伙伴中心创建新客户，并邀请他们在 Microsoft 365 管理中心查看并接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-171">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="d44b6-172">从合作伙伴中心的“客户”选项卡中，选择“添加客户”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-172">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="d44b6-173">在“帐户信息”下的所有必填字段中输入新客户的信息，包括客户的公司名称和主要联系人。</span><span class="sxs-lookup"><span data-stu-id="d44b6-173">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="d44b6-174">在“客户协议”下选择第一个选项，即“将要求客户在 Microsoft 365 管理中心接受 Microsoft 客户协议”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-174">Under **Customer Agreement**, select the first option, **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="d44b6-175">完成页面上的所有其他必填字段。</span><span class="sxs-lookup"><span data-stu-id="d44b6-175">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="d44b6-176">选择“下一步:查看”，然后继续执行创建客户租户的步骤。</span><span class="sxs-lookup"><span data-stu-id="d44b6-176">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="d44b6-177">新客户必须接受 Microsoft 客户协议才能进行新的购买。</span><span class="sxs-lookup"><span data-stu-id="d44b6-177">New customers cannot make a new purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="创建新客户":::

5. <span data-ttu-id="d44b6-179">到达新客户工作流中的“确认”屏幕后，保存客户凭据。</span><span class="sxs-lookup"><span data-stu-id="d44b6-179">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="d44b6-180">稍后需将这些凭据分配给客户。</span><span class="sxs-lookup"><span data-stu-id="d44b6-180">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="d44b6-181">在合作伙伴中心外部，创建并发送一封电子邮件，邀请客户在 Microsoft 365 管理中心接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-181">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="d44b6-182">请确保电子邮件中包含以下项：</span><span class="sxs-lookup"><span data-stu-id="d44b6-182">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="d44b6-183">此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的链接（需要登录）</span><span class="sxs-lookup"><span data-stu-id="d44b6-183">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="d44b6-184">在步骤 5 中保存的客户凭据。</span><span class="sxs-lookup"><span data-stu-id="d44b6-184">The customer's credentials you saved in Step 5.</span></span>

7. <span data-ttu-id="d44b6-185">然后，客户会收到来自合作伙伴的电子邮件邀请，并会选择 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="d44b6-185">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="d44b6-186">客户使用之前从合作伙伴处收到的客户凭据登录 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="d44b6-186">The customer signs into Microsoft 365 Admin Center using the customer credentials previously received from the partner.</span></span>

9. <span data-ttu-id="d44b6-187">然后，客户选中用于接受 Microsoft 客户协议的复选框。</span><span class="sxs-lookup"><span data-stu-id="d44b6-187">The customer then checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="d44b6-188">邀请新客户查看并接受经销商关系和 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-188">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="d44b6-189">通过以下步骤邀请新客户查看并接受经销商关系和 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-189">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="d44b6-190">从合作伙伴中心的“客户”选项卡中选择“请求建立经销商关系”链接。</span><span class="sxs-lookup"><span data-stu-id="d44b6-190">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="d44b6-191">系统会生成自动电子邮件模板，其中包括文本和参数化 URL，用于将客户定向到 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="d44b6-191">An automatic email template will be generated, including text and a parameterized URL which will direct the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="d44b6-192">可以自定义自动生成的电子邮件模板，然后选择“复制到剪贴板”或“在电子邮件中打开”。</span><span class="sxs-lookup"><span data-stu-id="d44b6-192">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="d44b6-193">使用此电子邮件模板邀请客户接受**经销商关系**请求和 **Microsoft 客户协议**。</span><span class="sxs-lookup"><span data-stu-id="d44b6-193">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="d44b6-194">（注意：在电子邮件邀请中，请确保合作伙伴还包括自动提供的 URL 以及最近创建的客户凭据。）</span><span class="sxs-lookup"><span data-stu-id="d44b6-194">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="创建关系":::

5. <span data-ttu-id="d44b6-196">客户通过电子邮件接收邀请，并单击参数化 URL。</span><span class="sxs-lookup"><span data-stu-id="d44b6-196">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="d44b6-197">客户使用电子邮件中合作伙伴提供的凭据登录 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="d44b6-197">Customer uses credentials provided by partner within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="d44b6-198">客户选中用于接受**经销商关系**和 **Microsoft 客户协议**的复选框。</span><span class="sxs-lookup"><span data-stu-id="d44b6-198">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="d44b6-199">在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。</span><span class="sxs-lookup"><span data-stu-id="d44b6-199">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="d44b6-200">客户可以选择一个合作伙伴来查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="d44b6-200">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="接受协议":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="d44b6-202">邀请现有客户查看并接受协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-202">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="d44b6-203">通过以下步骤邀请现有客户查看并接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-203">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="d44b6-204">创建包含嵌入 URL 的客户电子邮件，邀请客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-204">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="d44b6-205">客户通过电子邮件接收邀请，并单击 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="d44b6-205">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="d44b6-206">客户将其凭据输入 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="d44b6-206">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="d44b6-207">客户选中用于接受 Microsoft 客户协议的复选框。</span><span class="sxs-lookup"><span data-stu-id="d44b6-207">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="d44b6-208">在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。</span><span class="sxs-lookup"><span data-stu-id="d44b6-208">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="d44b6-209">客户可以选择一个合作伙伴来查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="d44b6-209">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="客户":::

>[!NOTE]
><span data-ttu-id="d44b6-211">在某些情况下，客户可能无法直接接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-211">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d44b6-212">若要详细了解这些情况，请参阅[需要代表客户证明的两种情况](attest-acceptance-customer-agreement.md)。</span><span class="sxs-lookup"><span data-stu-id="d44b6-212">To learn more about these situations, see [Two scenarios where you need to attest on behalf of your customer](attest-acceptance-customer-agreement.md).</span></span>

### <a name="historical-timeline-details"></a><span data-ttu-id="d44b6-213">历史时间线详细信息</span><span class="sxs-lookup"><span data-stu-id="d44b6-213">Historical timeline details</span></span>

| <span data-ttu-id="d44b6-214">日期</span><span class="sxs-lookup"><span data-stu-id="d44b6-214">Date</span></span> | <span data-ttu-id="d44b6-215">里程碑</span><span class="sxs-lookup"><span data-stu-id="d44b6-215">Milestone</span></span> | <span data-ttu-id="d44b6-216">详细信息</span><span class="sxs-lookup"><span data-stu-id="d44b6-216">Details</span></span> |
|------------|------------|--------------------------------|
|<span data-ttu-id="d44b6-217">2019 年 8 月 1 日</span><span class="sxs-lookup"><span data-stu-id="d44b6-217">August 01, 2019</span></span>|<span data-ttu-id="d44b6-218">在沙盒中提供 UX 预览版</span><span class="sxs-lookup"><span data-stu-id="d44b6-218">UX preview available in sandbox</span></span>|<span data-ttu-id="d44b6-219">合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心面板确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-219">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard in the CSP sandbox environment.</span></span> <span data-ttu-id="d44b6-220">有权访问 CSP 沙盒环境的合作伙伴可以预览用户体验更改。</span><span class="sxs-lookup"><span data-stu-id="d44b6-220">Partners with access to the CSP sandbox environment preview the user experience changes.</span></span> <span data-ttu-id="d44b6-221">无权访问沙盒的合作伙伴可以在本主题中了解这些更改。</span><span class="sxs-lookup"><span data-stu-id="d44b6-221">Partners without sandbox access can learn about the changes in this topic.</span></span>|
|<span data-ttu-id="d44b6-222">2019 年 9 月 3 日</span><span class="sxs-lookup"><span data-stu-id="d44b6-222">September 03, 2019</span></span>|<span data-ttu-id="d44b6-223">在沙盒中提供 API 预览版。</span><span class="sxs-lookup"><span data-stu-id="d44b6-223">API preview is available in sandbox.</span></span>|<span data-ttu-id="d44b6-224">合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心 API 确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-224">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center API in CSP sandbox environment.</span></span> <span data-ttu-id="d44b6-225">API 合作伙伴可以利用此机会预览 API 更改，并开始使用 API 集成为新协议提供支持。</span><span class="sxs-lookup"><span data-stu-id="d44b6-225">API partners can use this opportunity to preview the API changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="d44b6-226">2019 年 9 月 20 日</span><span class="sxs-lookup"><span data-stu-id="d44b6-226">September 20, 2019</span></span>|<span data-ttu-id="d44b6-227">在沙盒中提供 .NET SDK 预览版。</span><span class="sxs-lookup"><span data-stu-id="d44b6-227">.NET SDK preview is available in sandbox.</span></span>|<span data-ttu-id="d44b6-228">合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心 .NET SDK 来确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-228">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center .NET SDK in CSP sandbox environment.</span></span> <span data-ttu-id="d44b6-229">API 合作伙伴可以利用此机会预览 .NET SDK 更改，并开始使用 API 集成为新协议提供支持。</span><span class="sxs-lookup"><span data-stu-id="d44b6-229">API partners can use this opportunity to preview the .NET SDK changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="d44b6-230">2019 年 10 月 1 日</span><span class="sxs-lookup"><span data-stu-id="d44b6-230">October 01, 2019</span></span>|<span data-ttu-id="d44b6-231">在生产环境中提供 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-231">Microsoft Customer Agreement available in production</span></span>|<span data-ttu-id="d44b6-232">Microsoft 推出针对云解决方案提供商计划的 Microsoft 客户协议，替代 Microsoft 云协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-232">Microsoft introduces the Microsoft Customer Agreement to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="d44b6-233">合作伙伴可以在生产环境中使用合作伙伴中心面板和 API 确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-233">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span> <span data-ttu-id="d44b6-234">Microsoft 云协议在云解决方案提供商合作伙伴计划中仍受支持。</span><span class="sxs-lookup"><span data-stu-id="d44b6-234">The Microsoft Cloud Agreement remains supported within the CSP partner program.</span></span> <span data-ttu-id="d44b6-235">不过，我们建议合作伙伴着手迁移到 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-235">However, partners are advised to start migrating to the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d44b6-236">进行新的购买以及对现有订阅进行许可证计数更改时，都会要求合作伙伴确认 Microsoft 客户协议或 Microsoft 云协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-236">New purchases and license count changes to existing subscriptions will require partner confirmation of either the Microsoft Customer Agreement or the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="d44b6-237">某些新的套餐（例如，新的 Azure 计划）会要求确认 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-237">Certain new offers (for example, the new Azure plan) will require confirmation of the Microsoft Customer Agreement.</span></span>|
|<span data-ttu-id="d44b6-238">2020 年 1 月 31 日</span><span class="sxs-lookup"><span data-stu-id="d44b6-238">January 31, 2020</span></span>|<span data-ttu-id="d44b6-239">已从生产环境中删除 Microsoft 云协议</span><span class="sxs-lookup"><span data-stu-id="d44b6-239">Microsoft Cloud Agreement removed from production</span></span>|<span data-ttu-id="d44b6-240">云解决方案提供商合作伙伴计划不再接受 Microsoft 云协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-240">The Microsoft Cloud Agreement is no longer accepted within the CSP partner program.</span></span> <span data-ttu-id="d44b6-241">进行新的购买以及对现有订阅进行许可证计数更改时，都会要求合作伙伴确认 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-241">New purchases and license count changes to existing subscriptions will require the partner to provide confirmation of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="d44b6-242">此要求适用于新客户以及可能在以前接受了 Microsoft 云协议的现有客户。</span><span class="sxs-lookup"><span data-stu-id="d44b6-242">This requirement applies to new customers and existing customers who may have previously accepted the Microsoft Cloud Agreement.</span></span>|
|<span data-ttu-id="d44b6-243">2020 年 2 月 3 日</span><span class="sxs-lookup"><span data-stu-id="d44b6-243">February 3, 2020</span></span>|<span data-ttu-id="d44b6-244">合作伙伴现在可以使用相关选项，通过 URL 邀请客户在经身份验证的 Microsoft 365 管理中心查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-244">Partner now has the option to invite the customer via a URL to review and accept the agreement in authenticated Microsoft 365 Admin Center.</span></span> | <span data-ttu-id="d44b6-245">客户可以在 Microsoft 365 管理中心接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="d44b6-245">Customer can accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="d44b6-246">客户在 Microsoft 365 管理中心直接接受协议即可确认对条款进行了批准。</span><span class="sxs-lookup"><span data-stu-id="d44b6-246">Customer's direct acceptance of the agreement in Microsoft 365 Admin Center confirms approval of terms.</span></span> 
