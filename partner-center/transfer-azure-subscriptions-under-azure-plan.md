---
title: 在 Azure 计划下将 Azure 订阅转移到另一个 CSP 合作伙伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在 Azure 计划下更改与客户的 Azure 订阅关联的云解决方案提供商计划合作伙伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: f0abfdfd2fbb242f7cdbe0ded04d387ea712cce5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702716"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="b666e-103">将客户的 Azure 计划订阅转移到不同的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b666e-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="b666e-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="b666e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b666e-105">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="b666e-105">Account admin</span></span>
- <span data-ttu-id="b666e-106">销售代理</span><span class="sxs-lookup"><span data-stu-id="b666e-106">Sales agent</span></span>
- <span data-ttu-id="b666e-107">计费代理</span><span class="sxs-lookup"><span data-stu-id="b666e-107">Billing agent</span></span>

<span data-ttu-id="b666e-108">本文介绍了客户如何在 Azure 计划下从一个云解决方案提供商 (CSP) 切换到另一个云解决方案。</span><span class="sxs-lookup"><span data-stu-id="b666e-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="b666e-109">若要从其他合作伙伴切换客户的 Azure 订阅，请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="b666e-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="b666e-110">合作伙伴和客户都有完成的步骤。</span><span class="sxs-lookup"><span data-stu-id="b666e-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="b666e-111">只有与 Microsoft 直接计费关系的合作伙伴可以访问转换工具。</span><span class="sxs-lookup"><span data-stu-id="b666e-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="b666e-112">间接经销商必须与其间接提供商合作，才能利用此转换工具。</span><span class="sxs-lookup"><span data-stu-id="b666e-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="b666e-113">在利用此工具之前，客户必须与双方 (当前和未来) 合作。</span><span class="sxs-lookup"><span data-stu-id="b666e-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="b666e-114">脱机对话需要避免混淆和改动。</span><span class="sxs-lookup"><span data-stu-id="b666e-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="b666e-115">此外，在启动过渡之前，合作伙伴和客户应了解以下注意事项和先决条件：</span><span class="sxs-lookup"><span data-stu-id="b666e-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="b666e-116">**关键注意事项：**</span><span class="sxs-lookup"><span data-stu-id="b666e-116">**Key considerations:**</span></span>

- <span data-ttu-id="b666e-117">Azure 保留将不会随订阅向未来合作伙伴移动</span><span class="sxs-lookup"><span data-stu-id="b666e-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="b666e-118">当前合作伙伴提供的 Azure 服务的 CSP 定价将不会转换</span><span class="sxs-lookup"><span data-stu-id="b666e-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="b666e-119">客户的支持责任将转向未来的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b666e-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="b666e-120">计费和开具发票会在传输时移到未来合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b666e-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="b666e-121">Azure Role-Based 访问控制 (RBAC) 不受传输影响</span><span class="sxs-lookup"><span data-stu-id="b666e-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="b666e-122">默认情况下，将不会向未来伙伴授予 (AOBO) 的管理员</span><span class="sxs-lookup"><span data-stu-id="b666e-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="b666e-123">只要产品通过 Marketplace 资格检查，就会传输第三方 marketplace 产品。</span><span class="sxs-lookup"><span data-stu-id="b666e-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="b666e-124">无特殊折扣或区域限制</span><span class="sxs-lookup"><span data-stu-id="b666e-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="b666e-125">产品不是基于订阅的</span><span class="sxs-lookup"><span data-stu-id="b666e-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="b666e-126">将来的合作伙伴应与发布者合作，以确保它们位于产品部署的允许列表中</span><span class="sxs-lookup"><span data-stu-id="b666e-126">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="b666e-127">如果未满足所有这些条件，则应取消应用商店产品、已转让的 Azure 订阅，然后重新购买具有新合作伙伴的 Marketplace 产品</span><span class="sxs-lookup"><span data-stu-id="b666e-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="b666e-128">**先决条件：**</span><span class="sxs-lookup"><span data-stu-id="b666e-128">**Prerequisites:**</span></span>

- <span data-ttu-id="b666e-129">客户根据当前的 CSP 合作伙伴的转换意图</span><span class="sxs-lookup"><span data-stu-id="b666e-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="b666e-130">将来的 CSP 合作伙伴与客户合作，以确保可满足客户需求</span><span class="sxs-lookup"><span data-stu-id="b666e-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="b666e-131">将来的 CSP 合作伙伴与客户建立关系，并在转换开始之前购买 Azure 计划</span><span class="sxs-lookup"><span data-stu-id="b666e-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="b666e-132">客户必须向 Microsoft 客户协议签署未来的 CSP 合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b666e-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="b666e-133">将来的 CSP 合作伙伴必须已签署 Microsoft 合作伙伴协议，才能使用此工具</span><span class="sxs-lookup"><span data-stu-id="b666e-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="b666e-134">要完成的客户任务</span><span class="sxs-lookup"><span data-stu-id="b666e-134">Customer tasks to be completed</span></span>

