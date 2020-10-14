---
title: 联合销售引荐连接器疑难解答
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解有关使用共同销售连接器的常见问题的解答。 阅读有关如何排查共同销售连接器问题的常见问题解答。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031260"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="543db-104">联合销售引荐连接器疑难解答</span><span class="sxs-lookup"><span data-stu-id="543db-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="543db-105">**适用对象：**</span><span class="sxs-lookup"><span data-stu-id="543db-105">**Applies to:**</span></span>

- <span data-ttu-id="543db-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="543db-106">Partner Center</span></span>
- <span data-ttu-id="543db-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="543db-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="543db-108">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="543db-108">Salesforce CRM</span></span>

<span data-ttu-id="543db-109">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="543db-109">**Appropriate roles**</span></span>

- <span data-ttu-id="543db-110">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="543db-110">Referrals admin</span></span>
- <span data-ttu-id="543db-111">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="543db-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="543db-112">有关先决条件的问题和解答</span><span class="sxs-lookup"><span data-stu-id="543db-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="543db-113">能否为你的环境使用试用共同销售引用连接器解决方案？</span><span class="sxs-lookup"><span data-stu-id="543db-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="543db-114">如果你在测试/过渡环境中，则可以选择试用版解决方案。</span><span class="sxs-lookup"><span data-stu-id="543db-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="543db-115">AppSource 的付费版连接器可在美国 $ 15/month 提供。</span><span class="sxs-lookup"><span data-stu-id="543db-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="543db-116">通过付费连接，你每天将获得 10K API 调用。</span><span class="sxs-lookup"><span data-stu-id="543db-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="543db-117">连接器是位于合作伙伴中心引用 Api 之上的包装器。</span><span class="sxs-lookup"><span data-stu-id="543db-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="543db-118">每当连接器解决方案在合作伙伴中心或 CRM 端的机会中运行 " **创建** " 或 " **更新** " 事件时，就会进行 API 调用。</span><span class="sxs-lookup"><span data-stu-id="543db-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="543db-119">在 CRM 环境中创建节需要什么角色？</span><span class="sxs-lookup"><span data-stu-id="543db-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="543db-120">作为系统管理员或系统定制员的用户可以对所有人应用更改。</span><span class="sxs-lookup"><span data-stu-id="543db-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="543db-121">不过，所有应用程序用户都可以对系统进行个性化设置，甚至与他人共享某些自定义。</span><span class="sxs-lookup"><span data-stu-id="543db-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="543db-122">合作伙伴卖方是否需要特殊角色才能在合作伙伴中心工作？</span><span class="sxs-lookup"><span data-stu-id="543db-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="543db-123">必须为合作伙伴卖方分配 "引用管理员" 角色。</span><span class="sxs-lookup"><span data-stu-id="543db-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="543db-124">有关详细信息，请参阅以下 [权限概述) # B1 创建用户帐户) 。</span><span class="sxs-lookup"><span data-stu-id="543db-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="543db-125">需要首先在 CRM 环境中设置哪些字段？</span><span class="sxs-lookup"><span data-stu-id="543db-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="543db-126">•确保你的货币适用于你所在的位置，并准确地在 CRM 环境中。</span><span class="sxs-lookup"><span data-stu-id="543db-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="543db-127">•销售团队应作为 CRM 用户列在 CRM 环境中。</span><span class="sxs-lookup"><span data-stu-id="543db-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="543db-128">电源自动执行环境创建需要哪些先决条件？</span><span class="sxs-lookup"><span data-stu-id="543db-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="543db-129">若要使用电源自动执行环境，需要：</span><span class="sxs-lookup"><span data-stu-id="543db-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="543db-130">需要使用 Power 自动许可证。</span><span class="sxs-lookup"><span data-stu-id="543db-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="543db-131">至少需要 1 GB 的存储空间。</span><span class="sxs-lookup"><span data-stu-id="543db-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="543db-132">是否需要 Dynamics 365 订阅才能使用 Salesforce 连接器解决方案？</span><span class="sxs-lookup"><span data-stu-id="543db-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="543db-133">Salesforce 连接器解决方案的类型为 "Dynamics Flow"，它支持与其他 CRM 系统同步。</span><span class="sxs-lookup"><span data-stu-id="543db-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="543db-134">此解决方案不需要你拥有 Dynamics 365 实例或订阅。</span><span class="sxs-lookup"><span data-stu-id="543db-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="543db-135">安装 Salesforce 解决方案时，可能会出现一个包含公司中现有 CD 环境的下拉状态。</span><span class="sxs-lookup"><span data-stu-id="543db-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="543db-136">需要选择该环境。</span><span class="sxs-lookup"><span data-stu-id="543db-136">You need to select that environment.</span></span> <span data-ttu-id="543db-137">此外，如果收到 "找不到连接到已登录用户的 Dynamics 365 组织" 错误，则需要为连接器创建新的环境。</span><span class="sxs-lookup"><span data-stu-id="543db-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="543db-138">有关配置的问题和解答</span><span class="sxs-lookup"><span data-stu-id="543db-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="543db-139">如果在 Power 自动化平台中激活流时遇到以下错误，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="543db-140">错误：请求 Azure 资源管理器失败，出现错误： "{" 错误 "： {" 代码 "：" WorkflowTriggerNotFound "，" message "：" 找不到工作流 "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" 触发器 "manual"。 "}}"。</span><span class="sxs-lookup"><span data-stu-id="543db-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="543db-141">请遵循以下故障排除步骤：</span><span class="sxs-lookup"><span data-stu-id="543db-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="543db-142">删除 CD 连接，然后重新创建 CD 连接。</span><span class="sxs-lookup"><span data-stu-id="543db-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="543db-143">关闭和打开子流</span><span class="sxs-lookup"><span data-stu-id="543db-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="543db-144">删除解决方案，然后重新安装解决方案。</span><span class="sxs-lookup"><span data-stu-id="543db-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="543db-145">如果在 Power 自动化平台中添加合作伙伴中心连接器时遇到 "登录" 错误，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="需要登录的错误消息":::

