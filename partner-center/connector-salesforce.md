---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Salesforce CRM 同步。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284377"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="20749-104">用于 Salesforce CRM 的联合销售连接器 – 概述</span><span class="sxs-lookup"><span data-stu-id="20749-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="20749-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="20749-105">**Appropriate roles**</span></span>

- <span data-ttu-id="20749-106">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="20749-106">Referrals admin</span></span>
- <span data-ttu-id="20749-107">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="20749-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="20749-108">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="20749-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="20749-109">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="20749-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="20749-110">使用共同销售连接器，你可以创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用，接受/拒绝引用，修改交易数据（如交易价值）和结束日期。</span><span class="sxs-lookup"><span data-stu-id="20749-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="20749-111">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="20749-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="20749-112">你可以在所选的 CRM 中工作而不是在合作伙伴中心内工作时执行所有引用工作。</span><span class="sxs-lookup"><span data-stu-id="20749-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="20749-113">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="20749-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="20749-114">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="20749-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="20749-115">**主题**</span><span class="sxs-lookup"><span data-stu-id="20749-115">**Topics**</span></span>   |<span data-ttu-id="20749-116">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="20749-116">**Details**</span></span>   |<span data-ttu-id="20749-117">**链接**</span><span class="sxs-lookup"><span data-stu-id="20749-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="20749-118">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="20749-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="20749-119">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="20749-119">You need a valid MPN ID</span></span>|<span data-ttu-id="20749-120">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="20749-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="20749-121">已做好联合销售准备</span><span class="sxs-lookup"><span data-stu-id="20749-121">Co-sell ready</span></span>|<span data-ttu-id="20749-122">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="20749-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="20749-123">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="20749-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="20749-124">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="20749-124">Partner Center account</span></span>|<span data-ttu-id="20749-125">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="20749-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="20749-126">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="20749-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="20749-127">管理帐户</span><span class="sxs-lookup"><span data-stu-id="20749-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="20749-128">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="20749-128">Partner Center user roles</span></span>|<span data-ttu-id="20749-129">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="20749-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="20749-130">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="20749-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="20749-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="20749-131">Salesforce CRM</span></span>|<span data-ttu-id="20749-132">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="20749-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="20749-133">在 Salesforce CRM 中分配角色</span><span class="sxs-lookup"><span data-stu-id="20749-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="20749-134">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="20749-134">Power Automate Flow Account</span></span>|<span data-ttu-id="20749-135">CRM 系统管理员或系统定制员的有效 [电源自动完成](https://flow.microsoft.com) 帐户。</span><span class="sxs-lookup"><span data-stu-id="20749-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="20749-136">在安装之前，该用户至少应登录到一次 [电源](https://flow.microsoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="20749-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="20749-137">为 Microsoft 自定义字段安装 Salesforce 包</span><span class="sxs-lookup"><span data-stu-id="20749-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="20749-138">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要清楚地识别特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="20749-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="20749-139">此分界为合作伙伴卖方团队提供了决定他们要与 Microsoft 共享以共同销售的推荐的功能。</span><span class="sxs-lookup"><span data-stu-id="20749-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="20749-140">在 Salesforce 中，激活 **注释** 并将其添加到机会相关列表。</span><span class="sxs-lookup"><span data-stu-id="20749-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="20749-141">引用</span><span class="sxs-lookup"><span data-stu-id="20749-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="20749-142">按照以下步骤激活 **机会团队** ：</span><span class="sxs-lookup"><span data-stu-id="20749-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="20749-143">在安装程序中，使用 " **快速查找** " 框定位机会团队设置。</span><span class="sxs-lookup"><span data-stu-id="20749-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="20749-144">根据需要定义设置。</span><span class="sxs-lookup"><span data-stu-id="20749-144">Define the settings as needed.</span></span>
[<span data-ttu-id="20749-145">引用</span><span class="sxs-lookup"><span data-stu-id="20749-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="20749-146">在 Salesforce 中，使用 [包安装程序](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)安装自定义字段和对象。</span><span class="sxs-lookup"><span data-stu-id="20749-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="20749-147">使用此可将包安装到任何公司。</span><span class="sxs-lookup"><span data-stu-id="20749-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="20749-148">如果要安装到沙盒，则必须将 URL 的初始部分替换为 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="20749-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="20749-149">在 Salesforce 中，将 Microsoft 解决方案添加到 **机会** 相关列表。</span><span class="sxs-lookup"><span data-stu-id="20749-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="20749-150">添加后，选择 **扳手** 图标并更新属性</span><span class="sxs-lookup"><span data-stu-id="20749-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="20749-151">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="20749-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="20749-152">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="20749-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="20749-153">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="20749-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="20749-154">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="20749-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="20749-155">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="20749-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="20749-156">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="20749-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="20749-157">为 Salesforce CRM 安装合作伙伴中心引用同步</span><span class="sxs-lookup"><span data-stu-id="20749-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="20749-158">请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="20749-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="20749-159">这会显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="20749-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="20749-160">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="20749-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="20749-161">选择左侧导航栏上的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="20749-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="20749-162">在顶部菜单中选择 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="20749-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. <span data-ttu-id="20749-164">在弹出屏幕中搜索 Salesforce 的 " **合作伙伴中心引用连接器** "。</span><span class="sxs-lookup"><span data-stu-id="20749-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="20749-166">选择 " **立即获取** " 按钮，然后 **继续**。</span><span class="sxs-lookup"><span data-stu-id="20749-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="20749-167">这将打开可在其中选择要安装应用程序的 Salesforce CRM 环境的页面。</span><span class="sxs-lookup"><span data-stu-id="20749-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="20749-168">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="20749-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用 CRM":::

8. <span data-ttu-id="20749-170">然后，你将转到 " **管理你的解决方案** " 页。</span><span class="sxs-lookup"><span data-stu-id="20749-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="20749-171">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="20749-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="20749-172">**计划的安装** 应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="20749-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="20749-173">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="20749-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="20749-174">安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="20749-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="20749-175">请注意，"解决方案" 列表中提供了 **Salesforce 的合作伙伴中心引用同步** 。</span><span class="sxs-lookup"><span data-stu-id="20749-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="20749-176">**为 Salesforce 选择合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="20749-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="20749-177">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="20749-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 流":::



## <a name="configure-the-solution"></a><span data-ttu-id="20749-179">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="20749-179">Configure the solution</span></span>

1. <span data-ttu-id="20749-180">在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="20749-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="20749-181">在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="20749-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="20749-182">你将需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="20749-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="20749-183">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="20749-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="20749-184">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="20749-184">Partner Center Events</span></span>
    - <span data-ttu-id="20749-185">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="20749-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="20749-186">从左侧导航栏中选择 " **连接** "，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="20749-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="20749-187">通过单击 " **创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="20749-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="创建连接":::

- <span data-ttu-id="20749-189">在右上角的搜索栏中搜索 "合作伙伴中心引用 (预览") 。</span><span class="sxs-lookup"><span data-stu-id="20749-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="20749-190">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="20749-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="20749-191">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="20749-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="20749-192">为 CRM 管理员用户创建 Salesforce 连接。</span><span class="sxs-lookup"><span data-stu-id="20749-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="20749-193">添加所有连接后，你的环境中应会显示以下连接：</span><span class="sxs-lookup"><span data-stu-id="20749-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="观察连接":::

### <a name="edit-the-connections"></a><span data-ttu-id="20749-195">编辑连接</span><span class="sxs-lookup"><span data-stu-id="20749-195">Edit the connections</span></span>

1. <span data-ttu-id="20749-196">返回 "解决方案" 页，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="20749-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="20749-197">通过单击 "**全部**" **(预览) 选择 "连接引用**"。</span><span class="sxs-lookup"><span data-stu-id="20749-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="开始连接器编辑":::

2. <span data-ttu-id="20749-199">通过选择三个点图标，分别编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="20749-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="20749-200">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="20749-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="编辑连接器":::

3. <span data-ttu-id="20749-202">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="20749-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="20749-203"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="20749-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="20749-204">创建向合作伙伴中心 (内幕预览版的共同销售推荐-Salesforce) </span><span class="sxs-lookup"><span data-stu-id="20749-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20749-205">合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) </span><span class="sxs-lookup"><span data-stu-id="20749-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="20749-206">合作伙伴中心到 Salesforce (预览体验) </span><span class="sxs-lookup"><span data-stu-id="20749-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="20749-207">Salesforce 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="20749-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20749-208">合作机会到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="20749-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20749-209">Salesforce Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="20749-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="20749-210">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="20749-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="20749-211">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="20749-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="20749-212">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="20749-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="20749-213">若要注册 url，请选择 " **合作伙伴中心 Webhook 注册 (内幕预览版")** Power 自动流 "。</span><span class="sxs-lookup"><span data-stu-id="20749-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="20749-214">为 (a ) 合作伙伴中心用户添加连接， (b. ) 合作伙伴中心事件如下所示</span><span class="sxs-lookup"><span data-stu-id="20749-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="触发器":::

