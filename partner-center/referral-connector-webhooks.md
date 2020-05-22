---
title: 使用 Webhook 获取资源更改事件
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Webhook Api 了解何时发生了引用资源更改
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 引用，webhook api，资源更改事件
ms.localizationpriority: medium
ms.openlocfilehash: a141776f1b591ebe41bb740051802b4b55cf36f0
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "83796203"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="9ce20-104">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="9ce20-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="9ce20-105">相应的角色</span><span class="sxs-lookup"><span data-stu-id="9ce20-105">Appropriate roles</span></span>

- <span data-ttu-id="9ce20-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="9ce20-106">Referrals admin</span></span>
- <span data-ttu-id="9ce20-107">适用于 Dynamics 365 CRM 或 Salesforce CRM 的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="9ce20-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="9ce20-108">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="9ce20-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="9ce20-109">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="9ce20-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="9ce20-110">本主题介绍 Dynamics 365 CRM 和 Salesforce CRM 的 Webhook Api。</span><span class="sxs-lookup"><span data-stu-id="9ce20-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="9ce20-111">若要注册 url，请选择 "**合作伙伴中心 Webhook 注册" （有问必答预览版）** "电源自动流程"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="9ce20-112">为（a）添加连接。具有引用管理员凭据的合作伙伴中心用户（b.）以下突出显示的合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="9ce20-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![触发器](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="9ce20-114">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="9ce20-114">When you make these updates, you will see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="9ce20-116">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="9ce20-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="9ce20-117">若要使合作伙伴中心 webhook 能够侦听合作伙伴中心和 CRM 系统中的 IP 共同销售/独立引用对象中的事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="9ce20-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="9ce20-118">选择 "**合作伙伴中心到 Dynamics 365 （有问必答预览版）** " 或 "**合作伙伴中心到 Salesforce" （有问必答预览版）**。</span><span class="sxs-lookup"><span data-stu-id="9ce20-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="9ce20-119">选择 "**编辑**" 图标，然后选择 "**收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="9ce20-120">选择**复制**图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="9ce20-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![复制 URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="9ce20-122">现在，选择 "合作伙伴中心 Webhook 注册（有问必答预览版）" "电源自动流"，然后选择 "**运行**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="9ce20-123">确保在右侧窗格中打开 "运行流" 窗口，然后单击 "**继续**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="9ce20-124">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="9ce20-124">Enter the following details:</span></span> 

    <span data-ttu-id="9ce20-125">a.</span><span class="sxs-lookup"><span data-stu-id="9ce20-125">a.</span></span> <span data-ttu-id="9ce20-126">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="9ce20-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="9ce20-127">b.</span><span class="sxs-lookup"><span data-stu-id="9ce20-127">b.</span></span> <span data-ttu-id="9ce20-128">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="9ce20-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="9ce20-129">c.</span><span class="sxs-lookup"><span data-stu-id="9ce20-129">c.</span></span> <span data-ttu-id="9ce20-130">**覆盖现有触发器终结点（如果存在**）：是（这将覆盖任何现有终结点。）</span><span class="sxs-lookup"><span data-stu-id="9ce20-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="9ce20-131">Webhook 现在可以侦听更改（创建和更新事件）。</span><span class="sxs-lookup"><span data-stu-id="9ce20-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="9ce20-132">选择 "**运行**"，然后选择 "**完成"。**</span><span class="sxs-lookup"><span data-stu-id="9ce20-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="9ce20-133">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="9ce20-133">Customize synchronization steps</span></span>

<span data-ttu-id="9ce20-134">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="9ce20-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="9ce20-135">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="9ce20-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="9ce20-136">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="9ce20-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="9ce20-137">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="9ce20-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="9ce20-138">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="9ce20-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="9ce20-139">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="9ce20-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="9ce20-140">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="9ce20-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="9ce20-141">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="9ce20-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="9ce20-142">a.</span><span class="sxs-lookup"><span data-stu-id="9ce20-142">a.</span></span> <span data-ttu-id="9ce20-143">选择 "合作伙伴中心到 Dynamics 365 （有问必答预览版）" 或 "合作伙伴中心到 Salesforce" （有问必答预览版）。</span><span class="sxs-lookup"><span data-stu-id="9ce20-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="9ce20-144">b.</span><span class="sxs-lookup"><span data-stu-id="9ce20-144">b.</span></span> <span data-ttu-id="9ce20-145">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="9ce20-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="9ce20-146">c.</span><span class="sxs-lookup"><span data-stu-id="9ce20-146">c.</span></span> <span data-ttu-id="9ce20-147">选择 **（作用域）同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="9ce20-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="9ce20-148">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**如果是新的共享机会"，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="9ce20-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="9ce20-149">**如果是**，请选择 "子步骤"，然后**在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="9ce20-150">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="9ce20-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="9ce20-151">d.</span><span class="sxs-lookup"><span data-stu-id="9ce20-151">d.</span></span> <span data-ttu-id="9ce20-152">若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请单击 "（作用域）同步潜在客户或机会" 步骤。</span><span class="sxs-lookup"><span data-stu-id="9ce20-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="9ce20-153">e.</span><span class="sxs-lookup"><span data-stu-id="9ce20-153">e.</span></span> <span data-ttu-id="9ce20-154">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="9ce20-155">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。</span><span class="sxs-lookup"><span data-stu-id="9ce20-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="9ce20-156">f.</span><span class="sxs-lookup"><span data-stu-id="9ce20-156">f.</span></span> <span data-ttu-id="9ce20-157">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="9ce20-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="9ce20-158">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="9ce20-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="9ce20-159">a.</span><span class="sxs-lookup"><span data-stu-id="9ce20-159">a.</span></span> <span data-ttu-id="9ce20-160">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="9ce20-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="9ce20-161">b.</span><span class="sxs-lookup"><span data-stu-id="9ce20-161">b.</span></span> <span data-ttu-id="9ce20-162">选择 **（范围）同步机会**。</span><span class="sxs-lookup"><span data-stu-id="9ce20-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="9ce20-163">c.</span><span class="sxs-lookup"><span data-stu-id="9ce20-163">c.</span></span> <span data-ttu-id="9ce20-164">若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="9ce20-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="9ce20-165">d.</span><span class="sxs-lookup"><span data-stu-id="9ce20-165">d.</span></span> <span data-ttu-id="9ce20-166">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="9ce20-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="9ce20-167">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="9ce20-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="9ce20-168">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="9ce20-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="9ce20-169">a.</span><span class="sxs-lookup"><span data-stu-id="9ce20-169">a.</span></span> <span data-ttu-id="9ce20-170">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="9ce20-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="9ce20-171">b.</span><span class="sxs-lookup"><span data-stu-id="9ce20-171">b.</span></span> <span data-ttu-id="9ce20-172">选择 **（作用域）同步引用。**</span><span class="sxs-lookup"><span data-stu-id="9ce20-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="9ce20-173">c.</span><span class="sxs-lookup"><span data-stu-id="9ce20-173">c.</span></span> <span data-ttu-id="9ce20-174">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="9ce20-175">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="9ce20-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="9ce20-176">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="9ce20-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="9ce20-177">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 或 Salesforce 与合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="9ce20-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="9ce20-178">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ce20-178">Pre-requisites</span></span>

<span data-ttu-id="9ce20-179">若要跨伙伴中心和 Dynamics 365 CRM 或跨合作伙伴中心和 Salesforce CRM 同步检索，自动完成解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="9ce20-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="9ce20-180">这使您的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="9ce20-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="9ce20-181">对于 Dynamics 365 解决方案**机会**实体，合作伙伴中心引用同步中提供了一组自定义字段。</span><span class="sxs-lookup"><span data-stu-id="9ce20-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="9ce20-182">CRM 管理用户需要使用**机会**自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="9ce20-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="9ce20-183">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="9ce20-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="9ce20-184">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="9ce20-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="9ce20-185">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="9ce20-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="9ce20-186">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="9ce20-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="9ce20-187">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助</span><span class="sxs-lookup"><span data-stu-id="9ce20-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="9ce20-188">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="9ce20-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="9ce20-189">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="9ce20-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="9ce20-190">各种</span><span class="sxs-lookup"><span data-stu-id="9ce20-190">SCENARIOS:</span></span>

1. <span data-ttu-id="9ce20-191">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="9ce20-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="9ce20-192">a.</span><span class="sxs-lookup"><span data-stu-id="9ce20-192">a.</span></span> <span data-ttu-id="9ce20-193">在 CRM 的 "**机会**" 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境或 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="9ce20-193">Sign into your Dynamics 365 CRM environment or Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="9ce20-194">b.</span><span class="sxs-lookup"><span data-stu-id="9ce20-194">b.</span></span> <span data-ttu-id="9ce20-195">在 Dynamics 365 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="9ce20-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![机会](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="9ce20-197">c.</span><span class="sxs-lookup"><span data-stu-id="9ce20-197">c.</span></span> <span data-ttu-id="9ce20-198">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="9ce20-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="9ce20-199">"与合作伙伴中心同步"：是</span><span class="sxs-lookup"><span data-stu-id="9ce20-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="9ce20-200">"Microsoft help 怎样？"：从以下项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="9ce20-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![帮助选择](images/cosellconnectors/help.png)

    - <span data-ttu-id="9ce20-202">产品：产品的解决方案 Id</span><span class="sxs-lookup"><span data-stu-id="9ce20-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="9ce20-203">d.</span><span class="sxs-lookup"><span data-stu-id="9ce20-203">d.</span></span> <span data-ttu-id="9ce20-204">一旦在 Dynamics 365 中创建了商机，并将 "**伙伴中心同步**" 选项设置为 **"是"**，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="9ce20-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="9ce20-205">你的引用将与 Dynamics 365 同步。</span><span class="sxs-lookup"><span data-stu-id="9ce20-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="9ce20-206">e.</span><span class="sxs-lookup"><span data-stu-id="9ce20-206">e.</span></span> <span data-ttu-id="9ce20-207">因此，对于将 "与合作伙伴中心同步" 选项设置为 "是" 的机会，如果您更新 Dynamics 365 CRM 中的机会，则这些更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="9ce20-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="9ce20-208">f.</span><span class="sxs-lookup"><span data-stu-id="9ce20-208">f.</span></span> <span data-ttu-id="9ce20-209">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="9ce20-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="9ce20-210">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="9ce20-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="9ce20-211">a.</span><span class="sxs-lookup"><span data-stu-id="9ce20-211">a.</span></span> <span data-ttu-id="9ce20-212">登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="9ce20-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="9ce20-213">b.</span><span class="sxs-lookup"><span data-stu-id="9ce20-213">b.</span></span> <span data-ttu-id="9ce20-214">从左侧菜单中选择 "**引用**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="9ce20-215">c.</span><span class="sxs-lookup"><span data-stu-id="9ce20-215">c.</span></span> <span data-ttu-id="9ce20-216">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="9ce20-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="9ce20-217">d.</span><span class="sxs-lookup"><span data-stu-id="9ce20-217">d.</span></span> <span data-ttu-id="9ce20-218">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="9ce20-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="9ce20-219">e.</span><span class="sxs-lookup"><span data-stu-id="9ce20-219">e.</span></span> <span data-ttu-id="9ce20-220">导航到 "**开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="9ce20-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="9ce20-221">现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="9ce20-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="9ce20-222">f.</span><span class="sxs-lookup"><span data-stu-id="9ce20-222">f.</span></span> <span data-ttu-id="9ce20-223">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="9ce20-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="9ce20-224">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9ce20-224">Next steps</span></span>

- [<span data-ttu-id="9ce20-225">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="9ce20-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="9ce20-226">合作伙伴中心 webhook 事件</span><span class="sxs-lookup"><span data-stu-id="9ce20-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="9ce20-227">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="9ce20-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="9ce20-228">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="9ce20-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
