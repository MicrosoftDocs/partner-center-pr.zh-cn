---
title: 使用 Webhook 获取资源更改事件
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作伙伴中心 Webhook Api 了解 Dynamics 365 CRM 或 Salesforce CRM 何时发生了引用资源更改。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 引用，webhook api，资源更改事件
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43874556b5f3fd355f5c315bf06ca7daee0a699e
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467467"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="ba0da-104">使用 Webhook Api 为 Dynamics 365 CRM 和 Salesforce CRM 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="ba0da-104">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="ba0da-105">相应的角色</span><span class="sxs-lookup"><span data-stu-id="ba0da-105">Appropriate roles</span></span>

- <span data-ttu-id="ba0da-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="ba0da-106">Referrals admin</span></span>
- <span data-ttu-id="ba0da-107">适用于 Dynamics 365 CRM 或 Salesforce CRM 的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="ba0da-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="ba0da-108">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="ba0da-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="ba0da-109">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="ba0da-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="ba0da-110">本主题介绍 Dynamics 365 CRM 和 Salesforce CRM 的 Webhook Api。</span><span class="sxs-lookup"><span data-stu-id="ba0da-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="ba0da-111">配置 Webhook</span><span class="sxs-lookup"><span data-stu-id="ba0da-111">Configure the webhook</span></span>

1. <span data-ttu-id="ba0da-112">若要注册 url，请选择 "**合作伙伴中心 Webhook 注册" （有问必答预览版）** "电源自动流程"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-112">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="ba0da-113">为（a）添加连接。具有引用管理员凭据的合作伙伴中心用户（b.）以下突出显示的合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="ba0da-113">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   <span data-ttu-id="ba0da-114">触发器</span><span class="sxs-lookup"><span data-stu-id="ba0da-114">:::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::</span></span>

3. <span data-ttu-id="ba0da-115">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="ba0da-115">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="ba0da-117">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="ba0da-117">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="ba0da-118">若要使合作伙伴中心 webhook 能够侦听合作伙伴中心和 CRM 系统中的 IP 共同销售/独立引用对象中的事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="ba0da-118">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="ba0da-119">选择 "**合作伙伴中心到 Dynamics 365 （有问必答预览版）** " 或 "**合作伙伴中心到 Salesforce" （有问必答预览版）**。</span><span class="sxs-lookup"><span data-stu-id="ba0da-119">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="ba0da-120">选择 "**编辑**" 图标，然后选择 "**收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-120">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="ba0da-121">选择**复制**图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="ba0da-121">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="复制 URL":::

8. <span data-ttu-id="ba0da-123">现在，选择 "合作伙伴中心 Webhook 注册（有问必答预览版）" "电源自动流"，然后选择 "**运行**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-123">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="ba0da-124">确保在右侧窗格中打开 "运行流" 窗口，然后单击 "**继续**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-124">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="ba0da-125">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="ba0da-125">Enter the following details:</span></span>

    1. <span data-ttu-id="ba0da-126">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="ba0da-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="ba0da-127">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="ba0da-127">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="ba0da-128">**覆盖现有触发器终结点（如果存在**）：是（这将覆盖任何现有终结点。）</span><span class="sxs-lookup"><span data-stu-id="ba0da-128">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="ba0da-129">Webhook 现在可以侦听更改（创建和更新事件）。</span><span class="sxs-lookup"><span data-stu-id="ba0da-129">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="ba0da-130">选择 "**运行**"，然后选择 "**完成"。**</span><span class="sxs-lookup"><span data-stu-id="ba0da-130">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="ba0da-131">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="ba0da-131">Customize synchronization steps</span></span>

