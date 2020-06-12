---
title: Dynamics 365 CRM 合作伙伴中心的共同销售连接器
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Dynamics 365 CRM 同步
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: fef5468e0dc51cd9830fda6fb2ae60df5d9f39b5
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453244"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="2d64c-103">用于 Dynamics 365 CRM 的共同销售连接器–概述</span><span class="sxs-lookup"><span data-stu-id="2d64c-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="2d64c-104">相应的角色</span><span class="sxs-lookup"><span data-stu-id="2d64c-104">Appropriate roles</span></span>

- <span data-ttu-id="2d64c-105">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="2d64c-105">Referrals admin</span></span>
- <span data-ttu-id="2d64c-106">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="2d64c-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="2d64c-107">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="2d64c-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="2d64c-108">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="2d64c-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="2d64c-109">使用共同销售连接器，可以创建新的共同销售的引用，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受/拒绝引用、修改交易数据（如交易价值和结束日期）。</span><span class="sxs-lookup"><span data-stu-id="2d64c-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="2d64c-110">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="2d64c-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="2d64c-111">您可以在所选的 CRM 内而不是在合作伙伴中心内完成所有的引用工作。</span><span class="sxs-lookup"><span data-stu-id="2d64c-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="2d64c-112">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="2d64c-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="2d64c-113">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="2d64c-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="2d64c-114">**本节**</span><span class="sxs-lookup"><span data-stu-id="2d64c-114">**Topics**</span></span>   |<span data-ttu-id="2d64c-115">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="2d64c-115">**Details**</span></span>   |<span data-ttu-id="2d64c-116">**链接**</span><span class="sxs-lookup"><span data-stu-id="2d64c-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="2d64c-117">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="2d64c-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="2d64c-118">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="2d64c-118">You need a valid MPN ID</span></span>|<span data-ttu-id="2d64c-119">加入[MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="2d64c-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="2d64c-120">做好就绪</span><span class="sxs-lookup"><span data-stu-id="2d64c-120">Cosell ready</span></span>|<span data-ttu-id="2d64c-121">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="2d64c-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="2d64c-122">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="2d64c-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="2d64c-123">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="2d64c-123">Partner Center account</span></span>|<span data-ttu-id="2d64c-124">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="2d64c-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="2d64c-125">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="2d64c-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="2d64c-126">管理帐户</span><span class="sxs-lookup"><span data-stu-id="2d64c-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="2d64c-127">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="2d64c-127">Partner Center user roles</span></span>|<span data-ttu-id="2d64c-128">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="2d64c-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="2d64c-129">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="2d64c-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="2d64c-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="2d64c-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="2d64c-131">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="2d64c-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="2d64c-132">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="2d64c-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="2d64c-133">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="2d64c-133">Power Automate Flow Account</span></span>|<span data-ttu-id="2d64c-134">CRM 系统管理员或系统定制员的有效[电源自动完成](https://flow.microsoft.com)帐户。</span><span class="sxs-lookup"><span data-stu-id="2d64c-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="2d64c-135">在安装之前，该用户至少应登录到一次[电源](https://flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="2d64c-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="2d64c-136">为 Dynamics 365 安装合作伙伴中心引用同步（电源自动化解决方案）</span><span class="sxs-lookup"><span data-stu-id="2d64c-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="2d64c-137">请继续[执行 "电源自动](https://flow.microsoft.com)"，并选择右上角的 "**环境**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="2d64c-138">此步骤将显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="2d64c-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="2d64c-139">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="2d64c-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="2d64c-140">选择左侧导航栏上的 "**解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="2d64c-141">单击顶部菜单上的 "**打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="2d64c-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. <span data-ttu-id="2d64c-143">在弹出屏幕中搜索**Dynamics365 的合作伙伴中心引用连接器**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="2d64c-144">单击 "**立即获取**" 按钮，然后**继续**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-144">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="2d64c-145">这将打开一个页面，可以在其中选择要安装应用程序的 CRM （Dynamics 365）环境。</span><span class="sxs-lookup"><span data-stu-id="2d64c-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="2d64c-146">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="2d64c-146">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="2d64c-147">然后，你将转到 "**管理你的解决方案**" 页。</span><span class="sxs-lookup"><span data-stu-id="2d64c-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="2d64c-148">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="2d64c-149">**计划的安装**应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="2d64c-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="2d64c-150">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="2d64c-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="2d64c-151">安装完成后，导航回 "[自动启动](https://flow.microsoft.com)"，并从左侧导航区域中选择 "**解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="2d64c-152">请注意，"解决方案" 列表中提供了**Dynamics 365 的合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="2d64c-153">选择**Dynamics 365 的伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="2d64c-154">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="2d64c-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用 CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="2d64c-156">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="2d64c-156">Best practice: test before you go live</span></span>

<span data-ttu-id="2d64c-157">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="2d64c-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="2d64c-158">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="2d64c-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="2d64c-159">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="2d64c-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="2d64c-160">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="2d64c-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="2d64c-161">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="2d64c-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="2d64c-162">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="2d64c-162">Configure the solution</span></span>

1. <span data-ttu-id="2d64c-163">在 CRM 实例中安装解决方案后，请导航回 "[电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="2d64c-164">在右上角的 "**环境**" 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="2d64c-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="2d64c-165">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="2d64c-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="2d64c-166">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="2d64c-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="2d64c-167">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="2d64c-167">Partner Center Events</span></span>

   - <span data-ttu-id="2d64c-168">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="2d64c-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="2d64c-169">从左侧导航栏中选择 "**连接**"，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="2d64c-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="2d64c-170">通过单击 "**创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="2d64c-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="创建连接":::

      3. <span data-ttu-id="2d64c-172">在右上角的搜索栏中搜索 "**合作伙伴中心引用（预览版）** "。</span><span class="sxs-lookup"><span data-stu-id="2d64c-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="2d64c-173">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="2d64c-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="2d64c-174">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="2d64c-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="2d64c-175">为 CRM 管理员用户 Common Data Service （当前环境）创建连接。</span><span class="sxs-lookup"><span data-stu-id="2d64c-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="2d64c-176">若要将电源自动流与连接进行关联，请编辑每个电源自动流，以连接到 Common Data Service 和合作伙伴中心引用。</span><span class="sxs-lookup"><span data-stu-id="2d64c-176">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="2d64c-177">保存更改。</span><span class="sxs-lookup"><span data-stu-id="2d64c-177">Save the changes.</span></span>

5. <span data-ttu-id="2d64c-178">**启用**自动流功能。</span><span class="sxs-lookup"><span data-stu-id="2d64c-178">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="2d64c-179">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="2d64c-179">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="2d64c-180">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="2d64c-180">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="2d64c-181">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="2d64c-181">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="2d64c-182">若要注册 url，请选择 "**合作伙伴中心 Webhook 注册" （有问必答预览版）** "电源自动流程"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-182">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="2d64c-183">为（a）添加连接。具有引用管理员凭据的合作伙伴中心用户（b.）以下突出显示的合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="2d64c-183">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   <span data-ttu-id="2d64c-184">触发器</span><span class="sxs-lookup"><span data-stu-id="2d64c-184">:::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::</span></span>

3. <span data-ttu-id="2d64c-185">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="2d64c-185">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="2d64c-187">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-187">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="2d64c-188">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="2d64c-188">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="2d64c-189">选择 "**合作伙伴中心到 Dynamics 365 （有问必答预览版）**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-189">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="2d64c-190">选择 "**编辑**" 图标，然后选择 "**收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-190">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="2d64c-191">选择**复制**图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="2d64c-191">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="复制 URL":::

8. <span data-ttu-id="2d64c-193">现在，选择 "合作伙伴中心 Webhook 注册（有问必答预览版）" "电源自动流"，然后选择 "**运行**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-193">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="2d64c-194">确保在右侧窗格中打开 "运行流" 窗口，然后单击 "**继续**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-194">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="2d64c-195">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="2d64c-195">Enter the following details:</span></span>

    1. <span data-ttu-id="2d64c-196">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="2d64c-196">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="2d64c-197">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="2d64c-197">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="2d64c-198">**覆盖现有触发器终结点（如果存在**）：是（这将覆盖任何现有终结点。）</span><span class="sxs-lookup"><span data-stu-id="2d64c-198">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="2d64c-199">选择 "**运行**"，然后选择 "**完成"。**</span><span class="sxs-lookup"><span data-stu-id="2d64c-199">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="2d64c-200">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="2d64c-200">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="2d64c-201">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="2d64c-201">Customize synchronization steps</span></span>

<span data-ttu-id="2d64c-202">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="2d64c-202">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="2d64c-203">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="2d64c-203">Often CRM systems are highly customized.</span></span> <span data-ttu-id="2d64c-204">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="2d64c-204">You can customize the Power Automate flows.</span></span> <span data-ttu-id="2d64c-205">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="2d64c-205">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="2d64c-206">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="2d64c-206">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="2d64c-207">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="2d64c-207">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="2d64c-208">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="2d64c-208">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="2d64c-209">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="2d64c-209">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="2d64c-210">a.</span><span class="sxs-lookup"><span data-stu-id="2d64c-210">a.</span></span> <span data-ttu-id="2d64c-211">选择 "合作伙伴中心到 Dynamics 365 （有问必答预览版）" 或 "合作伙伴中心到 Salesforce" （有问必答预览版）。</span><span class="sxs-lookup"><span data-stu-id="2d64c-211">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="2d64c-212">b.</span><span class="sxs-lookup"><span data-stu-id="2d64c-212">b.</span></span> <span data-ttu-id="2d64c-213">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="2d64c-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="2d64c-214">c.</span><span class="sxs-lookup"><span data-stu-id="2d64c-214">c.</span></span> <span data-ttu-id="2d64c-215">选择 **（作用域）同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-215">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="2d64c-216">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**如果是新的共享机会"，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-216">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="2d64c-217">**如果是**，请选择 "子步骤"，然后**在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-217">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="2d64c-218">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="2d64c-218">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="2d64c-219">d.</span><span class="sxs-lookup"><span data-stu-id="2d64c-219">d.</span></span> <span data-ttu-id="2d64c-220">若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请单击 "（作用域）同步潜在客户或机会" 步骤。</span><span class="sxs-lookup"><span data-stu-id="2d64c-220">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="2d64c-221">e.</span><span class="sxs-lookup"><span data-stu-id="2d64c-221">e.</span></span> <span data-ttu-id="2d64c-222">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-222">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="2d64c-223">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。</span><span class="sxs-lookup"><span data-stu-id="2d64c-223">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="2d64c-224">f.</span><span class="sxs-lookup"><span data-stu-id="2d64c-224">f.</span></span> <span data-ttu-id="2d64c-225">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="2d64c-225">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="2d64c-226">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="2d64c-226">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="2d64c-227">a.</span><span class="sxs-lookup"><span data-stu-id="2d64c-227">a.</span></span> <span data-ttu-id="2d64c-228">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="2d64c-228">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="2d64c-229">b.</span><span class="sxs-lookup"><span data-stu-id="2d64c-229">b.</span></span> <span data-ttu-id="2d64c-230">选择 **（范围）同步机会**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-230">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="2d64c-231">c.</span><span class="sxs-lookup"><span data-stu-id="2d64c-231">c.</span></span> <span data-ttu-id="2d64c-232">若要为更新事件自定义 CRM 字段映射，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="2d64c-232">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="2d64c-233">d.</span><span class="sxs-lookup"><span data-stu-id="2d64c-233">d.</span></span> <span data-ttu-id="2d64c-234">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="2d64c-234">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="2d64c-235">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="2d64c-235">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="2d64c-236">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="2d64c-236">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="2d64c-237">a.</span><span class="sxs-lookup"><span data-stu-id="2d64c-237">a.</span></span> <span data-ttu-id="2d64c-238">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="2d64c-238">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="2d64c-239">b.</span><span class="sxs-lookup"><span data-stu-id="2d64c-239">b.</span></span> <span data-ttu-id="2d64c-240">选择 **（作用域）同步引用。**</span><span class="sxs-lookup"><span data-stu-id="2d64c-240">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="2d64c-241">c.</span><span class="sxs-lookup"><span data-stu-id="2d64c-241">c.</span></span> <span data-ttu-id="2d64c-242">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-242">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="2d64c-243">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="2d64c-243">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="2d64c-244">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="2d64c-244">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="2d64c-245">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="2d64c-245">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="2d64c-246">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d64c-246">Pre-requisites</span></span>

<span data-ttu-id="2d64c-247">若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="2d64c-247">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="2d64c-248">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="2d64c-248">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="2d64c-249">一组自定义字段作为 "**机会**" 实体的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="2d64c-249">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="2d64c-250">CRM 管理用户需要使用**机会**自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="2d64c-250">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="2d64c-251">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="2d64c-251">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="2d64c-252">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="2d64c-252">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="2d64c-253">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="2d64c-253">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="2d64c-254">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="2d64c-254">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="2d64c-255">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助</span><span class="sxs-lookup"><span data-stu-id="2d64c-255">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="2d64c-256">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="2d64c-256">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="2d64c-257">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="2d64c-257">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="2d64c-258">各种</span><span class="sxs-lookup"><span data-stu-id="2d64c-258">SCENARIOS:</span></span>

1. <span data-ttu-id="2d64c-259">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="2d64c-259">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="2d64c-260">在 CRM 的 "**机会**" 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="2d64c-260">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="2d64c-261">在 Dynamics 365 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="2d64c-261">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="机会":::

   3. <span data-ttu-id="2d64c-263">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="2d64c-263">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="2d64c-264">**与合作伙伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="2d64c-264">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="2d64c-265">**Microsoft Help 如何？**：选择以下各项：</span><span class="sxs-lookup"><span data-stu-id="2d64c-265">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="帮助选择":::

      - <span data-ttu-id="2d64c-267">**产品**：产品的解决方案 id</span><span class="sxs-lookup"><span data-stu-id="2d64c-267">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="2d64c-268">一旦在 Dynamics 365 中创建了商机，并将 "**伙伴中心同步**" 选项设置为 **"是"**，请等待10分钟，然后登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="2d64c-268">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="2d64c-269">你的引用将与 Dynamics 365 同步。</span><span class="sxs-lookup"><span data-stu-id="2d64c-269">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="2d64c-270">同样，如果将 "与合作伙伴中心同步" 选项设置为 "是"，则在 Dynamics 365 CRM 中更新此机会时，所做的更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="2d64c-270">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="2d64c-271">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="2d64c-271">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="2d64c-272">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="2d64c-272">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="2d64c-273">登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="2d64c-273">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="2d64c-274">从左侧菜单中选择 "**引用**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-274">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="2d64c-275">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="2d64c-275">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="2d64c-276">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="2d64c-276">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="2d64c-277">导航到 "**开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="2d64c-277">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="2d64c-278">现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="2d64c-278">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="2d64c-279">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="2d64c-279">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2d64c-280">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2d64c-280">Next steps</span></span>

- [<span data-ttu-id="2d64c-281">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="2d64c-281">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="2d64c-282">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="2d64c-282">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="2d64c-283">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="2d64c-283">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="2d64c-284">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="2d64c-284">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)