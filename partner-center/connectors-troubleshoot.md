---
title: 联合销售引荐连接器疑难解答
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解有关使用联合销售连接器的常见问题的解答。 阅读此常见问题解答，了解如何排查联合销售连接器问题。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276920"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="e23a8-104">联合销售引荐连接器疑难解答</span><span class="sxs-lookup"><span data-stu-id="e23a8-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="e23a8-105">**适用于：Dynamics** 365 CRM |Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e23a8-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="e23a8-106">**适当的角色**：引荐管理员|CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="e23a8-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="e23a8-107">有关先决条件的问题和解答</span><span class="sxs-lookup"><span data-stu-id="e23a8-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="e23a8-108">能否为环境使用试用联合销售引荐连接器解决方案？</span><span class="sxs-lookup"><span data-stu-id="e23a8-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="e23a8-109">如果位于测试/过渡环境中，可以选择试用解决方案。</span><span class="sxs-lookup"><span data-stu-id="e23a8-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="e23a8-110">AppSource 中提供的连接器付费版本为 15 美元/月。</span><span class="sxs-lookup"><span data-stu-id="e23a8-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="e23a8-111">使用付费连接时，你每天将收到 10，000 个 API 调用。</span><span class="sxs-lookup"><span data-stu-id="e23a8-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="e23a8-112">连接器是引用 API 合作伙伴中心包装器。</span><span class="sxs-lookup"><span data-stu-id="e23a8-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="e23a8-113">每当连接器解决方案在客户端或CRM端针对合作伙伴中心创建或更新事件运行时，都会进行 API 调用。</span><span class="sxs-lookup"><span data-stu-id="e23a8-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="e23a8-114">在 CRM 环境中创建节需要哪些角色？</span><span class="sxs-lookup"><span data-stu-id="e23a8-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="e23a8-115">作为系统管理员或系统定制员的用户可以针对每个人应用更改。</span><span class="sxs-lookup"><span data-stu-id="e23a8-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="e23a8-116">但是，所有应用用户可以对系统进行个性化设置，甚至可以与他人共享一些自定义项。</span><span class="sxs-lookup"><span data-stu-id="e23a8-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="e23a8-117">合作伙伴销售人员是否需要特殊角色来处理合作伙伴中心？</span><span class="sxs-lookup"><span data-stu-id="e23a8-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="e23a8-118">合作伙伴销售人员必须分配有"引荐管理员"角色。</span><span class="sxs-lookup"><span data-stu-id="e23a8-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="e23a8-119">有关详细信息，请参阅 [权限概述](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="e23a8-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="e23a8-120">首先需要在 CRM 环境中设置哪些字段？</span><span class="sxs-lookup"><span data-stu-id="e23a8-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="e23a8-121">• 确保你的货币适合你的位置，并且准确位于 CRM 环境中。</span><span class="sxs-lookup"><span data-stu-id="e23a8-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="e23a8-122">• 你的销售团队应作为 CRM 用户列在 CRM 环境中。</span><span class="sxs-lookup"><span data-stu-id="e23a8-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="e23a8-123">创建环境需要哪些Power Automate先决条件？</span><span class="sxs-lookup"><span data-stu-id="e23a8-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="e23a8-124">若要使用Power Automate环境，需要：</span><span class="sxs-lookup"><span data-stu-id="e23a8-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="e23a8-125">需要Power Automate许可证。</span><span class="sxs-lookup"><span data-stu-id="e23a8-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="e23a8-126">至少需要 1 GB 存储。</span><span class="sxs-lookup"><span data-stu-id="e23a8-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="e23a8-127">是否需要 Dynamics 365 订阅来使用 Salesforce Connectors 解决方案？</span><span class="sxs-lookup"><span data-stu-id="e23a8-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="e23a8-128">Salesforce 连接器解决方案的类型为"Dynamics Flow"，支持与其他 CRM 系统同步。</span><span class="sxs-lookup"><span data-stu-id="e23a8-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="e23a8-129">该解决方案不要求你拥有 Dynamics 365 实例或订阅。</span><span class="sxs-lookup"><span data-stu-id="e23a8-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="e23a8-130">安装 Salesforce 解决方案时，可能会显示公司中现有 CDS 环境的下拉列表。</span><span class="sxs-lookup"><span data-stu-id="e23a8-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="e23a8-131">需要选择该环境。</span><span class="sxs-lookup"><span data-stu-id="e23a8-131">You need to select that environment.</span></span> <span data-ttu-id="e23a8-132">此外，如果收到错误"找不到已登录用户的 Dynamics 365 组织"，则需要为连接器创建新环境。</span><span class="sxs-lookup"><span data-stu-id="e23a8-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="e23a8-133">有关配置的问题和解答</span><span class="sxs-lookup"><span data-stu-id="e23a8-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="e23a8-134">如果在激活 Power Automate Platform 中的流时出现以下错误，应Power Automate操作？</span><span class="sxs-lookup"><span data-stu-id="e23a8-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="e23a8-135">错误：对 Azure 资源管理器 的请求失败，出现错误："{"error"：{"code"："WorkflowTriggerNotFound"，"message"："找不到工作流 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' 触发器 'manual'"。"}}"。</span><span class="sxs-lookup"><span data-stu-id="e23a8-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="e23a8-136">请按照以下故障排除步骤操作：</span><span class="sxs-lookup"><span data-stu-id="e23a8-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="e23a8-137">删除 CDS 连接，然后重新创建 CDS 连接。</span><span class="sxs-lookup"><span data-stu-id="e23a8-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="e23a8-138">关闭和打开子流</span><span class="sxs-lookup"><span data-stu-id="e23a8-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="e23a8-139">删除解决方案，然后重新安装解决方案。</span><span class="sxs-lookup"><span data-stu-id="e23a8-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="e23a8-140">如果在 Power Automate Platform 中添加 合作伙伴中心 连接器时出现"登录"错误，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="需要登录的错误消息。":::

