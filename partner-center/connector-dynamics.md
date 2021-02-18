---
title: Dynamics 365 CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心中的引用与 Dynamics 365 CRM 的共同销售连接器同步。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645681"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="b798e-104">用于 Dynamics 365 CRM 的共同销售连接器–概述</span><span class="sxs-lookup"><span data-stu-id="b798e-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="b798e-105">相应的角色</span><span class="sxs-lookup"><span data-stu-id="b798e-105">Appropriate roles</span></span>

- <span data-ttu-id="b798e-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="b798e-106">Referrals admin</span></span>
- <span data-ttu-id="b798e-107">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="b798e-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b798e-108">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="b798e-108">Partner Center Co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b798e-109">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="b798e-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b798e-110">使用共同销售连接器，可以创建新的共同销售的引用，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受/拒绝引用、修改交易数据（如交易价值和结束日期）。</span><span class="sxs-lookup"><span data-stu-id="b798e-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="b798e-111">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="b798e-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b798e-112">你可以在所选的 CRM 中（而不是在合作伙伴中心）管理你的所有引用。</span><span class="sxs-lookup"><span data-stu-id="b798e-112">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b798e-113">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="b798e-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b798e-114">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="b798e-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b798e-115">**主题**</span><span class="sxs-lookup"><span data-stu-id="b798e-115">**Topics**</span></span>   |<span data-ttu-id="b798e-116">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="b798e-116">**Details**</span></span>   |<span data-ttu-id="b798e-117">**链接**</span><span class="sxs-lookup"><span data-stu-id="b798e-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b798e-118">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="b798e-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b798e-119">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="b798e-119">You need a valid MPN ID</span></span>|<span data-ttu-id="b798e-120">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="b798e-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b798e-121">做好就绪</span><span class="sxs-lookup"><span data-stu-id="b798e-121">Cosell ready</span></span>|<span data-ttu-id="b798e-122">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="b798e-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b798e-123">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="b798e-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b798e-124">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="b798e-124">Partner Center account</span></span>|<span data-ttu-id="b798e-125">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="b798e-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b798e-126">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="b798e-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b798e-127">管理帐户</span><span class="sxs-lookup"><span data-stu-id="b798e-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b798e-128">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="b798e-128">Partner Center user roles</span></span>|<span data-ttu-id="b798e-129">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="b798e-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b798e-130">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="b798e-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| 
|<span data-ttu-id="b798e-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="b798e-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="b798e-132">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="b798e-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b798e-133">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="b798e-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="b798e-134">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="b798e-134">Power Automate Flow Account</span></span>|<span data-ttu-id="b798e-135">创建新的生产环境，其中包含用于测试/过渡和生产的数据库。</span><span class="sxs-lookup"><span data-stu-id="b798e-135">Create new production environment with database for test/staging and production.</span></span> <span data-ttu-id="b798e-136">如果你有包含数据库的现有生产环境，则可以重复使用它。</span><span class="sxs-lookup"><span data-stu-id="b798e-136">If you have an existing production environment with database it can be re-used.</span></span> <span data-ttu-id="b798e-137">要安装连接器解决方案的用户需要具有对此环境的电源自动许可证和访问权限。可以通过单击 "解决方案" [下的 "](https://flow.microsoft.com/) 查看历史记录"，来监视进度并获得更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="b798e-137">User who is going to install connector solution needs to have Power Automate license and access to this environment.You can monitor the progress and get more details should the installation fail in [Power Automate](https://flow.microsoft.com/) by clicking See history under Solutions.</span></span>|[<span data-ttu-id="b798e-138">创建或管理环境</span><span class="sxs-lookup"><span data-stu-id="b798e-138">Create or manage environment</span></span>](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="b798e-139">安装适用于 Dynamics 365 (Power 自动化解决方案的合作伙伴中心引用同步) </span><span class="sxs-lookup"><span data-stu-id="b798e-139">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="b798e-140">请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="b798e-140">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b798e-141">此步骤将显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="b798e-141">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b798e-142">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="b798e-142">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="b798e-143">选择左侧导航栏上的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="b798e-143">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b798e-144">单击顶部菜单上的 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="b798e-144">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. <span data-ttu-id="b798e-146">在弹出屏幕中搜索 **Dynamics365 的合作伙伴中心引用连接器** 。</span><span class="sxs-lookup"><span data-stu-id="b798e-146">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="b798e-147">单击 " **立即获取** " 按钮，然后 **继续**。</span><span class="sxs-lookup"><span data-stu-id="b798e-147">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="b798e-148">这将打开一个页面，可在其中选择 CRM (Dynamics 365) 环境以安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="b798e-148">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="b798e-149">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="b798e-149">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="b798e-150">可以通过单击 "**解决方案**" 下的 "**查看历史记录**"，来监视进度并获得更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="b798e-150">You can monitor the progress and get more details should the installation fail in Power Automate by clicking **See history** under **Solutions**.</span></span>
 

9. <span data-ttu-id="b798e-151">安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="b798e-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b798e-152">请注意，"解决方案" 列表中提供了 **Dynamics 365 的合作伙伴中心引用同步** 。</span><span class="sxs-lookup"><span data-stu-id="b798e-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b798e-153">选择 **Dynamics 365 的伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="b798e-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="b798e-154">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="b798e-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用 CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b798e-156">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="b798e-156">Best practice: test before you go live</span></span>

<span data-ttu-id="b798e-157">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b798e-158">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="b798e-159">在过渡环境中配置和自定义 Microsoft Power 自动化解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-159">Configure and customize the Microsoft Power Automate solution in staging environment.</span></span>
- <span data-ttu-id="b798e-160">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="b798e-161">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="b798e-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="b798e-162">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="b798e-162">Configure the solution</span></span>

1. <span data-ttu-id="b798e-163">在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="b798e-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="b798e-164">在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="b798e-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="b798e-165">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="b798e-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="b798e-166">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="b798e-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="b798e-167">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="b798e-167">Partner Center Events</span></span>

   - <span data-ttu-id="b798e-168">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="b798e-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="b798e-169">从左侧导航栏中选择 " **连接** "，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="b798e-170">通过单击 " **创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="b798e-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="创建连接":::

      3. <span data-ttu-id="b798e-172">在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。</span><span class="sxs-lookup"><span data-stu-id="b798e-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="b798e-173">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="b798e-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="b798e-174">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="b798e-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="b798e-175">为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。</span><span class="sxs-lookup"><span data-stu-id="b798e-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
      7. <span data-ttu-id="b798e-176">添加所有连接后，你的环境中应会显示以下连接：</span><span class="sxs-lookup"><span data-stu-id="b798e-176">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="连接":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="b798e-178">编辑连接</span><span class="sxs-lookup"><span data-stu-id="b798e-178">Edit the connections</span></span>

1. <span data-ttu-id="b798e-179">返回 " **解决方案** " 页，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-179">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="b798e-180">通过单击 "**全部**" **(预览) 选择 "连接引用**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-180">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="“连接”":::

2. <span data-ttu-id="b798e-182">通过选择三个点图标，逐个编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="b798e-182">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="b798e-183">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="b798e-183">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="列出的连接"::: 

3.  <span data-ttu-id="b798e-185">返回到 "解决方案" 页，为 Dynamics 365 选择 "合作伙伴中心引用同步"，然后单击以下序列中每个流旁边的三个点图标，打开流。</span><span class="sxs-lookup"><span data-stu-id="b798e-185">Return to the Solutions page, select Partner Center Referrals Synchronization for Dynamics 365 and turn on the flow by clicking on three dots icon next to each flow in the following sequence.</span></span> <span data-ttu-id="b798e-186">如果在打开流时遇到任何问题，请参阅 [自定义步骤](connector-dynamics.md#customize-synchronization-steps) 和 [故障排除步骤](connectors-troubleshoot.md)。</span><span class="sxs-lookup"><span data-stu-id="b798e-186">If you encounter any issues while turning on the flow refer to [customization steps](connector-dynamics.md#customize-synchronization-steps) and [troubleshooting steps](connectors-troubleshoot.md).</span></span> 

<span data-ttu-id="b798e-187">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="b798e-187">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="b798e-188"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="b798e-188">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="b798e-189">创建共同销售引用– Dynamics 365 到合作伙伴中心 (预览体验中心) </span><span class="sxs-lookup"><span data-stu-id="b798e-189">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b798e-190">来自创建或获取 Dynamics 365 流中的详细信息</span><span class="sxs-lookup"><span data-stu-id="b798e-190">[Customize] Create or Get Details from Dynamics 365 flow</span></span> 
- <span data-ttu-id="b798e-191">合作伙伴中心到 Dynamics 365-Helper (预览体验中心) </span><span class="sxs-lookup"><span data-stu-id="b798e-191">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="b798e-192">合作伙伴中心 Microsoft 共同销售对 Dynamics 365 (预览体验的引用更新) </span><span class="sxs-lookup"><span data-stu-id="b798e-192">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="b798e-193">合作伙伴中心到 Dynamics 365 (预览体验体验) </span><span class="sxs-lookup"><span data-stu-id="b798e-193">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="b798e-194">Dynamics 365 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="b798e-194">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b798e-195">Dynamics 365 到合作伙伴中心 (有问必答预览版的机会) </span><span class="sxs-lookup"><span data-stu-id="b798e-195">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b798e-196">Dynamics 365 的 Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="b798e-196">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b798e-197">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="b798e-197">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b798e-198">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="b798e-198">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b798e-199">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="b798e-199">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b798e-200">选择 " **合作伙伴中心到 Dynamics 365 (预览体验预览")**。</span><span class="sxs-lookup"><span data-stu-id="b798e-200">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

2. <span data-ttu-id="b798e-201">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-201">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

3. <span data-ttu-id="b798e-202">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="b798e-202">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="复制 URL":::

4. <span data-ttu-id="b798e-204">现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-204">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

5. <span data-ttu-id="b798e-205">确保在右侧窗格中打开 "运行流" 窗口，然后单击 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-205">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

6. <span data-ttu-id="b798e-206">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="b798e-206">Enter the following details:</span></span>

   - <span data-ttu-id="b798e-207">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="b798e-207">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

   - <span data-ttu-id="b798e-208">**要注册的事件**：选择所有可用事件 ( "引用已创建"、"引用已更新"、"相关-引用已创建"、"相关引用-已更新" ) </span><span class="sxs-lookup"><span data-stu-id="b798e-208">**Events to Register**: Select all available events (“referral-created”, “referral-updated”, “related-referral-created”, “related-referral-updated”)</span></span>

   <span data-ttu-id="b798e-209">-**覆盖现有触发器终结点（如果存在**）：是重要的，请务必注意，只能为给定 webhook 事件注册一个 URL。</span><span class="sxs-lookup"><span data-stu-id="b798e-209">-**Overwrite existing trigger endpoints if present**: Yes It is important to note that only one URL can be registered for a given webhook event.</span></span> <span data-ttu-id="b798e-210">请务必注意，只能为给定 webhook 事件注册一个 URL。</span><span class="sxs-lookup"><span data-stu-id="b798e-210">It is important to note that only one URL can be registered for a given webhook event.</span></span> 

7. <span data-ttu-id="b798e-211">选择 " **运行** "，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="b798e-211">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b798e-212">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="b798e-212">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b798e-213">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="b798e-213">Customize synchronization steps</span></span>

<span data-ttu-id="b798e-214">CRM 系统经过高度自定义，你可以基于 CRM 设置自定义电源自动化解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-214">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span>  <span data-ttu-id="b798e-215">当共同销售的引用在合作伙伴中心与你的 CRM 系统之间同步时，在 " [自定义字段映射指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)" 中列出了在合作伙伴中心电脑上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-215">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="b798e-216">按照字段映射指南进行操作，如有必要，请在 **[自定义] 创建或获取 Dynamics 365 flow**  或环境变量的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b798e-216">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow**  or environment variables.</span></span> <span data-ttu-id="b798e-217">建议不要更新 Power 自动解决方案中的任何其他流，因为它可能会影响将来的解决方案升级。</span><span class="sxs-lookup"><span data-stu-id="b798e-217">It is recommended not to update any other flows in Power Automate solution as it can impact future solution upgrades.</span></span> 

<span data-ttu-id="b798e-218">可用的自定义如下：</span><span class="sxs-lookup"><span data-stu-id="b798e-218">The following are the available customizations:</span></span>

- <span data-ttu-id="b798e-219">"复选标记出现机会名称"：默认情况下，将在 "机会名称" 旁显示一个复选标记，指示合作伙伴中心与 Dynamics 365 CRM 之间的同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="b798e-219">Check mark in Opportunity name: By default, a check mark will be displayed next to Opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="b798e-220">同样，如果同步失败，将显示交叉标记。</span><span class="sxs-lookup"><span data-stu-id="b798e-220">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="b798e-221">若要避免在 "机会名称" 中添加复选标记或交叉标记，请将机会 name 环境变量中显示复选标记的当前值设置为 "否"。</span><span class="sxs-lookup"><span data-stu-id="b798e-221">To avoid adding check or cross mark in Opportunity name, set the current value of Display check mark in opportunity name environment variable to No.</span></span>

- <span data-ttu-id="b798e-222">交易价值：默认情况下，来自合作伙伴中心的交易值将与 CRM 中的 **estimatedvalue** 同步。</span><span class="sxs-lookup"><span data-stu-id="b798e-222">Deal value: By default, deal value from Partner Center will be synced to and from **estimatedvalue** in CRM.</span></span> <span data-ttu-id="b798e-223">如果 CRM 中有不同的字段要从中同步值，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b798e-223">If you have a different field in CRM for deal value to sync from:</span></span>

    <span data-ttu-id="b798e-224">a.</span><span class="sxs-lookup"><span data-stu-id="b798e-224">a.</span></span>    <span data-ttu-id="b798e-225">在 Dynamics 365 环境变量中，用 CRM 的字段名称更新交易值字段名称。</span><span class="sxs-lookup"><span data-stu-id="b798e-225">Update Deal value field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="b798e-226">请注意，应提供字段名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="b798e-226">Note that you should provide the field’s name not its display name.</span></span>

    <span data-ttu-id="b798e-227">b.</span><span class="sxs-lookup"><span data-stu-id="b798e-227">b.</span></span>    <span data-ttu-id="b798e-228">编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**  ，并导航到 crm 中的 " **创建或更新** 机会" 和 "更新" " **创建新机会** 并 **更新现有机会** 操作"，将 **DealValue** 值分配到 CRM 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update** opportunity in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign **DealValue** value to correct field in CRM.</span></span> <span data-ttu-id="b798e-229">同时，从 "**估计收入**" 字段中删除 **DealValue 分配**。</span><span class="sxs-lookup"><span data-stu-id="b798e-229">Also, remove **DealValue assignment** from **Estimated Revenue** field.</span></span>

- <span data-ttu-id="b798e-230">客户帐户国家/地区代码：创建新引用时，必须提供两个字母的国家/地区代码 (ISO 3166) 。</span><span class="sxs-lookup"><span data-stu-id="b798e-230">Customer Account Country Code: It is mandatory to provide a two-letter country code (ISO 3166) when creating a new referral.</span></span> <span data-ttu-id="b798e-231">默认情况下，国家/地区代码将同步到 CRM 中的帐户 address1_country 字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-231">By default, country code will be synced to and from Account’s address1_country field in CRM.</span></span> <span data-ttu-id="b798e-232">如果 CRM 中的 "国家/地区代码" 字段不同，则：</span><span class="sxs-lookup"><span data-stu-id="b798e-232">If you have a different field in CRM for country code to sync from:</span></span>

   <span data-ttu-id="b798e-233">a.</span><span class="sxs-lookup"><span data-stu-id="b798e-233">a.</span></span>    <span data-ttu-id="b798e-234">对于包含两个字母代码的帐户的非查找国家/地区代码字段：</span><span class="sxs-lookup"><span data-stu-id="b798e-234">For a non-lookup country code field in Account which contains two-letter code:</span></span>

   - <span data-ttu-id="b798e-235">用 CRM 的字段名称更新 Dynamics 365 环境变量中的客户帐户国家/地区代码字段名称。</span><span class="sxs-lookup"><span data-stu-id="b798e-235">Update Customer account country code field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="b798e-236">请注意，应提供字段名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="b798e-236">Note that you should provide the field’s name not its display name.</span></span>

   - <span data-ttu-id="b798e-237">编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息**  ，并导航到 "创建或获取 crm 中的客户帐户" 操作，以将国家/地区值分配到 crm 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-237">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to Create or get customer account in CRM action to assign Country value to correct field in CRM.</span></span> <span data-ttu-id="b798e-238">同时，从地址1：国家/地区字段中删除国家/地区值分配。</span><span class="sxs-lookup"><span data-stu-id="b798e-238">Also, remove Country value assignment from Address 1: Country/Region field.</span></span>

   <span data-ttu-id="b798e-239">b.</span><span class="sxs-lookup"><span data-stu-id="b798e-239">b.</span></span>    <span data-ttu-id="b798e-240">对于帐户中的基于查找的国家/地区代码字段：</span><span class="sxs-lookup"><span data-stu-id="b798e-240">For a lookup-based country code field in Account:</span></span>

   - <span data-ttu-id="b798e-241">在帐户中添加新的自定义字段并使用两个字母的国家/地区代码自动填充它 (ISO 3166) 基于基于查找的字段中选择的值，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="b798e-241">Add a new custom field in Account and auto-populate it with two-letter country code (ISO 3166) based on the value selected in lookup-based field and vice-versa.</span></span>

   - <span data-ttu-id="b798e-242">对于非查找国家/地区代码字段，请按照上述步骤将新的自定义字段从 CRM 同步到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="b798e-242">Follow the steps above for non-lookup country code field to sync new custom field from CRM to and from Partner Center.</span></span>

- <span data-ttu-id="b798e-243">机会字段：如果存在需要填充的商机中的必填字段，则编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息**  ，并导航到 "在 CRM 中 **创建或更新机会** " 和 "更新" " **创建新机会" 操作** ，以根据业务要求向必填字段分配值。</span><span class="sxs-lookup"><span data-stu-id="b798e-243">Opportunity fields: If there are mandatory fields in Opportunity that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update opportunity** in CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="b798e-244">潜在客户字段：如果潜在顾客需要填充，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息**  ，并导航到 **创建或更新** CRM 中的潜在客户，并更新 **创建新的潜在客户操作** ，根据业务需求将值分配到必填字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-244">Lead fields: If there are mandatory fields in Lead that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update lead** in CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="b798e-245">客户帐户：如果新的引用从合作伙伴中心同步到 CRM，则 Power 自动解决方案将尝试使用客户公司名称和邮政编码搜索 CRM 中的现有帐户。</span><span class="sxs-lookup"><span data-stu-id="b798e-245">Customer Account: When a new referral is synced from Partner Center to CRM, Power Automate solution tries to search for an existing account in CRM using customer company name and postal code.</span></span> <span data-ttu-id="b798e-246">如果找不到，将在 CRM 中创建新的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="b798e-246">If it does not find one, a new customer account will be created in CRM.</span></span> <span data-ttu-id="b798e-247">若要更新搜索条件和创建新帐户的详细信息，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息** ，然后导航到 **创建或获取** CRM 中的客户帐户并 **创建客户帐户操作**。</span><span class="sxs-lookup"><span data-stu-id="b798e-247">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and navigate to **Create or get customer account** in CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="b798e-248">更新环境变量</span><span class="sxs-lookup"><span data-stu-id="b798e-248">Update environment variable</span></span>

<span data-ttu-id="b798e-249">更新环境变量值：</span><span class="sxs-lookup"><span data-stu-id="b798e-249">To update an environment variable value:</span></span>

1. <span data-ttu-id="b798e-250">单击 " **解决方案** " 页，然后选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-250">Go to **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="b798e-251">通过单击 "全部" 选择 **环境变量** 。</span><span class="sxs-lookup"><span data-stu-id="b798e-251">Select **Environment Variable** by clicking All.</span></span>

2. <span data-ttu-id="b798e-252">为需要更新的值选择环境变量，然后单击 "使用三个点图标 **编辑** " 图标。</span><span class="sxs-lookup"><span data-stu-id="b798e-252">Select the environment variable for the value that needs to be updated and click **Edit** using three dots icon.</span></span>

3. <span data-ttu-id="b798e-253">更新 **当前值** (不要使用 **新值** 选项更新默认值) 并提供值。</span><span class="sxs-lookup"><span data-stu-id="b798e-253">Update **Current Value** (do not update Default Value) using **New value** option and provide the value.</span></span> <span data-ttu-id="b798e-254">值必须与变量的数据类型相匹配，例如 Yes/No 数据类型将接受 Yes 或 No 值。</span><span class="sxs-lookup"><span data-stu-id="b798e-254">Value must match the Data type of the variable for e.g. Yes/No data type will accept either Yes or No value.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="默认值的编辑框":::

- <span data-ttu-id="b798e-256">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="b798e-256">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b798e-257">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="b798e-257">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b798e-258">先决条件</span><span class="sxs-lookup"><span data-stu-id="b798e-258">Pre-requisites</span></span>

<span data-ttu-id="b798e-259">若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-259">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="b798e-260">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="b798e-260">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b798e-261">一组自定义字段和对象将作为解决方案安装的一部分添加。</span><span class="sxs-lookup"><span data-stu-id="b798e-261">A set of custom fields and objects will get added as part of the solution installation.</span></span> <span data-ttu-id="b798e-262">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="b798e-262">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b798e-263">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="b798e-263">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b798e-264">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步。</span><span class="sxs-lookup"><span data-stu-id="b798e-264">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center.</span></span> <span data-ttu-id="b798e-265">默认情况下，此字段的值为 "否"，并且你的卖方需要将其显式设置为 "是"，以便与 Microsoft 共享机会。</span><span class="sxs-lookup"><span data-stu-id="b798e-265">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="b798e-266">从合作伙伴中心到 CRM 共享的新引用将此字段值设置为 "是"。</span><span class="sxs-lookup"><span data-stu-id="b798e-266">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="b798e-267">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="b798e-267">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b798e-268">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="b798e-268">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>
- <span data-ttu-id="b798e-269">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助。</span><span class="sxs-lookup"><span data-stu-id="b798e-269">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="b798e-270">若要创建共同销售引用，请选择 Microsoft 所需的适当帮助。</span><span class="sxs-lookup"><span data-stu-id="b798e-270">To create a co-sell referral, select appropriate help required from Microsoft.</span></span> <span data-ttu-id="b798e-271">必须将客户联系人关联到创建共同销售引用的机会。</span><span class="sxs-lookup"><span data-stu-id="b798e-271">A customer contact must be associated to the Opportunity to create a co-sell referral.</span></span> <span data-ttu-id="b798e-272">若要创建非共同销售引用，请将此字段取消选中状态。</span><span class="sxs-lookup"><span data-stu-id="b798e-272">To create a non co-sell referral leave this field un-selected.</span></span> <span data-ttu-id="b798e-273">通过选择相应的 "必需帮助" 选项，可以随时将非共同销售引用转换为共同销售引用。</span><span class="sxs-lookup"><span data-stu-id="b798e-273">A non co-sell referral can be converted to a co-sell referral anytime by selecting appropriate help required option.</span></span>

- <span data-ttu-id="b798e-274">**Microsoft 合作伙伴中心引用可见性**：选择 Microsoft 合作伙伴中心引用的可见性。</span><span class="sxs-lookup"><span data-stu-id="b798e-274">**Microsoft Partner Center Referral Visibility**: Select visibility for Microsoft Partner Center Referral.</span></span> <span data-ttu-id="b798e-275">通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。</span><span class="sxs-lookup"><span data-stu-id="b798e-275">By making it visible to Microsoft sellers, a non co-sell referral may get converted to co-sell.</span></span> <span data-ttu-id="b798e-276">如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会看到引用。</span><span class="sxs-lookup"><span data-stu-id="b798e-276">When Microsoft help is required, referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="b798e-277">标记为可见后，此字段将无法还原。</span><span class="sxs-lookup"><span data-stu-id="b798e-277">Once marked as visible this field cannot be reverted.</span></span>

- <span data-ttu-id="b798e-278">**MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。</span><span class="sxs-lookup"><span data-stu-id="b798e-278">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft’s CRM identifier.</span></span>

- <span data-ttu-id="b798e-279">**产品：已过时** –不要使用此字段或将其添加到 CRM 部分，仅可用于向后兼容性。</span><span class="sxs-lookup"><span data-stu-id="b798e-279">**Products: Obsolete** – do not use this field or add it to CRM section, it is available for backward compatibility only.</span></span> <span data-ttu-id="b798e-280">改为使用 Microsoft 合作伙伴中心解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-280">Use Microsoft Partner Center Solutions instead.</span></span>

- <span data-ttu-id="b798e-281">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="b798e-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

- <span data-ttu-id="b798e-282">**Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。</span><span class="sxs-lookup"><span data-stu-id="b798e-282">**Microsoft Partner Center Solutions**: A custom object to associate Co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="b798e-283">可以在商机中添加和/或删除一个或多个解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-283">One or more solutions can be added and/or removed from the Opportunity.</span></span> <span data-ttu-id="b798e-284">在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-284">It is mandatory to add at least one Co-sell ready or Microsoft solution to the Opportunity before sharing it with Microsoft.</span></span> <span data-ttu-id="b798e-285">若要将此对象与商机关联，请在 CRM 中更新商机窗体：</span><span class="sxs-lookup"><span data-stu-id="b798e-285">To associate this object to Opportunity, update the Opportunity form in CRM:</span></span>

  <span data-ttu-id="b798e-286">选择 "机会窗体" 中适当的选项卡，并添加子网格，如下所示：</span><span class="sxs-lookup"><span data-stu-id="b798e-286">Select the appropriate tab in Opportunity form and add a sub-grid as shown below:</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="机会窗体":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- <span data-ttu-id="b798e-289">添加 Microsoft 解决方案后，你可以预先填充联合销售就绪解决方案的详细信息，以便你的卖方不必添加它们。</span><span class="sxs-lookup"><span data-stu-id="b798e-289">After adding Microsoft Solutions, you can pre-populate Co-sell ready solutions details so that your sellers don’t have to add them.</span></span> <span data-ttu-id="b798e-290">若要添加新的解决方案详细信息，请前往 CRM 中的 Microsoft 解决方案详细信息对象，然后单击 " **添加记录** " 添加一个条目或使用 **Excel 上传** 添加多个条目。</span><span class="sxs-lookup"><span data-stu-id="b798e-290">To add a new solution detail, go to Microsoft Solution Details object in CRM and click on **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

:::image type="content" source="images/dynamic-1a.png" alt-text="解决方案详细信息":::

### <a name="scenarios"></a><span data-ttu-id="b798e-292">各种</span><span class="sxs-lookup"><span data-stu-id="b798e-292">SCENARIOS:</span></span>

1. <span data-ttu-id="b798e-293">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="b798e-293">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="b798e-294">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="b798e-294">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="b798e-295">确保在 Dynamics 365 环境中创建 "新机会" 时出现 Microsoft 合作伙伴中心部分</span><span class="sxs-lookup"><span data-stu-id="b798e-295">Ensure that the Microsoft Partner Center section  is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   :::image type="content" source="images/dynamic-2a.png" alt-text="新机会"::: 

   3. <span data-ttu-id="b798e-297">若要将此机会与合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="b798e-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="b798e-298">**Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。</span><span class="sxs-lookup"><span data-stu-id="b798e-298">**How can Microsoft help?**: To create a Co-sell referral select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="如何在卡片视图中获取相应的字段":::

      - <span data-ttu-id="b798e-300">**客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。</span><span class="sxs-lookup"><span data-stu-id="b798e-300">**Customer Contact**: To create a Co-sell referral, add a customer contact to Opportunity.</span></span>
      - <span data-ttu-id="b798e-301">**与合作伙伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="b798e-301">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="b798e-302">Microsoft 解决方案：若要与 Microsoft 共享引用，请向商机添加有效的合作销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="b798e-302">Microsoft Solutions: To share a referral with Microsoft, add a valid Co-sell ready or Microsoft solution to Opportunity.</span></span>
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="解决方案 ID":::

   4. <span data-ttu-id="b798e-304">一旦在 Dynamics 365 中创建了商机，并将 "伙伴中心同步" 选项设置为 "是"，请等待10分钟，然后登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="b798e-304">Once the opportunity is created in Dynamics 365 with Sync with Partner Center option set to Yes, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="b798e-305">你的引用将与 Dynamics 365 和引用标识符同步。</span><span class="sxs-lookup"><span data-stu-id="b798e-305">Your referrals will be synchronized with Dynamics 365 and Referral Identifier.</span></span> <span data-ttu-id="b798e-306">将填充引用链接。</span><span class="sxs-lookup"><span data-stu-id="b798e-306">Referral Link will get populated.</span></span> <span data-ttu-id="b798e-307">如果失败，将使用错误信息填充审核字段。</span><span class="sxs-lookup"><span data-stu-id="b798e-307">In case of a failure, the audit field will be populated with error information.</span></span>
     
    5. <span data-ttu-id="b798e-308">同样，如果将 "与合作伙伴中心同步" 选项设置为 "是"，则在 Dynamics 365 CRM 中更新此机会时，所做的更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="b798e-308">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    6. <span data-ttu-id="b798e-309">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="b798e-309">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="b798e-310">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="b798e-310">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="b798e-311">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="b798e-311">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="b798e-312">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="b798e-312">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="b798e-313">通过选择 "  **新建交易** " 选项，从合作伙伴中心创建新的共同销售引用。</span><span class="sxs-lookup"><span data-stu-id="b798e-313">Create a new Co-sell referral from Partner Center by selecting the  **New deal** option.</span></span>

   4. <span data-ttu-id="b798e-314">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="b798e-314">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="b798e-315">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="b798e-315">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b798e-316">现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="b798e-316">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="b798e-317">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="b798e-317">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b798e-318">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b798e-318">Next steps</span></span>

- [<span data-ttu-id="b798e-319">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="b798e-319">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b798e-320">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="b798e-320">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b798e-321">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="b798e-321">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="b798e-322">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="b798e-322">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)