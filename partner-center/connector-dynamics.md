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
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947719"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="bbc01-104">用于 Dynamics 365 CRM 的共同销售连接器–概述</span><span class="sxs-lookup"><span data-stu-id="bbc01-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="bbc01-105">相应的角色</span><span class="sxs-lookup"><span data-stu-id="bbc01-105">Appropriate roles</span></span>

- <span data-ttu-id="bbc01-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="bbc01-106">Referrals admin</span></span>
- <span data-ttu-id="bbc01-107">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="bbc01-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="bbc01-108">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="bbc01-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="bbc01-109">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="bbc01-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="bbc01-110">使用共同销售连接器，可以创建新的共同销售的引用，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受/拒绝引用、修改交易数据（如交易价值和结束日期）。</span><span class="sxs-lookup"><span data-stu-id="bbc01-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="bbc01-111">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="bbc01-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="bbc01-112">您可以在所选的 CRM 内而不是在合作伙伴中心内完成所有的引用工作。</span><span class="sxs-lookup"><span data-stu-id="bbc01-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="bbc01-113">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="bbc01-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="bbc01-114">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="bbc01-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="bbc01-115">**主题**</span><span class="sxs-lookup"><span data-stu-id="bbc01-115">**Topics**</span></span>   |<span data-ttu-id="bbc01-116">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="bbc01-116">**Details**</span></span>   |<span data-ttu-id="bbc01-117">**链接**</span><span class="sxs-lookup"><span data-stu-id="bbc01-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="bbc01-118">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="bbc01-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="bbc01-119">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="bbc01-119">You need a valid MPN ID</span></span>|<span data-ttu-id="bbc01-120">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="bbc01-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="bbc01-121">做好就绪</span><span class="sxs-lookup"><span data-stu-id="bbc01-121">Cosell ready</span></span>|<span data-ttu-id="bbc01-122">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="bbc01-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="bbc01-123">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="bbc01-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="bbc01-124">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="bbc01-124">Partner Center account</span></span>|<span data-ttu-id="bbc01-125">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="bbc01-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="bbc01-126">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="bbc01-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="bbc01-127">管理帐户</span><span class="sxs-lookup"><span data-stu-id="bbc01-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="bbc01-128">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="bbc01-128">Partner Center user roles</span></span>|<span data-ttu-id="bbc01-129">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="bbc01-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="bbc01-130">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="bbc01-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="bbc01-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="bbc01-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="bbc01-132">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="bbc01-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="bbc01-133">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="bbc01-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="bbc01-134">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="bbc01-134">Power Automate Flow Account</span></span>|<span data-ttu-id="bbc01-135">CRM 系统管理员或系统定制员的有效 [电源自动完成](https://flow.microsoft.com) 帐户。</span><span class="sxs-lookup"><span data-stu-id="bbc01-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="bbc01-136">在安装之前，该用户至少应登录到一次 [电源](https://flow.microsoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="bbc01-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="bbc01-137">安装适用于 Dynamics 365 (Power 自动化解决方案的合作伙伴中心引用同步) </span><span class="sxs-lookup"><span data-stu-id="bbc01-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="bbc01-138">请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="bbc01-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="bbc01-139">此步骤将显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="bbc01-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="bbc01-140">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="bbc01-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="bbc01-141">选择左侧导航栏上的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="bbc01-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="bbc01-142">单击顶部菜单上的 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. <span data-ttu-id="bbc01-144">在弹出屏幕中搜索 **Dynamics365 的合作伙伴中心引用连接器** 。</span><span class="sxs-lookup"><span data-stu-id="bbc01-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="bbc01-145">单击 " **立即获取** " 按钮，然后 **继续**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="bbc01-146">这将打开一个页面，可在其中选择 CRM (Dynamics 365) 环境以安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="bbc01-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="bbc01-147">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="bbc01-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="bbc01-148">然后，你将转到 " **管理你的解决方案** " 页。</span><span class="sxs-lookup"><span data-stu-id="bbc01-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="bbc01-149">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="bbc01-150">**计划的安装** 应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="bbc01-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="bbc01-151">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="bbc01-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="bbc01-152">安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="bbc01-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="bbc01-153">请注意，"解决方案" 列表中提供了 **Dynamics 365 的合作伙伴中心引用同步** 。</span><span class="sxs-lookup"><span data-stu-id="bbc01-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="bbc01-154">选择 **Dynamics 365 的伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="bbc01-155">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="bbc01-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用 CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="bbc01-157">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="bbc01-157">Best practice: test before you go live</span></span>

<span data-ttu-id="bbc01-158">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="bbc01-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="bbc01-159">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="bbc01-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="bbc01-160">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="bbc01-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="bbc01-161">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="bbc01-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="bbc01-162">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="bbc01-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="bbc01-163">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="bbc01-163">Configure the solution</span></span>

1. <span data-ttu-id="bbc01-164">在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="bbc01-165">在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="bbc01-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="bbc01-166">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="bbc01-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="bbc01-167">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="bbc01-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="bbc01-168">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="bbc01-168">Partner Center Events</span></span>

   - <span data-ttu-id="bbc01-169">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="bbc01-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="bbc01-170">从左侧导航栏中选择 " **连接** "，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="bbc01-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="bbc01-171">通过单击 " **创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="创建连接":::

      3. <span data-ttu-id="bbc01-173">在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。</span><span class="sxs-lookup"><span data-stu-id="bbc01-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="bbc01-174">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="bbc01-175">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="bbc01-176">为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="bbc01-177">添加所有连接后，你的环境中应会显示以下连接：</span><span class="sxs-lookup"><span data-stu-id="bbc01-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="连接":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="bbc01-179">编辑连接</span><span class="sxs-lookup"><span data-stu-id="bbc01-179">Edit the connections</span></span>

1. <span data-ttu-id="bbc01-180">返回 " **解决方案** " 页，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="bbc01-181">通过单击 "**全部**" **(预览) 选择 "连接引用**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="“连接”":::

2. <span data-ttu-id="bbc01-183">通过选择三个点图标，逐个编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="bbc01-184">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="bbc01-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="列出的连接"::: 

3.  <span data-ttu-id="bbc01-186">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="bbc01-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="bbc01-187"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="bbc01-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="bbc01-188">创建共同销售引用– Dynamics 365 到合作伙伴中心 (预览体验中心) </span><span class="sxs-lookup"><span data-stu-id="bbc01-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="bbc01-189">合作伙伴中心 Microsoft 共同销售对 Dynamics 365 (预览体验的引用更新) </span><span class="sxs-lookup"><span data-stu-id="bbc01-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="bbc01-190">合作伙伴中心到 Dynamics 365 (预览体验体验) </span><span class="sxs-lookup"><span data-stu-id="bbc01-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="bbc01-191">Dynamics 365 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="bbc01-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="bbc01-192">Dynamics 365 到合作伙伴中心 (有问必答预览版的机会) </span><span class="sxs-lookup"><span data-stu-id="bbc01-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="bbc01-193">Dynamics 365 的 Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="bbc01-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="bbc01-194">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="bbc01-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="bbc01-195">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="bbc01-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="bbc01-196">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="bbc01-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="bbc01-197">若要注册 url，请选择 " **合作伙伴中心 Webhook 注册 (内幕预览版")** Power 自动流 "。</span><span class="sxs-lookup"><span data-stu-id="bbc01-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="bbc01-198">为 (a ) 合作伙伴中心用户添加连接， (b. ) 合作伙伴中心事件如下所示</span><span class="sxs-lookup"><span data-stu-id="bbc01-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="触发器":::

3. <span data-ttu-id="bbc01-200">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="bbc01-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="bbc01-202">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="bbc01-203">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="bbc01-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="bbc01-204">选择 " **合作伙伴中心到 Dynamics 365 (预览体验预览")**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="bbc01-205">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="bbc01-206">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="bbc01-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="复制 URL":::

8. <span data-ttu-id="bbc01-208">现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="bbc01-209">确保在右侧窗格中打开 "运行流" 窗口，然后单击 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="bbc01-210">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="bbc01-210">Enter the following details:</span></span>

    1. <span data-ttu-id="bbc01-211">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="bbc01-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="bbc01-212">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="bbc01-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="bbc01-213">**覆盖现有触发器终结点（如果存在**）：是 (这将覆盖任何现有终结点。 ) </span><span class="sxs-lookup"><span data-stu-id="bbc01-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="bbc01-214">选择 " **运行** "，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="bbc01-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="bbc01-215">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="bbc01-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="bbc01-216">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="bbc01-216">Customize synchronization steps</span></span>

<span data-ttu-id="bbc01-217">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="bbc01-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="bbc01-218">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="bbc01-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="bbc01-219">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="bbc01-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="bbc01-220">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="bbc01-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="bbc01-221">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="bbc01-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="bbc01-222">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="bbc01-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="bbc01-223">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="bbc01-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="bbc01-224">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="bbc01-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="bbc01-225">a.</span><span class="sxs-lookup"><span data-stu-id="bbc01-225">a.</span></span> <span data-ttu-id="bbc01-226">选择 "合作伙伴中心到 Dynamics 365 (预览体验预览") 或 "合作伙伴中心到 Salesforce (内幕预览版) "。</span><span class="sxs-lookup"><span data-stu-id="bbc01-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="bbc01-227">b.</span><span class="sxs-lookup"><span data-stu-id="bbc01-227">b.</span></span> <span data-ttu-id="bbc01-228">选择 " **编辑** " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="bbc01-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="bbc01-229">c.</span><span class="sxs-lookup"><span data-stu-id="bbc01-229">c.</span></span> <span data-ttu-id="bbc01-230">选择 " **(范围") 同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="bbc01-231">若要基于字段映射自定义 CRM 字段映射 (请) 对于 "创建事件"，选择 " **如果是新的共享机会"，然后选择 "是**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="bbc01-232">**如果是**，请选择 "子步骤"，然后 **在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="bbc01-233">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="bbc01-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="bbc01-234">d.</span><span class="sxs-lookup"><span data-stu-id="bbc01-234">d.</span></span> <span data-ttu-id="bbc01-235">对于 "基于字段映射 (自定义 CRM 字段映射" 指南) 对于 "更新事件"，请单击步骤 " (范围) 同步潜在顾客或机会"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="bbc01-236">e.</span><span class="sxs-lookup"><span data-stu-id="bbc01-236">e.</span></span> <span data-ttu-id="bbc01-237">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="bbc01-238">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后** 展开。</span><span class="sxs-lookup"><span data-stu-id="bbc01-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="bbc01-239">f.</span><span class="sxs-lookup"><span data-stu-id="bbc01-239">f.</span></span> <span data-ttu-id="bbc01-240">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="bbc01-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="bbc01-241">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="bbc01-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="bbc01-242">a.</span><span class="sxs-lookup"><span data-stu-id="bbc01-242">a.</span></span> <span data-ttu-id="bbc01-243">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="bbc01-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="bbc01-244">b.</span><span class="sxs-lookup"><span data-stu-id="bbc01-244">b.</span></span> <span data-ttu-id="bbc01-245">选择 **(范围) 同步机会**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="bbc01-246">c.</span><span class="sxs-lookup"><span data-stu-id="bbc01-246">c.</span></span> <span data-ttu-id="bbc01-247">若要为更新事件自定义 CRM 字段映射，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="bbc01-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="bbc01-248">d.</span><span class="sxs-lookup"><span data-stu-id="bbc01-248">d.</span></span> <span data-ttu-id="bbc01-249">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="bbc01-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="bbc01-250">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="bbc01-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="bbc01-251">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="bbc01-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="bbc01-252">a.</span><span class="sxs-lookup"><span data-stu-id="bbc01-252">a.</span></span> <span data-ttu-id="bbc01-253">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="bbc01-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="bbc01-254">b.</span><span class="sxs-lookup"><span data-stu-id="bbc01-254">b.</span></span> <span data-ttu-id="bbc01-255">选择 **) 同步引用 (范围。**</span><span class="sxs-lookup"><span data-stu-id="bbc01-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="bbc01-256">c.</span><span class="sxs-lookup"><span data-stu-id="bbc01-256">c.</span></span> <span data-ttu-id="bbc01-257">对于 "基于字段映射自定义 CRM 字段映射 (" 指南) 对于创建事件，请选择 " **创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="bbc01-258">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="bbc01-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="bbc01-259">创建了两个环境变量：</span><span class="sxs-lookup"><span data-stu-id="bbc01-259">There are two environment variables created:</span></span>

