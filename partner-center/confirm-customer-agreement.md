---
title: 如何确认客户已接受 CSP 计划的 Microsoft 客户协议
description: 云解决方案提供商 (CSP) 合作伙伴在为客户订购 Microsoft 服务之前，需要确认客户接受 Microsoft 客户协议。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633772"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="81a10-103">如何确认客户已接受 CSP 计划的 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="81a10-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="81a10-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="81a10-104">**Appropriate roles**</span></span>

- <span data-ttu-id="81a10-105">管理员代理</span><span class="sxs-lookup"><span data-stu-id="81a10-105">Admin agent</span></span>
- <span data-ttu-id="81a10-106">销售代理</span><span class="sxs-lookup"><span data-stu-id="81a10-106">Sales agent</span></span>


<span data-ttu-id="81a10-107">关于是否接受 Microsoft 客户协议，客户有两种选择。</span><span class="sxs-lookup"><span data-stu-id="81a10-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="81a10-108">**选项 1**：合作伙伴证明客户已接受 - 合作伙伴可以通过合作伙伴中心 API/SDK 或合作伙伴中心仪表板确认客户接受。</span><span class="sxs-lookup"><span data-stu-id="81a10-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="81a10-109">**选项 2**：客户直接接受 - 合作伙伴可以通过 URL 邀请客户在 Microsoft 365 管理中心查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="81a10-110">访问 Microsoft 客户协议模板</span><span class="sxs-lookup"><span data-stu-id="81a10-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="81a10-111">可以从[此处](https://aka.ms/customeragreement)手动下载最新版 Microsoft 客户协议模板。</span><span class="sxs-lookup"><span data-stu-id="81a10-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="81a10-112">Microsoft 客户协议特定于国家/地区。</span><span class="sxs-lookup"><span data-stu-id="81a10-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="81a10-113">在请求 Microsoft 客户协议模板时，请确保根据客户的位置选择正确的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="81a10-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="81a10-114">选项 1：在合作伙伴中心中确认客户已接受协议</span><span class="sxs-lookup"><span data-stu-id="81a10-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="81a10-115">对于新客户和现有客户，直接计费合作伙伴可以在合作伙伴中心确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="81a10-116">间接经销商不能代表其客户进行证明，需通过其间接提供商来完成证明。</span><span class="sxs-lookup"><span data-stu-id="81a10-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="81a10-117">确认新客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="81a10-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="81a10-118">在合作伙伴中心创建新客户租户时，请按以下步骤确认客户接受了 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="81a10-119">必须是管理员代理或销售代理才能执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="81a10-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="81a10-120">选择“客户”，然后选择“新客户”。</span><span class="sxs-lookup"><span data-stu-id="81a10-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="81a10-121">在“帐户信息”下，输入公司及其主要联系人的信息。</span><span class="sxs-lookup"><span data-stu-id="81a10-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="81a10-122">在“Microsoft 协议”下，选中相应的框来证明客户已接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="81a10-123">在“协议接受日期”  下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="81a10-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="81a10-124">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="81a10-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="81a10-125">确保显示的主要用户联系人信息正确。</span><span class="sxs-lookup"><span data-stu-id="81a10-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="81a10-126">如果不正确，请选择“更新”并输入接受该协议的人员的准确信息。</span><span class="sxs-lookup"><span data-stu-id="81a10-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="81a10-127">选择“下一步”继续创建客户租户。</span><span class="sxs-lookup"><span data-stu-id="81a10-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客户":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="81a10-129">确认现有客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="81a10-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="81a10-130">必须是管理员代理或销售代理才能执行此操作：</span><span class="sxs-lookup"><span data-stu-id="81a10-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="81a10-131">选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="81a10-131">Select **Customers**.</span></span> <span data-ttu-id="81a10-132">找到并选择客户。</span><span class="sxs-lookup"><span data-stu-id="81a10-132">Find and select the customer.</span></span>

2. <span data-ttu-id="81a10-133">选择“帐户信息”。 </span><span class="sxs-lookup"><span data-stu-id="81a10-133">Select **Account info**.</span></span>

3. <span data-ttu-id="81a10-134">在“Microsoft 客户协议”下选择“更新”。</span><span class="sxs-lookup"><span data-stu-id="81a10-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="81a10-135">输入已接受协议的人员的 **名字**、**姓氏**、**电子邮件地址** 和 **电话号码**（可选）。</span><span class="sxs-lookup"><span data-stu-id="81a10-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="81a10-136">在“协议接受日期”  下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="81a10-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="81a10-137">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="81a10-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="81a10-138">选择“保存”，然后继续操作。</span><span class="sxs-lookup"><span data-stu-id="81a10-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="现有客户":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="81a10-140">检索客户接受协议的确认信息</span><span class="sxs-lookup"><span data-stu-id="81a10-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="81a10-141">若要检索关于现有客户已接受 Microsoft 客户协议的确认信息，请使用下述步骤。</span><span class="sxs-lookup"><span data-stu-id="81a10-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="81a10-142">必须是管理员代理或销售代理才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="81a10-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="81a10-143">选择“客户”，然后找到并选择要查看的客户。</span><span class="sxs-lookup"><span data-stu-id="81a10-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="81a10-144">选择“帐户信息”。 </span><span class="sxs-lookup"><span data-stu-id="81a10-144">Select **Account info**.</span></span>