3. <span data-ttu-id="20749-216">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="20749-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="20749-218">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="20749-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="20749-219">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="20749-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="20749-220">选择 " **合作伙伴中心到 SALESFORCE CRM (内幕预览版")**。</span><span class="sxs-lookup"><span data-stu-id="20749-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="20749-221">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="20749-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="20749-222">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="20749-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="复制 URL":::

8. <span data-ttu-id="20749-224">现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="20749-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="20749-225">确保在右侧窗格中打开 "运行流" 窗口，并选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="20749-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="20749-226">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="20749-226">Enter the following details:</span></span>

    1. <span data-ttu-id="20749-227">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="20749-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="20749-228">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="20749-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="20749-229">**覆盖现有触发器终结点（如果存在**）：是 (这将覆盖任何现有终结点。 ) </span><span class="sxs-lookup"><span data-stu-id="20749-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="20749-230">选择 " **运行** "，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="20749-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="20749-231">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="20749-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="20749-232">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="20749-232">Customize synchronization steps</span></span>

<span data-ttu-id="20749-233">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="20749-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="20749-234">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="20749-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="20749-235">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="20749-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="20749-236">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="20749-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="20749-237">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="20749-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="20749-238">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="20749-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="20749-239">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="20749-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="20749-240">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="20749-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="20749-241">选择 "合作伙伴中心到 Salesforce CRM (内幕预览版") 。</span><span class="sxs-lookup"><span data-stu-id="20749-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="20749-242">选择 " **编辑** " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="20749-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="20749-243">选择 " **(范围") 同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="20749-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="20749-244">若要为创建事件自定义 CRM 字段映射，请选择 **新的共享机会，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="20749-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="20749-245">选择 " **是"** ，然后 **在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="20749-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="20749-246">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="20749-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="20749-247">若要为更新事件自定义 CRM 字段映射，请选择步骤 " (范围) 同步潜在客户或机会"。</span><span class="sxs-lookup"><span data-stu-id="20749-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="20749-248">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="20749-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="20749-249">选择 " **是"** ，然后展开 " **如果合作伙伴中心和 CRM 中的机会对象之间的差异"，然后** 展开。</span><span class="sxs-lookup"><span data-stu-id="20749-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="20749-250">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="20749-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="20749-251">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="20749-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="20749-252">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="20749-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="20749-253">选择 **(范围) 同步机会**。</span><span class="sxs-lookup"><span data-stu-id="20749-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="20749-254">对于 "基于字段映射 (自定义 CRM 字段映射" 指南) 对于 "更新事件"，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="20749-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="20749-255">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="20749-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="20749-256">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="20749-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="20749-257">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="20749-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="20749-258">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="20749-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="20749-259">选择 **) 同步引用 (范围。**</span><span class="sxs-lookup"><span data-stu-id="20749-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="20749-260">对于 "基于字段映射自定义 CRM 字段映射 (" 指南) 对于创建事件，请选择 " **创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="20749-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="20749-261">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="20749-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="20749-262">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="20749-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="20749-263">安装、配置和自定义电源自动解决方案后，可以测试 Salesforce CRM 与合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="20749-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="20749-264">先决条件</span><span class="sxs-lookup"><span data-stu-id="20749-264">Pre-requisites</span></span>

<span data-ttu-id="20749-265">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="20749-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="20749-266">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="20749-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="20749-267">一组自定义字段作为 Salesforce CRM 解决方案 **机会** 实体的合作伙伴中心引用同步的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="20749-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="20749-268">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="20749-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="20749-269">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="20749-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="20749-270">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="20749-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="20749-271">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="20749-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="20749-272">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="20749-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="20749-273">**Microsoft 如何帮助**： microsoft 提供的有关推荐的帮助</span><span class="sxs-lookup"><span data-stu-id="20749-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="20749-274">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="20749-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="20749-275">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="20749-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="20749-276">各种</span><span class="sxs-lookup"><span data-stu-id="20749-276">SCENARIOS:</span></span>

1. <span data-ttu-id="20749-277">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="20749-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="20749-278">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="20749-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="20749-279">在 Salesforce CRM 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="20749-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 环境":::

   3. <span data-ttu-id="20749-281">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="20749-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="20749-282">"与合作伙伴中心同步"：是</span><span class="sxs-lookup"><span data-stu-id="20749-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="20749-283">"Microsoft help 怎样？"：从以下选项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="20749-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="20749-284">产品：产品的解决方案 Id</span><span class="sxs-lookup"><span data-stu-id="20749-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="20749-285">将 "机会  **与合作伙伴中心同步** " 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="20749-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="20749-286">你的引用将与 Salesforce CRM 同步。</span><span class="sxs-lookup"><span data-stu-id="20749-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="20749-287">当 "与合作伙伴中心同步" 选项设置为 "是" 时，如果您更新了 Salesforce CRM 中的机会，则这些更改将与合作伙伴中心帐户同步。</span><span class="sxs-lookup"><span data-stu-id="20749-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="20749-288">与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="20749-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="20749-289">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="20749-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="20749-290">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="20749-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="20749-291">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="20749-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="20749-292">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="20749-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="20749-293">登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="20749-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="20749-294">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="20749-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="20749-295">Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。</span><span class="sxs-lookup"><span data-stu-id="20749-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 机会屏幕":::

    6. <span data-ttu-id="20749-297">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="20749-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20749-298">后续步骤</span><span class="sxs-lookup"><span data-stu-id="20749-298">Next steps</span></span>

- [<span data-ttu-id="20749-299">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="20749-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="20749-300">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="20749-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="20749-301">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="20749-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
