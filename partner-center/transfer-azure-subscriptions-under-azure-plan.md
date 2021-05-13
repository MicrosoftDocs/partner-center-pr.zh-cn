---
title: 将 Azure 计划下的 Azure 订阅转移到其他 CSP 合作伙伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何更改与云解决方案提供商 Azure 计划下客户的 Azure 订阅关联的计划合作伙伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856043"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="adc6b-103">将客户的 Azure 计划订阅转移到其他合作伙伴</span><span class="sxs-lookup"><span data-stu-id="adc6b-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="adc6b-104">**适当角色**：帐户管理员|销售代理|计费代理</span><span class="sxs-lookup"><span data-stu-id="adc6b-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="adc6b-105">本文介绍客户如何在 Azure 计划下将 Azure 订阅从一个云解决方案提供商云解决方案提供商 (切换到另) 云解决方案提供商。</span><span class="sxs-lookup"><span data-stu-id="adc6b-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="adc6b-106">若要从其他合作伙伴切换客户的 Azure 订阅，请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="adc6b-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="adc6b-107">合作伙伴和客户都有完成的步骤。</span><span class="sxs-lookup"><span data-stu-id="adc6b-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="adc6b-108">只有与 Microsoft 有直接计费关系的合作伙伴才能访问转换工具。</span><span class="sxs-lookup"><span data-stu-id="adc6b-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="adc6b-109">间接经销商必须与间接提供商合作，以利用此转换工具。</span><span class="sxs-lookup"><span data-stu-id="adc6b-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="adc6b-110">在利用此工具之前，客户 (与) 合作伙伴对话。</span><span class="sxs-lookup"><span data-stu-id="adc6b-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="adc6b-111">需要使脱机对话避免混淆和改动。</span><span class="sxs-lookup"><span data-stu-id="adc6b-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="adc6b-112">此外，合作伙伴和客户应在启动转换之前了解这些注意事项和先决条件：</span><span class="sxs-lookup"><span data-stu-id="adc6b-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="adc6b-113">**主要注意事项：**</span><span class="sxs-lookup"><span data-stu-id="adc6b-113">**Key considerations:**</span></span>

- <span data-ttu-id="adc6b-114">Azure 预留不会随订阅转移到未来的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="adc6b-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="adc6b-115">当前合作伙伴下 Azure 服务的 CSP 定价不会转换</span><span class="sxs-lookup"><span data-stu-id="adc6b-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="adc6b-116">客户的支持责任将转移到未来的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="adc6b-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="adc6b-117">转移时，计费和开票将转移到未来的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="adc6b-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="adc6b-118">Azure Role-Based 访问控制 (RBAC) 不受传输影响</span><span class="sxs-lookup"><span data-stu-id="adc6b-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="adc6b-119">默认情况下， (AOBO) 不会向未来合作伙伴授予管理员权限</span><span class="sxs-lookup"><span data-stu-id="adc6b-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="adc6b-120">只要产品通过市场资格检查，第三方市场产品就会转移。</span><span class="sxs-lookup"><span data-stu-id="adc6b-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="adc6b-121">没有特殊折扣或区域限制</span><span class="sxs-lookup"><span data-stu-id="adc6b-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="adc6b-122">产品不是基于订阅的</span><span class="sxs-lookup"><span data-stu-id="adc6b-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="adc6b-123">将来的合作伙伴应与发布者合作，以确保它们位于产品部署的允许列表中</span><span class="sxs-lookup"><span data-stu-id="adc6b-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="adc6b-124">如果未满足所有这些条件，则应取消应用商店产品、已转让的 Azure 订阅，然后重新购买具有新合作伙伴的 Marketplace 产品</span><span class="sxs-lookup"><span data-stu-id="adc6b-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="adc6b-125">**先决条件：**</span><span class="sxs-lookup"><span data-stu-id="adc6b-125">**Prerequisites:**</span></span>

- <span data-ttu-id="adc6b-126">客户根据当前的 CSP 合作伙伴的转换意图</span><span class="sxs-lookup"><span data-stu-id="adc6b-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="adc6b-127">将来的 CSP 合作伙伴与客户合作，以确保可满足客户需求</span><span class="sxs-lookup"><span data-stu-id="adc6b-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="adc6b-128">将来的 CSP 合作伙伴与客户建立关系，并在转换开始之前购买 Azure 计划</span><span class="sxs-lookup"><span data-stu-id="adc6b-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="adc6b-129">客户必须向 Microsoft 客户协议签署未来的 CSP 合作伙伴</span><span class="sxs-lookup"><span data-stu-id="adc6b-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="adc6b-130">将来的 CSP 合作伙伴必须已签署 Microsoft 合作伙伴协议，才能使用此工具</span><span class="sxs-lookup"><span data-stu-id="adc6b-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="adc6b-131">要完成的客户任务</span><span class="sxs-lookup"><span data-stu-id="adc6b-131">Customer tasks to be completed</span></span>