- <span data-ttu-id="bbc01-260">复选标记：表示是否需要除了在合作伙伴中心与 Dynamics 365 CRM 之间同步双向的商机以外，是否需要复选标记图标。</span><span class="sxs-lookup"><span data-stu-id="bbc01-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="bbc01-261">仅同步共同销售机会：指示是否只同步共同销售机会。</span><span class="sxs-lookup"><span data-stu-id="bbc01-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="bbc01-262">您可以选择编辑环境变量的默认值。</span><span class="sxs-lookup"><span data-stu-id="bbc01-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="默认值的编辑框":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="bbc01-264">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="bbc01-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="bbc01-265">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="bbc01-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="bbc01-266">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbc01-266">Pre-requisites</span></span>

<span data-ttu-id="bbc01-267">若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="bbc01-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="bbc01-268">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="bbc01-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="bbc01-269">一组自定义字段作为 " **机会** " 实体的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="bbc01-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="bbc01-270">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="bbc01-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="bbc01-271">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="bbc01-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="bbc01-272">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="bbc01-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="bbc01-273">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="bbc01-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="bbc01-274">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="bbc01-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="bbc01-275">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助</span><span class="sxs-lookup"><span data-stu-id="bbc01-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="bbc01-276">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="bbc01-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="bbc01-277">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="bbc01-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="bbc01-278">更新 Dynamics 365 CRM 中的机会窗体，使其包含 "产品解决方案" 字段。</span><span class="sxs-lookup"><span data-stu-id="bbc01-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="机会窗体":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="bbc01-281">各种</span><span class="sxs-lookup"><span data-stu-id="bbc01-281">SCENARIOS:</span></span>

