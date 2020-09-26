---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Salesforce CRM 同步
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 1b658f04b1348eb48f694fac069518a7a7fc6a70
ms.sourcegitcommit: 505c38436780a31692f5f5694830fcfe01502977
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "91372812"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="042af-103">用于 Salesforce CRM 的联合销售连接器 – 概述</span><span class="sxs-lookup"><span data-stu-id="042af-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="042af-104">相应的角色</span><span class="sxs-lookup"><span data-stu-id="042af-104">Appropriate roles</span></span>

- <span data-ttu-id="042af-105">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="042af-105">Referrals admin</span></span>
- <span data-ttu-id="042af-106">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="042af-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="042af-107">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="042af-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="042af-108">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="042af-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="042af-109">使用共同销售连接器，你可以创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用，接受/拒绝引用，修改交易数据（如交易价值）和结束日期。</span><span class="sxs-lookup"><span data-stu-id="042af-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="042af-110">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="042af-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="042af-111">你可以在所选的 CRM 中工作而不是在合作伙伴中心内工作时执行所有引用工作。</span><span class="sxs-lookup"><span data-stu-id="042af-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="042af-112">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="042af-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="042af-113">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="042af-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="042af-114">**主题**</span><span class="sxs-lookup"><span data-stu-id="042af-114">**Topics**</span></span>   |<span data-ttu-id="042af-115">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="042af-115">**Details**</span></span>   |<span data-ttu-id="042af-116">**链接**</span><span class="sxs-lookup"><span data-stu-id="042af-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="042af-117">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="042af-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="042af-118">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="042af-118">You need a valid MPN ID</span></span>|<span data-ttu-id="042af-119">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="042af-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="042af-120">合作销售就绪</span><span class="sxs-lookup"><span data-stu-id="042af-120">Co-sell ready</span></span>|<span data-ttu-id="042af-121">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="042af-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="042af-122">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="042af-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="042af-123">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="042af-123">Partner Center account</span></span>|<span data-ttu-id="042af-124">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="042af-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="042af-125">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="042af-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="042af-126">管理帐户</span><span class="sxs-lookup"><span data-stu-id="042af-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="042af-127">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="042af-127">Partner Center user roles</span></span>|<span data-ttu-id="042af-128">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="042af-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="042af-129">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="042af-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="042af-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="042af-130">Salesforce CRM</span></span>|<span data-ttu-id="042af-131">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="042af-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="042af-132">在 Salesforce CRM 中分配角色</span><span class="sxs-lookup"><span data-stu-id="042af-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="042af-133">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="042af-133">Power Automate Flow Account</span></span>|<span data-ttu-id="042af-134">CRM 系统管理员或系统定制员的有效 [电源自动完成](https://flow.microsoft.com) 帐户。</span><span class="sxs-lookup"><span data-stu-id="042af-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="042af-135">在安装之前，该用户至少应登录到一次 [电源](https://flow.microsoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="042af-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="042af-136">为 Microsoft 自定义字段安装 Salesforce 包</span><span class="sxs-lookup"><span data-stu-id="042af-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="042af-137">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要清楚地识别 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="042af-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="042af-138">此分界为合作伙伴卖方团队提供了决定他们要与 Microsoft 共享以共同销售的推荐的功能。</span><span class="sxs-lookup"><span data-stu-id="042af-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="042af-139">在 Salesforce 中，激活 **注释** 并将其添加到机会相关列表。</span><span class="sxs-lookup"><span data-stu-id="042af-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="042af-140">引用</span><span class="sxs-lookup"><span data-stu-id="042af-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="042af-141">按照以下步骤激活 **机会团队** ：</span><span class="sxs-lookup"><span data-stu-id="042af-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="042af-142">在安装程序中，使用 " **快速查找** " 框定位机会团队设置。</span><span class="sxs-lookup"><span data-stu-id="042af-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="042af-143">根据需要定义设置。</span><span class="sxs-lookup"><span data-stu-id="042af-143">Define the settings as needed.</span></span>
[<span data-ttu-id="042af-144">引用</span><span class="sxs-lookup"><span data-stu-id="042af-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="042af-145">在 Salesforce 中，使用下面的包安装程序安装自定义字段和对象。</span><span class="sxs-lookup"><span data-stu-id="042af-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="042af-146">请访问 [此处](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) ，将包安装到任何公司：</span><span class="sxs-lookup"><span data-stu-id="042af-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="042af-147">注意：如果要安装到沙盒，则必须将 URL 的初始部分替换为 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="042af-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="042af-148">在 Salesforce 中，将 Microsoft 解决方案添加到 **机会** 相关列表。</span><span class="sxs-lookup"><span data-stu-id="042af-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="042af-149">添加后，单击 **扳手** 图标并更新属性</span><span class="sxs-lookup"><span data-stu-id="042af-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="042af-150">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="042af-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="042af-151">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="042af-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="042af-152">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="042af-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="042af-153">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="042af-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="042af-154">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="042af-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="042af-155">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="042af-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="042af-156">为 Salesforce CRM 安装合作伙伴中心引用同步</span><span class="sxs-lookup"><span data-stu-id="042af-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="042af-157">请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="042af-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="042af-158">这会显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="042af-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="042af-159">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="042af-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="042af-160">选择左侧导航栏上的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="042af-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="042af-161">单击顶部菜单上的 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="042af-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. <span data-ttu-id="042af-163">在弹出屏幕中搜索 Salesforce 的 " **合作伙伴中心引用连接器** "。</span><span class="sxs-lookup"><span data-stu-id="042af-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="042af-165">单击 " **立即获取** " 按钮，然后 **继续**。</span><span class="sxs-lookup"><span data-stu-id="042af-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="042af-166">这将打开可在其中选择要安装应用程序的 Salesforce CRM 环境的页面。</span><span class="sxs-lookup"><span data-stu-id="042af-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="042af-167">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="042af-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用 CRM":::

8. <span data-ttu-id="042af-169">然后，你将转到 " **管理你的解决方案** " 页。</span><span class="sxs-lookup"><span data-stu-id="042af-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="042af-170">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="042af-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="042af-171">**计划的安装** 应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="042af-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="042af-172">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="042af-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="042af-173">安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="042af-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="042af-174">请注意，"解决方案" 列表中提供了 **Salesforce 的合作伙伴中心引用同步** 。</span><span class="sxs-lookup"><span data-stu-id="042af-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="042af-175">**为 Salesforce 选择合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="042af-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="042af-176">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="042af-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 流":::



## <a name="configure-the-solution"></a><span data-ttu-id="042af-178">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="042af-178">Configure the solution</span></span>

1. <span data-ttu-id="042af-179">在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="042af-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="042af-180">在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="042af-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="042af-181">你将需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="042af-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="042af-182">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="042af-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="042af-183">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="042af-183">Partner Center Events</span></span>
    - <span data-ttu-id="042af-184">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="042af-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="042af-185">从左侧导航栏中选择 " **连接** "，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="042af-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="042af-186">通过单击 " **创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="042af-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="创建连接":::

- <span data-ttu-id="042af-188">在右上角的搜索栏中搜索 "合作伙伴中心引用 (预览") 。</span><span class="sxs-lookup"><span data-stu-id="042af-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="042af-189">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="042af-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="042af-190">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="042af-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="042af-191">为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。</span><span class="sxs-lookup"><span data-stu-id="042af-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="042af-192">添加所有连接后，你的环境中应会显示以下连接：</span><span class="sxs-lookup"><span data-stu-id="042af-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="观察连接":::

### <a name="edit-the-connections"></a><span data-ttu-id="042af-194">编辑连接</span><span class="sxs-lookup"><span data-stu-id="042af-194">Edit the connections</span></span>

1. <span data-ttu-id="042af-195">返回 "解决方案" 页，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="042af-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="042af-196">通过单击 "**全部**" \*\* (预览) 选择 "连接引用\*\*"。</span><span class="sxs-lookup"><span data-stu-id="042af-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="开始连接器编辑":::

2. <span data-ttu-id="042af-198">通过选择三个点图标，逐个编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="042af-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="042af-199">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="042af-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="编辑连接器":::

3. <span data-ttu-id="042af-201">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="042af-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="042af-202"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="042af-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="042af-203">创建向合作伙伴中心 (内幕预览版的共同销售推荐-Salesforce) </span><span class="sxs-lookup"><span data-stu-id="042af-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="042af-204">合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) </span><span class="sxs-lookup"><span data-stu-id="042af-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="042af-205">合作伙伴中心到 Salesforce (预览体验) </span><span class="sxs-lookup"><span data-stu-id="042af-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="042af-206">Salesforce 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="042af-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="042af-207">合作机会到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="042af-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="042af-208">Salesforce Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="042af-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="042af-209">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="042af-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="042af-210">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="042af-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="042af-211">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="042af-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="042af-212">若要注册 url，请选择 " \*\*合作伙伴中心 Webhook 注册 (内幕预览版") \*\* Power 自动流 "。</span><span class="sxs-lookup"><span data-stu-id="042af-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="042af-213">为 (a ) 合作伙伴中心用户添加连接， (b. ) 合作伙伴中心事件如下所示</span><span class="sxs-lookup"><span data-stu-id="042af-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="触发器":::

3. <span data-ttu-id="042af-215">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="042af-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="042af-217">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="042af-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="042af-218">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="042af-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="042af-219">选择 " \*\*合作伙伴中心到 SALESFORCE CRM (内幕预览版") \*\*。</span><span class="sxs-lookup"><span data-stu-id="042af-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="042af-220">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="042af-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="042af-221">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="042af-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="复制 URL":::

8. <span data-ttu-id="042af-223">现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="042af-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="042af-224">确保在右侧窗格中打开 "运行流" 窗口，然后单击 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="042af-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="042af-225">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="042af-225">Enter the following details:</span></span>

    1. <span data-ttu-id="042af-226">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="042af-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="042af-227">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="042af-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="042af-228">**覆盖现有触发器终结点（如果存在**）：是 (这将覆盖任何现有终结点。 ) </span><span class="sxs-lookup"><span data-stu-id="042af-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="042af-229">选择 " **运行** "，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="042af-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="042af-230">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="042af-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="042af-231">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="042af-231">Customize synchronization steps</span></span>

<span data-ttu-id="042af-232">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="042af-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="042af-233">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="042af-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="042af-234">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="042af-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="042af-235">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="042af-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="042af-236">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="042af-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="042af-237">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="042af-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="042af-238">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="042af-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="042af-239">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="042af-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="042af-240">选择 "合作伙伴中心到 Salesforce CRM (内幕预览版") 。</span><span class="sxs-lookup"><span data-stu-id="042af-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="042af-241">选择 " **编辑** " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="042af-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="042af-242">选择 " \*\* (范围") 同步潜在客户或机会\*\*。</span><span class="sxs-lookup"><span data-stu-id="042af-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="042af-243">若要为创建事件自定义 CRM 字段映射，请选择 **新的共享机会，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="042af-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="042af-244">选择 " **是"** ，然后 **在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="042af-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="042af-245">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="042af-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="042af-246">若要为更新事件自定义 CRM 字段映射，请单击步骤 " (范围) 同步潜在客户或机会"。</span><span class="sxs-lookup"><span data-stu-id="042af-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="042af-247">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="042af-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="042af-248">**如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。</span><span class="sxs-lookup"><span data-stu-id="042af-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="042af-249">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="042af-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="042af-250">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="042af-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="042af-251">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="042af-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="042af-252">选择 \*\* (范围) 同步机会\*\*。</span><span class="sxs-lookup"><span data-stu-id="042af-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="042af-253">对于 "基于字段映射 (自定义 CRM 字段映射" 指南) 对于 "更新事件"，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="042af-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="042af-254">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="042af-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="042af-255">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="042af-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="042af-256">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="042af-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="042af-257">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="042af-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="042af-258">选择 **) 同步引用 (范围。**</span><span class="sxs-lookup"><span data-stu-id="042af-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="042af-259">对于 "基于字段映射自定义 CRM 字段映射 (" 指南) 对于创建事件，请选择 " **创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="042af-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="042af-260">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="042af-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="042af-261">设置字段和关系</span><span class="sxs-lookup"><span data-stu-id="042af-261">Set up fields and relationships</span></span>

1. <span data-ttu-id="042af-262">登录到 Salesforce 帐户，然后再进入 " **机会**"。</span><span class="sxs-lookup"><span data-stu-id="042af-262">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="042af-263">单击 " **设置** " 和 " **编辑对象** " 选项以添加所需的字段。</span><span class="sxs-lookup"><span data-stu-id="042af-263">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="042af-264">从左侧导航栏中选择**字段 & 关系**</span><span class="sxs-lookup"><span data-stu-id="042af-264">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="042af-266">将以下字段添加 **& 关系** 表中：</span><span class="sxs-lookup"><span data-stu-id="042af-266">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="042af-267">**字段标签**</span><span class="sxs-lookup"><span data-stu-id="042af-267">**Field label**</span></span>   |<span data-ttu-id="042af-268">**字段名称**</span><span class="sxs-lookup"><span data-stu-id="042af-268">**Field name**</span></span>|<span data-ttu-id="042af-269">**Data type**</span><span class="sxs-lookup"><span data-stu-id="042af-269">**Data type**</span></span>|<span data-ttu-id="042af-270">**作**</span><span class="sxs-lookup"><span data-stu-id="042af-270">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="042af-271">审核</span><span class="sxs-lookup"><span data-stu-id="042af-271">Audit</span></span>| <span data-ttu-id="042af-272">Audit__c</span><span class="sxs-lookup"><span data-stu-id="042af-272">Audit__c</span></span>|<span data-ttu-id="042af-273">长文本区域 (100000) # B2 可见行 4) </span><span class="sxs-lookup"><span data-stu-id="042af-273">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="042af-274">Microsoft 如何帮助？</span><span class="sxs-lookup"><span data-stu-id="042af-274">How can Microsoft help?</span></span>|<span data-ttu-id="042af-275">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="042af-275">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="042af-276">列表</span><span class="sxs-lookup"><span data-stu-id="042af-276">Picklist\*</span></span>|
   |<span data-ttu-id="042af-277">产品</span><span class="sxs-lookup"><span data-stu-id="042af-277">Products</span></span>|<span data-ttu-id="042af-278">Products_c</span><span class="sxs-lookup"><span data-stu-id="042af-278">Products_c</span></span>|<span data-ttu-id="042af-279">文本 (255) </span><span class="sxs-lookup"><span data-stu-id="042af-279">text (255)</span></span>||
   |<span data-ttu-id="042af-280">引荐</span><span class="sxs-lookup"><span data-stu-id="042af-280">Referral</span></span> | <span data-ttu-id="042af-281">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="042af-281">Referral_Identfier_c</span></span>|<span data-ttu-id="042af-282">文本 (100) # B2 外部 ID) </span><span class="sxs-lookup"><span data-stu-id="042af-282">Text(100)(External ID)</span></span>|<span data-ttu-id="042af-283">是</span><span class="sxs-lookup"><span data-stu-id="042af-283">yes</span></span>|
   |<span data-ttu-id="042af-284">引用链接</span><span class="sxs-lookup"><span data-stu-id="042af-284">Referral Link</span></span>| <span data-ttu-id="042af-285">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="042af-285">Referral_Link_c_</span></span>|<span data-ttu-id="042af-286">URL (255) </span><span class="sxs-lookup"><span data-stu-id="042af-286">URL(255)</span></span>||
   |<span data-ttu-id="042af-287">与合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="042af-287">Sync with Partner Center</span></span>|<span data-ttu-id="042af-288">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="042af-288">sync_with_partner_center_c</span></span>|<span data-ttu-id="042af-289">复选框 (默认未选中) </span><span class="sxs-lookup"><span data-stu-id="042af-289">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="042af-290">\* 选择列表值：</span><span class="sxs-lookup"><span data-stu-id="042af-290">\*Picklist values:</span></span>

   - <span data-ttu-id="042af-291">特定于工作负荷的价值主张</span><span class="sxs-lookup"><span data-stu-id="042af-291">Workload specific value proposition</span></span>
   - <span data-ttu-id="042af-292">客户技术体系结构</span><span class="sxs-lookup"><span data-stu-id="042af-292">Customer technical architecture</span></span>
   - <span data-ttu-id="042af-293">概念证明或演示</span><span class="sxs-lookup"><span data-stu-id="042af-293">Proof of concept or demo</span></span>
   - <span data-ttu-id="042af-294">报价单或许可</span><span class="sxs-lookup"><span data-stu-id="042af-294">Quotes or licensing</span></span>
   - <span data-ttu-id="042af-295">销售客户成功后</span><span class="sxs-lookup"><span data-stu-id="042af-295">Post sales customer success</span></span>
   - <span data-ttu-id="042af-296">常规或其他</span><span class="sxs-lookup"><span data-stu-id="042af-296">General or other</span></span>

5. <span data-ttu-id="042af-297">字段将在 **& 关系的字段**下创建</span><span class="sxs-lookup"><span data-stu-id="042af-297">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="已创建字段":::

6. <span data-ttu-id="042af-299">在 "机会布局" 中，创建一个单独的部分，其中包含上面列出的字段。</span><span class="sxs-lookup"><span data-stu-id="042af-299">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="042af-300">此部分应该适用于机会布局中的卖方</span><span class="sxs-lookup"><span data-stu-id="042af-300">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="合作伙伴中心字段布局":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="042af-302">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="042af-302">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="042af-303">安装、配置和自定义电源自动解决方案后，可以测试 Salesforce CRM 与合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="042af-303">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="042af-304">先决条件</span><span class="sxs-lookup"><span data-stu-id="042af-304">Pre-requisites</span></span>

<span data-ttu-id="042af-305">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="042af-305">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="042af-306">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="042af-306">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="042af-307">一组自定义字段作为 Salesforce CRM 解决方案 **机会** 实体的合作伙伴中心引用同步的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="042af-307">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="042af-308">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="042af-308">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="042af-309">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="042af-309">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="042af-310">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="042af-310">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="042af-311">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="042af-311">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="042af-312">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="042af-312">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="042af-313">**Microsoft 如何帮助**： microsoft 提供的有关推荐的帮助</span><span class="sxs-lookup"><span data-stu-id="042af-313">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="042af-314">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="042af-314">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="042af-315">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="042af-315">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="042af-316">各种</span><span class="sxs-lookup"><span data-stu-id="042af-316">SCENARIOS:</span></span>

1. <span data-ttu-id="042af-317">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="042af-317">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="042af-318">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="042af-318">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="042af-319">在 Salesforce CRM 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="042af-319">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 环境":::

   3. <span data-ttu-id="042af-321">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="042af-321">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="042af-322">"与合作伙伴中心同步"：是</span><span class="sxs-lookup"><span data-stu-id="042af-322">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="042af-323">"Microsoft help 怎样？"：从以下选项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="042af-323">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="042af-324">产品：产品的解决方案 Id</span><span class="sxs-lookup"><span data-stu-id="042af-324">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="042af-325">将 "机会  **与合作伙伴中心同步** " 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="042af-325">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="042af-326">你的引用将与 Salesforce CRM 同步。</span><span class="sxs-lookup"><span data-stu-id="042af-326">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="042af-327">当 "与合作伙伴中心同步" 选项设置为 "是" 时，如果您更新了 Salesforce CRM 中的机会，则这些更改将与合作伙伴中心帐户同步。</span><span class="sxs-lookup"><span data-stu-id="042af-327">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="042af-328">与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="042af-328">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="042af-329">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="042af-329">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="042af-330">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="042af-330">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="042af-331">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="042af-331">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="042af-332">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="042af-332">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="042af-333">登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="042af-333">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="042af-334">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="042af-334">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="042af-335">Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。</span><span class="sxs-lookup"><span data-stu-id="042af-335">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 机会屏幕":::

    6. <span data-ttu-id="042af-337">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="042af-337">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="042af-338">后续步骤</span><span class="sxs-lookup"><span data-stu-id="042af-338">Next steps</span></span>

- [<span data-ttu-id="042af-339">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="042af-339">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="042af-340">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="042af-340">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="042af-341">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="042af-341">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)