<span data-ttu-id="adc6b-132">若要在 Azure 计划下传输 Azure 订阅，客户必须通过联系当前合作伙伴来启动该过程。</span><span class="sxs-lookup"><span data-stu-id="adc6b-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="adc6b-133">他们应收集当前合作伙伴的公司名称和域，以使其未来合作伙伴可以代表他们填写传输请求表单。</span><span class="sxs-lookup"><span data-stu-id="adc6b-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="adc6b-134">客户还必须确定他们希望从当前合作伙伴那里传输的订阅。</span><span class="sxs-lookup"><span data-stu-id="adc6b-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="adc6b-135">不能更改 Office 365、企业移动性套件或 Microsoft Dynamics CRM 订阅的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="adc6b-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="adc6b-136">这是未来合作伙伴负责完成传输请求窗体的责任。</span><span class="sxs-lookup"><span data-stu-id="adc6b-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="adc6b-137">Microsoft 不能代表客户或当前合作伙伴进行干预。</span><span class="sxs-lookup"><span data-stu-id="adc6b-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="adc6b-138">客户应计划与未来和当前合作伙伴密切合作，使过渡顺利进行。</span><span class="sxs-lookup"><span data-stu-id="adc6b-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="adc6b-139">要完成的未来合作伙伴任务</span><span class="sxs-lookup"><span data-stu-id="adc6b-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="adc6b-140">未来的订阅合作伙伴需要从合作伙伴中心完成一个传输请求表单，请求订阅转让：</span><span class="sxs-lookup"><span data-stu-id="adc6b-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="adc6b-141">从 "合作伙伴中心" 菜单中，选择 " **客户**"，然后选择要代表其完成传输请求表单的客户。</span><span class="sxs-lookup"><span data-stu-id="adc6b-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="adc6b-142">从 "客户" 菜单中选择 " **订阅**"。</span><span class="sxs-lookup"><span data-stu-id="adc6b-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="adc6b-143">选择" **转移请求"** 部分。</span><span class="sxs-lookup"><span data-stu-id="adc6b-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="adc6b-144">在"**传输请求"部分中**，选择 **"添加新请求"。**</span><span class="sxs-lookup"><span data-stu-id="adc6b-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="传输部分":::

5.  <span data-ttu-id="adc6b-146">填写" **新建转移请求"** 表单。</span><span class="sxs-lookup"><span data-stu-id="adc6b-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="adc6b-147">选择 **"发送传输请求发送**  >  **"。**</span><span class="sxs-lookup"><span data-stu-id="adc6b-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="完整的转移请求表单":::

7.  <span data-ttu-id="adc6b-149">查看传输请求确认</span><span class="sxs-lookup"><span data-stu-id="adc6b-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="查看挂起的传输":::

    >[!Note]
    ><span data-ttu-id="adc6b-151">只有当转移请求状态为"挂起"时，未来的合作伙伴才能通过在右上角选择"取消请求"来取消转移请求。</span><span class="sxs-lookup"><span data-stu-id="adc6b-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="adc6b-152">传输请求状态为"正在进行"或"已完成"后，将不能取消。</span><span class="sxs-lookup"><span data-stu-id="adc6b-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="adc6b-153">当前要完成的合作伙伴任务</span><span class="sxs-lookup"><span data-stu-id="adc6b-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="adc6b-154">客户的当前合作伙伴的管理员代理将收到一封电子邮件，其中客户正在请求转移其订阅：</span><span class="sxs-lookup"><span data-stu-id="adc6b-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="检讨":::

<span data-ttu-id="adc6b-156">查看并接受来自 合作伙伴中心的转移请求表单，以完成订阅转移。</span><span class="sxs-lookup"><span data-stu-id="adc6b-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="adc6b-157">如果当前合作伙伴在 30 天内未采取任何操作，则请求将过期，并且未来合作伙伴将拥有创建新的转移请求的 。</span><span class="sxs-lookup"><span data-stu-id="adc6b-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="adc6b-158">从 **电子邮件中选择"查看** 转移请求"或</span><span class="sxs-lookup"><span data-stu-id="adc6b-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="adc6b-159">在"合作伙伴中心"菜单中，选择"客户"，然后选择已代表提交转移请求的客户。</span><span class="sxs-lookup"><span data-stu-id="adc6b-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="adc6b-160">在"客户"菜单中，选择"**订阅"。**</span><span class="sxs-lookup"><span data-stu-id="adc6b-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="adc6b-161">选择" **转移请求"** 部分。</span><span class="sxs-lookup"><span data-stu-id="adc6b-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="adc6b-162">通过在"已接收请求"下选择 **所选的"传输请求 ID"\*\*\*\*来展开传输信息**</span><span class="sxs-lookup"><span data-stu-id="adc6b-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="源审阅传输请求":::