1. <span data-ttu-id="bbc01-282">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="bbc01-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="bbc01-283">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="bbc01-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="bbc01-284">在 Dynamics 365 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="bbc01-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="显示 Dynamics 365 中的 Microsoft 合作伙伴中心信息的 &quot;示例机会&quot; 部分。":::

   3. <span data-ttu-id="bbc01-286">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="bbc01-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="bbc01-287">**与合作伙伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="bbc01-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="bbc01-288">**Microsoft Help 如何？**：选择以下各项：</span><span class="sxs-lookup"><span data-stu-id="bbc01-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 中的 &quot;示例机会&quot; 部分，其中显示了一个名为 &quot;Microsoft 如何帮助&quot; 的字段旁边的 Microsoft 合作伙伴中心帮助选项？":::

      - <span data-ttu-id="bbc01-290">**产品**：产品的解决方案 id</span><span class="sxs-lookup"><span data-stu-id="bbc01-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="bbc01-291">一旦在 Dynamics 365 中创建了商机，并将 " **伙伴中心同步** " 选项设置为 **"是"**，请等待10分钟，然后登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="bbc01-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="bbc01-292">你的引用将与 Dynamics 365 同步。</span><span class="sxs-lookup"><span data-stu-id="bbc01-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="bbc01-293">同样，如果将 "与合作伙伴中心同步" 选项设置为 "是"，则在 Dynamics 365 CRM 中更新此机会时，所做的更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="bbc01-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="bbc01-294">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="bbc01-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="bbc01-295">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="bbc01-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="bbc01-296">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="bbc01-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="bbc01-297">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="bbc01-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="bbc01-298">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="bbc01-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="bbc01-299">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="bbc01-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="bbc01-300">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="bbc01-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="bbc01-301">现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="bbc01-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="bbc01-302">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="bbc01-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bbc01-303">后续步骤</span><span class="sxs-lookup"><span data-stu-id="bbc01-303">Next steps</span></span>

- [<span data-ttu-id="bbc01-304">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="bbc01-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="bbc01-305">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="bbc01-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="bbc01-306">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="bbc01-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="bbc01-307">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="bbc01-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)