<span data-ttu-id="b666e-135">若要在 Azure 计划下传输 Azure 订阅，客户必须通过联系当前合作伙伴来启动该过程。</span><span class="sxs-lookup"><span data-stu-id="b666e-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="b666e-136">他们应收集当前合作伙伴的公司名称和域，以使其未来合作伙伴可以代表他们填写传输请求表单。</span><span class="sxs-lookup"><span data-stu-id="b666e-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="b666e-137">客户还必须确定他们希望从当前合作伙伴那里传输的订阅。</span><span class="sxs-lookup"><span data-stu-id="b666e-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="b666e-138">不能更改 Office 365、企业移动性套件或 Microsoft Dynamics CRM 订阅的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="b666e-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="b666e-139">这是未来合作伙伴负责完成传输请求窗体的责任。</span><span class="sxs-lookup"><span data-stu-id="b666e-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="b666e-140">Microsoft 不能代表客户或当前合作伙伴进行干预。</span><span class="sxs-lookup"><span data-stu-id="b666e-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="b666e-141">客户应计划与未来和当前合作伙伴密切合作，使过渡顺利进行。</span><span class="sxs-lookup"><span data-stu-id="b666e-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="b666e-142">要完成的未来合作伙伴任务</span><span class="sxs-lookup"><span data-stu-id="b666e-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="b666e-143">未来的订阅合作伙伴需要从合作伙伴中心完成一个传输请求表单，请求订阅转让：</span><span class="sxs-lookup"><span data-stu-id="b666e-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="b666e-144">从 "合作伙伴中心" 菜单中，选择 " **客户**"，然后选择要代表其完成传输请求表单的客户。</span><span class="sxs-lookup"><span data-stu-id="b666e-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="b666e-145">从 "客户" 菜单中选择 " **订阅**"。</span><span class="sxs-lookup"><span data-stu-id="b666e-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="b666e-146">选择 " **传输请求** " 部分。</span><span class="sxs-lookup"><span data-stu-id="b666e-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="b666e-147">从 " **传输请求" 部分** 中，选择 " **添加新请求**"。</span><span class="sxs-lookup"><span data-stu-id="b666e-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="传输部分":::

5.  <span data-ttu-id="b666e-149">完成 " **新建传输请求** " 窗体。</span><span class="sxs-lookup"><span data-stu-id="b666e-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="b666e-150">选择 **发送传输请求**  >  **发送**。</span><span class="sxs-lookup"><span data-stu-id="b666e-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="完成传输请求窗体":::

7.  <span data-ttu-id="b666e-152">查看传输请求确认</span><span class="sxs-lookup"><span data-stu-id="b666e-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="查看挂起的传输":::

    >[!Note]
    ><span data-ttu-id="b666e-154">只有在传输请求状态为 "挂起" 时，才能通过选择右上角的 " **取消请求** " 来取消传输请求。</span><span class="sxs-lookup"><span data-stu-id="b666e-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="b666e-155">传输请求状态为 "正在进行" 或 "完成" 后，将无法取消取消。</span><span class="sxs-lookup"><span data-stu-id="b666e-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="b666e-156">当前要完成的合作伙伴任务</span><span class="sxs-lookup"><span data-stu-id="b666e-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="b666e-157">客户的当前合作伙伴的管理员代理将收到一封电子邮件，指出其客户正在请求传输其订阅：</span><span class="sxs-lookup"><span data-stu-id="b666e-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="审校":::

<span data-ttu-id="b666e-159">查看并接受合作伙伴中心的传输请求窗体，以完成订阅转移。</span><span class="sxs-lookup"><span data-stu-id="b666e-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="b666e-160">如果当前合作伙伴在30天内没有执行任何操作，则该请求将过期，将来的合作伙伴将拥有来创建新的传输请求。</span><span class="sxs-lookup"><span data-stu-id="b666e-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="b666e-161">选择电子邮件中的 " **查看传输请求** " 或</span><span class="sxs-lookup"><span data-stu-id="b666e-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="b666e-162">从 "合作伙伴中心" 菜单中，选择 " **客户**"，然后选择代表其提交了传输请求的客户。</span><span class="sxs-lookup"><span data-stu-id="b666e-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="b666e-163">从 "客户" 菜单中选择 " **订阅**"。</span><span class="sxs-lookup"><span data-stu-id="b666e-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="b666e-164">选择 " **传输请求** " 部分。</span><span class="sxs-lookup"><span data-stu-id="b666e-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="b666e-165">通过选择 "**接收的请求**" 下的所选 **传输请求 ID** 展开传输信息。</span><span class="sxs-lookup"><span data-stu-id="b666e-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="源审阅传输请求":::