3. <span data-ttu-id="81a10-145">在“Microsoft 客户协议”下，查看该客户是否提供过确认。</span><span class="sxs-lookup"><span data-stu-id="81a10-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="81a10-146">使用合作伙伴中心 API/SDK 确认客户接受协议</span><span class="sxs-lookup"><span data-stu-id="81a10-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="81a10-147">可以使用合作伙伴中心 API/SDK 确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="81a10-148">有关 API/SDK 的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="81a10-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="81a10-149">获取 Microsoft 客户协议的协议元数据</span><span class="sxs-lookup"><span data-stu-id="81a10-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="81a10-150">确认客户接受 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="81a10-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="81a10-151">获取客户接受 Microsoft 客户协议的确认</span><span class="sxs-lookup"><span data-stu-id="81a10-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="81a10-152">获取 Microsoft 客户协议模板的下载链接</span><span class="sxs-lookup"><span data-stu-id="81a10-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="81a10-153">选项 2：客户在 Microsoft 365 管理中心接受协议</span><span class="sxs-lookup"><span data-stu-id="81a10-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="81a10-154">合作伙伴可以通过 URL 邀请新客户和现有客户在 Microsoft 365 管理中心查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="81a10-155">接下来的几部分介绍如何执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="81a10-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="81a10-156">创建一个新客户，并邀请该客户查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="81a10-157">邀请新客户查看并接受经销商关系和协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="81a10-158">邀请现有客户查看并接受协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="81a10-159">可以使用[合作伙伴中心 API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) 来获取客户直接接受 Microsoft 客户协议的状态。</span><span class="sxs-lookup"><span data-stu-id="81a10-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="81a10-160">创建一个新客户，并邀请该客户查看并接受协议</span><span class="sxs-lookup"><span data-stu-id="81a10-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="81a10-161">使用以下步骤在合作伙伴中心创建新客户，并邀请他们在 Microsoft 365 管理中心查看并接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="81a10-162">从合作伙伴中心的“客户”选项卡中，选择“添加客户”。</span><span class="sxs-lookup"><span data-stu-id="81a10-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="81a10-163">在“帐户信息”下的所有必填字段中输入新客户的信息，包括客户的公司名称和主要联系人。</span><span class="sxs-lookup"><span data-stu-id="81a10-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="81a10-164">在“客户协议”下选择“将要求客户在 Microsoft 365 管理中心接受 Microsoft 客户协议”。</span><span class="sxs-lookup"><span data-stu-id="81a10-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="81a10-165">完成页面上的所有其他必填字段。</span><span class="sxs-lookup"><span data-stu-id="81a10-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="81a10-166">选择“下一步:查看”，然后继续执行创建客户租户的步骤。</span><span class="sxs-lookup"><span data-stu-id="81a10-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="81a10-167">新客户必须接受 Microsoft 客户协议才能进行购买。</span><span class="sxs-lookup"><span data-stu-id="81a10-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="创建新客户":::

5. <span data-ttu-id="81a10-169">到达新客户工作流中的“确认”屏幕后，保存客户凭据。</span><span class="sxs-lookup"><span data-stu-id="81a10-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="81a10-170">稍后需将这些凭据分配给客户。</span><span class="sxs-lookup"><span data-stu-id="81a10-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="81a10-171">在合作伙伴中心外部，创建并发送一封电子邮件，邀请客户在 Microsoft 365 管理中心接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="81a10-172">请确保电子邮件中包含以下项：</span><span class="sxs-lookup"><span data-stu-id="81a10-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="81a10-173">此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的链接（需要登录）</span><span class="sxs-lookup"><span data-stu-id="81a10-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="81a10-174">在步骤 5 中保存的客户凭据。</span><span class="sxs-lookup"><span data-stu-id="81a10-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="81a10-175">然后，客户会收到来自合作伙伴的电子邮件邀请，并会选择 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="81a10-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="81a10-176">客户使用你提供的客户凭据登录 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="81a10-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="81a10-177">客户选中用于接受 Microsoft 客户协议的复选框。</span><span class="sxs-lookup"><span data-stu-id="81a10-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="81a10-178">邀请新客户查看并接受经销商关系和 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="81a10-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="81a10-179">通过以下步骤邀请新客户查看并接受经销商关系和 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="81a10-180">从合作伙伴中心的“客户”选项卡中选择“请求建立经销商关系”链接。</span><span class="sxs-lookup"><span data-stu-id="81a10-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="81a10-181">系统会生成自动电子邮件模板，其中包括文本和参数化 URL，用于将客户定向到 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="81a10-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="81a10-182">可以自定义自动生成的电子邮件模板，然后选择“复制到剪贴板”或“在电子邮件中打开”。</span><span class="sxs-lookup"><span data-stu-id="81a10-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="81a10-183">使用此电子邮件模板邀请客户接受 **经销商关系** 请求和 **Microsoft 客户协议**。</span><span class="sxs-lookup"><span data-stu-id="81a10-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="81a10-184">（注意：在电子邮件邀请中，请确保合作伙伴还包括自动提供的 URL 以及最近创建的客户凭据。）</span><span class="sxs-lookup"><span data-stu-id="81a10-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="创建关系":::

