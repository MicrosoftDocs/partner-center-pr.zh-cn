---
title: Salesforce CRM 合作伙伴中心 联合销售连接器
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将你的引荐合作伙伴中心 Salesforce CRM 同步。 然后，销售人员可以从 CRM 系统内部与 Microsoft 联合销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276971"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="b61fb-104">用于 Salesforce CRM 的联合销售连接器 – 概述</span><span class="sxs-lookup"><span data-stu-id="b61fb-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="b61fb-105">**适当的角色**：引荐管理员|CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="b61fb-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b61fb-106">合作伙伴中心联合销售连接器可让销售人员从 CRM 系统内部与 Microsoft 联合销售。</span><span class="sxs-lookup"><span data-stu-id="b61fb-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b61fb-107">他们不需要经过训练，就可使用合作伙伴中心联合销售交易。</span><span class="sxs-lookup"><span data-stu-id="b61fb-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b61fb-108">使用联合销售连接器，可以创建一个新的联合销售引荐来吸引 Microsoft 销售人员、接收来自 Microsoft 卖方的引荐、接受/拒绝引荐、修改交易数据（例如交易值）和结束日期。</span><span class="sxs-lookup"><span data-stu-id="b61fb-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="b61fb-109">还可以从 Microsoft 卖方处收到有关这些联合销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="b61fb-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b61fb-110">可以在你选择的 CRM 中工作，而不是在自己选择的 CRM 中工作，而不是在 合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="b61fb-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b61fb-111">该解决方案基于 Microsoft Power Automate 解决方案，并使用 合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="b61fb-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b61fb-112">安装前 - 先决条件</span><span class="sxs-lookup"><span data-stu-id="b61fb-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b61fb-113">**主题**</span><span class="sxs-lookup"><span data-stu-id="b61fb-113">**Topics**</span></span>   |<span data-ttu-id="b61fb-114">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="b61fb-114">**Details**</span></span>   |<span data-ttu-id="b61fb-115">**链接**</span><span class="sxs-lookup"><span data-stu-id="b61fb-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b61fb-116">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="b61fb-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b61fb-117">需要有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="b61fb-117">You need a valid MPN ID</span></span>|<span data-ttu-id="b61fb-118">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="b61fb-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b61fb-119">已做好联合销售准备</span><span class="sxs-lookup"><span data-stu-id="b61fb-119">Co-sell ready</span></span>|<span data-ttu-id="b61fb-120">IP/服务解决方案必须可供联合销售。</span><span class="sxs-lookup"><span data-stu-id="b61fb-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b61fb-121">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="b61fb-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b61fb-122">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="b61fb-122">Partner Center account</span></span>|<span data-ttu-id="b61fb-123">与联合销售合作伙伴中心关联的 MPN ID 必须与与联合销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="b61fb-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b61fb-124">在部署连接器之前，请验证是否可在 合作伙伴中心门户中查看联合销售引荐。</span><span class="sxs-lookup"><span data-stu-id="b61fb-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b61fb-125">管理帐户</span><span class="sxs-lookup"><span data-stu-id="b61fb-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b61fb-126">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="b61fb-126">Partner Center user roles</span></span>|<span data-ttu-id="b61fb-127">将安装和使用连接器的员工必须是引荐管理员</span><span class="sxs-lookup"><span data-stu-id="b61fb-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b61fb-128">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="b61fb-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b61fb-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b61fb-129">Salesforce CRM</span></span>|<span data-ttu-id="b61fb-130">CRM 用户角色为"系统管理员"或"系统定制员"</span><span class="sxs-lookup"><span data-stu-id="b61fb-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b61fb-131">在 Salesforce CRM 中分配角色</span><span class="sxs-lookup"><span data-stu-id="b61fb-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="b61fb-132">Power Automate Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="b61fb-132">Power Automate Flow Account</span></span>|<span data-ttu-id="b61fb-133">CRM [Power Automate](https://flow.microsoft.com) 或系统定制员的活动帐户。</span><span class="sxs-lookup"><span data-stu-id="b61fb-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="b61fb-134">该用户应在安装 [Power Automate](https://flow.microsoft.com) 至少登录一次。</span><span class="sxs-lookup"><span data-stu-id="b61fb-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="b61fb-135">安装 Microsoft 自定义字段的 Salesforce 包</span><span class="sxs-lookup"><span data-stu-id="b61fb-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="b61fb-136">若要跨 合作伙伴中心 Salesforce CRM 同步引荐，Power Automate解决方案需要明确标识 Microsoft 特定的引荐字段。</span><span class="sxs-lookup"><span data-stu-id="b61fb-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="b61fb-137">合作伙伴销售人员团队能够决定要与 Microsoft 共享哪些引荐进行联合销售。</span><span class="sxs-lookup"><span data-stu-id="b61fb-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="b61fb-138">在 Salesforce 中，激活 **"** 备注"，并将其添加到与商机相关的列表中。</span><span class="sxs-lookup"><span data-stu-id="b61fb-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="b61fb-139">引用</span><span class="sxs-lookup"><span data-stu-id="b61fb-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="b61fb-140">按照 **以下步骤** 激活机会团队：</span><span class="sxs-lookup"><span data-stu-id="b61fb-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="b61fb-141">在"设置"中，使用" **快速查找** "框查找"机会团队设置"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="b61fb-142">根据需要定义设置。</span><span class="sxs-lookup"><span data-stu-id="b61fb-142">Define the settings as needed.</span></span>
[<span data-ttu-id="b61fb-143">引用</span><span class="sxs-lookup"><span data-stu-id="b61fb-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="b61fb-144">在 Salesforce 中，使用包安装程序 安装 [自定义字段和对象](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)。</span><span class="sxs-lookup"><span data-stu-id="b61fb-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="b61fb-145">使用此包将包安装到任何公司。</span><span class="sxs-lookup"><span data-stu-id="b61fb-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="b61fb-146">如果要安装到沙盒中，则必须将 URL 的初始部分替换为 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="b61fb-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="b61fb-147">在 Salesforce 中，将 Microsoft Solutions 添加到 **"机会相关"** 列表。</span><span class="sxs-lookup"><span data-stu-id="b61fb-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="b61fb-148">添加后，选择 **手部** 图标并更新属性</span><span class="sxs-lookup"><span data-stu-id="b61fb-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b61fb-149">最佳做法：在上台之前进行测试</span><span class="sxs-lookup"><span data-stu-id="b61fb-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="b61fb-150">在生产环境中安装、配置Power Automate自定义解决方案之前，请务必在过渡 CRM 实例上测试该解决方案。</span><span class="sxs-lookup"><span data-stu-id="b61fb-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b61fb-151">在Power Automate/CRM 实例上安装 Microsoft Power Automate 解决方案。</span><span class="sxs-lookup"><span data-stu-id="b61fb-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="b61fb-152">创建解决方案的副本，在过渡Power Automate运行配置和流自定义。</span><span class="sxs-lookup"><span data-stu-id="b61fb-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="b61fb-153">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="b61fb-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="b61fb-154">成功后，作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="b61fb-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="b61fb-155">安装合作伙伴中心 Salesforce CRM 的推荐同步</span><span class="sxs-lookup"><span data-stu-id="b61fb-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="b61fb-156">转到 [Power Automate，](https://flow.microsoft.com)**然后选择右上角** 的"环境"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b61fb-157">此时会显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="b61fb-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b61fb-158">从右上角的下拉列表中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="b61fb-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="b61fb-159">在 **左侧** 导航栏中选择"解决方案"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b61fb-160">选择顶部 **菜单上的"打开 AppSource"** 链接。</span><span class="sxs-lookup"><span data-stu-id="b61fb-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource。":::

5. <span data-ttu-id="b61fb-162">在 **合作伙伴中心屏幕中搜索 Salesforce** 的推荐连接器。</span><span class="sxs-lookup"><span data-stu-id="b61fb-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce。":::

6. <span data-ttu-id="b61fb-164">选择"**现在获取"按钮**，然后选择"**继续"。**</span><span class="sxs-lookup"><span data-stu-id="b61fb-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="b61fb-165">这将打开一个页面，可在其中选择要安装应用程序的 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="b61fb-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="b61fb-166">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="b61fb-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用的 CRMS。":::

8. <span data-ttu-id="b61fb-168">然后，你被定向到 **"管理解决方案"页** 。</span><span class="sxs-lookup"><span data-stu-id="b61fb-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="b61fb-169">使用页面底部的箭头按钮导航到"合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="b61fb-170">**计划的安装** 应显示在"引荐合作伙伴中心旁边。</span><span class="sxs-lookup"><span data-stu-id="b61fb-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="b61fb-171">安装需要 10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="b61fb-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="b61fb-172">安装完成后，导航回 [Power Automate左侧导航](https://flow.microsoft.com) 区域中 **选择"解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="b61fb-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b61fb-173">请注意 **，合作伙伴中心解决方案列表中提供了 Salesforce** 的推荐同步。</span><span class="sxs-lookup"><span data-stu-id="b61fb-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b61fb-174">选择 **合作伙伴中心 Salesforce 的引荐同步"**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="b61fb-175">以下Power Automate流和实体可用：</span><span class="sxs-lookup"><span data-stu-id="b61fb-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 流。":::



## <a name="configure-the-solution"></a><span data-ttu-id="b61fb-177">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="b61fb-177">Configure the solution</span></span>

1. <span data-ttu-id="b61fb-178">在 CRM 实例中安装解决方案后，导航回[Power Automate。](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="b61fb-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="b61fb-179">从 **右上角** 的"环境"下拉列表中，选择安装了 Power Automate 解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="b61fb-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="b61fb-180">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="b61fb-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="b61fb-181">合作伙伴中心管理员凭据的用户</span><span class="sxs-lookup"><span data-stu-id="b61fb-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="b61fb-182">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="b61fb-182">Partner Center Events</span></span>
    - <span data-ttu-id="b61fb-183">具有解决方案Power Automate流的 CRM 管理员。</span><span class="sxs-lookup"><span data-stu-id="b61fb-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="b61fb-184">从 **左侧** 导航栏中选择"连接"，然后从列表中选择"合作伙伴中心推荐"解决方案。</span><span class="sxs-lookup"><span data-stu-id="b61fb-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="b61fb-185">通过单击"创建连接 **"创建连接**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="创建连接。":::

- <span data-ttu-id="b61fb-187">在合作伙伴中心的 (搜索) 搜索"中，搜索"引荐"和"预览版"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="b61fb-188">使用引荐管理员合作伙伴中心为用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="b61fb-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="b61fb-189">接下来，使用合作伙伴中心管理员的凭据为合作伙伴中心用户创建一个事件连接。</span><span class="sxs-lookup"><span data-stu-id="b61fb-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="b61fb-190">为 CRM 管理员用户创建 Salesforce 连接。</span><span class="sxs-lookup"><span data-stu-id="b61fb-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="b61fb-191">添加所有连接后，应在环境中看到以下连接：</span><span class="sxs-lookup"><span data-stu-id="b61fb-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="观察连接。":::

### <a name="edit-the-connections"></a><span data-ttu-id="b61fb-193">编辑连接</span><span class="sxs-lookup"><span data-stu-id="b61fb-193">Edit the connections</span></span>

1. <span data-ttu-id="b61fb-194">返回到"解决方案"页，然后选择"**默认解决方案"。**</span><span class="sxs-lookup"><span data-stu-id="b61fb-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="b61fb-195">单击 **"所有" (") "\*\*\*\*连接引用**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="开始连接器编辑。":::

2. <span data-ttu-id="b61fb-197">通过选择三个点图标单独编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="b61fb-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="b61fb-198">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="b61fb-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="编辑连接器。":::

3. <span data-ttu-id="b61fb-200">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="b61fb-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="b61fb-201"> (内幕预览版) 合作伙伴中心 Webhook 注册</span><span class="sxs-lookup"><span data-stu-id="b61fb-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="b61fb-202">创建向合作伙伴中心 (内幕预览版的共同销售推荐-Salesforce) </span><span class="sxs-lookup"><span data-stu-id="b61fb-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b61fb-203">合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) </span><span class="sxs-lookup"><span data-stu-id="b61fb-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b61fb-204">合作伙伴中心到 Salesforce (预览体验) </span><span class="sxs-lookup"><span data-stu-id="b61fb-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b61fb-205">Salesforce 到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="b61fb-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b61fb-206">合作机会到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="b61fb-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b61fb-207">Salesforce Microsoft 解决方案到合作伙伴中心 (预览体验) </span><span class="sxs-lookup"><span data-stu-id="b61fb-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b61fb-208">使用 Webhook Api 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="b61fb-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b61fb-209">合作伙伴中心 Webhook Api 允许你注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="b61fb-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b61fb-210">这些更改事件以 HTTP post 的形式发送到你的 url。</span><span class="sxs-lookup"><span data-stu-id="b61fb-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b61fb-211">若要注册 url，请选择 " **合作伙伴中心 Webhook 注册 (内幕预览版")** Power 自动流 "。</span><span class="sxs-lookup"><span data-stu-id="b61fb-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b61fb-212">为 (a ) 合作伙伴中心用户添加连接， (b. ) 合作伙伴中心事件如下所示</span><span class="sxs-lookup"><span data-stu-id="b61fb-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="界限.":::