<span data-ttu-id="e23a8-142">按照以下故障排除步骤操作：</span><span class="sxs-lookup"><span data-stu-id="e23a8-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="e23a8-143">使用合作伙伴中心凭据登录流环境后 (flow.microsoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="e23a8-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="e23a8-144">如果在 Power Automate Platform 中激活 合作伙伴中心 CRM 流时收到以下错误，应Power Automate操作？</span><span class="sxs-lookup"><span data-stu-id="e23a8-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="需要更新的错误消息。":::

<span data-ttu-id="e23a8-146">请按照以下故障排除步骤操作：</span><span class="sxs-lookup"><span data-stu-id="e23a8-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="e23a8-147">先激活以下两个子流，然后再激活合作伙伴中心 CRM 流。</span><span class="sxs-lookup"><span data-stu-id="e23a8-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="e23a8-148">合作伙伴中心 CRM - Helper (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="e23a8-149">合作伙伴中心 Microsoft 联合销售 CRM 引荐更新 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="e23a8-150">尝试编辑流时，如果无法向流添加连接，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="e23a8-151">在流运行时向流添加连接，并单独添加到每个流。</span><span class="sxs-lookup"><span data-stu-id="e23a8-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="e23a8-152">如果在编辑流时用于添加连接的对话框未自动打开，可以单独编辑流的每个步骤和子步骤。</span><span class="sxs-lookup"><span data-stu-id="e23a8-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="e23a8-153">选择每个流并单独编辑它们。</span><span class="sxs-lookup"><span data-stu-id="e23a8-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="e23a8-154">展开流中的所有步骤</span><span class="sxs-lookup"><span data-stu-id="e23a8-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="需要连接的步骤。":::

- <span data-ttu-id="e23a8-156">选择一些步骤，其中会显示一个警告图标，要求关联连接并添加连接。</span><span class="sxs-lookup"><span data-stu-id="e23a8-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="分步编辑流。":::


5. <span data-ttu-id="e23a8-158">如果联合销售引荐连接器解决方案流没有打开，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="e23a8-159">A.</span><span class="sxs-lookup"><span data-stu-id="e23a8-159">A.</span></span> <span data-ttu-id="e23a8-160">在Power Automate中，需要按以下顺序编辑流，并更新流以使用正确的连接：</span><span class="sxs-lookup"><span data-stu-id="e23a8-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="e23a8-161">合作伙伴中心预览体验版 (Webhook 注册) </span><span class="sxs-lookup"><span data-stu-id="e23a8-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="e23a8-162">创建联合销售引荐 - Salesforce 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e23a8-163">合作伙伴中心 Microsoft 联合销售 Salesforce (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e23a8-164">合作伙伴中心 Insider Preview (Salesforce) </span><span class="sxs-lookup"><span data-stu-id="e23a8-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e23a8-165">Salesforce 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e23a8-166">Salesforce 预览体验合作伙伴中心 (预览版) </span><span class="sxs-lookup"><span data-stu-id="e23a8-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e23a8-167">Salesforce Microsoft Solutions to 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="e23a8-168">B.</span><span class="sxs-lookup"><span data-stu-id="e23a8-168">B.</span></span> <span data-ttu-id="e23a8-169">对于每个流，选择" **仅运行用户"** 选项。</span><span class="sxs-lookup"><span data-stu-id="e23a8-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="e23a8-170">选择 **"使用连接**"，而不是"**由仅运行用户提供"。**</span><span class="sxs-lookup"><span data-stu-id="e23a8-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="激活流。":::


<span data-ttu-id="e23a8-172">C.</span><span class="sxs-lookup"><span data-stu-id="e23a8-172">C.</span></span> <span data-ttu-id="e23a8-173">激活下面提到的流：</span><span class="sxs-lookup"><span data-stu-id="e23a8-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="e23a8-174">合作伙伴中心 Microsoft 联合销售 Salesforce (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="e23a8-175">Salesforce 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="e23a8-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="e23a8-176">D.</span><span class="sxs-lookup"><span data-stu-id="e23a8-176">D.</span></span> <span data-ttu-id="e23a8-177">激活所有剩余流。</span><span class="sxs-lookup"><span data-stu-id="e23a8-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="e23a8-178">E.</span><span class="sxs-lookup"><span data-stu-id="e23a8-178">E.</span></span> <span data-ttu-id="e23a8-179">在"Webhook 合作伙伴中心流中，选择"运行 **"。**</span><span class="sxs-lookup"><span data-stu-id="e23a8-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="e23a8-180">提供 **Salesforce** 流中第一个合作伙伴中心 **的 http** URL。</span><span class="sxs-lookup"><span data-stu-id="e23a8-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="e23a8-181">在"要注册的事件 **"下选择所有四个选项，然后选择\*\*\*\*"是**"作为"覆盖"。</span><span class="sxs-lookup"><span data-stu-id="e23a8-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="e23a8-182">有关运行/维护的问题和解答</span><span class="sxs-lookup"><span data-stu-id="e23a8-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="e23a8-183">如何排查流执行Power Automate故障？</span><span class="sxs-lookup"><span data-stu-id="e23a8-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="e23a8-184">若要确保流Power Automate运行，并排查执行期间失败的问题，请参阅 [修复流失败](/power-automate/fix-flow-failures)。</span><span class="sxs-lookup"><span data-stu-id="e23a8-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="e23a8-185">如果看到在用户或 CRM 环境中未正确同步的引荐合作伙伴中心该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="e23a8-186">若要确定引荐同步的状态，请选择"审核 **"。**</span><span class="sxs-lookup"><span data-stu-id="e23a8-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="如何同步引荐。":::

<span data-ttu-id="e23a8-188">确保满足以下条件：</span><span class="sxs-lookup"><span data-stu-id="e23a8-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="e23a8-189">解决方案 ID 作为机会的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="e23a8-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="e23a8-190">需要两个字母的国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="e23a8-190">Two letter country code is required.</span></span>

- <span data-ttu-id="e23a8-191">选择 Microsoft 的帮助作为机会时，需要客户联系信息。</span><span class="sxs-lookup"><span data-stu-id="e23a8-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="e23a8-192">如何确保引荐双向同步？</span><span class="sxs-lookup"><span data-stu-id="e23a8-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="e23a8-193">执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="e23a8-193">Do the following steps:</span></span>

- <span data-ttu-id="e23a8-194">合作伙伴销售人员需要确保他们已启用 CRM 部分 **中的"合作伙伴中心** 同步"选项。</span><span class="sxs-lookup"><span data-stu-id="e23a8-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="确保已启用 Synch。":::

- <span data-ttu-id="e23a8-196">在限定潜在客户时，销售人员需要提供收入和结束日期。</span><span class="sxs-lookup"><span data-stu-id="e23a8-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="e23a8-197">如果在联合销售机会的创建或更新阶段中提供了 CRM ID，但在 CRM 中找不到具有该 ID 的潜在顾客机会，则更新或创建将被忽略。</span><span class="sxs-lookup"><span data-stu-id="e23a8-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="e23a8-198">确保在 Salesforce 环境中配置引荐货币字段。</span><span class="sxs-lookup"><span data-stu-id="e23a8-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="e23a8-199">如果连接器断开连接并错过引荐同步，该怎么办？。</span><span class="sxs-lookup"><span data-stu-id="e23a8-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="e23a8-200">下面是可以尝试的一些选项：</span><span class="sxs-lookup"><span data-stu-id="e23a8-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="e23a8-201">检查具有引荐管理员角色的用户的用户名合作伙伴中心密码是否已过期。</span><span class="sxs-lookup"><span data-stu-id="e23a8-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="e23a8-202">可以转到未同步的机会，进行次要更新，并观察引荐是否已同步。</span><span class="sxs-lookup"><span data-stu-id="e23a8-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="e23a8-203">如果流已运行且失败，请选择流，然后重新提交失败的运行。</span><span class="sxs-lookup"><span data-stu-id="e23a8-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="e23a8-204">出现访问被拒绝错误时，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="e23a8-205">确保存在适当的角色</span><span class="sxs-lookup"><span data-stu-id="e23a8-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="e23a8-206">卖方的引荐合作伙伴中心管理员角色</span><span class="sxs-lookup"><span data-stu-id="e23a8-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="e23a8-207">CRM 实例上的系统管理员或系统定制员角色</span><span class="sxs-lookup"><span data-stu-id="e23a8-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="e23a8-208">确保Power Automate帐户用户事先至少 https://flow.microsoft.com 登录一次</span><span class="sxs-lookup"><span data-stu-id="e23a8-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="e23a8-209">如果在创建联合销售机会 **时** 发现缺少客户帐户国家/地区代码，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="e23a8-210">需要将 ISO 双字母国家/地区代码添加到 CRM 中的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="e23a8-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="e23a8-211">如果在创建联合销售机会时看到"解决方案 **ID** 是必需的"错误，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="e23a8-212">若要创建联合销售引荐，需要 Microsoft 联合销售就绪解决方案。</span><span class="sxs-lookup"><span data-stu-id="e23a8-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="e23a8-213">如果看到在云中创建的联合销售机会合作伙伴中心即使没有流错误，也未同步到 CRM 时，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="e23a8-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="e23a8-214">请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e23a8-214">Do the following:</span></span>

- <span data-ttu-id="e23a8-215">在 合作伙伴中心 中创建了新的联合销售交易后，请检查是否调用了 合作伙伴中心 到 Dynamics 365 流的 (它可能会多次) 。</span><span class="sxs-lookup"><span data-stu-id="e23a8-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="e23a8-216">如果调用了流，请检查所有调用的流，并确定将更新 CRM 的流运行。</span><span class="sxs-lookup"><span data-stu-id="e23a8-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="e23a8-217">可以按照操作操作并验证它是否更新了 CRM 或遇到了问题。</span><span class="sxs-lookup"><span data-stu-id="e23a8-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="e23a8-218">检查 **"新建** 合作伙伴中心，查看其是否填充了 CRM ID。</span><span class="sxs-lookup"><span data-stu-id="e23a8-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="e23a8-219">确保交易不会意外以"赢得"或"丢失"状态在合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="e23a8-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e23a8-220">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e23a8-220">Next steps</span></span>

- [<span data-ttu-id="e23a8-221">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="e23a8-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="e23a8-222">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="e23a8-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