<span data-ttu-id="543db-147">请按照以下故障排除步骤操作：</span><span class="sxs-lookup"><span data-stu-id="543db-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="543db-148"> (flow.microsoft.com) 后，使用合作伙伴中心凭据登录到流环境。</span><span class="sxs-lookup"><span data-stu-id="543db-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="543db-149">如果在 Power 自动化平台中激活合作伙伴中心到 CRM 流时收到以下错误，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="需要登录的错误消息":::

<span data-ttu-id="543db-151">请遵循以下故障排除步骤：</span><span class="sxs-lookup"><span data-stu-id="543db-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="543db-152">激活合作伙伴中心到 CRM 流之前，先激活以下两个子流。</span><span class="sxs-lookup"><span data-stu-id="543db-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="543db-153">合作伙伴中心到 CRM-助手 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="543db-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="543db-154">合作伙伴中心 Microsoft 共同销售 CRM (有问必答预览版的参考更新) </span><span class="sxs-lookup"><span data-stu-id="543db-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="543db-155">尝试编辑流时，如果无法将连接添加到流，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="543db-156">在流运行时，将连接添加到流，并分别添加到每个流。</span><span class="sxs-lookup"><span data-stu-id="543db-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="543db-157">如果在编辑流时未自动打开用于添加连接的对话框，则可以单独编辑流的每个步骤和子步骤。</span><span class="sxs-lookup"><span data-stu-id="543db-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="543db-158">选择每个流并分别对其进行编辑。</span><span class="sxs-lookup"><span data-stu-id="543db-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="543db-159">展开流中的所有步骤</span><span class="sxs-lookup"><span data-stu-id="543db-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="需要登录的错误消息":::

- <span data-ttu-id="543db-161">选择显示警告图标的步骤，要求关联连接，然后添加连接。</span><span class="sxs-lookup"><span data-stu-id="543db-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="需要登录的错误消息":::