5.  <span data-ttu-id="adc6b-164">查看传输请求。</span><span class="sxs-lookup"><span data-stu-id="adc6b-164">Review transfer request.</span></span> <span data-ttu-id="adc6b-165">选择要传输的请求的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="adc6b-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="adc6b-166">请注意，在继续操作之前，你将无法再访问所选订阅。</span><span class="sxs-lookup"><span data-stu-id="adc6b-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="adc6b-167">不会向你开具发票以便进一步使用。</span><span class="sxs-lookup"><span data-stu-id="adc6b-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="adc6b-168">Azure 预订不会与订阅一起传输。</span><span class="sxs-lookup"><span data-stu-id="adc6b-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="adc6b-169">然后选择 " **接受并传输** " 完成传输过程。</span><span class="sxs-lookup"><span data-stu-id="adc6b-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="选择要在 Azure 计划下传输的订阅":::

7.  <span data-ttu-id="adc6b-171">查看传输接受确认。</span><span class="sxs-lookup"><span data-stu-id="adc6b-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="adc6b-172">此时，将通过电子邮件向未来合作伙伴、客户和当前合作伙伴发送接受的传输请求通知。</span><span class="sxs-lookup"><span data-stu-id="adc6b-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="adc6b-173">在此之后，转换已被接受：传输状态可能在系统更新时保持挂起状态最多15分钟。</span><span class="sxs-lookup"><span data-stu-id="adc6b-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="adc6b-174">如果需要更长时间，系统将继续尝试3天。</span><span class="sxs-lookup"><span data-stu-id="adc6b-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="adc6b-175">如果传输状态仍处于挂起状态，则合作伙伴应提交服务请求。</span><span class="sxs-lookup"><span data-stu-id="adc6b-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="adc6b-176">传输完成后，请求中包含的订阅将显示在未来合作伙伴的 Azure 计划中，不再与你一起列出。</span><span class="sxs-lookup"><span data-stu-id="adc6b-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="adc6b-177">对于间接提供程序：请通知间接经销商已接受传输请求。</span><span class="sxs-lookup"><span data-stu-id="adc6b-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="adc6b-178">管理已传输的客户订阅</span><span class="sxs-lookup"><span data-stu-id="adc6b-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="adc6b-179">在转换期间，使用 Azure 基于角色的访问控制 (RBAC) 为现有用户、组或服务主体分配的访问权限不受影响。</span><span class="sxs-lookup"><span data-stu-id="adc6b-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="adc6b-180">Azure [ RBAC) ](/azure/role-based-access-control/overview) 的基于角色的访问控制 (可帮助你的客户管理有权访问 Azure 资源的人员、他们可以使用这些资源执行哪些操作，以及他们有权访问哪些区域。</span><span class="sxs-lookup"><span data-stu-id="adc6b-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="adc6b-181">作为新合作伙伴，你不会在订阅转让后向你的客户的资源提供任何 RBAC 访问权限。</span><span class="sxs-lookup"><span data-stu-id="adc6b-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="adc6b-182">你的客户的上一个合作伙伴将保留其 RBAC 访问权限。</span><span class="sxs-lookup"><span data-stu-id="adc6b-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="adc6b-183">与客户合作，了解谁有权了解他们的订阅以及如何进行任何所需的更改。</span><span class="sxs-lookup"><span data-stu-id="adc6b-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="adc6b-184">因此，客户必须删除其上一合作伙伴的 Azure RBAC 访问权限，并添加新合作伙伴的访问权限。</span><span class="sxs-lookup"><span data-stu-id="adc6b-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="adc6b-185">有关客户提供新访问权限的信息，请参阅什么是[Azure RBAC](/azure/role-based-access-control/overview) (Azure 基于角色的) ？</span><span class="sxs-lookup"><span data-stu-id="adc6b-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="adc6b-186">有关客户删除以前合作伙伴的 RBAC 访问权限详细信息，请参阅 [删除角色分配](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。</span><span class="sxs-lookup"><span data-stu-id="adc6b-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="adc6b-187">此外，你不会自动代表管理员访问 ([AOBO ](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)) 订阅。</span><span class="sxs-lookup"><span data-stu-id="adc6b-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="adc6b-188">合作伙伴的 需要 AOBO 来代表他们管理客户的 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="adc6b-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="adc6b-189">有关 Azure 特权的信息，请参阅 [获取管理客户的服务或订阅的权限。](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="adc6b-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="adc6b-190">后续步骤：</span><span class="sxs-lookup"><span data-stu-id="adc6b-190">Next steps:</span></span>

- [<span data-ttu-id="adc6b-191"> (Azure RBAC) </span><span class="sxs-lookup"><span data-stu-id="adc6b-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="adc6b-192">获取管理客户的服务或订阅的权限。</span><span class="sxs-lookup"><span data-stu-id="adc6b-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