<span data-ttu-id="ba0da-132">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="ba0da-132">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="ba0da-133">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="ba0da-133">Often CRM systems are highly customized.</span></span> <span data-ttu-id="ba0da-134">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="ba0da-134">You can customize the Power Automate flows.</span></span> <span data-ttu-id="ba0da-135">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="ba0da-135">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="ba0da-136">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="ba0da-136">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="ba0da-137">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="ba0da-137">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="ba0da-138">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="ba0da-138">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="ba0da-139">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ba0da-139">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="ba0da-140">选择 "合作伙伴中心到 Dynamics 365 （有问必答预览版）" 或 "合作伙伴中心到 Salesforce" （有问必答预览版）。</span><span class="sxs-lookup"><span data-stu-id="ba0da-140">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="ba0da-141">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="ba0da-141">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="ba0da-142">选择 **（作用域）同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="ba0da-142">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="ba0da-143">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**如果是新的共享机会"，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="ba0da-143">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="ba0da-144">**如果是**，请选择 "子步骤"，然后**在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-144">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="ba0da-145">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="ba0da-145">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="ba0da-146">若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请单击 "（作用域）同步潜在客户或机会" 步骤。</span><span class="sxs-lookup"><span data-stu-id="ba0da-146">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="ba0da-147">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-147">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="ba0da-148">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。</span><span class="sxs-lookup"><span data-stu-id="ba0da-148">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="ba0da-149">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="ba0da-149">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="ba0da-150">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="ba0da-150">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="ba0da-151">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="ba0da-151">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ba0da-152">选择 **（范围）同步机会**。</span><span class="sxs-lookup"><span data-stu-id="ba0da-152">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="ba0da-153">若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="ba0da-153">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="ba0da-154">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="ba0da-154">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="ba0da-155">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="ba0da-155">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="ba0da-156">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="ba0da-156">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="ba0da-157">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="ba0da-157">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ba0da-158">选择 **（作用域）同步引用。**</span><span class="sxs-lookup"><span data-stu-id="ba0da-158">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="ba0da-159">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-159">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="ba0da-160">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="ba0da-160">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="ba0da-161">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="ba0da-161">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="ba0da-162">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 或 Salesforce 与合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="ba0da-162">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="ba0da-163">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba0da-163">Pre-requisites</span></span>

<span data-ttu-id="ba0da-164">若要跨伙伴中心和 Dynamics 365 CRM 或跨合作伙伴中心和 Salesforce CRM 同步检索，自动完成解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="ba0da-164">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="ba0da-165">这使您的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="ba0da-165">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="ba0da-166">对于 Dynamics 365 解决方案**机会**实体，合作伙伴中心引用同步中提供了一组自定义字段。</span><span class="sxs-lookup"><span data-stu-id="ba0da-166">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="ba0da-167">CRM 管理用户需要使用**机会**自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="ba0da-167">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="ba0da-168">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="ba0da-168">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="ba0da-169">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="ba0da-169">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="ba0da-170">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="ba0da-170">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="ba0da-171">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="ba0da-171">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="ba0da-172">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助</span><span class="sxs-lookup"><span data-stu-id="ba0da-172">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="ba0da-173">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="ba0da-173">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="ba0da-174">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="ba0da-174">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="ba0da-175">各种</span><span class="sxs-lookup"><span data-stu-id="ba0da-175">SCENARIOS:</span></span>

1. <span data-ttu-id="ba0da-176">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="ba0da-176">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="ba0da-177">在 CRM 的 "**机会**" 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="ba0da-177">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="ba0da-178">在 Dynamics 365 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="ba0da-178">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="机会":::

   3. <span data-ttu-id="ba0da-180">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="ba0da-180">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="ba0da-181">**与合作伙伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="ba0da-181">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="ba0da-182">**Microsoft Help 如何？**：选择以下各项：</span><span class="sxs-lookup"><span data-stu-id="ba0da-182">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="帮助选择":::

      - <span data-ttu-id="ba0da-184">**产品**：产品的解决方案 id</span><span class="sxs-lookup"><span data-stu-id="ba0da-184">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="ba0da-185">一旦在 Dynamics 365 中创建了商机，并将 "**伙伴中心同步**" 选项设置为 **"是"**，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="ba0da-185">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="ba0da-186">你的引用将与 Dynamics 365 同步。</span><span class="sxs-lookup"><span data-stu-id="ba0da-186">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="ba0da-187">因此，对于将 "与合作伙伴中心同步" 选项设置为 "是" 的机会，如果您更新 Dynamics 365 CRM 中的机会，则这些更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="ba0da-187">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="ba0da-188">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="ba0da-188">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="ba0da-189">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="ba0da-189">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="ba0da-190">登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="ba0da-190">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="ba0da-191">从左侧菜单中选择 "**引用**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-191">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="ba0da-192">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="ba0da-192">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="ba0da-193">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="ba0da-193">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="ba0da-194">导航到 "**开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="ba0da-194">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="ba0da-195">现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="ba0da-195">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="ba0da-196">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="ba0da-196">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba0da-197">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ba0da-197">Next steps</span></span>

- [<span data-ttu-id="ba0da-198">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="ba0da-198">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="ba0da-199">合作伙伴中心 webhook 事件</span><span class="sxs-lookup"><span data-stu-id="ba0da-199">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="ba0da-200">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="ba0da-200">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="ba0da-201">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="ba0da-201">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)