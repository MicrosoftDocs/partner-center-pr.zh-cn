---
title: Dynamics 365 CRM 合作伙伴中心的共同销售连接器
description: 将合作伙伴中心中的引用与 Dynamics 365 CRM 的共同销售连接器同步。 然后，你可以在 CRM 系统中与 Microsoft 进行共同销售。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: c399e00394208ec29dd59a41afe7cce1b1d07253
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284326"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a><span data-ttu-id="fb244-104">用于 Dynamics 365 CRM 概述的共同销售连接器</span><span class="sxs-lookup"><span data-stu-id="fb244-104">Co-sell connector for Dynamics 365 CRM overview</span></span>

<span data-ttu-id="fb244-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="fb244-105">**Appropriate roles**</span></span>

- <span data-ttu-id="fb244-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="fb244-106">Referrals admin</span></span>
- <span data-ttu-id="fb244-107">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="fb244-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="fb244-108">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="fb244-108">Partner Center co-sell connectors enable your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="fb244-109">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="fb244-109">They won't have to be trained to use Partner Center to manage co-sell deals.</span></span> <span data-ttu-id="fb244-110">使用共同销售连接器创建新的共同销售的参考，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受或拒绝推荐，并修改交易数据（如交易价值和结束日期）。</span><span class="sxs-lookup"><span data-stu-id="fb244-110">Use the co-sell connectors to create a new co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept or decline referrals, and modify deal data such as deal value and closing date.</span></span> <span data-ttu-id="fb244-111">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="fb244-111">You can also receive any updates from the Microsoft sellers on these co-sell deals.</span></span> <span data-ttu-id="fb244-112">你可以在所选的 CRM 中（而不是在合作伙伴中心）管理你的所有引用。</span><span class="sxs-lookup"><span data-stu-id="fb244-112">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="fb244-113">此解决方案基于电源自动化，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="fb244-113">The solution is based on Power Automate and uses Partner Center APIs.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb244-114">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb244-114">Prerequisites</span></span>

<span data-ttu-id="fb244-115">在安装解决方案之前，请确保满足以下先决条件。</span><span class="sxs-lookup"><span data-stu-id="fb244-115">Before you install the solution, make sure to meet the following prerequisites.</span></span>