5. <span data-ttu-id="81a10-186">客户通过电子邮件接收邀请，并单击参数化 URL。</span><span class="sxs-lookup"><span data-stu-id="81a10-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="81a10-187">客户使用你在电子邮件中提供的凭据登录 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="81a10-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="81a10-188">客户选中用于接受 **经销商关系** 和 **Microsoft 客户协议** 的复选框。</span><span class="sxs-lookup"><span data-stu-id="81a10-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="81a10-189">在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。</span><span class="sxs-lookup"><span data-stu-id="81a10-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="81a10-190">客户可以选择一个合作伙伴来查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="81a10-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="接受协议":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="81a10-192">邀请现有客户查看并接受协议</span><span class="sxs-lookup"><span data-stu-id="81a10-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="81a10-193">通过以下步骤邀请现有客户查看并接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="81a10-194">创建包含嵌入 URL 的客户电子邮件，邀请客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="81a10-195">客户通过电子邮件接收邀请，并单击 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="81a10-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="81a10-196">客户将其凭据输入 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="81a10-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="81a10-197">客户选中用于接受 Microsoft 客户协议的复选框。</span><span class="sxs-lookup"><span data-stu-id="81a10-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="81a10-198">在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。</span><span class="sxs-lookup"><span data-stu-id="81a10-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="81a10-199">客户可以选择一个合作伙伴来查看详细信息。</span><span class="sxs-lookup"><span data-stu-id="81a10-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="客户":::

>[!NOTE]
><span data-ttu-id="81a10-201">在某些情况下，客户可能无法直接接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="81a10-202">若要详细了解这些情况，请参阅下面的“需要代表客户证明的两种情况”。</span><span class="sxs-lookup"><span data-stu-id="81a10-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="81a10-203">需要代表客户证明的两种情况</span><span class="sxs-lookup"><span data-stu-id="81a10-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="81a10-204">在两种情况下，客户可能无法在 Microsoft 365 管理中心直接接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="81a10-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="81a10-205">**情况 1**：现有客户已通过现有合作伙伴关系购买以下任何一项：产品/服务、软件或软件订阅、预留实例或 Azure 计划。</span><span class="sxs-lookup"><span data-stu-id="81a10-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="81a10-206">客户现在正在尝试进行新的购买（不包括自动续订）。</span><span class="sxs-lookup"><span data-stu-id="81a10-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="81a10-207">该客户在单击 URL 时会收到消息：“请联系你的合作伙伴，确认你接受 Microsoft 客户协议。”</span><span class="sxs-lookup"><span data-stu-id="81a10-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="81a10-208">**解决方法**：必须代表客户进行证明。</span><span class="sxs-lookup"><span data-stu-id="81a10-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Microsoft 365 管理中心页的屏幕截图，其中要求你与合作伙伴联系以确认接受 Microsoft 客户协议。":::

<span data-ttu-id="81a10-210">**情况 2**：现有客户已购买以下任何一项：产品/服务、软件和软件订阅、预留实例和 Azure 计划。</span><span class="sxs-lookup"><span data-stu-id="81a10-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="81a10-211">客户现在正在尝试通过新的合作伙伴进行新的购买。</span><span class="sxs-lookup"><span data-stu-id="81a10-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="81a10-212">在单击 Microsoft 365 管理中心的 URL 以接受新的合作伙伴关系和协议时，该客户会收到消息：“请联系你的合作伙伴，确认你接受 Microsoft 客户协议。”</span><span class="sxs-lookup"><span data-stu-id="81a10-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="81a10-213">**解决方法**：必须代表客户进行证明。</span><span class="sxs-lookup"><span data-stu-id="81a10-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="81a10-214">确认客户已接受该协议</span><span class="sxs-lookup"><span data-stu-id="81a10-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="81a10-215">如果为之前未确认过是否接受了协议的现有客户创建新订单，你将收到完成确认的提示。</span><span class="sxs-lookup"><span data-stu-id="81a10-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="81a10-216">请使用下面的过程执行此操作。</span><span class="sxs-lookup"><span data-stu-id="81a10-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="81a10-217">输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    </span><span class="sxs-lookup"><span data-stu-id="81a10-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="81a10-218">在“协议接受日期”  下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="81a10-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="81a10-219">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="81a10-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="81a10-220">选择“保存并继续”。 </span><span class="sxs-lookup"><span data-stu-id="81a10-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="81a10-221">后续步骤</span><span class="sxs-lookup"><span data-stu-id="81a10-221">Next steps</span></span>

- [<span data-ttu-id="81a10-222">验证或更新你的公司资料信息</span><span class="sxs-lookup"><span data-stu-id="81a10-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="81a10-223">Microsoft 客户协议（按区域和语言排列）</span><span class="sxs-lookup"><span data-stu-id="81a10-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
