---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Salesforce CRM 同步
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145101"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="088d1-103">Salesforce CRM 的共同销售连接器-概述</span><span class="sxs-lookup"><span data-stu-id="088d1-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="088d1-104">相应的角色</span><span class="sxs-lookup"><span data-stu-id="088d1-104">Appropriate roles</span></span>

- <span data-ttu-id="088d1-105">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="088d1-105">Referrals admin</span></span>
- <span data-ttu-id="088d1-106">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="088d1-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="088d1-107">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="088d1-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="088d1-108">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="088d1-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="088d1-109">使用共同销售连接器，你可以创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用，接受/拒绝引用，修改交易数据（如交易价值）和结束日期。</span><span class="sxs-lookup"><span data-stu-id="088d1-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="088d1-110">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="088d1-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="088d1-111">你可以在所选的 CRM 中工作而不是在合作伙伴中心内工作时执行所有引用工作。</span><span class="sxs-lookup"><span data-stu-id="088d1-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="088d1-112">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="088d1-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="088d1-113">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="088d1-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="088d1-114">**主题**</span><span class="sxs-lookup"><span data-stu-id="088d1-114">**Topics**</span></span>   |<span data-ttu-id="088d1-115">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="088d1-115">**Details**</span></span>   |<span data-ttu-id="088d1-116">**链接**</span><span class="sxs-lookup"><span data-stu-id="088d1-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="088d1-117">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="088d1-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="088d1-118">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="088d1-118">You need a valid MPN ID</span></span>|<span data-ttu-id="088d1-119">加入[MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="088d1-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="088d1-120">合作销售就绪</span><span class="sxs-lookup"><span data-stu-id="088d1-120">Co-sell ready</span></span>|<span data-ttu-id="088d1-121">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="088d1-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="088d1-122">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="088d1-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="088d1-123">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="088d1-123">Partner Center account</span></span>|<span data-ttu-id="088d1-124">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="088d1-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="088d1-125">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="088d1-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="088d1-126">管理帐户</span><span class="sxs-lookup"><span data-stu-id="088d1-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="088d1-127">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="088d1-127">Partner Center user roles</span></span>|<span data-ttu-id="088d1-128">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="088d1-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="088d1-129">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="088d1-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="088d1-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="088d1-130">Salesforce CRM</span></span>|<span data-ttu-id="088d1-131">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="088d1-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="088d1-132">在 Salesforce CRM 中分配角色</span><span class="sxs-lookup"><span data-stu-id="088d1-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="088d1-133">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="088d1-133">Power Automate Flow Account</span></span>|<span data-ttu-id="088d1-134">CRM 系统管理员或系统定制员的有效[电源自动完成](https://flow.microsoft.com)帐户。</span><span class="sxs-lookup"><span data-stu-id="088d1-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="088d1-135">在安装之前，该用户至少应登录到一次[电源](https://flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="088d1-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="088d1-136">为 Salesforce CRM 安装合作伙伴中心引用同步</span><span class="sxs-lookup"><span data-stu-id="088d1-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="088d1-137">请继续[执行 "电源自动](https://flow.microsoft.com)"，并选择右上角的 "**环境**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="088d1-138">这会显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="088d1-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="088d1-139">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="088d1-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="088d1-140">选择左侧导航栏上的 "**解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="088d1-141">单击顶部菜单上的 "**打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="088d1-141">Click on the **Open AppSource** link on the top menu.</span></span>

![打开 AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="088d1-143">在弹出屏幕中搜索 Salesforce 的 "**合作伙伴中心引用连接器**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

![Salesforce](images/salesforce/salesforce1.png)

6. <span data-ttu-id="088d1-145">单击 "**立即获取**" 按钮，然后**继续**。</span><span class="sxs-lookup"><span data-stu-id="088d1-145">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="088d1-146">这将打开可在其中选择要安装应用程序的 Salesforce CRM 环境的页面。</span><span class="sxs-lookup"><span data-stu-id="088d1-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="088d1-147">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="088d1-147">Agree to terms and conditions.</span></span>

![可用 CRM](images/salesforce/available-crm.png)

8. <span data-ttu-id="088d1-149">然后，你将转到 "**管理你的解决方案**" 页。</span><span class="sxs-lookup"><span data-stu-id="088d1-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="088d1-150">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="088d1-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="088d1-151">**计划的安装**应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="088d1-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="088d1-152">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="088d1-152">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="088d1-153">安装完成后，导航回 "[自动启动](https://flow.microsoft.com)"，并从左侧导航区域中选择 "**解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="088d1-154">请注意，"解决方案" 列表中提供了**Salesforce 的合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="088d1-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="088d1-155">**为 Salesforce 选择合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="088d1-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="088d1-156">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="088d1-156">The following Power Automate flows and entities are available:</span></span>

![Salesforce 流](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="088d1-158">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="088d1-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="088d1-159">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="088d1-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="088d1-160">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="088d1-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="088d1-161">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="088d1-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="088d1-162">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="088d1-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="088d1-163">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="088d1-163">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="088d1-164">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="088d1-164">Configure the solution</span></span>

1. <span data-ttu-id="088d1-165">在 CRM 实例中安装解决方案后，请导航回 "[电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="088d1-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="088d1-166">在右上角的 "**环境**" 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="088d1-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="088d1-167">你将需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="088d1-167">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="088d1-168">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="088d1-168">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="088d1-169">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="088d1-169">Partner Center Events</span></span>
- <span data-ttu-id="088d1-170">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="088d1-170">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="088d1-171">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-171">a.</span></span> <span data-ttu-id="088d1-172">从左侧导航栏中选择 "**连接**"，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="088d1-172">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="088d1-173">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-173">b.</span></span> <span data-ttu-id="088d1-174">通过单击 "**创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="088d1-174">Create a connection by clicking **Create a connection**.</span></span> 

    ![创建连接](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="088d1-176">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-176">c.</span></span> <span data-ttu-id="088d1-177">在右上角的搜索栏中搜索 "**合作伙伴中心引用（预览版）** "。</span><span class="sxs-lookup"><span data-stu-id="088d1-177">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

    <span data-ttu-id="088d1-178">d.</span><span class="sxs-lookup"><span data-stu-id="088d1-178">d.</span></span> <span data-ttu-id="088d1-179">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="088d1-179">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="088d1-180">e.</span><span class="sxs-lookup"><span data-stu-id="088d1-180">e.</span></span> <span data-ttu-id="088d1-181">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="088d1-181">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>
    
    <span data-ttu-id="088d1-182">f.</span><span class="sxs-lookup"><span data-stu-id="088d1-182">f.</span></span> <span data-ttu-id="088d1-183">为 CRM 管理员用户 Common Data Service （当前环境）创建连接。</span><span class="sxs-lookup"><span data-stu-id="088d1-183">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="088d1-184">若要将电源自动流与连接进行关联，请编辑每个电源自动流，以连接到 Common Data Service 和合作伙伴中心引用。</span><span class="sxs-lookup"><span data-stu-id="088d1-184">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="088d1-185">保存更改。</span><span class="sxs-lookup"><span data-stu-id="088d1-185">Save the changes.</span></span>

5. <span data-ttu-id="088d1-186">**打开**"自动执行流" 功能。</span><span class="sxs-lookup"><span data-stu-id="088d1-186">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="088d1-187">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="088d1-187">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="088d1-188">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="088d1-188">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="088d1-189">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="088d1-189">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="088d1-190">若要注册 url，请选择 "**合作伙伴中心 Webhook 注册" （有问必答预览版）** "电源自动流程"。</span><span class="sxs-lookup"><span data-stu-id="088d1-190">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="088d1-191">为（a）添加连接。具有引用管理员凭据的合作伙伴中心用户（b.）以下突出显示的合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="088d1-191">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![触发器](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="088d1-193">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="088d1-193">When you make these updates, you'll see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="088d1-195">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="088d1-195">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="088d1-196">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="088d1-196">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="088d1-197">选择 "**合作伙伴中心到 SALESFORCE CRM （有问必答预览版）**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-197">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="088d1-198">选择 "**编辑**" 图标，然后选择 "**收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-198">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="088d1-199">选择**复制**图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="088d1-199">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![复制 URL](images/salesforce/copy-url.png)

8. <span data-ttu-id="088d1-201">现在，选择 "合作伙伴中心 Webhook 注册（有问必答预览版）" "电源自动流"，然后选择 "**运行**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-201">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="088d1-202">确保在右侧窗格中打开 "运行流" 窗口，然后单击 "**继续**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-202">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="088d1-203">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="088d1-203">Enter the following details:</span></span> 

    <span data-ttu-id="088d1-204">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-204">a.</span></span> <span data-ttu-id="088d1-205">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="088d1-205">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="088d1-206">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-206">b.</span></span> <span data-ttu-id="088d1-207">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="088d1-207">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="088d1-208">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-208">c.</span></span> <span data-ttu-id="088d1-209">**覆盖现有触发器终结点（如果存在**）：是（这将覆盖任何现有终结点。）</span><span class="sxs-lookup"><span data-stu-id="088d1-209">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="088d1-210">选择 "**运行**"，然后选择 "**完成"。**</span><span class="sxs-lookup"><span data-stu-id="088d1-210">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="088d1-211">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="088d1-211">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="088d1-212">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="088d1-212">Customize synchronization steps</span></span>

<span data-ttu-id="088d1-213">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="088d1-213">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="088d1-214">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="088d1-214">Often CRM systems are highly customized.</span></span> <span data-ttu-id="088d1-215">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="088d1-215">You can customize the Power Automate flows.</span></span> <span data-ttu-id="088d1-216">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="088d1-216">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="088d1-217">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="088d1-217">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="088d1-218">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="088d1-218">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="088d1-219">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="088d1-219">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="088d1-220">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="088d1-220">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="088d1-221">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-221">a.</span></span> <span data-ttu-id="088d1-222">选择 "合作伙伴中心到 Salesforce CRM （有问必答预览版）"。</span><span class="sxs-lookup"><span data-stu-id="088d1-222">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

    <span data-ttu-id="088d1-223">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-223">b.</span></span> <span data-ttu-id="088d1-224">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="088d1-224">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="088d1-225">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-225">c.</span></span> <span data-ttu-id="088d1-226">选择 **（作用域）同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="088d1-226">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="088d1-227">若要为创建事件自定义 CRM 字段映射，请选择**新的共享机会，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="088d1-227">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="088d1-228">选择 "**是"** ，然后**在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-228">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="088d1-229">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="088d1-229">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="088d1-230">d.</span><span class="sxs-lookup"><span data-stu-id="088d1-230">d.</span></span> <span data-ttu-id="088d1-231">若要为更新事件自定义 CRM 字段映射，请单击 "（作用域）同步潜在客户或机会" 步骤。</span><span class="sxs-lookup"><span data-stu-id="088d1-231">To customize CRM field mappings for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="088d1-232">e.</span><span class="sxs-lookup"><span data-stu-id="088d1-232">e.</span></span> <span data-ttu-id="088d1-233">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="088d1-233">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="088d1-234">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。</span><span class="sxs-lookup"><span data-stu-id="088d1-234">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="088d1-235">f.</span><span class="sxs-lookup"><span data-stu-id="088d1-235">f.</span></span> <span data-ttu-id="088d1-236">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="088d1-236">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="088d1-237">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="088d1-237">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="088d1-238">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-238">a.</span></span> <span data-ttu-id="088d1-239">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="088d1-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="088d1-240">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-240">b.</span></span> <span data-ttu-id="088d1-241">选择 **（范围）同步机会**。</span><span class="sxs-lookup"><span data-stu-id="088d1-241">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="088d1-242">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-242">c.</span></span> <span data-ttu-id="088d1-243">若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="088d1-243">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="088d1-244">d.</span><span class="sxs-lookup"><span data-stu-id="088d1-244">d.</span></span> <span data-ttu-id="088d1-245">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="088d1-245">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="088d1-246">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="088d1-246">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="088d1-247">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="088d1-247">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="088d1-248">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-248">a.</span></span> <span data-ttu-id="088d1-249">选择 "**编辑**" 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="088d1-249">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="088d1-250">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-250">b.</span></span> <span data-ttu-id="088d1-251">选择 **（作用域）同步引用。**</span><span class="sxs-lookup"><span data-stu-id="088d1-251">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="088d1-252">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-252">c.</span></span> <span data-ttu-id="088d1-253">若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-253">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="088d1-254">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="088d1-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="088d1-255">在 Salesforce CRM 机会布局中创建单独的部分</span><span class="sxs-lookup"><span data-stu-id="088d1-255">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="088d1-256">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="088d1-256">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="088d1-257">这使您的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="088d1-257">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="088d1-258">一组自定义字段作为 Salesforce CRM**商机**实体的合作伙伴中心引用同步的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="088d1-258">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="088d1-259">CRM 管理用户需要使用**机会**自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="088d1-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="088d1-260">Salesforce CRM 管理员用户需要创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="088d1-260">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="088d1-261">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="088d1-261">The following custom fields should be part of the CRM section:</span></span>

<span data-ttu-id="088d1-262">•**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="088d1-262">• **Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

<span data-ttu-id="088d1-263">•**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="088d1-263">• **Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

<span data-ttu-id="088d1-264">•**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="088d1-264">• **Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

<span data-ttu-id="088d1-265">• **Microsoft 如何帮助？**</span><span class="sxs-lookup"><span data-stu-id="088d1-265">• **How can Microsoft help?**</span></span> <span data-ttu-id="088d1-266">Microsoft 提供的有关引用的帮助</span><span class="sxs-lookup"><span data-stu-id="088d1-266">Help required from Microsoft for the referral</span></span>

<span data-ttu-id="088d1-267">•**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="088d1-267">• **Products**: List of products associated with this opportunity</span></span>

<span data-ttu-id="088d1-268">•**审核**：与 Microsoft 合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="088d1-268">• **Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="088d1-269">设置字段和关系</span><span class="sxs-lookup"><span data-stu-id="088d1-269">Set up fields and relationships</span></span>

1. <span data-ttu-id="088d1-270">登录到 Salesforce 帐户，然后再进入 "**机会**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-270">Sign into your Salesforce account and go to **Opportunity**.</span></span> 

2. <span data-ttu-id="088d1-271">单击 "**设置**" 和 "**编辑对象**" 选项以添加所需的字段。</span><span class="sxs-lookup"><span data-stu-id="088d1-271">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>


3. <span data-ttu-id="088d1-272">从左侧导航栏中选择**字段 & 关系**</span><span class="sxs-lookup"><span data-stu-id="088d1-272">Select **Fields & Relationships** from the left navigation</span></span>

![字段](images/salesforce/fields1.png)

4. <span data-ttu-id="088d1-274">在 "字段 & 关系" 表中添加以下字段：</span><span class="sxs-lookup"><span data-stu-id="088d1-274">Add the following fields in the “Fields & Relationship” table:</span></span>

|<span data-ttu-id="088d1-275">**字段标签**</span><span class="sxs-lookup"><span data-stu-id="088d1-275">**Field label**</span></span>   |<span data-ttu-id="088d1-276">**字段名称**</span><span class="sxs-lookup"><span data-stu-id="088d1-276">**Field name**</span></span>|<span data-ttu-id="088d1-277">**Data type**</span><span class="sxs-lookup"><span data-stu-id="088d1-277">**Data type**</span></span>|<span data-ttu-id="088d1-278">**作**</span><span class="sxs-lookup"><span data-stu-id="088d1-278">**Indexed**</span></span>|
|---------------------|:-------------------|:--------------|:----------------|
|<span data-ttu-id="088d1-279">与合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="088d1-279">Sync with Partner Center</span></span>|<span data-ttu-id="088d1-280">与合作伙伴同步-中心-c</span><span class="sxs-lookup"><span data-stu-id="088d1-280">sync-with-partner-center-c</span></span>|<span data-ttu-id="088d1-281">Checkbox （默认未选中）</span><span class="sxs-lookup"><span data-stu-id="088d1-281">Checkbox (default unchecked)</span></span>||
|<span data-ttu-id="088d1-282">产品</span><span class="sxs-lookup"><span data-stu-id="088d1-282">Products</span></span>|<span data-ttu-id="088d1-283">Products-c</span><span class="sxs-lookup"><span data-stu-id="088d1-283">Products-c</span></span>|<span data-ttu-id="088d1-284">文本（255）</span><span class="sxs-lookup"><span data-stu-id="088d1-284">text (255)</span></span>||
|<span data-ttu-id="088d1-285">引荐</span><span class="sxs-lookup"><span data-stu-id="088d1-285">Referral</span></span> | <span data-ttu-id="088d1-286">Referral_Identifier__c</span><span class="sxs-lookup"><span data-stu-id="088d1-286">Referral_Identifier__c</span></span>|<span data-ttu-id="088d1-287">文本（100）（外部 ID）</span><span class="sxs-lookup"><span data-stu-id="088d1-287">Text(100)(External ID)</span></span>|<span data-ttu-id="088d1-288">是</span><span class="sxs-lookup"><span data-stu-id="088d1-288">yes</span></span>|
|<span data-ttu-id="088d1-289">引用链接</span><span class="sxs-lookup"><span data-stu-id="088d1-289">Referral Link</span></span>| <span data-ttu-id="088d1-290">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="088d1-290">Referral_Link__c_</span></span>|<span data-ttu-id="088d1-291">URL （255）</span><span class="sxs-lookup"><span data-stu-id="088d1-291">URL(255)</span></span>||
|<span data-ttu-id="088d1-292">审核</span><span class="sxs-lookup"><span data-stu-id="088d1-292">Audit</span></span>| <span data-ttu-id="088d1-293">Audit__c</span><span class="sxs-lookup"><span data-stu-id="088d1-293">Audit__c</span></span>|<span data-ttu-id="088d1-294">长文本区域（100000）（显示第4行）</span><span class="sxs-lookup"><span data-stu-id="088d1-294">Long Text Area(100000)(visible line 4)</span></span>||
|<span data-ttu-id="088d1-295">Microsoft 如何帮助？</span><span class="sxs-lookup"><span data-stu-id="088d1-295">How can Microsoft help?</span></span>|<span data-ttu-id="088d1-296">How_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="088d1-296">How_can_Microsoft_help__c</span></span>|<span data-ttu-id="088d1-297">列表</span><span class="sxs-lookup"><span data-stu-id="088d1-297">Picklist\*</span></span>|

<span data-ttu-id="088d1-298">\* 选择列表值：</span><span class="sxs-lookup"><span data-stu-id="088d1-298">\*Picklist values:</span></span>

<span data-ttu-id="088d1-299">•特定于工作负荷的价值主张</span><span class="sxs-lookup"><span data-stu-id="088d1-299">• Workload specific value proposition</span></span>

<span data-ttu-id="088d1-300">•客户技术体系结构</span><span class="sxs-lookup"><span data-stu-id="088d1-300">• Customer technical architecture</span></span>

<span data-ttu-id="088d1-301">•概念证明或演示</span><span class="sxs-lookup"><span data-stu-id="088d1-301">• Proof of concept or demo</span></span>

<span data-ttu-id="088d1-302">•报价单或许可</span><span class="sxs-lookup"><span data-stu-id="088d1-302">• Quotes or licensing</span></span>

<span data-ttu-id="088d1-303">•销售客户成功后</span><span class="sxs-lookup"><span data-stu-id="088d1-303">• Post sales customer success</span></span>

<span data-ttu-id="088d1-304">•常规或其他</span><span class="sxs-lookup"><span data-stu-id="088d1-304">• General or other</span></span>

<span data-ttu-id="088d1-305">5. 将在 "字段 & 关系" 下创建字段</span><span class="sxs-lookup"><span data-stu-id="088d1-305">5.The fields would get created under “Fields & Relationships”</span></span>

![已创建字段](images/salesforce/fields2.png)

6. <span data-ttu-id="088d1-307">在 "机会布局" 中，创建一个单独的部分，其中包含上面列出的字段。</span><span class="sxs-lookup"><span data-stu-id="088d1-307">In the Opportunity layout, create a separate section with the fields as listed above.</span></span> 

    <span data-ttu-id="088d1-308">•此部分应该适用于机会布局中的卖方</span><span class="sxs-lookup"><span data-stu-id="088d1-308">• This section should be available for the sellers in the Opportunity layout</span></span>


![合作伙伴中心字段布局](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="088d1-310">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="088d1-310">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="088d1-311">安装、配置和自定义电源自动解决方案后，可以测试 Salesforce CRM 与合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="088d1-311">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="088d1-312">先决条件</span><span class="sxs-lookup"><span data-stu-id="088d1-312">Pre-requisites</span></span>

<span data-ttu-id="088d1-313">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="088d1-313">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="088d1-314">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="088d1-314">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="088d1-315">一组自定义字段作为 Salesforce CRM 解决方案**机会**实体的合作伙伴中心引用同步的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="088d1-315">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="088d1-316">CRM 管理用户需要使用**机会**自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="088d1-316">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="088d1-317">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="088d1-317">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="088d1-318">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="088d1-318">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="088d1-319">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="088d1-319">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="088d1-320">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="088d1-320">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="088d1-321">**Microsoft 如何帮助**： microsoft 提供的有关推荐的帮助</span><span class="sxs-lookup"><span data-stu-id="088d1-321">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="088d1-322">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="088d1-322">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="088d1-323">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="088d1-323">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="088d1-324">各种</span><span class="sxs-lookup"><span data-stu-id="088d1-324">SCENARIOS:</span></span>

1. <span data-ttu-id="088d1-325">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="088d1-325">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="088d1-326">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-326">a.</span></span> <span data-ttu-id="088d1-327">在 CRM 的 "**机会**" 部分中具有可见性的用户登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="088d1-327">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="088d1-328">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-328">b.</span></span> <span data-ttu-id="088d1-329">在 Salesforce CRM 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="088d1-329">Ensure that the following section is present when you create a “New Opportunity” in Salesforce CRM environment</span></span>

    ![Salesforce 环境](images/salesforce/salesforce-scenario-1.png)

   

    <span data-ttu-id="088d1-331">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-331">c.</span></span> <span data-ttu-id="088d1-332">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="088d1-332">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="088d1-333">"与合作伙伴中心同步"：是</span><span class="sxs-lookup"><span data-stu-id="088d1-333">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="088d1-334">"Microsoft help 怎样？"：从以下选项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="088d1-334">"How can Microsoft help?”: Select from the following options:</span></span>

   

    - <span data-ttu-id="088d1-335">产品：产品的解决方案 Id</span><span class="sxs-lookup"><span data-stu-id="088d1-335">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="088d1-336">d.</span><span class="sxs-lookup"><span data-stu-id="088d1-336">d.</span></span> <span data-ttu-id="088d1-337">将 "机会**与合作伙伴中心同步**" 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="088d1-337">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="088d1-338">你的引用将与 Salesforce CRM 同步。</span><span class="sxs-lookup"><span data-stu-id="088d1-338">Your referrals will be synchronized with Salesforce CRM.</span></span>

    <span data-ttu-id="088d1-339">e.</span><span class="sxs-lookup"><span data-stu-id="088d1-339">e.</span></span> <span data-ttu-id="088d1-340">当 "与合作伙伴中心同步" 选项设置为 "是" 时，如果您更新了 Salesforce CRM 中的机会，则这些更改将与合作伙伴中心帐户同步。</span><span class="sxs-lookup"><span data-stu-id="088d1-340">When the “Sync with Partner Center” option is set to “Yes”, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

    <span data-ttu-id="088d1-341">f.</span><span class="sxs-lookup"><span data-stu-id="088d1-341">f.</span></span> <span data-ttu-id="088d1-342">与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="088d1-342">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="088d1-343">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="088d1-343">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span> 

    <span data-ttu-id="088d1-344">a.</span><span class="sxs-lookup"><span data-stu-id="088d1-344">a.</span></span> <span data-ttu-id="088d1-345">登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="088d1-345">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="088d1-346">b.</span><span class="sxs-lookup"><span data-stu-id="088d1-346">b.</span></span> <span data-ttu-id="088d1-347">从左侧菜单中选择 "**引用**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-347">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="088d1-348">c.</span><span class="sxs-lookup"><span data-stu-id="088d1-348">c.</span></span> <span data-ttu-id="088d1-349">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="088d1-349">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="088d1-350">d.</span><span class="sxs-lookup"><span data-stu-id="088d1-350">d.</span></span> <span data-ttu-id="088d1-351">登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="088d1-351">Sign into your Salesforce CRM environment.</span></span> 

    <span data-ttu-id="088d1-352">e.</span><span class="sxs-lookup"><span data-stu-id="088d1-352">e.</span></span> <span data-ttu-id="088d1-353">导航到 "**开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="088d1-353">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="088d1-354">Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。</span><span class="sxs-lookup"><span data-stu-id="088d1-354">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    ![Salesforce 机会屏幕](images/salesforce/salesforce-casino-e.png)

    <span data-ttu-id="088d1-356">f.</span><span class="sxs-lookup"><span data-stu-id="088d1-356">f.</span></span> <span data-ttu-id="088d1-357">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="088d1-357">When you select a synchronized referral, the card view details are populated.</span></span>





## <a name="next-steps"></a><span data-ttu-id="088d1-358">后续步骤</span><span class="sxs-lookup"><span data-stu-id="088d1-358">Next steps</span></span>

- [<span data-ttu-id="088d1-359">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="088d1-359">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="088d1-360">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="088d1-360">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="088d1-361">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="088d1-361">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="088d1-362">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="088d1-362">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)