|<span data-ttu-id="fb244-116">**主题**</span><span class="sxs-lookup"><span data-stu-id="fb244-116">**Topics**</span></span>   |<span data-ttu-id="fb244-117">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="fb244-117">**Details**</span></span>   |<span data-ttu-id="fb244-118">**链接**</span><span class="sxs-lookup"><span data-stu-id="fb244-118">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="fb244-119">Microsoft 合作伙伴网络 (MPN) ID</span><span class="sxs-lookup"><span data-stu-id="fb244-119">Microsoft Partner Network (MPN) ID</span></span> |<span data-ttu-id="fb244-120">需要一个有效的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="fb244-120">You need a valid MPN ID.</span></span>|[<span data-ttu-id="fb244-121">加入合作伙伴网络</span><span class="sxs-lookup"><span data-stu-id="fb244-121">Join the Partner Network</span></span>](https://partner.microsoft.com/)|
|<span data-ttu-id="fb244-122">已做好联合销售准备</span><span class="sxs-lookup"><span data-stu-id="fb244-122">Co-sell ready</span></span>|<span data-ttu-id="fb244-123">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="fb244-123">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="fb244-124">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="fb244-124">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="fb244-125">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="fb244-125">Partner Center account</span></span>|<span data-ttu-id="fb244-126">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="fb244-126">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your co-sell solution.</span></span> <span data-ttu-id="fb244-127">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="fb244-127">Verify that you can see your co-sell referrals in the Partner Center portal before you deploy the connectors.</span></span>|[<span data-ttu-id="fb244-128">管理帐户</span><span class="sxs-lookup"><span data-stu-id="fb244-128">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="fb244-129">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="fb244-129">Partner Center user roles</span></span>|<span data-ttu-id="fb244-130">将安装和使用连接器的员工必须是推荐管理员。</span><span class="sxs-lookup"><span data-stu-id="fb244-130">The employee who will install and use the connectors must be a Referrals admin.</span></span>|[<span data-ttu-id="fb244-131">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="fb244-131">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="fb244-132">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="fb244-132">Dynamics 365 CRM</span></span>|<span data-ttu-id="fb244-133">CRM 用户角色是系统管理员或系统定制员。</span><span class="sxs-lookup"><span data-stu-id="fb244-133">The CRM user role is System admin or System customizer.</span></span>|[<span data-ttu-id="fb244-134">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="fb244-134">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="fb244-135">Power 自动化 flow 帐户</span><span class="sxs-lookup"><span data-stu-id="fb244-135">Power Automate flow account</span></span>|<span data-ttu-id="fb244-136">使用数据库创建新的生产环境，以便进行测试、过渡和生产。</span><span class="sxs-lookup"><span data-stu-id="fb244-136">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="fb244-137">如果你有一个具有数据库的现有生产环境，则可以重复使用它。</span><span class="sxs-lookup"><span data-stu-id="fb244-137">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="fb244-138">要安装连接器解决方案的用户必须具有对此环境的电源自动执行许可和访问权限。</span><span class="sxs-lookup"><span data-stu-id="fb244-138">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="fb244-139">如果安装失败，你可以监视进度并在 [电源自动执行](https://flow.microsoft.com/) 中获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="fb244-139">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="fb244-140">选择 "**解决方案**" 下的 "**查看历史记录**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-140">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="fb244-141">创建或管理环境</span><span class="sxs-lookup"><span data-stu-id="fb244-141">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="fb244-142">安装适用于 Dynamics 365 (Power 自动化解决方案的合作伙伴中心引用同步) </span><span class="sxs-lookup"><span data-stu-id="fb244-142">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate solution)</span></span>

1. <span data-ttu-id="fb244-143">请继续 [执行 "电源自动](https://flow.microsoft.com)"，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="fb244-143">Go to [Power Automate](https://flow.microsoft.com), and select **Environments** in the upper-right corner.</span></span> <span data-ttu-id="fb244-144">此步骤将显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="fb244-144">This step will show you the available CRM instances.</span></span>

1. <span data-ttu-id="fb244-145">从右上角的下拉列表中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="fb244-145">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="fb244-146">选择左侧的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="fb244-146">Select **Solutions** on the left.</span></span>

1. <span data-ttu-id="fb244-147">在顶部菜单中选择 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="fb244-147">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="显示 &quot;打开 AppSource&quot; 的屏幕截图。":::

1. <span data-ttu-id="fb244-149">在弹出屏幕上搜索 **Dynamics 365 的合作伙伴中心引用连接器** 。</span><span class="sxs-lookup"><span data-stu-id="fb244-149">Search for **Partner Center Referrals Connectors for Dynamics 365** in the pop-up screen.</span></span>  

1. <span data-ttu-id="fb244-150">选择 " **立即获取** " 按钮，然后选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-150">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="fb244-151">此时将显示一个页面，可在其中选择 CRM (Dynamics 365) 环境以安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="fb244-151">A page appears where you can select the CRM (Dynamics 365) environment to install the application.</span></span> <span data-ttu-id="fb244-152">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="fb244-152">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="fb244-153">你可以监视进度，如果安装失败，你可以通过选择 "**解决方案**" 下的 "**查看历史记录**" 来获取有关 Power 自动功能的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="fb244-153">You can monitor the progress and, if the installation fails, you can get more details in Power Automate by selecting **See history** under **Solutions**.</span></span>

1. <span data-ttu-id="fb244-154">安装完成后，请返回到 " [自动执行电源](https://flow.microsoft.com) "，并选择左侧的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="fb244-154">After the installation is complete, go back to [Power Automate](https://flow.microsoft.com) and select **Solutions** on the left.</span></span> <span data-ttu-id="fb244-155">**合作伙伴中心引用同步 Dynamics 365** 现已在 **解决方案** 列表中提供。</span><span class="sxs-lookup"><span data-stu-id="fb244-155">**Partner Center Referrals Synchronization for Dynamics 365** is now available in the **Solutions** list.</span></span>

1. <span data-ttu-id="fb244-156">选择 **Dynamics 365 的伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="fb244-156">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="fb244-157">可以使用以下功能自动执行流和实体。</span><span class="sxs-lookup"><span data-stu-id="fb244-157">The following Power Automate flows and entities are available.</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="显示可用 Crm 的屏幕截图。":::

## <a name="test-before-you-go-live"></a><span data-ttu-id="fb244-159">投入之前测试</span><span class="sxs-lookup"><span data-stu-id="fb244-159">Test before you go live</span></span>

<span data-ttu-id="fb244-160">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-160">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span> <span data-ttu-id="fb244-161">你将需要：</span><span class="sxs-lookup"><span data-stu-id="fb244-161">You'll need to:</span></span>

- <span data-ttu-id="fb244-162">在过渡环境 CRM 实例上安装电源自动化解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-162">Install the Power Automate solution on a staging environment CRM instance.</span></span>
- <span data-ttu-id="fb244-163">在过渡环境中配置和自定义电源自动化解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-163">Configure and customize the Power Automate solution in a staging environment.</span></span>
- <span data-ttu-id="fb244-164">在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-164">Test the solution on a staging CRM instance.</span></span>
- <span data-ttu-id="fb244-165">成功测试后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="fb244-165">After a successful test, import as a managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="fb244-166">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="fb244-166">Configure the solution</span></span>

1. <span data-ttu-id="fb244-167">在 CRM 实例中安装解决方案后，请返回到 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="fb244-167">After you've installed the solution in your CRM instance, go back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="fb244-168">在右上角的 " **环境** " 下拉列表中，选择在其中安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="fb244-168">From the **Environments** drop-down list in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="fb244-169">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="fb244-169">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="fb244-170">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="fb244-170">Partner Center user with Referrals admin credentials</span></span>
   - <span data-ttu-id="fb244-171">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="fb244-171">Partner Center Events</span></span>
   - <span data-ttu-id="fb244-172">CRM 管理员，并在解决方案中自动执行流程</span><span class="sxs-lookup"><span data-stu-id="fb244-172">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="fb244-173">选择左侧的 " **连接** "，并从列表中选择 " **合作伙伴中心引用** " 解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-173">Select **Connections** on the left, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="fb244-174">通过选择 " **创建连接**" 来创建连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-174">Create a connection by selecting **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="显示 &quot;创建连接&quot; 的屏幕截图。":::

   1. <span data-ttu-id="fb244-176">在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。</span><span class="sxs-lookup"><span data-stu-id="fb244-176">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="fb244-177">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-177">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="fb244-178">接下来，使用 "引用管理员" 凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-178">Next, create a Partner Center Events connection for your Partner Center user with the Referrals admin credentials.</span></span>

   1. <span data-ttu-id="fb244-179">为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-179">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
   1. <span data-ttu-id="fb244-180">添加所有连接后，你的环境中应会显示以下连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-180">After you've added all the connections, you should see the following connections in your environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="显示连接的屏幕截图。":::

## <a name="edit-the-connections"></a><span data-ttu-id="fb244-182">编辑连接</span><span class="sxs-lookup"><span data-stu-id="fb244-182">Edit the connections</span></span>

1. <span data-ttu-id="fb244-183">返回 " **解决方案** " 页，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-183">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="fb244-184">通过选择 "**全部**" **(预览) 选择 "连接引用**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-184">Select **Connection Reference (preview)** by selecting **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="显示编辑连接的屏幕截图。":::

1. <span data-ttu-id="fb244-186">通过选择省略号图标，分别编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-186">Edit each of the connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="fb244-187">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="fb244-187">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="显示连接的屏幕截图。":::

1.  <span data-ttu-id="fb244-189">返回到 " **解决方案** " 页，选择 **Dynamics 365 的 "合作伙伴中心引用同步**"，并通过选择以下序列中每个流旁边的省略号图标来打开流。</span><span class="sxs-lookup"><span data-stu-id="fb244-189">Return to the **Solutions** page, select **Partner Center Referrals Synchronization for Dynamics 365**, and turn on the flow by selecting the ellipsis icon next to each flow in the following sequence.</span></span> <span data-ttu-id="fb244-190">如果在打开流时遇到任何问题，请参阅 [自定义步骤](connector-dynamics.md#customize-synchronization-steps) 和 [故障排除步骤](connectors-troubleshoot.md)。</span><span class="sxs-lookup"><span data-stu-id="fb244-190">If you encounter any issues while you turn on the flow, see [Customization steps](connector-dynamics.md#customize-synchronization-steps) and [Troubleshooting steps](connectors-troubleshoot.md).</span></span>

<span data-ttu-id="fb244-191">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="fb244-191">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="fb244-192"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="fb244-192">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="fb244-193">创建共同销售引用– Dynamics 365 到合作伙伴中心 (预览体验中心) </span><span class="sxs-lookup"><span data-stu-id="fb244-193">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fb244-194">来自创建或获取 Dynamics 365 流中的详细信息</span><span class="sxs-lookup"><span data-stu-id="fb244-194">[Customize] Create or Get Details from Dynamics 365 flow</span></span>
- <span data-ttu-id="fb244-195">合作伙伴中心到 Dynamics 365-Helper (预览体验中心) </span><span class="sxs-lookup"><span data-stu-id="fb244-195">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="fb244-196">合作伙伴中心 Microsoft 共同销售对 Dynamics 365 (预览体验的引用更新) </span><span class="sxs-lookup"><span data-stu-id="fb244-196">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="fb244-197">合作伙伴中心到 Dynamics 365 (预览体验体验) </span><span class="sxs-lookup"><span data-stu-id="fb244-197">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="fb244-198">Dynamics 365 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="fb244-198">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fb244-199">Dynamics 365 到合作伙伴中心 (有问必答预览版的机会) </span><span class="sxs-lookup"><span data-stu-id="fb244-199">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fb244-200">Dynamics 365 的 Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="fb244-200">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="fb244-201">使用 webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="fb244-201">Use webhook APIs to register for resource change events</span></span>

<span data-ttu-id="fb244-202">你可以使用合作伙伴中心 webhook Api 来注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="fb244-202">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="fb244-203">这些更改事件以 HTTP post 的形式发送到你的 URL。</span><span class="sxs-lookup"><span data-stu-id="fb244-203">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="fb244-204">选择 " **合作伙伴中心到 Dynamics 365 (预览体验预览")**。</span><span class="sxs-lookup"><span data-stu-id="fb244-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

1. <span data-ttu-id="fb244-205">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-205">Select the **Edit** icon, and select **When a HTTP request is received**.</span></span>

1. <span data-ttu-id="fb244-206">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="fb244-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/webhook-video.gif" alt-text="屏幕截图，显示如何使用 webhook 来注册资源更改。":::

1. <span data-ttu-id="fb244-208">选择 " **合作伙伴中心 Webhook 注册 (内幕预览版")** "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-208">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="fb244-209">确保在右窗格中打开 " **运行流** " 窗口，并选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-209">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="fb244-210">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="fb244-210">Enter the following details:</span></span>

   - <span data-ttu-id="fb244-211">**Http 触发器终结点**：此 URL 已从前面的步骤中复制。</span><span class="sxs-lookup"><span data-stu-id="fb244-211">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="fb244-212">**要注册的事件**：选择所有可用事件 (**引用创建** 的、 **引用更新**、 **相关的** 引用-已创建的、与引用 **相关** 的) 。</span><span class="sxs-lookup"><span data-stu-id="fb244-212">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="fb244-213">**是否覆盖现有触发器终结点（如果存在**）：是。</span><span class="sxs-lookup"><span data-stu-id="fb244-213">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="fb244-214">对于给定的 webhook 事件，只能注册一个 URL。</span><span class="sxs-lookup"><span data-stu-id="fb244-214">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="fb244-215">选择 " **运行流**"，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="fb244-215">Select **Run flow**, and then select **Done.**</span></span>

<span data-ttu-id="fb244-216">Webhook 现在可以侦听、创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="fb244-216">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="fb244-217">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="fb244-217">Customize synchronization steps</span></span>

<span data-ttu-id="fb244-218">CRM 系统经过高度自定义，你可以基于 CRM 设置自定义电源自动化解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-218">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="fb244-219">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，在 " [自定义字段映射指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)" 中列出了在合作伙伴中心电脑上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-219">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="fb244-220">按照字段映射指南进行操作，如有必要，请在 **[自定义] 创建或获取 Dynamics 365 flow** 或环境变量的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fb244-220">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow** or environment variables.</span></span> <span data-ttu-id="fb244-221">请勿更新 Power 自动化解决方案中的任何其他流，因为它可能会影响将来的解决方案升级。</span><span class="sxs-lookup"><span data-stu-id="fb244-221">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="fb244-222">提供下列自定义项：</span><span class="sxs-lookup"><span data-stu-id="fb244-222">The following customizations are available:</span></span>

- <span data-ttu-id="fb244-223">**显示机会名称中的复选标记**：默认情况下，机会名称旁边将显示一个复选标记，指示在合作伙伴中心与 DYNAMICS 365 CRM 之间的同步成功发生。</span><span class="sxs-lookup"><span data-stu-id="fb244-223">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="fb244-224">同样，如果同步失败，将显示交叉标记。</span><span class="sxs-lookup"><span data-stu-id="fb244-224">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="fb244-225">若要避免在机会名称中添加复选标记或交叉标记，请将 **机会 name 环境变量中显示复选标记** 的当前值设置为 "否"。</span><span class="sxs-lookup"><span data-stu-id="fb244-225">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>
- <span data-ttu-id="fb244-226">**交易价值**：默认情况下，来自合作伙伴中心的交易值将与 CRM 中的 **estimatedvalue** 同步。</span><span class="sxs-lookup"><span data-stu-id="fb244-226">**Deal value**: By default, the deal value from Partner Center will be synced to and from **estimatedvalue** in the CRM.</span></span> <span data-ttu-id="fb244-227">如果 CRM 中有其他字段要从中同步交易值：</span><span class="sxs-lookup"><span data-stu-id="fb244-227">If you have a different field in the CRM for the deal value to sync from:</span></span>

  - <span data-ttu-id="fb244-228">用 CRM 的字段名称更新 Dynamics 365 环境变量中的 " **交易值** " 字段名称。</span><span class="sxs-lookup"><span data-stu-id="fb244-228">Update the **Deal value** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="fb244-229">请确保提供字段名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="fb244-229">Make sure that you provide the field's name, not its display name.</span></span>
  - <span data-ttu-id="fb244-230">编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**，转到 **创建或更新** crm 中的机会，更新 **创建新机会** 并 **更新现有机会** 操作，将 **DealValue** 值分配到 CRM 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-230">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or update opportunity** in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** value to the correct field in the CRM.</span></span> <span data-ttu-id="fb244-231">同时，从 "**估计收入**" 字段中删除 **DealValue** 分配。</span><span class="sxs-lookup"><span data-stu-id="fb244-231">Also, remove the **DealValue** assignment from the **Estimated Revenue** field.</span></span>

- <span data-ttu-id="fb244-232">**客户帐户国家/地区代码**：创建新引用时，必须提供两个字母的国家/地区代码 (ISO 3166) 。</span><span class="sxs-lookup"><span data-stu-id="fb244-232">**Customer Account Country Code**: It's mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="fb244-233">默认情况下，国家/地区代码将与 CRM 中帐户的 **address1_country** 字段同步。</span><span class="sxs-lookup"><span data-stu-id="fb244-233">By default, the country code will be synced to and from the account's **address1_country** field in the CRM.</span></span> <span data-ttu-id="fb244-234">如果 CRM 中的 "国家/地区代码" 字段不同，则：</span><span class="sxs-lookup"><span data-stu-id="fb244-234">If you have a different field in the CRM for the country code to sync from:</span></span>

   - <span data-ttu-id="fb244-235">对于包含两个字母代码的帐户中的 nonlookup "国家/地区代码" 字段：</span><span class="sxs-lookup"><span data-stu-id="fb244-235">For a nonlookup country code field in the account that contains a two-letter code:</span></span>
     - <span data-ttu-id="fb244-236">将 Dynamics 365 环境变量中的 **客户帐户 "国家/地区代码** " 字段名称更新为 CRM 的字段名称。</span><span class="sxs-lookup"><span data-stu-id="fb244-236">Update the **Customer Account Country Code** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="fb244-237">请确保提供字段名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="fb244-237">Make sure that you provide the field's name, not its display name.</span></span>
     - <span data-ttu-id="fb244-238">编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**，然后转到 **创建或获取** crm 操作中的客户帐户，将 **国家/地区** 值分配给 crm 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-238">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or get customer account** in the CRM action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="fb244-239">同时，从 "**地址1：国家/地区**" 字段中删除 **国家**/地区值分配。</span><span class="sxs-lookup"><span data-stu-id="fb244-239">Also, remove the **Country** value assignment from the **Address 1: Country/Region** field.</span></span>

   - <span data-ttu-id="fb244-240">对于帐户中的基于查找的国家/地区代码字段：</span><span class="sxs-lookup"><span data-stu-id="fb244-240">For a lookup-based country code field in the account:</span></span>
     - <span data-ttu-id="fb244-241">在帐户中添加新的自定义字段，并使用两个字母的国家/地区代码自动填充该字段 (ISO 3166) 基于在查找字段中选择的值，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="fb244-241">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>
     - <span data-ttu-id="fb244-242">按照前面的步骤为 nonlookup "国家/地区代码" 字段，将新的自定义字段从 CRM 同步到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="fb244-242">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="fb244-243">**机会字段**：如果存在需要填充的 **机会** 中的必填字段，请编辑 **[自定义] 创建或获取来自 Dynamics 365 flow 的详细信息** ，然后转到 CRM 中的 " **创建" 或 "更新机会** "，然后根据您的业务要求，"更新 **创建新的机会" 操作** 以将值分配到必填字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-243">**Opportunity fields**: If there are mandatory fields in **Opportunity** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update opportunity** in the CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="fb244-244">**潜在顾客字段**：如果 **lead** 中有需要填充的必填字段，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息** ，然后转到 **创建或更新** CRM 中的潜在客户，并更新 **创建新的潜在客户操作** ，根据业务需求将值分配到必填字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-244">**Lead fields**: If there are mandatory fields in **Lead** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update lead** in the CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="fb244-245">**客户帐户**：如果新的引用从合作伙伴中心同步到 crm，则 Power 自动解决方案将尝试使用客户公司名称和邮政编码搜索 CRM 中的现有帐户。</span><span class="sxs-lookup"><span data-stu-id="fb244-245">**Customer account**: When a new referral is synced from Partner Center to the CRM, the Power Automate solution tries to search for an existing account in the CRM by using the customer company name and postal code.</span></span> <span data-ttu-id="fb244-246">如果找不到，将在 CRM 中创建新的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="fb244-246">If it doesn't find one, a new customer account will be created in the CRM.</span></span> <span data-ttu-id="fb244-247">若要更新搜索条件和新建帐户创建详细信息，请编辑 **[自定义] 创建或从 Dynamics 365 流中获取详细信息** ，然后转到 **创建或获取** CRM 中的客户帐户并 **创建客户帐户操作**。</span><span class="sxs-lookup"><span data-stu-id="fb244-247">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or get customer account** in the CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="fb244-248">更新环境变量</span><span class="sxs-lookup"><span data-stu-id="fb244-248">Update environment variable</span></span>

<span data-ttu-id="fb244-249">更新环境变量值：</span><span class="sxs-lookup"><span data-stu-id="fb244-249">To update an environment variable value:</span></span>

1. <span data-ttu-id="fb244-250">请在 " **解决方案** " 页上，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="fb244-250">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="fb244-251">选择 "**全部**" 以选择 **环境变量**。</span><span class="sxs-lookup"><span data-stu-id="fb244-251">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="fb244-252">选择需要更新的值的环境变量，并使用省略号图标选择 " **编辑** "。</span><span class="sxs-lookup"><span data-stu-id="fb244-252">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="fb244-253">更新 **当前值** (不要使用 "**新建值**" 选项并提供值来更新 **默认值**) 。</span><span class="sxs-lookup"><span data-stu-id="fb244-253">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="fb244-254">该值必须与变量的数据类型匹配。</span><span class="sxs-lookup"><span data-stu-id="fb244-254">The value must match the data type of the variable.</span></span> <span data-ttu-id="fb244-255">例如，"是" 或 "否" 数据类型将接受 Yes 或 No 值。</span><span class="sxs-lookup"><span data-stu-id="fb244-255">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/environment-variables-video.gif" alt-text="显示更新环境变量的屏幕截图。":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a><span data-ttu-id="fb244-257">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="fb244-257">End-to-end bidirectional co-sell referral synchronization</span></span>

<span data-ttu-id="fb244-258">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="fb244-258">After you've installed, configured, and customized the Power Automate solution, you can test for co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="fb244-259">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb244-259">Prerequisites</span></span>

<span data-ttu-id="fb244-260">若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-260">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="fb244-261">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="fb244-261">This identification gives your seller teams the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="fb244-262">一组自定义字段和对象将作为解决方案安装的一部分添加。</span><span class="sxs-lookup"><span data-stu-id="fb244-262">A set of custom fields and objects will be added as part of the solution installation.</span></span> <span data-ttu-id="fb244-263">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="fb244-263">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="fb244-264">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="fb244-264">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="fb244-265">**与合作伙伴中心同步**：是否要将此机会与合作伙伴中心同步。</span><span class="sxs-lookup"><span data-stu-id="fb244-265">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="fb244-266">默认情况下，此字段的值为 "否"，并且你的卖方需要将其显式设置为 "是"，以便与 Microsoft 共享机会。</span><span class="sxs-lookup"><span data-stu-id="fb244-266">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="fb244-267">从合作伙伴中心到 CRM 共享的新引用将此字段值设置为 "是"。</span><span class="sxs-lookup"><span data-stu-id="fb244-267">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>
- <span data-ttu-id="fb244-268">**引用标识符**：合作伙伴中心引用的只读标识符字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-268">**Referral Identifier**: A read-only identifier field for the Partner Center referral.</span></span>
- <span data-ttu-id="fb244-269">**引用链接**：指向合作伙伴中心中的引用的只读链接。</span><span class="sxs-lookup"><span data-stu-id="fb244-269">**Referral Link**: A read-only link to the referral in Partner Center.</span></span>
- <span data-ttu-id="fb244-270">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助。</span><span class="sxs-lookup"><span data-stu-id="fb244-270">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="fb244-271">若要创建共同销售引用，请选择 Microsoft 所需的适当帮助。</span><span class="sxs-lookup"><span data-stu-id="fb244-271">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="fb244-272">必须将客户联系人关联到创建共同销售引用的机会。</span><span class="sxs-lookup"><span data-stu-id="fb244-272">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="fb244-273">若要创建非共同销售引用，请不要选择此字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-273">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="fb244-274">通过选择适当的帮助-必需选项，可以随时将非共同销售引用转换为共同销售引用。</span><span class="sxs-lookup"><span data-stu-id="fb244-274">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>
- <span data-ttu-id="fb244-275">**Microsoft 合作伙伴中心引用可见性**：选择合作伙伴中心引用的可见性。</span><span class="sxs-lookup"><span data-stu-id="fb244-275">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="fb244-276">通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。</span><span class="sxs-lookup"><span data-stu-id="fb244-276">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="fb244-277">如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会显示该引用。</span><span class="sxs-lookup"><span data-stu-id="fb244-277">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="fb244-278">将此字段标记为可见后，将无法还原它。</span><span class="sxs-lookup"><span data-stu-id="fb244-278">After this field is marked as visible, it can't be reverted.</span></span>
- <span data-ttu-id="fb244-279">**MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。</span><span class="sxs-lookup"><span data-stu-id="fb244-279">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>
- <span data-ttu-id="fb244-280">**产品：已过时**：请勿使用此字段或将其添加到 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="fb244-280">**Products: Obsolete**: Don't use this field or add it to the CRM section.</span></span> <span data-ttu-id="fb244-281">它仅可用于向后兼容。</span><span class="sxs-lookup"><span data-stu-id="fb244-281">It's available for backward compatibility only.</span></span> <span data-ttu-id="fb244-282">请改用合作伙伴中心解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-282">Use Partner Center solutions instead.</span></span>
- <span data-ttu-id="fb244-283">**Audit**：与合作伙伴中心引用同步的只读审核记录。</span><span class="sxs-lookup"><span data-stu-id="fb244-283">**Audit**: A read-only audit trail for syncing with Partner Center referrals.</span></span>
- <span data-ttu-id="fb244-284">**Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。</span><span class="sxs-lookup"><span data-stu-id="fb244-284">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="fb244-285">可以在商机中添加或删除一个或多个解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-285">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="fb244-286">在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-286">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="fb244-287">若要将此对象与商机关联，请在 CRM 中更新 **商机** 窗体。</span><span class="sxs-lookup"><span data-stu-id="fb244-287">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

  <span data-ttu-id="fb244-288">选择 " **机会** " 窗体上的相应选项卡，并添加子网格，如下所示。</span><span class="sxs-lookup"><span data-stu-id="fb244-288">Select the appropriate tab on the **Opportunity** form, and add a subgrid as shown here.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="显示机会窗体的屏幕截图。":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="显示 Microsoft 解决方案的屏幕截图。":::

- <span data-ttu-id="fb244-291">添加 Microsoft 解决方案后，你可以预填充联合销售就绪解决方案详细信息，以便你的卖方不必添加它们。</span><span class="sxs-lookup"><span data-stu-id="fb244-291">After you add Microsoft solutions, you can prepopulate co-sell ready solution details so that your sellers don't have to add them.</span></span> <span data-ttu-id="fb244-292">若要添加新的解决方案详细信息，请前往 CRM 中的 Microsoft 解决方案详细信息对象，然后选择 " **添加记录** " 以添加一个条目或使用 **Excel 上传** 添加多个条目。</span><span class="sxs-lookup"><span data-stu-id="fb244-292">To add a new solution detail, go to the Microsoft Solution Details object in the CRM and select **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

  :::image type="content" source="images/dynamic-1a.png" alt-text="显示新的 Microsoft 解决方案详细信息的屏幕截图。":::

### <a name="scenarios"></a><span data-ttu-id="fb244-294">方案</span><span class="sxs-lookup"><span data-stu-id="fb244-294">Scenarios</span></span>

1. <span data-ttu-id="fb244-295">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="fb244-295">Referral synchronization when referral is created or updated in the CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="fb244-296">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="fb244-296">Sign in to your Dynamics 365 CRM environment with the user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="fb244-297">在 Dynamics 365 环境中创建新机会时，请确保 **Microsoft 合作伙伴中心** 部分存在。</span><span class="sxs-lookup"><span data-stu-id="fb244-297">Ensure that the **Microsoft Partner Center** section is present when you create a new opportunity in the Dynamics 365 environment.</span></span>

      :::image type="content" source="images/dynamic-2a.png" alt-text="显示新机会的屏幕截图。":::

   1. <span data-ttu-id="fb244-299">若要将此机会与合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="fb244-299">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="fb244-300">**Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。</span><span class="sxs-lookup"><span data-stu-id="fb244-300">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="显示如何在卡片视图中获取相应字段的屏幕截图。":::

      - <span data-ttu-id="fb244-302">**客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。</span><span class="sxs-lookup"><span data-stu-id="fb244-302">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="fb244-303">**与合作伙伴中心同步**：是。</span><span class="sxs-lookup"><span data-stu-id="fb244-303">**Sync With Partner Center**: Yes.</span></span>
      - <span data-ttu-id="fb244-304">**Microsoft 解决方案**：若要与 microsoft 共享引用，请向此机会添加有效的合作销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="fb244-304">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="显示解决方案 ID 的屏幕截图。":::

   1. <span data-ttu-id="fb244-306">在 Dynamics 365 中创建机会后，在 " **与合作伙伴中心同步** " 选项设置为 "是" 后，等待10分钟。</span><span class="sxs-lookup"><span data-stu-id="fb244-306">After the opportunity is created in Dynamics 365 with the **Sync With Partner Center** option set to Yes, wait 10 minutes.</span></span> <span data-ttu-id="fb244-307">然后登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="fb244-307">Then sign in to your Partner Center account.</span></span> <span data-ttu-id="fb244-308">你的引用将与 Dynamics 365 和 **引用标识符** 同步。</span><span class="sxs-lookup"><span data-stu-id="fb244-308">Your referrals will be synchronized with Dynamics 365 and **Referral Identifier**.</span></span> <span data-ttu-id="fb244-309">将填充 **引用链接**。</span><span class="sxs-lookup"><span data-stu-id="fb244-309">**Referral Link** will get populated.</span></span> <span data-ttu-id="fb244-310">如果出现故障，则将使用错误信息填充 **审核** 字段。</span><span class="sxs-lookup"><span data-stu-id="fb244-310">If there's a failure, the **Audit** field will be populated with error information.</span></span>
     
    1. <span data-ttu-id="fb244-311">同样，如果将 " **与合作伙伴中心同步** " 选项设置为 "是"，则在 DYNAMICS 365 CRM 中更新该机会时，所做的更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="fb244-311">Likewise, for an opportunity that had the **Sync With Partner Center** option set to Yes, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    1. <span data-ttu-id="fb244-312">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="fb244-312">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

1. <span data-ttu-id="fb244-313">当在合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时，引用同步：</span><span class="sxs-lookup"><span data-stu-id="fb244-313">Referral synchronization when the referral is created or updated in Partner Center and synchronized in the Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="fb244-314">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="fb244-314">Sign in to your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   1. <span data-ttu-id="fb244-315">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="fb244-315">Select **Referrals** from the left menu.</span></span>

   1. <span data-ttu-id="fb244-316">通过选择 " **新建交易** " 选项，从合作伙伴中心创建新的共同销售引用。</span><span class="sxs-lookup"><span data-stu-id="fb244-316">Create a new co-sell referral from Partner Center by selecting the **New deal** option.</span></span>

   1. <span data-ttu-id="fb244-317">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="fb244-317">Sign in to your Dynamics 365 CRM environment.</span></span>

   1. <span data-ttu-id="fb244-318">前往 **开放机会**。</span><span class="sxs-lookup"><span data-stu-id="fb244-318">Go to **Open Opportunities**.</span></span> <span data-ttu-id="fb244-319">现在，在合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="fb244-319">The referral created in Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   1. <span data-ttu-id="fb244-320">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="fb244-320">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fb244-321">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fb244-321">Next steps</span></span>

- [<span data-ttu-id="fb244-322">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="fb244-322">Manage leads</span></span>](manage-leads.md)
- [<span data-ttu-id="fb244-323">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="fb244-323">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
- [<span data-ttu-id="fb244-324">有关 Microsoft Power 自动化平台的详细信息</span><span class="sxs-lookup"><span data-stu-id="fb244-324">More about Microsoft Power Automate platform</span></span>](/power-automate/)
- [<span data-ttu-id="fb244-325">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="fb244-325">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