5. <span data-ttu-id="543db-163">如果共同销售引用连接器解决方案的流未打开，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="543db-164">A.</span><span class="sxs-lookup"><span data-stu-id="543db-164">A.</span></span> <span data-ttu-id="543db-165">在 "自动启动" 中，需要按以下顺序编辑流，并将其更新为使用正确的连接：</span><span class="sxs-lookup"><span data-stu-id="543db-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="543db-166"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="543db-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="543db-167">创建向合作伙伴中心 (内幕预览版的共同销售推荐-Salesforce) </span><span class="sxs-lookup"><span data-stu-id="543db-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="543db-168">合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) </span><span class="sxs-lookup"><span data-stu-id="543db-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="543db-169">合作伙伴中心到 Salesforce (预览体验) </span><span class="sxs-lookup"><span data-stu-id="543db-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="543db-170">Salesforce 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="543db-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="543db-171">合作机会到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="543db-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="543db-172">Salesforce Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="543db-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="543db-173">B.</span><span class="sxs-lookup"><span data-stu-id="543db-173">B.</span></span> <span data-ttu-id="543db-174">对于每个 flow，选择 " **仅运行用户** " 选项。</span><span class="sxs-lookup"><span data-stu-id="543db-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="543db-175">选择 " **使用连接** ，而不是 **由仅运行用户提供**"。</span><span class="sxs-lookup"><span data-stu-id="543db-175">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="需要登录的错误消息":::


<span data-ttu-id="543db-177">C.</span><span class="sxs-lookup"><span data-stu-id="543db-177">C.</span></span> <span data-ttu-id="543db-178">激活以下所述的流：</span><span class="sxs-lookup"><span data-stu-id="543db-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="543db-179">合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) </span><span class="sxs-lookup"><span data-stu-id="543db-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="543db-180">Salesforce 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="543db-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="543db-181">D.</span><span class="sxs-lookup"><span data-stu-id="543db-181">D.</span></span> <span data-ttu-id="543db-182">激活所有剩余流。</span><span class="sxs-lookup"><span data-stu-id="543db-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="543db-183">E.</span><span class="sxs-lookup"><span data-stu-id="543db-183">E.</span></span> <span data-ttu-id="543db-184">在流伙伴中心 Webhook 注册中，选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="543db-184">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="543db-185">提供从合作伙伴中心的第一个操作**到 Salesforce**流的**http url** 。</span><span class="sxs-lookup"><span data-stu-id="543db-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="543db-186">选择 **要注册的事件** 下的所有四个选项，然后选择 **"是"** 进行覆盖。</span><span class="sxs-lookup"><span data-stu-id="543db-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="543db-187">有关运行/维护的问题和解答</span><span class="sxs-lookup"><span data-stu-id="543db-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="543db-188">如果在自动执行流程的过程中出现故障，如何排查问题？</span><span class="sxs-lookup"><span data-stu-id="543db-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="543db-189">若要确保电源自动流按预期运行，并在执行过程中排除故障，请参阅 [修复流故障](/power-automate/fix-flow-failures)。</span><span class="sxs-lookup"><span data-stu-id="543db-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="543db-190">如果在合作伙伴中心或 CRM 环境中看到未正确同步的引用，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="543db-191">若要确定引用同步的状态，请选择 " **审核**"。</span><span class="sxs-lookup"><span data-stu-id="543db-191">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="需要登录的错误消息":::

<span data-ttu-id="543db-193">确保满足以下条件：</span><span class="sxs-lookup"><span data-stu-id="543db-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="543db-194">解决方案 id 作为机会的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="543db-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="543db-195">需要两个字母的国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="543db-195">Two letter country code is required.</span></span>

- <span data-ttu-id="543db-196">为此机会选择了 "Microsoft 帮助" 时，需要客户联系信息。</span><span class="sxs-lookup"><span data-stu-id="543db-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="543db-197">如何确保引用会双向同步？</span><span class="sxs-lookup"><span data-stu-id="543db-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="543db-198">执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="543db-198">Do the following steps:</span></span>