3. <span data-ttu-id="b61fb-214">进行这些更新后，你将看到</span><span class="sxs-lookup"><span data-stu-id="b61fb-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook.":::

4. <span data-ttu-id="b61fb-216">保存更改，然后选择 **"打开"**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="b61fb-217">若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="b61fb-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="b61fb-218">选择 " **合作伙伴中心到 SALESFORCE CRM (内幕预览版")**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="b61fb-219">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b61fb-220">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="b61fb-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="复制 URL。":::

8. <span data-ttu-id="b61fb-222">现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b61fb-223">确保在右侧窗格中打开 "运行流" 窗口，并选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="b61fb-224">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="b61fb-224">Enter the following details:</span></span>

    1. <span data-ttu-id="b61fb-225">**Http 触发器终结点**：从前面的步骤中复制的 URL</span><span class="sxs-lookup"><span data-stu-id="b61fb-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="b61fb-226">**要注册的事件**： "引用已创建" 和 "引用已更新"</span><span class="sxs-lookup"><span data-stu-id="b61fb-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="b61fb-227">**覆盖现有触发器终结点（如果存在**）：是 (这将覆盖任何现有终结点。 ) </span><span class="sxs-lookup"><span data-stu-id="b61fb-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="b61fb-228">选择 " **运行** "，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="b61fb-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b61fb-229">Webhook 现在可以侦听以创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="b61fb-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b61fb-230">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="b61fb-230">Customize synchronization steps</span></span>

<span data-ttu-id="b61fb-231">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="b61fb-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b61fb-232">通常，CRM 系统是高度自定义的。</span><span class="sxs-lookup"><span data-stu-id="b61fb-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b61fb-233">您可以自定义自动执行流的功能。</span><span class="sxs-lookup"><span data-stu-id="b61fb-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b61fb-234">按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="b61fb-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b61fb-235">我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。</span><span class="sxs-lookup"><span data-stu-id="b61fb-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b61fb-236">可根据需要自定义每个电源自动流的多个步骤。</span><span class="sxs-lookup"><span data-stu-id="b61fb-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b61fb-237">下面是可用自定义的示例：</span><span class="sxs-lookup"><span data-stu-id="b61fb-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b61fb-238">若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b61fb-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="b61fb-239">选择 "合作伙伴中心到 Salesforce CRM (内幕预览版") 。</span><span class="sxs-lookup"><span data-stu-id="b61fb-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="b61fb-240">选择 " **编辑** " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="b61fb-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="b61fb-241">选择 " **(范围") 同步潜在客户或机会**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b61fb-242">若要为创建事件自定义 CRM 字段映射，请选择 **新的共享机会，然后选择 "是"**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b61fb-243">选择 " **是"** ，然后 **在 CRM 中展开 "创建新机会**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b61fb-244">您可以使用字段映射指南来编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="b61fb-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="b61fb-245">若要为更新事件自定义 CRM 字段映射，请选择步骤 " (范围) 同步潜在客户或机会"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="b61fb-246">**如果是对机会的更新，** 请选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b61fb-247">选择 " **是"** ，然后展开 " **如果合作伙伴中心和 CRM 中的机会对象之间的差异"，然后** 展开。</span><span class="sxs-lookup"><span data-stu-id="b61fb-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="b61fb-248">**如果是，则选择 "是"** ，然后选择 "**更新现有机会**</span><span class="sxs-lookup"><span data-stu-id="b61fb-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="b61fb-249">为更新事件自定义 CRM 到 PC 引用同步的字段：</span><span class="sxs-lookup"><span data-stu-id="b61fb-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="b61fb-250">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="b61fb-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b61fb-251">选择 **(范围) 同步机会**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="b61fb-252">对于 "基于字段映射 (自定义 CRM 字段映射" 指南) 对于 "更新事件"，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。</span><span class="sxs-lookup"><span data-stu-id="b61fb-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="b61fb-253">**如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。</span><span class="sxs-lookup"><span data-stu-id="b61fb-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="b61fb-254">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="b61fb-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b61fb-255">为创建事件自定义 CRM 到 PC 引用同步的字段？</span><span class="sxs-lookup"><span data-stu-id="b61fb-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="b61fb-256">选择 " **编辑**  " 以编辑/自定义电源自动流程。</span><span class="sxs-lookup"><span data-stu-id="b61fb-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b61fb-257">选择 **) 同步引用 (范围。**</span><span class="sxs-lookup"><span data-stu-id="b61fb-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="b61fb-258">对于 "基于字段映射自定义 CRM 字段映射 (" 指南) 对于创建事件，请选择 " **创建 Microsoft 引用**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="b61fb-259">您可以根据字段映射指南编辑此部分中的映射。</span><span class="sxs-lookup"><span data-stu-id="b61fb-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b61fb-260">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="b61fb-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b61fb-261">安装、配置和自定义电源自动解决方案后，可以测试 Salesforce CRM 与合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="b61fb-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b61fb-262">先决条件</span><span class="sxs-lookup"><span data-stu-id="b61fb-262">Pre-requisites</span></span>