5.  <span data-ttu-id="b666e-167">查看传输请求。</span><span class="sxs-lookup"><span data-stu-id="b666e-167">Review transfer request.</span></span> <span data-ttu-id="b666e-168">选择要传输的请求的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="b666e-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="b666e-169">请注意，在继续操作之前，你将无法再访问所选订阅。</span><span class="sxs-lookup"><span data-stu-id="b666e-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="b666e-170">不会向你开具发票以便进一步使用。</span><span class="sxs-lookup"><span data-stu-id="b666e-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="b666e-171">Azure 预订不会与订阅一起传输。</span><span class="sxs-lookup"><span data-stu-id="b666e-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="b666e-172">然后选择 " **接受并传输** " 完成传输过程。</span><span class="sxs-lookup"><span data-stu-id="b666e-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="选择要在 Azure 计划下传输的订阅":::

7.  <span data-ttu-id="b666e-174">查看传输接受确认。</span><span class="sxs-lookup"><span data-stu-id="b666e-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="b666e-175">此时，将通过电子邮件向未来合作伙伴、客户和当前合作伙伴发送接受的传输请求通知。</span><span class="sxs-lookup"><span data-stu-id="b666e-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="b666e-176">在此之后，转换已被接受：传输状态可能在系统更新时保持挂起状态最多15分钟。</span><span class="sxs-lookup"><span data-stu-id="b666e-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="b666e-177">如果需要更长时间，系统将继续尝试3天。</span><span class="sxs-lookup"><span data-stu-id="b666e-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="b666e-178">如果传输状态仍处于挂起状态，则合作伙伴应提交服务请求。</span><span class="sxs-lookup"><span data-stu-id="b666e-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="b666e-179">传输完成后，请求中包含的订阅将显示在未来合作伙伴的 Azure 计划中，不再与你一起列出。</span><span class="sxs-lookup"><span data-stu-id="b666e-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="b666e-180">对于间接提供程序：请通知间接经销商已接受传输请求。</span><span class="sxs-lookup"><span data-stu-id="b666e-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="b666e-181">管理已传输的客户订阅</span><span class="sxs-lookup"><span data-stu-id="b666e-181">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="b666e-182">在转换期间，使用 Azure 基于角色的访问控制 (RBAC) 为现有用户、组或服务主体分配的访问权限不受影响。</span><span class="sxs-lookup"><span data-stu-id="b666e-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="b666e-183">Azure [ RBAC) ](/azure/role-based-access-control/overview) 的基于角色的访问控制 (可帮助你的客户管理有权访问 Azure 资源的人员、他们可以使用这些资源执行哪些操作，以及他们有权访问哪些区域。</span><span class="sxs-lookup"><span data-stu-id="b666e-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="b666e-184">作为新合作伙伴，你不会在订阅转让后向你的客户的资源提供任何 RBAC 访问权限。</span><span class="sxs-lookup"><span data-stu-id="b666e-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="b666e-185">你的客户的上一个合作伙伴将保留其 RBAC 访问权限。</span><span class="sxs-lookup"><span data-stu-id="b666e-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="b666e-186">与客户合作，了解谁有权了解他们的订阅以及如何进行任何所需的更改。</span><span class="sxs-lookup"><span data-stu-id="b666e-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="b666e-187">因此，重要的是，您的客户必须删除其以前合作伙伴的 Azure RBAC 访问权限，并为新合作伙伴添加访问权限。</span><span class="sxs-lookup"><span data-stu-id="b666e-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="b666e-188">有关提供新访问权限的客户的详细信息，请参阅 [什么是 AZURE RBAC)  (azure 基于角色的访问控制？](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="b666e-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="b666e-189">若要详细了解你的客户如何删除以前合作伙伴的 RBAC 访问权限，请参阅 [删除角色分配](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。</span><span class="sxs-lookup"><span data-stu-id="b666e-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="b666e-190">此外，不会 [代表 (AOBO) ](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 访问订阅来自动获取管理员。</span><span class="sxs-lookup"><span data-stu-id="b666e-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="b666e-191">若要使合作伙伴自行管理客户的 Azure 订阅，AOBO 是必需的。</span><span class="sxs-lookup"><span data-stu-id="b666e-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="b666e-192">有关 Azure 特权的详细信息，请参阅 [获取管理客户服务或订阅的权限。](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="b666e-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="b666e-193">后续步骤：</span><span class="sxs-lookup"><span data-stu-id="b666e-193">Next steps:</span></span>

- [<span data-ttu-id="b666e-194"> (Azure RBAC) </span><span class="sxs-lookup"><span data-stu-id="b666e-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="b666e-195">获取管理客户服务或订阅的权限。</span><span class="sxs-lookup"><span data-stu-id="b666e-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
