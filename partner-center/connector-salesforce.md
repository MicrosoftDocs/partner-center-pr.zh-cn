---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Salesforce CRM 同步。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029042"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="0e1fa-104">用于 Salesforce CRM 的联合销售连接器 – 概述</span><span class="sxs-lookup"><span data-stu-id="0e1fa-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="0e1fa-105">**适当的角色**：引用管理 |CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="0e1fa-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="0e1fa-106">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="0e1fa-107">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-107">They won't have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="0e1fa-108">使用共同销售连接器，你可以创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用，接受/拒绝引用，修改交易数据（如交易价值）和结束日期。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="0e1fa-109">你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="0e1fa-110">你可以在所选的 CRM 中工作而不是在合作伙伴中心内工作时执行所有引用工作。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="0e1fa-111">此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="0e1fa-112">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="0e1fa-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="0e1fa-113">**主题**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-113">**Topics**</span></span>|<span data-ttu-id="0e1fa-114">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-114">**Details**</span></span>|<span data-ttu-id="0e1fa-115">**链接**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-115">**Links**</span></span>|
|--------------|--------------------|------|
|<span data-ttu-id="0e1fa-116">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="0e1fa-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="0e1fa-117">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="0e1fa-117">You need a valid MPN ID</span></span>|<span data-ttu-id="0e1fa-118">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="0e1fa-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="0e1fa-119">已做好联合销售准备</span><span class="sxs-lookup"><span data-stu-id="0e1fa-119">Co-sell ready</span></span>|<span data-ttu-id="0e1fa-120">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="0e1fa-121">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="0e1fa-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="0e1fa-122">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="0e1fa-122">Partner Center account</span></span>|<span data-ttu-id="0e1fa-123">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="0e1fa-124">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="0e1fa-125">管理帐户</span><span class="sxs-lookup"><span data-stu-id="0e1fa-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="0e1fa-126">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="0e1fa-126">Partner Center user roles</span></span>|<span data-ttu-id="0e1fa-127">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="0e1fa-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="0e1fa-128">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="0e1fa-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="0e1fa-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="0e1fa-129">Salesforce CRM</span></span>|<span data-ttu-id="0e1fa-130">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="0e1fa-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="0e1fa-131">在 Salesforce CRM 中分配角色</span><span class="sxs-lookup"><span data-stu-id="0e1fa-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="0e1fa-132">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="0e1fa-132">Power Automate Flow Account</span></span>|<span data-ttu-id="0e1fa-133">使用数据库创建新的生产环境，以便进行测试、过渡和生产。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-133">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="0e1fa-134">如果你有一个具有数据库的现有生产环境，则可以重复使用它。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-134">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="0e1fa-135">要安装连接器解决方案的用户必须具有对此环境的电源自动执行许可和访问权限。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-135">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="0e1fa-136">如果安装失败，你可以监视进度并在 [电源自动执行](https://flow.microsoft.com/) 中获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-136">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="0e1fa-137">选择 "**解决方案**" 下的 "**查看历史记录**"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-137">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="0e1fa-138">创建或管理环境</span><span class="sxs-lookup"><span data-stu-id="0e1fa-138">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="0e1fa-139">为 Microsoft 自定义字段安装 Salesforce 包</span><span class="sxs-lookup"><span data-stu-id="0e1fa-139">Installation of Salesforce Package for Microsoft Custom Fields</span></span>

<span data-ttu-id="0e1fa-140">若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要清楚地识别特定于 Microsoft 的引用字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-140">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="0e1fa-141">此分界为合作伙伴卖方团队提供了决定他们要与 Microsoft 共享以共同销售的推荐的功能。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-141">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="0e1fa-142">在 Salesforce 中，激活 **注释** 并将其添加到机会相关列表。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-142">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> [<span data-ttu-id="0e1fa-143">引用</span><span class="sxs-lookup"><span data-stu-id="0e1fa-143">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. <span data-ttu-id="0e1fa-144">按照以下步骤激活 **机会团队** ：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-144">Activate **Opportunity teams** by following the steps:</span></span>
    - <span data-ttu-id="0e1fa-145">在安装程序中，使用 " **快速查找** " 框定位机会团队设置。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-145">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="0e1fa-146">根据需要定义设置。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-146">Define the settings as needed.</span></span> [<span data-ttu-id="0e1fa-147">引用</span><span class="sxs-lookup"><span data-stu-id="0e1fa-147">Reference</span></span>](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. <span data-ttu-id="0e1fa-148">在 Salesforce 中，使用 [包安装程序](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)安装自定义字段和对象。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-148">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="0e1fa-149">使用此安装程序将包安装到任何公司。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-149">Use this installer to install the package into any company.</span></span>

    >[!NOTE]
    ><span data-ttu-id="0e1fa-150">如果要安装到沙盒，则必须将 URL 的初始部分替换为 `http://test.salesforce.com` 。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-150">If you are installing into a sandbox, you must replace the initial portion of the URL with `http://test.salesforce.com`.</span></span>

1. <span data-ttu-id="0e1fa-151">在 Salesforce 中，将 Microsoft 解决方案添加到 **机会** 相关列表。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-151">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="0e1fa-152">添加后，选择 **扳手** 图标并更新属性</span><span class="sxs-lookup"><span data-stu-id="0e1fa-152">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="0e1fa-153">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="0e1fa-153">Best Practice: Test before you go live</span></span>

<span data-ttu-id="0e1fa-154">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-154">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="0e1fa-155">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-155">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="0e1fa-156">制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-156">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="0e1fa-157">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-157">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="0e1fa-158">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-158">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="0e1fa-159">为 Salesforce CRM 安装合作伙伴中心引用同步</span><span class="sxs-lookup"><span data-stu-id="0e1fa-159">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="0e1fa-160">请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-160">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="0e1fa-161">这会显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-161">This will show you the available CRM instances.</span></span>

1. <span data-ttu-id="0e1fa-162">从右上角的下拉列表中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-162">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="0e1fa-163">选择左侧导航栏上的 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-163">Select **Solutions** on the left navigation bar.</span></span>

1. <span data-ttu-id="0e1fa-164">在顶部菜单中选择 " **打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-164">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="打开 AppSource":::

1. <span data-ttu-id="0e1fa-166">在弹出屏幕中搜索 Salesforce 的 " **合作伙伴中心引用连接器** "。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-166">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="立即获取屏幕截图。":::

1. <span data-ttu-id="0e1fa-168">选择 " **立即获取** " 按钮，然后选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-168">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="0e1fa-169">在下一页中，选择 "Salesforce CRM 环境" 以安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-169">In the next page, select the Salesforce CRM environment to install the application.</span></span> <span data-ttu-id="0e1fa-170">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-170">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="0e1fa-171">然后，你将转到 " **管理你的解决方案** " 页。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-171">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="0e1fa-172">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-172">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="0e1fa-173">**计划的安装** 应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-173">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="0e1fa-174">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-174">Installation will take 10-15 minutes.</span></span>

1. <span data-ttu-id="0e1fa-175">安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，然后从左侧导航区域中选择 " **解决方案** "。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-175">After the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="0e1fa-176">请注意，在 "解决方案" 列表中现在提供了 **Salesforce 的合作伙伴中心引用同步** 。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-176">Notice that **Partner Center Referrals Synchronization for Salesforce** is now available in the Solutions list.</span></span>

1. <span data-ttu-id="0e1fa-177">**为 Salesforce 选择合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-177">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="0e1fa-178">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-178">The following Power Automate flows and entities are available:</span></span>

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce 流":::

## <a name="configure-the-solution"></a><span data-ttu-id="0e1fa-180">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="0e1fa-180">Configure the solution</span></span>

1. <span data-ttu-id="0e1fa-181">在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-181">After you've installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="0e1fa-182">在右上角的 " **环境** " 下拉部分中，选择在其中安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-182">From the **Environments** drop-down in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="0e1fa-183">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-183">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="0e1fa-184">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="0e1fa-184">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="0e1fa-185">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="0e1fa-185">Partner Center Events</span></span>
   - <span data-ttu-id="0e1fa-186">CRM 管理员，并在解决方案中自动执行流程</span><span class="sxs-lookup"><span data-stu-id="0e1fa-186">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="0e1fa-187">从左侧导航栏中选择 " **连接** "，然后从列表中选择 " **合作伙伴中心引用** " 解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-187">Select **Connections** from the left navigation bar, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="0e1fa-188">通过选择 " **创建连接**" 来创建连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-188">Create a connection by selecting **Create a connection**.</span></span>

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="显示 &quot;创建连接&quot; 的屏幕截图。":::

   1. <span data-ttu-id="0e1fa-190">在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-190">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="0e1fa-191">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-191">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="0e1fa-192">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-192">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   1. <span data-ttu-id="0e1fa-193">为 CRM 管理员用户创建 Salesforce 连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-193">Create a connection for Salesforce for the CRM administrator user.</span></span>
  
   1. <span data-ttu-id="0e1fa-194">为 CRM 管理员用户创建 Microsoft Dataverse 的连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-194">Create a connection for Microsoft Dataverse for the CRM administrator user.</span></span>

   1. <span data-ttu-id="0e1fa-195">添加所有连接后，你的环境中应会显示以下连接：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-195">After you've added all the Connections, you should see the following connections in your environment:</span></span>

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="显示连接的屏幕截图。":::

### <a name="edit-the-connections"></a><span data-ttu-id="0e1fa-197">编辑连接</span><span class="sxs-lookup"><span data-stu-id="0e1fa-197">Edit the connections</span></span>

1. <span data-ttu-id="0e1fa-198">返回 " **解决方案** " 页，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-198">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="0e1fa-199">通过单击 "**全部**" **(预览) 选择 "连接引用**"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-199">Select **Connection Reference (preview)** by clicking **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="显示编辑连接的屏幕截图。":::

1. <span data-ttu-id="0e1fa-201">通过选择省略号图标单独编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-201">Edit each of the Connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="0e1fa-202">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-202">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="显示如何编辑连接器的屏幕截图。":::

1. <span data-ttu-id="0e1fa-204">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-204">Turn on the flows in the following sequence:</span></span>
   - <span data-ttu-id="0e1fa-205">合作伙伴中心预览体验版 (Webhook 注册) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-205">Partner Center Webhook Registration (Insider Preview)</span></span>
   - <span data-ttu-id="0e1fa-206">[自定义]从 Salesforce 创建或获取详细信息</span><span class="sxs-lookup"><span data-stu-id="0e1fa-206">[Customize] Create or Get Details from Salesforce</span></span>
   - <span data-ttu-id="0e1fa-207">创建联合销售Referral-Salesforce预览合作伙伴中心 (预览) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-207">Create Co-sell Referral-Salesforce to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="0e1fa-208">合作伙伴中心 Microsoft 联合销售 Salesforce (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-208">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>  
   - <span data-ttu-id="0e1fa-209">合作伙伴中心 Insider Preview (Salesforce) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-209">Partner Center to Salesforce (Insider Preview)</span></span>
   - <span data-ttu-id="0e1fa-210">Salesforce 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-210">Salesforce to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="0e1fa-211">Salesforce 预览体验合作伙伴中心 (预览版) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-211">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="0e1fa-212">Salesforce Microsoft Solutions to 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="0e1fa-212">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="0e1fa-213">使用 Webhook API 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="0e1fa-213">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="0e1fa-214">可以使用 webhook 合作伙伴中心注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-214">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="0e1fa-215">这些更改事件作为 HTTP 帖子发送到 URL。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-215">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="0e1fa-216">选择 **合作伙伴中心预览体验成员预览 (Salesforce CRM) "**。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-216">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

1. <span data-ttu-id="0e1fa-217">选择"**编辑"图标**，**然后选择"收到 HTTP 请求时"。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-217">Select the **Edit icon** and select **When an HTTP request is received**.</span></span>

1. <span data-ttu-id="0e1fa-218">选择" **复制** "图标以复制提供的 **HTTP POST URL**。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-218">Select the **Copy** icon to copy the provided **HTTP POST URL**.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="显示如何复制 URL 的屏幕截图。":::

1. <span data-ttu-id="0e1fa-220">选择 **"合作伙伴中心预览 (预览版) Power Automate Webhook** 注册"，然后选择"运行 **"。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-220">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="0e1fa-221">确保在右 **窗格中打开"运行** 流"窗口，然后选择"继续 **"。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-221">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="0e1fa-222">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-222">Enter the following details:</span></span>

   - <span data-ttu-id="0e1fa-223">**Http 触发器终结点**：此 URL 是从前面步骤复制的。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-223">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="0e1fa-224">**要注册的事件**：选择所有可用事件 (引用 **创建**、引荐更新、**相关** 引荐创建以及相关引荐 **更新**) 。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-224">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="0e1fa-225">**覆盖现有的触发器终结点（如果存在）？：** 是。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-225">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="0e1fa-226">只能为给定的 Webhook 事件注册一个 URL。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-226">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="0e1fa-227">选择 **"运行流**"，然后选择"**完成"。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-227">Select **Run flow**, and then select **Done**.</span></span>

<span data-ttu-id="0e1fa-228">Webhook 现在可以侦听、创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-228">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="0e1fa-229">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="0e1fa-229">Customize synchronization steps</span></span>

<span data-ttu-id="0e1fa-230">CRM 系统是高度自定义的，你可以根据 CRM Power Automate自定义自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-230">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="0e1fa-231">当联合销售引荐在 合作伙伴中心 和 CRM 系统之间同步时，合作伙伴中心 电脑上同步的字段将列在自定义 [字段映射指南 中](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-231">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="0e1fa-232">按照字段映射指南操作，如有必要，在 **[自定义]** 从 Salesforce 或环境变量创建或获取详细信息中做出适当的更改。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-232">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Salesforce** or environment variables.</span></span> <span data-ttu-id="0e1fa-233">请勿更新解决方案中任何其他Power Automate流，因为它可能会影响将来的解决方案升级。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-233">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="0e1fa-234">以下自定义项可用：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-234">The following customizations are available:</span></span>

- <span data-ttu-id="0e1fa-235">**在机会名称中** 显示选中标记：默认情况下，机会名称旁边会显示一个选中标记，指示 合作伙伴中心 与 Salesforce CRM 之间的同步已成功进行。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-235">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Salesforce CRM is happening successfully.</span></span> <span data-ttu-id="0e1fa-236">同样，如果同步失败，将显示交叉标记。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-236">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="0e1fa-237">若要避免在机会名称中添加选中或交叉标记，请在机会名称环境变量中将"显示选中标记 **"的当前值** 设置为"否"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-237">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>

- <span data-ttu-id="0e1fa-238">**阶段名称**：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-238">**Stage name**:</span></span>

  - <span data-ttu-id="0e1fa-239">**活动阶段名称**：这是 Salesforce 中商机销售管道中的阶段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-239">**Active stage name**: This is the stage in an opportunity's sales pipeline in Salesforce.</span></span>  <span data-ttu-id="0e1fa-240">它表示活动阶段，等效于在活动状态中处于接受合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-240">It represents an active stage and is equivalent to a referral in accepted state in Partner Center.</span></span> <span data-ttu-id="0e1fa-241">这可以是保留阶段后销售管道的下一阶段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-241">This can be the next stage in the sales pipeline after the on-hold stage.</span></span> <span data-ttu-id="0e1fa-242">将机会的销售阶段从"保留"阶段移动到"活动"阶段将接受合作伙伴中心更改将开始同步。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-242">Moving Opportunity's sales stage out of the on-hold stage into active stage will accept the referral in Partner Center and changes will start synchronizing.</span></span>

  - <span data-ttu-id="0e1fa-243">**保留阶段名称**：Salesforce 中商机销售管道中的阶段名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-243">**On-hold stage name**: Name of the stage in an opportunity's sales pipeline in Salesforce.</span></span> <span data-ttu-id="0e1fa-244">它表示保留阶段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-244">It represents an on-hold stage.</span></span> <span data-ttu-id="0e1fa-245">尚未接受的 Microsoft 共享的新联合销售引荐将在 Salesforce 中设置为此阶段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-245">New co-sell referrals shared from Microsoft that are not yet accepted will be set to this stage in Salesforce.</span></span> <span data-ttu-id="0e1fa-246">在机会处于保留阶段时对机会进行的任何更改将不会同步到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-246">Any changes made in an opportunity while it is on-hold stage will not synchronize to Partner Center.</span></span> <span data-ttu-id="0e1fa-247">将机会的销售阶段从此保留阶段移开将接受 合作伙伴中心 中的引荐，更改将开始同步。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-247">Moving Opportunity's sales stage out of this on-hold stage will accept the referral in Partner Center and changes will start synchronizing.</span></span>

- <span data-ttu-id="0e1fa-248">**客户帐户国家**/地区代码：创建新引荐时，必须提供两个字母 (ISO 3166) 国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-248">**Customer Account Country Code**: It is mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="0e1fa-249">默认情况下，国家/地区代码将同步到 Salesforce 中帐户的 **BillingCountry 字段** ，</span><span class="sxs-lookup"><span data-stu-id="0e1fa-249">By default, the country code will be synced to and from the account's **BillingCountry** field in Salesforce.</span></span> <span data-ttu-id="0e1fa-250">如果 Salesforce 中有不同的字段，用于同步国家/地区代码：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-250">If you have a different field in Salesforce for the country code to sync from:</span></span>

  - <span data-ttu-id="0e1fa-251">对于帐户中包含双字母代码的非列表国家/地区代码字段：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-251">For a nonlookup country code field in the account that contains a two-letter code:</span></span>

    - <span data-ttu-id="0e1fa-252">使用 CRM **的字段** 名称更新 Salesforce 环境变量中的"客户帐户国家/地区代码"字段名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-252">Update the **Customer Account Country Code** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="0e1fa-253">请确保提供字段的名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-253">Make sure that you provide the field's name, not its display name.</span></span>

    - <span data-ttu-id="0e1fa-254">编辑 **[自定义] 从 Salesforce** 创建或获取详细信息，然后转到在 **CRM** 操作中创建或获取客户帐户，以将国家/地区值分配给 CRM 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-254">Edit **[Customize] Create or Get Details from Salesforce**, and go to **Create or get customer account in CRM** action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="0e1fa-255">此外，从 **BillingCountry** 中删除 Country 值分配。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-255">Also, remove the **Country** value assignment from the **BillingCountry**.</span></span>

  - <span data-ttu-id="0e1fa-256">对于帐户中基于查找的国家/地区代码字段：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-256">For a lookup-based country code field in the account:</span></span>

    - <span data-ttu-id="0e1fa-257">在帐户中添加新的自定义字段，并使用两个字母的国家/地区代码 (ISO 3166) 基于基于查找的字段中选择的值自动填充该字段，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-257">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>

    - <span data-ttu-id="0e1fa-258">按照 nonlookup 国家/地区代码字段的上述步骤，将新的自定义字段从 CRM 同步到和从 合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-258">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="0e1fa-259">**交易值**：默认情况下，来自 合作伙伴中心的交易值将同步到 CRM 中的 Amount 和 **Amount。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-259">**Deal value**: By default, the deal value from Partner Center will be synchronized to and from **Amount** in the CRM.</span></span> <span data-ttu-id="0e1fa-260">如果 CRM 中有不同的字段，用于从以下位置同步交易值：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-260">If you have a different field in the CRM for the deal value to synchronize from:</span></span>

  - <span data-ttu-id="0e1fa-261">使用 CRM **的字段** 名称更新 Salesforce 环境变量中的"交易值"字段名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-261">Update the **Deal value** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="0e1fa-262">请确保提供字段的名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-262">Make sure that you provide the field's name, not its display name.</span></span>

  - <span data-ttu-id="0e1fa-263">编辑 **[自定义]** 从 Salesforce 创建或获取详细信息，转到在 CRM 中创建或更新机会，并更新"创建新机会"和"更新现有机会"操作，将 **DealValue** 分配给 Salesforce 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-263">Edit **[Customize] Create or Get Details from Salesforce** and go to **Create or update opportunity** in CRM and update both **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** to the correct field in Salesforce.</span></span>

- <span data-ttu-id="0e1fa-264">**交易值货币代码**：Salesforce 中交易值货币代码字段的名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-264">**Deal value currency code**: Name of the deal value currency code field in Salesforce.</span></span> <span data-ttu-id="0e1fa-265">在 Microsoft 合作伙伴中心 中创建或更新引荐时，此字段 API 名称将用于获取机会的交易值货币合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-265">This field API name will be used to get Opportunity's deal value currency code when creating or updating referral in Microsoft Partner Center.</span></span> <span data-ttu-id="0e1fa-266">如果交易值货币代码字段不同于默认字段 **CurrencyIsoCode，** 请更新此环境变量的当前值。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-266">If deal value currency code field is different than default field **CurrencyIsoCode**, update the current value of this environment variable.</span></span>

  - <span data-ttu-id="0e1fa-267">使用 CRM **的字段名称** 更新 Salesforce 环境变量中的"交易值货币"字段名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-267">Update the **Deal value currency** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="0e1fa-268">请确保提供字段的名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-268">Make sure that you provide the field's name, not its display name.</span></span>

  - <span data-ttu-id="0e1fa-269">编辑 **[自定义]** 从 Salesforce 创建或获取详细信息，转到在 CRM 中创建或更新机会，并更新"创建新机会"和"更新现有机会"操作，以将 **DealValueCurrency** 分配到 Salesforce 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-269">Edit **[Customize] Create or Get Details from Salesforce** and go to **Create or update opportunity** in CRM and update both **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValueCurrency** to the correct field in Salesforce.</span></span>

- <span data-ttu-id="0e1fa-270">**同步联合销售机会**：如果设置为 **"是**"，则只有联合销售机会和管道共享机会合作伙伴中心 Salesforce。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-270">**Sync Co-sell opportunity**: If set to **yes**, only co-sell and pipeline sharing opportunities will be synchronized from Partner Center to Salesforce.</span></span> <span data-ttu-id="0e1fa-271">如果设置为 **"否"，** 则潜在顾客、联合销售和管道共享机会将合作伙伴中心 Salesforce。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-271">If set to **no**, leads, co-sell, and pipeline sharing opportunities will be synchronized from Partner Center to Salesforce.</span></span> <span data-ttu-id="0e1fa-272">此变量对从 Salesforce 同步到销售合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-272">This variable does not have any impact on the opportunities synchronized from Salesforce to Partner Center.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="0e1fa-273">更新环境变量</span><span class="sxs-lookup"><span data-stu-id="0e1fa-273">Update environment variable</span></span>

<span data-ttu-id="0e1fa-274">更新环境变量值：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-274">To update an environment variable value:</span></span>

1. <span data-ttu-id="0e1fa-275">转到"解决方案 **"页**，然后选择"**默认解决方案"。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-275">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="0e1fa-276">选择 **"所有"，** 选择"环境 **变量"。**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-276">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="0e1fa-277">为需要更新的值选择环境变量，然后使用省略号图标选择"编辑"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-277">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="0e1fa-278">更新 **当前 (** 不通过使用"新建值") 提供值来更新默认值值。 </span><span class="sxs-lookup"><span data-stu-id="0e1fa-278">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="0e1fa-279">值必须与变量的数据类型匹配。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-279">The value must match the data type of the variable.</span></span> <span data-ttu-id="0e1fa-280">例如，"是"或"否"数据类型将接受"是"或"否"值。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-280">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="显示&quot;更新环境变量&quot;的屏幕截图。":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="0e1fa-282">端到端双向联合销售引荐同步</span><span class="sxs-lookup"><span data-stu-id="0e1fa-282">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="0e1fa-283">安装、配置和自定义 Power Automate解决方案后，可以测试 Salesforce CRM 与 合作伙伴中心 之间的联合销售引荐同步。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-283">After you've installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="0e1fa-284">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e1fa-284">Pre-requisites</span></span>

<span data-ttu-id="0e1fa-285">若要跨 合作伙伴中心 Salesforce CRM 同步引荐，Power Automate解决方案需要明确划分特定于 Microsoft 的引荐字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-285">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="0e1fa-286">此标识使卖方团队能够决定要与 Microsoft 共享哪些引荐进行联合销售。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-286">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="0e1fa-287">一组自定义字段作为 Salesforce CRM 解决方案机会实体合作伙伴中心引荐同步的 **一** 部分提供。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-287">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="0e1fa-288">CRM 管理员用户需要创建包含"机会"自定义字段 **的单独** CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-288">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="0e1fa-289">以下自定义字段应是 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-289">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="0e1fa-290">**与 合作伙伴中心** 同步：是否将商机与合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-290">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="0e1fa-291">默认情况下，此字段的值为"否"，需要由卖方显式设置为"是"，以与 Microsoft 共享机会。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-291">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="0e1fa-292">从 合作伙伴中心 CRM 共享的新引荐将此字段值设置为"是"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-292">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="0e1fa-293">**引荐** 标识符：Microsoft 引用的只读合作伙伴中心字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-293">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral.</span></span>

- <span data-ttu-id="0e1fa-294">**引荐** 链接：指向 Microsoft 合作伙伴中心 中的引荐的只读合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-294">**Referral Link**: A read-only link to the referral in Microsoft Partner Center.</span></span>

- <span data-ttu-id="0e1fa-295">**Microsoft 如何提供帮助**：需要 Microsoft 提供引荐的帮助。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-295">**How can Microsoft help**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="0e1fa-296">若要创建联合销售引荐，请选择 Microsoft 所需的相应帮助。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-296">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="0e1fa-297">客户联系人必须与创建联合销售引荐的机会相关联。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-297">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="0e1fa-298">若要创建非联合销售引荐，请勿选择此字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-298">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="0e1fa-299">通过选择相应的"需要帮助"选项，可以随时将非联合销售引荐转换为联合销售引荐。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-299">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>

- <span data-ttu-id="0e1fa-300">**Microsoft 合作伙伴中心引荐可见性**：选择该引荐合作伙伴中心可见性。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-300">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="0e1fa-301">通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-301">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="0e1fa-302">如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会显示该引用。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-302">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="0e1fa-303">将此字段标记为可见后，将无法还原它。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-303">After this field is marked as visible, it can't be reverted.</span></span>

- <span data-ttu-id="0e1fa-304">**MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-304">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>

- <span data-ttu-id="0e1fa-305">**Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-305">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="0e1fa-306">可以在商机中添加或删除一个或多个解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-306">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="0e1fa-307">在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-307">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="0e1fa-308">若要将此对象与商机关联，请在 CRM 中更新 **商机** 窗体。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-308">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

- <span data-ttu-id="0e1fa-309">**Audit**：与合作伙伴中心引用同步的只读审核记录</span><span class="sxs-lookup"><span data-stu-id="0e1fa-309">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="0e1fa-310">各种</span><span class="sxs-lookup"><span data-stu-id="0e1fa-310">SCENARIOS</span></span>

1. <span data-ttu-id="0e1fa-311">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-311">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="0e1fa-312">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-312">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="0e1fa-313">请确保在 Salesforce CRM 环境中创建 **新机会** 时， **Microsoft 合作伙伴中心** 出现在此部分。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-313">Ensure that the section, **Microsoft Partner Center** is present when you create a **New Opportunity** in Salesforce CRM environment.</span></span>

   1. <span data-ttu-id="0e1fa-314">与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔ icon in Salesforce CRM.</span></span>
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce 环境的屏幕截图。":::

   1. <span data-ttu-id="0e1fa-316">若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-316">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="0e1fa-317">**Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-317">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="显示如何在卡片视图中获取相应字段的屏幕截图。":::

      - <span data-ttu-id="0e1fa-319">**与合作伙伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="0e1fa-319">**Sync with Partner Center**: Yes</span></span>
      - <span data-ttu-id="0e1fa-320">**客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-320">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="0e1fa-321">**Microsoft 解决方案**：若要与 microsoft 共享引用，请向此机会添加有效的合作销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-321">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>

   1. <span data-ttu-id="0e1fa-322">将 "机会 **与合作伙伴中心同步** " 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-322">After you have set the opportunity **Sync with Partner Center** option to **Yes**, wait for 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="0e1fa-323">你的参考将与 Salesforce CRM 同步，并将填充引用链接。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-323">Your referrals will be synchronized with Salesforce CRM, and Referral Link will get populated.</span></span> <span data-ttu-id="0e1fa-324">如果出现故障，则将使用错误信息填充审核字段。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-324">If there's a failure, the Audit field will be populated with error information.</span></span>

   1. <span data-ttu-id="0e1fa-325">同样，在 " **与合作伙伴中心同步** " 选项设置为 **"是"** 时，如果你更新了 Salesforce CRM 中的机会，则所做的更改将与你的合作伙伴中心帐户同步。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-325">Similarly, when the **Sync with Partner Center** option is set to **Yes**, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

2. <span data-ttu-id="0e1fa-326">引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：</span><span class="sxs-lookup"><span data-stu-id="0e1fa-326">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="0e1fa-327">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-327">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    1. <span data-ttu-id="0e1fa-328">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-328">Select **Referrals** from the left-hand menu.</span></span>

    1. <span data-ttu-id="0e1fa-329">单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-329">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    1. <span data-ttu-id="0e1fa-330">登录到 Salesforce CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-330">Sign into your Salesforce CRM environment.</span></span>

    1. <span data-ttu-id="0e1fa-331">导航到 " **开放式机会**"。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-331">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="0e1fa-332">Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-332">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    1. <span data-ttu-id="0e1fa-333">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-333">When you select a synchronized referral, the card view details are populated.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce 机会页的屏幕截图。":::

>[!NOTE]
><span data-ttu-id="0e1fa-335">**需要有关部署的帮助？**</span><span class="sxs-lookup"><span data-stu-id="0e1fa-335">**Need help with deployment?**</span></span>
><span data-ttu-id="0e1fa-336">若要获得有关共同销售引用连接器部署的帮助，可以参与合作伙伴技术顾问。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-336">For assistance with your Co-sell referral connector deployment, you can engage a Partner Technical Consultant.</span></span> <span data-ttu-id="0e1fa-337">他们可以为成功实现提供部署帮助和最佳实践。</span><span class="sxs-lookup"><span data-stu-id="0e1fa-337">They can provide deployment assistance and best practices for a successful implementation.</span></span>
>
><span data-ttu-id="0e1fa-338">有关详细信息，请参阅 [如何提交技术预售和部署服务请求](technical-benefits.md)</span><span class="sxs-lookup"><span data-stu-id="0e1fa-338">For more information, see [How to Submit a technical presales and deployment services request](technical-benefits.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="0e1fa-339">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0e1fa-339">Next steps</span></span>

- [<span data-ttu-id="0e1fa-340">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="0e1fa-340">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="0e1fa-341">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="0e1fa-341">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="0e1fa-342">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="0e1fa-342">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