<span data-ttu-id="b61fb-263">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要明确界定特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="b61fb-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b61fb-264">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="b61fb-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b61fb-265">一组自定义字段作为 Salesforce CRM 解决方案 **机会** 实体的合作伙伴中心引用同步的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="b61fb-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="b61fb-266">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="b61fb-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b61fb-267">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="b61fb-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b61fb-268">**与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步</span><span class="sxs-lookup"><span data-stu-id="b61fb-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b61fb-269">**引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段</span><span class="sxs-lookup"><span data-stu-id="b61fb-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b61fb-270">**引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接</span><span class="sxs-lookup"><span data-stu-id="b61fb-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b61fb-271">**Microsoft 如何帮助**： microsoft 提供的有关推荐的帮助</span><span class="sxs-lookup"><span data-stu-id="b61fb-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b61fb-272">**产品**：与此机会关联的产品列表</span><span class="sxs-lookup"><span data-stu-id="b61fb-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b61fb-273">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="b61fb-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="b61fb-274">各种</span><span class="sxs-lookup"><span data-stu-id="b61fb-274">SCENARIOS:</span></span>

1. <span data-ttu-id="b61fb-275">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="b61fb-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="b61fb-276">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="b61fb-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="b61fb-277">在 Salesforce CRM 环境中创建 "新机会" 时，请确保以下部分存在</span><span class="sxs-lookup"><span data-stu-id="b61fb-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 环境。":::

   3. <span data-ttu-id="b61fb-279">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="b61fb-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="b61fb-280">"与合作伙伴中心同步"：是</span><span class="sxs-lookup"><span data-stu-id="b61fb-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="b61fb-281">"Microsoft help 怎样？"：从以下选项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="b61fb-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="b61fb-282">产品：产品的解决方案 Id</span><span class="sxs-lookup"><span data-stu-id="b61fb-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="b61fb-283">将 "机会  **与合作伙伴中心同步** " 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="b61fb-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b61fb-284">你的引用将与 Salesforce CRM 同步。</span><span class="sxs-lookup"><span data-stu-id="b61fb-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="b61fb-285">当 "与合作伙伴中心同步" 选项设置为 "是" 时，如果您更新了 Salesforce CRM 中的机会，则这些更改将与合作伙伴中心帐户同步。</span><span class="sxs-lookup"><span data-stu-id="b61fb-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="b61fb-286">与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="b61fb-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="b61fb-287">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="b61fb-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="b61fb-288">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="b61fb-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="b61fb-289">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="b61fb-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="b61fb-290">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="b61fb-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="b61fb-291">登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="b61fb-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="b61fb-292">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="b61fb-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b61fb-293">Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。</span><span class="sxs-lookup"><span data-stu-id="b61fb-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 机会屏幕。":::

    6. <span data-ttu-id="b61fb-295">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="b61fb-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b61fb-296">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b61fb-296">Next steps</span></span>

- [<span data-ttu-id="b61fb-297">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="b61fb-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b61fb-298">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="b61fb-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b61fb-299">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="b61fb-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
