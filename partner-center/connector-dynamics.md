---
title: Dynamics 365 CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心中的引用同步到 Dynamics 365 CRM 的共同销售连接器。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031330"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="3b459-104">用于 Dynamics 365 CRM 的共同销售连接器–概述</span><span class="sxs-lookup"><span data-stu-id="3b459-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="3b459-105">相应的角色</span><span class="sxs-lookup"><span data-stu-id="3b459-105">Appropriate roles</span></span>

- <span data-ttu-id="3b459-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="3b459-106">Referrals admin</span></span>
- <span data-ttu-id="3b459-107">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="3b459-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="3b459-108">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="3b459-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="3b459-109">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="3b459-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="3b459-110">使用共同销售连接器，可以创建新的共同销售的引用，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受/拒绝引用、修改交易数据（如交易价值和结束日期）。</span><span class="sxs-lookup"><span data-stu-id="3b459-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="3b459-111">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="3b459-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="3b459-112">您可以在所选的 CRM 内而不是在合作伙伴中心内完成所有的引用工作。</span><span class="sxs-lookup"><span data-stu-id="3b459-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="3b459-113">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="3b459-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="3b459-114">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="3b459-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="3b459-115">**主题**</span><span class="sxs-lookup"><span data-stu-id="3b459-115">**Topics**</span></span>   |<span data-ttu-id="3b459-116">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="3b459-116">**Details**</span></span>   |<span data-ttu-id="3b459-117">**链接**</span><span class="sxs-lookup"><span data-stu-id="3b459-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="3b459-118">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="3b459-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="3b459-119">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="3b459-119">You need a valid MPN ID</span></span>|<span data-ttu-id="3b459-120">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="3b459-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="3b459-121">做好就绪</span><span class="sxs-lookup"><span data-stu-id="3b459-121">Cosell ready</span></span>|<span data-ttu-id="3b459-122">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="3b459-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="3b459-123">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="3b459-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="3b459-124">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="3b459-124">Partner Center account</span></span>|<span data-ttu-id="3b459-125">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="3b459-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="3b459-126">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="3b459-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="3b459-127">管理帐户</span><span class="sxs-lookup"><span data-stu-id="3b459-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="3b459-128">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="3b459-128">Partner Center user roles</span></span>|<span data-ttu-id="3b459-129">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="3b459-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="3b459-130">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="3b459-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="3b459-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="3b459-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="3b459-132">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="3b459-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="3b459-133">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="3b459-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="3b459-134">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="3b459-134">Power Automate Flow Account</span></span>|<span data-ttu-id="3b459-135">CRM 系统管理员或系统定制员的有效 [电源自动完成](https://flow.microsoft.com) 帐户。</span><span class="sxs-lookup"><span data-stu-id="3b459-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="3b459-136">在安装之前，该用户至少应登录到一次 [电源](https://flow.microsoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="3b459-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="3b459-137">安装适用于 Dynamics 365 (Power 自动化解决方案的合作伙伴中心引用同步) </span><span class="sxs-lookup"><span data-stu-id="3b459-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="3b459-138">请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="3b459-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="3b459-139">此步骤将显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="3b459-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="3b459-140">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="3b459-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="3b459-141">选择左侧导航栏上的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="3b459-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="3b459-142">单击顶部菜单上的 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="3b459-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. <span data-ttu-id="3b459-144">在弹出屏幕中搜索 **Dynamics365 的合作伙伴中心引用连接器** 。</span><span class="sxs-lookup"><span data-stu-id="3b459-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="3b459-145">单击 " **立即获取** " 按钮，然后 **继续**。</span><span class="sxs-lookup"><span data-stu-id="3b459-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="3b459-146">这将打开一个页面，可在其中选择 CRM (Dynamics 365) 环境以安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="3b459-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="3b459-147">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="3b459-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="3b459-148">然后，你将转到 " **管理你的解决方案** " 页。</span><span class="sxs-lookup"><span data-stu-id="3b459-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="3b459-149">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="3b459-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="3b459-150">**计划的安装** 应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="3b459-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="3b459-151">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="3b459-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="3b459-152">安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="3b459-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="3b459-153">请注意，"解决方案" 列表中提供了 **Dynamics 365 的合作伙伴中心引用同步** 。</span><span class="sxs-lookup"><span data-stu-id="3b459-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="3b459-154">选择 **Dynamics 365 的伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="3b459-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="3b459-155">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="3b459-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="打开 AppSource":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="3b459-157">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="3b459-157">Best practice: test before you go live</span></span>

<span data-ttu-id="3b459-158">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="3b459-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="3b459-159">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="3b459-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="3b459-160">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="3b459-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="3b459-161">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="3b459-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="3b459-162">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="3b459-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="3b459-163">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="3b459-163">Configure the solution</span></span>

1. <span data-ttu-id="3b459-164">在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="3b459-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="3b459-165">在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="3b459-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="3b459-166">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="3b459-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="3b459-167">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="3b459-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="3b459-168">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="3b459-168">Partner Center Events</span></span>

   - <span data-ttu-id="3b459-169">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="3b459-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="3b459-170">从左侧导航栏中选择 " **连接** "，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="3b459-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="3b459-171">通过单击 " **创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="3b459-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="打开 AppSource":::

      3. <span data-ttu-id="3b459-173">在右上角的搜索栏中搜索 " \*\*合作伙伴中心引用 (预览") \*\* 。</span><span class="sxs-lookup"><span data-stu-id="3b459-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="3b459-174">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="3b459-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="3b459-175">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="3b459-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="3b459-176">为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。</span><span class="sxs-lookup"><span data-stu-id="3b459-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="3b459-177">若要将电源自动流与连接进行关联，请编辑每个电源自动流，以连接到 Common Data Service 和合作伙伴中心引用。</span><span class="sxs-lookup"><span data-stu-id="3b459-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="3b459-178">保存更改。</span><span class="sxs-lookup"><span data-stu-id="3b459-178">Save the changes.</span></span>