- <span data-ttu-id="543db-199">合作伙伴卖方需要确保客户在 CRM 部分启用了 **与合作伙伴中心的同步** 选项。</span><span class="sxs-lookup"><span data-stu-id="543db-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="需要登录的错误消息":::

- <span data-ttu-id="543db-201">卖方需要在确认潜在客户时提供收入和结束日期。</span><span class="sxs-lookup"><span data-stu-id="543db-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="543db-202">如果在共同销售机会的 **创建** 或 **更新** 阶段提供 CRM ID，但 crm 中找不到具有该 id 的潜在顾客机会，则将忽略 update 或 create。</span><span class="sxs-lookup"><span data-stu-id="543db-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="543db-203">确保在 Salesforce 环境中配置了参考货币字段。</span><span class="sxs-lookup"><span data-stu-id="543db-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="543db-204">如果连接器断开连接并且错过了引用同步，应该怎么做。</span><span class="sxs-lookup"><span data-stu-id="543db-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="543db-205">下面是一些你可以尝试的选项：</span><span class="sxs-lookup"><span data-stu-id="543db-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="543db-206">通过引用管理员角色检查伙伴中心用户的用户名或密码是否已过期。</span><span class="sxs-lookup"><span data-stu-id="543db-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="543db-207">您可以使用未同步的机会，进行次要更新，并观察引用是否已同步。</span><span class="sxs-lookup"><span data-stu-id="543db-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="543db-208">如果流已运行并失败，请选择该流，并重新提交失败的运行。</span><span class="sxs-lookup"><span data-stu-id="543db-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="543db-209">收到拒绝访问错误后，应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="543db-210">请确保存在适当的角色</span><span class="sxs-lookup"><span data-stu-id="543db-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="543db-211">合作伙伴中心卖方的引用管理员角色</span><span class="sxs-lookup"><span data-stu-id="543db-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="543db-212">CRM 实例上的系统管理员或系统定制员角色</span><span class="sxs-lookup"><span data-stu-id="543db-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="543db-213">确保自动将流量帐户用户登录 https://flow.microsoft.com 至少一次</span><span class="sxs-lookup"><span data-stu-id="543db-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="543db-214">如果在创建共同销售机会时看到 **客户帐户国家/地区代码** 缺失，你应该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="543db-215">需要将 ISO 双字母国家/地区代码添加到 CRM 中的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="543db-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="543db-216">如果在创建共同销售机会时看到 **需要解决方案 ID** 的错误，该怎么办？</span><span class="sxs-lookup"><span data-stu-id="543db-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="543db-217">若要创建共同销售引用，你需要一个 Microsoft 共同销售好的解决方案。</span><span class="sxs-lookup"><span data-stu-id="543db-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="543db-218">当你看到在合作伙伴中心创建的共同销售机会（即使没有流错误）时，你应该怎么办：</span><span class="sxs-lookup"><span data-stu-id="543db-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="543db-219">请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="543db-219">Do the following:</span></span>

- <span data-ttu-id="543db-220">在合作伙伴中心创建新的共同销售交易后，请检查是否调用了 "合作伙伴中心到 Dynamics 365" 流 (它可能会) 调用多次。</span><span class="sxs-lookup"><span data-stu-id="543db-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="543db-221">如果调用了流，请检查所有调用的流，并识别将更新 CRM 的流运行。</span><span class="sxs-lookup"><span data-stu-id="543db-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="543db-222">你可以执行这些操作，并验证其是否更新了 CRM 或遇到了问题。</span><span class="sxs-lookup"><span data-stu-id="543db-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="543db-223">请查看合作伙伴中心的 \*新交易\*\*，查看其是否已用 CRM ID 填充。</span><span class="sxs-lookup"><span data-stu-id="543db-223">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="543db-224">请确保在合作伙伴中心，交易不会意外地被视为 "赢单" 或 "丢失"。</span><span class="sxs-lookup"><span data-stu-id="543db-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="543db-225">后续步骤</span><span class="sxs-lookup"><span data-stu-id="543db-225">Next steps</span></span>

- [<span data-ttu-id="543db-226">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="543db-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="543db-227">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="543db-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)