5. <span data-ttu-id="3b459-179">**启用** 自动流功能。</span><span class="sxs-lookup"><span data-stu-id="3b459-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="3b459-180">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="3b459-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="3b459-181">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="3b459-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="3b459-182">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="3b459-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="3b459-183">若要注册 url，请选择 " \*\*合作伙伴中心 Webhook 注册 (内幕预览版") \*\* Power 自动流 "。</span><span class="sxs-lookup"><span data-stu-id="3b459-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="3b459-184">为 (a ) 合作伙伴中心用户添加连接， (b. ) 合作伙伴中心事件如下所示</span><span class="sxs-lookup"><span data-stu-id="3b459-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="打开 AppSource":::

3. <span data-ttu-id="3b459-186">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="3b459-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="打开 AppSource":::

4. <span data-ttu-id="3b459-188">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="3b459-188">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="3b459-189">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="3b459-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="3b459-190">选择 " \*\*合作伙伴中心到 Dynamics 365 (预览体验预览") \*\*。</span><span class="sxs-lookup"><span data-stu-id="3b459-190">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="3b459-191">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-191">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="3b459-192">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="3b459-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="打开 AppSource":::

8. <span data-ttu-id="3b459-194">现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="3b459-195">确保在右侧窗格中打开 "运行流" 窗口，然后单击 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="3b459-196">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="3b459-196">Enter the following details:</span></span>

    1. <span data-ttu-id="3b459-197">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="3b459-197">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="3b459-198">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="3b459-198">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="3b459-199">**覆盖现有触发器终结点（如果存在**）：是 (这将覆盖任何现有终结点。 ) </span><span class="sxs-lookup"><span data-stu-id="3b459-199">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="3b459-200">选择 " **运行** "，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="3b459-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="3b459-201">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="3b459-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="3b459-202">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="3b459-202">Customize synchronization steps</span></span>

<span data-ttu-id="3b459-203">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="3b459-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="3b459-204">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="3b459-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="3b459-205">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="3b459-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="3b459-206">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="3b459-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="3b459-207">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="3b459-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="3b459-208">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="3b459-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="3b459-209">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="3b459-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="3b459-210">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3b459-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="3b459-211">a.</span><span class="sxs-lookup"><span data-stu-id="3b459-211">a.</span></span> <span data-ttu-id="3b459-212">选择 "合作伙伴中心到 Dynamics 365 (预览体验预览") 或 "合作伙伴中心到 Salesforce (内幕预览版) "。</span><span class="sxs-lookup"><span data-stu-id="3b459-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="3b459-213">b.</span><span class="sxs-lookup"><span data-stu-id="3b459-213">b.</span></span> <span data-ttu-id="3b459-214">选择 " **编辑** " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="3b459-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="3b459-215">c.</span><span class="sxs-lookup"><span data-stu-id="3b459-215">c.</span></span> <span data-ttu-id="3b459-216">选择 " \*\* (范围") 同步潜在客户或机会\*\*。</span><span class="sxs-lookup"><span data-stu-id="3b459-216">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="3b459-217">若要基于字段映射自定义 CRM 字段映射 (请) 对于 "创建事件"，选择 " **如果是新的共享机会"，然后选择 "是**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="3b459-218">**如果是**，请选择 "子步骤"，然后**在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="3b459-219">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="3b459-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="3b459-220">d.</span><span class="sxs-lookup"><span data-stu-id="3b459-220">d.</span></span> <span data-ttu-id="3b459-221">对于 "基于字段映射 (自定义 CRM 字段映射" 指南) 对于 "更新事件"，请单击步骤 " (范围) 同步潜在顾客或机会"。</span><span class="sxs-lookup"><span data-stu-id="3b459-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="3b459-222">e.</span><span class="sxs-lookup"><span data-stu-id="3b459-222">e.</span></span> <span data-ttu-id="3b459-223">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="3b459-223">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="3b459-224">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。</span><span class="sxs-lookup"><span data-stu-id="3b459-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="3b459-225">f.</span><span class="sxs-lookup"><span data-stu-id="3b459-225">f.</span></span> <span data-ttu-id="3b459-226">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="3b459-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="3b459-227">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="3b459-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="3b459-228">a.</span><span class="sxs-lookup"><span data-stu-id="3b459-228">a.</span></span> <span data-ttu-id="3b459-229">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="3b459-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="3b459-230">b.</span><span class="sxs-lookup"><span data-stu-id="3b459-230">b.</span></span> <span data-ttu-id="3b459-231">选择 \*\* (范围) 同步机会\*\*。</span><span class="sxs-lookup"><span data-stu-id="3b459-231">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="3b459-232">c.</span><span class="sxs-lookup"><span data-stu-id="3b459-232">c.</span></span> <span data-ttu-id="3b459-233">若要为更新事件自定义 CRM 字段映射，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="3b459-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="3b459-234">d.</span><span class="sxs-lookup"><span data-stu-id="3b459-234">d.</span></span> <span data-ttu-id="3b459-235">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="3b459-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="3b459-236">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="3b459-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="3b459-237">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="3b459-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="3b459-238">a.</span><span class="sxs-lookup"><span data-stu-id="3b459-238">a.</span></span> <span data-ttu-id="3b459-239">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="3b459-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="3b459-240">b.</span><span class="sxs-lookup"><span data-stu-id="3b459-240">b.</span></span> <span data-ttu-id="3b459-241">选择 **) 同步引用 (范围。**</span><span class="sxs-lookup"><span data-stu-id="3b459-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="3b459-242">c.</span><span class="sxs-lookup"><span data-stu-id="3b459-242">c.</span></span> <span data-ttu-id="3b459-243">对于 "基于字段映射自定义 CRM 字段映射 (" 指南) 对于创建事件，请选择 " **创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="3b459-244">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="3b459-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="3b459-245">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="3b459-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="3b459-246">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="3b459-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="3b459-247">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b459-247">Pre-requisites</span></span>

<span data-ttu-id="3b459-248">若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="3b459-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="3b459-249">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="3b459-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="3b459-250">一组自定义字段作为 " **机会** " 实体的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="3b459-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="3b459-251">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="3b459-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="3b459-252">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="3b459-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="3b459-253">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="3b459-253">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="3b459-254">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="3b459-254">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="3b459-255">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="3b459-255">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="3b459-256">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助</span><span class="sxs-lookup"><span data-stu-id="3b459-256">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="3b459-257">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="3b459-257">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="3b459-258">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="3b459-258">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="3b459-259">各种</span><span class="sxs-lookup"><span data-stu-id="3b459-259">SCENARIOS:</span></span>

1. <span data-ttu-id="3b459-260">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="3b459-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="3b459-261">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="3b459-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="3b459-262">在 Dynamics 365 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="3b459-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="打开 AppSource":::

   3. <span data-ttu-id="3b459-264">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="3b459-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="3b459-265">**与合作伙伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="3b459-265">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="3b459-266">**Microsoft Help 如何？**：选择以下各项：</span><span class="sxs-lookup"><span data-stu-id="3b459-266">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="打开 AppSource":::

      - <span data-ttu-id="3b459-268">**产品**：产品的解决方案 id</span><span class="sxs-lookup"><span data-stu-id="3b459-268">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="3b459-269">一旦在 Dynamics 365 中创建了商机，并将 " **伙伴中心同步** " 选项设置为 **"是"**，请等待10分钟，然后登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="3b459-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="3b459-270">你的引用将与 Dynamics 365 同步。</span><span class="sxs-lookup"><span data-stu-id="3b459-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="3b459-271">同样，如果将 "与合作伙伴中心同步" 选项设置为 "是"，则在 Dynamics 365 CRM 中更新此机会时，所做的更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="3b459-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="3b459-272">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="3b459-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="3b459-273">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="3b459-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="3b459-274">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="3b459-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="3b459-275">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="3b459-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="3b459-276">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="3b459-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="3b459-277">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="3b459-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="3b459-278">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="3b459-278">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="3b459-279">现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="3b459-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="3b459-280">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="3b459-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b459-281">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3b459-281">Next steps</span></span>

- [<span data-ttu-id="3b459-282">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="3b459-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="3b459-283">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="3b459-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="3b459-284">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="3b459-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="3b459-285">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="3b459-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)