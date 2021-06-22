---
title: Dynamics 365 CRM 联合销售合作伙伴中心
description: 将 合作伙伴中心中的引荐与 Dynamics 365 CRM 联合销售连接器同步。 然后，可以从 CRM 系统内部与 Microsoft 联合销售。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425044"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a><span data-ttu-id="29b50-104">Dynamics 365 CRM 联合销售连接器概述</span><span class="sxs-lookup"><span data-stu-id="29b50-104">Co-sell connector for Dynamics 365 CRM overview</span></span>

<span data-ttu-id="29b50-105">**适当的角色**：引荐管理员|CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="29b50-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="29b50-106">合作伙伴中心联合销售连接器可让销售人员在 CRM 系统中与 Microsoft 联合销售。</span><span class="sxs-lookup"><span data-stu-id="29b50-106">Partner Center co-sell connectors enable your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="29b50-107">他们不需要经过训练，就可使用合作伙伴中心联合销售交易。</span><span class="sxs-lookup"><span data-stu-id="29b50-107">They won't have to be trained to use Partner Center to manage co-sell deals.</span></span> <span data-ttu-id="29b50-108">使用联合销售连接器创建新的联合销售引荐，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引荐、接受或拒绝引荐，以及修改交易数据（例如交易值和结束日期）。</span><span class="sxs-lookup"><span data-stu-id="29b50-108">Use the co-sell connectors to create a new co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept or decline referrals, and modify deal data such as deal value and closing date.</span></span> <span data-ttu-id="29b50-109">还可以从 Microsoft 卖方处收到有关这些联合销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="29b50-109">You can also receive any updates from the Microsoft sellers on these co-sell deals.</span></span> <span data-ttu-id="29b50-110">可以在你选择的 CRM 中管理所有引荐工作，而不是在 合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="29b50-110">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="29b50-111">该解决方案基于 Power Automate，并使用合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="29b50-111">The solution is based on Power Automate and uses Partner Center APIs.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b50-112">先决条件</span><span class="sxs-lookup"><span data-stu-id="29b50-112">Prerequisites</span></span>

<span data-ttu-id="29b50-113">在安装解决方案之前，请确保满足以下先决条件。</span><span class="sxs-lookup"><span data-stu-id="29b50-113">Before you install the solution, make sure to meet the following prerequisites.</span></span>

|<span data-ttu-id="29b50-114">**主题**</span><span class="sxs-lookup"><span data-stu-id="29b50-114">**Topics**</span></span>   |<span data-ttu-id="29b50-115">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="29b50-115">**Details**</span></span>   |<span data-ttu-id="29b50-116">**链接**</span><span class="sxs-lookup"><span data-stu-id="29b50-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="29b50-117">Microsoft 合作伙伴网络 (MPN) ID</span><span class="sxs-lookup"><span data-stu-id="29b50-117">Microsoft Partner Network (MPN) ID</span></span> |<span data-ttu-id="29b50-118">需要有效的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="29b50-118">You need a valid MPN ID.</span></span>|[<span data-ttu-id="29b50-119">加入合作伙伴网络</span><span class="sxs-lookup"><span data-stu-id="29b50-119">Join the Partner Network</span></span>](https://partner.microsoft.com/)|
|<span data-ttu-id="29b50-120">已做好联合销售准备</span><span class="sxs-lookup"><span data-stu-id="29b50-120">Co-sell ready</span></span>|<span data-ttu-id="29b50-121">IP/服务解决方案必须可供联合销售。</span><span class="sxs-lookup"><span data-stu-id="29b50-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="29b50-122">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="29b50-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="29b50-123">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="29b50-123">Partner Center account</span></span>|<span data-ttu-id="29b50-124">与联合销售合作伙伴中心关联的 MPN ID 必须与与联合销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="29b50-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your co-sell solution.</span></span> <span data-ttu-id="29b50-125">在部署连接器之前，请验证能否在 合作伙伴中心 门户中查看联合销售引荐。</span><span class="sxs-lookup"><span data-stu-id="29b50-125">Verify that you can see your co-sell referrals in the Partner Center portal before you deploy the connectors.</span></span>|[<span data-ttu-id="29b50-126">管理帐户</span><span class="sxs-lookup"><span data-stu-id="29b50-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="29b50-127">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="29b50-127">Partner Center user roles</span></span>|<span data-ttu-id="29b50-128">将安装和使用连接器的员工必须是引荐管理员。</span><span class="sxs-lookup"><span data-stu-id="29b50-128">The employee who will install and use the connectors must be a Referrals admin.</span></span>|[<span data-ttu-id="29b50-129">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="29b50-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="29b50-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="29b50-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="29b50-131">CRM 用户角色是"系统管理员"或"系统定制员"。</span><span class="sxs-lookup"><span data-stu-id="29b50-131">The CRM user role is System admin or System customizer.</span></span>|[<span data-ttu-id="29b50-132">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="29b50-132">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="29b50-133">Power Automate流帐户</span><span class="sxs-lookup"><span data-stu-id="29b50-133">Power Automate flow account</span></span>|<span data-ttu-id="29b50-134">使用数据库创建新的生产环境，用于测试、暂存和生产。</span><span class="sxs-lookup"><span data-stu-id="29b50-134">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="29b50-135">如果有包含数据库的现有生产环境，可以重复使用它。</span><span class="sxs-lookup"><span data-stu-id="29b50-135">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="29b50-136">要安装连接器解决方案的用户必须具有此Power Automate和访问权限。</span><span class="sxs-lookup"><span data-stu-id="29b50-136">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="29b50-137">如果安装失败，可以监视进度 [，Power Automate](https://flow.microsoft.com/) 获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="29b50-137">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="29b50-138">在"**解决方案"下选择"** 查看 **历史记录"。**</span><span class="sxs-lookup"><span data-stu-id="29b50-138">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="29b50-139">创建或管理环境</span><span class="sxs-lookup"><span data-stu-id="29b50-139">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="29b50-140">安装合作伙伴中心 Dynamics 365 (Power Automate解决方案) </span><span class="sxs-lookup"><span data-stu-id="29b50-140">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate solution)</span></span>

1. <span data-ttu-id="29b50-141">转到[Power Automate"，](https://flow.microsoft.com)然后选择右上角的"环境"。</span><span class="sxs-lookup"><span data-stu-id="29b50-141">Go to [Power Automate](https://flow.microsoft.com), and select **Environments** in the upper-right corner.</span></span> <span data-ttu-id="29b50-142">此步骤将显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="29b50-142">This step will show you the available CRM instances.</span></span>

1. <span data-ttu-id="29b50-143">从右上角的下拉列表中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="29b50-143">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="29b50-144">选择 **左侧** 的"解决方案"。</span><span class="sxs-lookup"><span data-stu-id="29b50-144">Select **Solutions** on the left.</span></span>

1. <span data-ttu-id="29b50-145">选择顶部 **菜单上的"打开 AppSource"** 链接。</span><span class="sxs-lookup"><span data-stu-id="29b50-145">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="显示 Open AppSource 的屏幕截图。":::

1. <span data-ttu-id="29b50-147">在合作伙伴中心屏幕中搜索 **Dynamics 365** 的推荐连接器。</span><span class="sxs-lookup"><span data-stu-id="29b50-147">Search for **Partner Center Referrals Connectors for Dynamics 365** in the pop-up screen.</span></span>  

1. <span data-ttu-id="29b50-148">选择"**现在获取"** 按钮，然后选择"继续 **"。**</span><span class="sxs-lookup"><span data-stu-id="29b50-148">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="29b50-149">将出现一个页面，可在其中选择 DYNAMICs 365 (环境) CRM 应用程序。</span><span class="sxs-lookup"><span data-stu-id="29b50-149">A page appears where you can select the CRM (Dynamics 365) environment to install the application.</span></span> <span data-ttu-id="29b50-150">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="29b50-150">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="29b50-151">可以监视进度，如果安装失败，可以通过选择"解决方案"下的"查看历史记录Power Automate **获取详细信息\*\*\*\*。**</span><span class="sxs-lookup"><span data-stu-id="29b50-151">You can monitor the progress and, if the installation fails, you can get more details in Power Automate by selecting **See history** under **Solutions**.</span></span>

1. <span data-ttu-id="29b50-152">安装完成后，返回到"Power Automate [并选择左侧](https://flow.microsoft.com)**的"** 解决方案"。</span><span class="sxs-lookup"><span data-stu-id="29b50-152">After the installation is complete, go back to [Power Automate](https://flow.microsoft.com) and select **Solutions** on the left.</span></span> <span data-ttu-id="29b50-153">合作伙伴中心解决方案列表中现提供 **Dynamics 365** 的推荐 **同步**。</span><span class="sxs-lookup"><span data-stu-id="29b50-153">**Partner Center Referrals Synchronization for Dynamics 365** is now available in the **Solutions** list.</span></span>

1. <span data-ttu-id="29b50-154">选择 **合作伙伴中心 Dynamics 365 的推荐同步"**。</span><span class="sxs-lookup"><span data-stu-id="29b50-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="29b50-155">以下Power Automate流和实体可用。</span><span class="sxs-lookup"><span data-stu-id="29b50-155">The following Power Automate flows and entities are available.</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="显示可用 CCR 的屏幕截图。":::

## <a name="test-before-you-go-live"></a><span data-ttu-id="29b50-157">上台前进行测试</span><span class="sxs-lookup"><span data-stu-id="29b50-157">Test before you go live</span></span>

<span data-ttu-id="29b50-158">在生产环境中安装、配置Power Automate自定义解决方案之前，请务必在过渡 CRM 实例上测试该解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span> <span data-ttu-id="29b50-159">你将需要：</span><span class="sxs-lookup"><span data-stu-id="29b50-159">You'll need to:</span></span>

- <span data-ttu-id="29b50-160">在Power Automate CRM 实例上安装 Power Automate 解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-160">Install the Power Automate solution on a staging environment CRM instance.</span></span>
- <span data-ttu-id="29b50-161">在过渡Power Automate配置和自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-161">Configure and customize the Power Automate solution in a staging environment.</span></span>
- <span data-ttu-id="29b50-162">在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-162">Test the solution on a staging CRM instance.</span></span>
- <span data-ttu-id="29b50-163">成功测试后，作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="29b50-163">After a successful test, import as a managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="29b50-164">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="29b50-164">Configure the solution</span></span>

1. <span data-ttu-id="29b50-165">在 CRM 实例中安装解决方案后，返回到[Power Automate。](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="29b50-165">After you've installed the solution in your CRM instance, go back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="29b50-166">从 **右上角** 的"环境"下拉列表中，选择安装了 Power Automate 解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="29b50-166">From the **Environments** drop-down list in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="29b50-167">需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="29b50-167">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="29b50-168">合作伙伴中心引荐管理员凭据的用户</span><span class="sxs-lookup"><span data-stu-id="29b50-168">Partner Center user with Referrals admin credentials</span></span>
   - <span data-ttu-id="29b50-169">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="29b50-169">Partner Center Events</span></span>
   - <span data-ttu-id="29b50-170">具有解决方案中Power Automate流的 CRM 管理员</span><span class="sxs-lookup"><span data-stu-id="29b50-170">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="29b50-171">选择 **左侧** 的"连接"，然后从 **合作伙伴中心选择"** 引荐"解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-171">Select **Connections** on the left, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="29b50-172">通过选择"创建连接 **"创建连接**。</span><span class="sxs-lookup"><span data-stu-id="29b50-172">Create a connection by selecting **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="显示&quot;创建连接&quot;的屏幕截图。":::

   1. <span data-ttu-id="29b50-174">在 **合作伙伴中心的 (搜索)** 搜索栏中，搜索"引荐"和"预览版"。</span><span class="sxs-lookup"><span data-stu-id="29b50-174">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="29b50-175">使用引荐管理员合作伙伴中心为用户创建连接。</span><span class="sxs-lookup"><span data-stu-id="29b50-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="29b50-176">接下来，使用合作伙伴中心管理员凭据为合作伙伴中心用户创建一个事件连接。</span><span class="sxs-lookup"><span data-stu-id="29b50-176">Next, create a Partner Center Events connection for your Partner Center user with the Referrals admin credentials.</span></span>

   1. <span data-ttu-id="29b50-177">为 CRM 管理员用户 (Common Data Service) 环境创建连接。</span><span class="sxs-lookup"><span data-stu-id="29b50-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
   1. <span data-ttu-id="29b50-178">添加所有连接后，应在环境中看到以下连接。</span><span class="sxs-lookup"><span data-stu-id="29b50-178">After you've added all the connections, you should see the following connections in your environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="显示连接的屏幕截图。":::

## <a name="edit-the-connections"></a><span data-ttu-id="29b50-180">编辑连接</span><span class="sxs-lookup"><span data-stu-id="29b50-180">Edit the connections</span></span>

1. <span data-ttu-id="29b50-181">返回到"解决方案 **"页**，然后选择"**默认解决方案"。**</span><span class="sxs-lookup"><span data-stu-id="29b50-181">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="29b50-182">通过 **选择" (") "，** 选择"连接引用"和"预览 **"。**</span><span class="sxs-lookup"><span data-stu-id="29b50-182">Select **Connection Reference (preview)** by selecting **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="显示&quot;编辑连接&quot;的屏幕截图。":::

1. <span data-ttu-id="29b50-184">通过选择省略号图标单独编辑每个连接。</span><span class="sxs-lookup"><span data-stu-id="29b50-184">Edit each of the connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="29b50-185">添加相关连接。</span><span class="sxs-lookup"><span data-stu-id="29b50-185">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="显示列出的连接的屏幕截图。":::

1. <span data-ttu-id="29b50-187">返回到" **解决方案"** 页，选择 **"合作伙伴中心 Dynamics 365** 的引荐同步"，然后按以下顺序选择每个流旁边的省略号图标来打开流。</span><span class="sxs-lookup"><span data-stu-id="29b50-187">Return to the **Solutions** page, select **Partner Center Referrals Synchronization for Dynamics 365**, and turn on the flow by selecting the ellipsis icon next to each flow in the following sequence.</span></span> <span data-ttu-id="29b50-188">如果在打开流时遇到任何问题，请参阅自定义 [步骤](connector-dynamics.md#customize-synchronization-steps) 和 [故障排除步骤](connectors-troubleshoot.md)。</span><span class="sxs-lookup"><span data-stu-id="29b50-188">If you encounter any issues while you turn on the flow, see [Customization steps](connector-dynamics.md#customize-synchronization-steps) and [Troubleshooting steps](connectors-troubleshoot.md).</span></span>

<span data-ttu-id="29b50-189">按以下顺序打开流：</span><span class="sxs-lookup"><span data-stu-id="29b50-189">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="29b50-190">合作伙伴中心预览体验版 (Webhook 注册) </span><span class="sxs-lookup"><span data-stu-id="29b50-190">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="29b50-191">创建联合销售引荐 - Dynamics 365 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="29b50-191">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="29b50-192">[自定义]从 Dynamics 365 流创建或获取详细信息</span><span class="sxs-lookup"><span data-stu-id="29b50-192">[Customize] Create or Get Details from Dynamics 365 flow</span></span>
- <span data-ttu-id="29b50-193">合作伙伴中心 Dynamics 365 - Helper (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="29b50-193">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="29b50-194">合作伙伴中心 Microsoft 联合销售 Dynamics 365 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="29b50-194">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="29b50-195">合作伙伴中心 Dynamics 365 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="29b50-195">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="29b50-196">Dynamics 365 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="29b50-196">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="29b50-197">Dynamics 365 预览体验合作伙伴中心 (预览版) </span><span class="sxs-lookup"><span data-stu-id="29b50-197">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="29b50-198">Dynamics 365 Microsoft Solutions to 合作伙伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="29b50-198">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="29b50-199">使用 Webhook API 注册资源更改事件</span><span class="sxs-lookup"><span data-stu-id="29b50-199">Use webhook APIs to register for resource change events</span></span>

<span data-ttu-id="29b50-200">可以使用 webhook 合作伙伴中心注册资源更改事件。</span><span class="sxs-lookup"><span data-stu-id="29b50-200">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="29b50-201">这些更改事件以 HTTP post 的形式发送到你的 URL。</span><span class="sxs-lookup"><span data-stu-id="29b50-201">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="29b50-202">选择 " **合作伙伴中心到 Dynamics 365 (预览体验预览")**。</span><span class="sxs-lookup"><span data-stu-id="29b50-202">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

1. <span data-ttu-id="29b50-203">选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。</span><span class="sxs-lookup"><span data-stu-id="29b50-203">Select the **Edit** icon, and select **When a HTTP request is received**.</span></span>

1. <span data-ttu-id="29b50-204">选择 **复制** 图标以复制提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="29b50-204">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/webhook-video.gif" alt-text="屏幕截图，显示如何使用 webhook 来注册资源更改。":::

1. <span data-ttu-id="29b50-206">选择 " **合作伙伴中心 Webhook 注册 (内幕预览版")** "Power 自动流"，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="29b50-206">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="29b50-207">确保在右窗格中打开 " **运行流** " 窗口，并选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="29b50-207">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="29b50-208">输入以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="29b50-208">Enter the following details:</span></span>

   - <span data-ttu-id="29b50-209">**Http 触发器终结点**：此 URL 已从前面的步骤中复制。</span><span class="sxs-lookup"><span data-stu-id="29b50-209">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="29b50-210">**要注册的事件**：选择所有可用事件 (**引用创建** 的、 **引用更新**、 **相关的** 引用-已创建的、与引用 **相关** 的) 。</span><span class="sxs-lookup"><span data-stu-id="29b50-210">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="29b50-211">**是否覆盖现有触发器终结点（如果存在**）：是。</span><span class="sxs-lookup"><span data-stu-id="29b50-211">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="29b50-212">对于给定的 webhook 事件，只能注册一个 URL。</span><span class="sxs-lookup"><span data-stu-id="29b50-212">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="29b50-213">选择 " **运行流**"，然后选择 " **完成"。**</span><span class="sxs-lookup"><span data-stu-id="29b50-213">Select **Run flow**, and then select **Done.**</span></span>

<span data-ttu-id="29b50-214">Webhook 现在可以侦听、创建和更新事件。</span><span class="sxs-lookup"><span data-stu-id="29b50-214">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="29b50-215">自定义同步步骤</span><span class="sxs-lookup"><span data-stu-id="29b50-215">Customize synchronization steps</span></span>

<span data-ttu-id="29b50-216">CRM 系统经过高度自定义，你可以基于 CRM 设置自定义电源自动化解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-216">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="29b50-217">当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，在 " [自定义字段映射指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)" 中列出了在合作伙伴中心电脑上同步的字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-217">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="29b50-218">按照字段映射指南进行操作，如有必要，请在 **[自定义] 创建或获取 Dynamics 365 flow** 或环境变量的详细信息。</span><span class="sxs-lookup"><span data-stu-id="29b50-218">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow** or environment variables.</span></span> <span data-ttu-id="29b50-219">请勿更新 Power 自动化解决方案中的任何其他流，因为它可能会影响将来的解决方案升级。</span><span class="sxs-lookup"><span data-stu-id="29b50-219">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="29b50-220">提供下列自定义项：</span><span class="sxs-lookup"><span data-stu-id="29b50-220">The following customizations are available:</span></span>

- <span data-ttu-id="29b50-221">**显示机会名称中的复选标记**：默认情况下，机会名称旁边将显示一个复选标记，指示在合作伙伴中心与 DYNAMICS 365 CRM 之间的同步成功发生。</span><span class="sxs-lookup"><span data-stu-id="29b50-221">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="29b50-222">同样，如果同步失败，将显示交叉标记。</span><span class="sxs-lookup"><span data-stu-id="29b50-222">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="29b50-223">若要避免在机会名称中添加复选标记或交叉标记，请将 **机会 name 环境变量中显示复选标记** 的当前值设置为 "否"。</span><span class="sxs-lookup"><span data-stu-id="29b50-223">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>
- <span data-ttu-id="29b50-224">**交易价值**：默认情况下，来自合作伙伴中心的交易值将与 CRM 中的 **estimatedvalue** 同步。</span><span class="sxs-lookup"><span data-stu-id="29b50-224">**Deal value**: By default, the deal value from Partner Center will be synced to and from **estimatedvalue** in the CRM.</span></span> <span data-ttu-id="29b50-225">如果 CRM 中有其他字段要从中同步交易值：</span><span class="sxs-lookup"><span data-stu-id="29b50-225">If you have a different field in the CRM for the deal value to sync from:</span></span>

  - <span data-ttu-id="29b50-226">用 CRM 的字段名称更新 Dynamics 365 环境变量中的 " **交易值** " 字段名称。</span><span class="sxs-lookup"><span data-stu-id="29b50-226">Update the **Deal value** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="29b50-227">请确保提供字段名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="29b50-227">Make sure that you provide the field's name, not its display name.</span></span>
  - <span data-ttu-id="29b50-228">编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**，转到 **创建或更新** crm 中的机会，更新 **创建新机会** 并 **更新现有机会** 操作，将 **DealValue** 值分配到 CRM 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or update opportunity** in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** value to the correct field in the CRM.</span></span> <span data-ttu-id="29b50-229">同时，从 "**估计收入**" 字段中删除 **DealValue** 分配。</span><span class="sxs-lookup"><span data-stu-id="29b50-229">Also, remove the **DealValue** assignment from the **Estimated Revenue** field.</span></span>

- <span data-ttu-id="29b50-230">**客户帐户国家/地区代码**：创建新引用时，必须提供两个字母的国家/地区代码 (ISO 3166) 。</span><span class="sxs-lookup"><span data-stu-id="29b50-230">**Customer Account Country Code**: It's mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="29b50-231">默认情况下，国家/地区代码将与 CRM 中帐户的 **address1_country** 字段同步。</span><span class="sxs-lookup"><span data-stu-id="29b50-231">By default, the country code will be synced to and from the account's **address1_country** field in the CRM.</span></span> <span data-ttu-id="29b50-232">如果 CRM 中的 "国家/地区代码" 字段不同，则：</span><span class="sxs-lookup"><span data-stu-id="29b50-232">If you have a different field in the CRM for the country code to sync from:</span></span>

  - <span data-ttu-id="29b50-233">对于包含两个字母代码的帐户中的 nonlookup "国家/地区代码" 字段：</span><span class="sxs-lookup"><span data-stu-id="29b50-233">For a nonlookup country code field in the account that contains a two-letter code:</span></span>
    - <span data-ttu-id="29b50-234">将 Dynamics 365 环境变量中的 **客户帐户 "国家/地区代码** " 字段名称更新为 CRM 的字段名称。</span><span class="sxs-lookup"><span data-stu-id="29b50-234">Update the **Customer Account Country Code** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="29b50-235">请确保提供字段名称，而不是其显示名称。</span><span class="sxs-lookup"><span data-stu-id="29b50-235">Make sure that you provide the field's name, not its display name.</span></span>
    - <span data-ttu-id="29b50-236">编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**，然后转到 **创建或获取** crm 操作中的客户帐户，将 **国家/地区** 值分配给 crm 中的正确字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-236">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or get customer account** in the CRM action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="29b50-237">同时，从 "**地址1：国家/地区**" 字段中删除 **国家**/地区值分配。</span><span class="sxs-lookup"><span data-stu-id="29b50-237">Also, remove the **Country** value assignment from the **Address 1: Country/Region** field.</span></span>

  - <span data-ttu-id="29b50-238">对于帐户中的基于查找的国家/地区代码字段：</span><span class="sxs-lookup"><span data-stu-id="29b50-238">For a lookup-based country code field in the account:</span></span>
    - <span data-ttu-id="29b50-239">在帐户中添加新的自定义字段，并使用两个字母的国家/地区代码自动填充该字段 (ISO 3166) 基于在查找字段中选择的值，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="29b50-239">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>
    - <span data-ttu-id="29b50-240">按照前面的步骤为 nonlookup "国家/地区代码" 字段，将新的自定义字段从 CRM 同步到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="29b50-240">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="29b50-241">**机会字段**：如果存在需要填充的 **机会** 中的必填字段，请编辑 **[自定义] 创建或获取来自 Dynamics 365 flow 的详细信息** ，然后转到 CRM 中的 " **创建" 或 "更新机会** "，然后根据您的业务要求，"更新 **创建新的机会" 操作** 以将值分配到必填字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-241">**Opportunity fields**: If there are mandatory fields in **Opportunity** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update opportunity** in the CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="29b50-242">**潜在顾客字段**：如果 **lead** 中有需要填充的必填字段，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息** ，然后转到 **创建或更新** CRM 中的潜在客户，并更新 **创建新的潜在客户操作** ，根据业务需求将值分配到必填字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-242">**Lead fields**: If there are mandatory fields in **Lead** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update lead** in the CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="29b50-243">**客户帐户**：如果新的引用从合作伙伴中心同步到 crm，则 Power 自动解决方案将尝试使用客户公司名称和邮政编码搜索 CRM 中的现有帐户。</span><span class="sxs-lookup"><span data-stu-id="29b50-243">**Customer account**: When a new referral is synced from Partner Center to the CRM, the Power Automate solution tries to search for an existing account in the CRM by using the customer company name and postal code.</span></span> <span data-ttu-id="29b50-244">如果找不到，将在 CRM 中创建新的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="29b50-244">If it doesn't find one, a new customer account will be created in the CRM.</span></span> <span data-ttu-id="29b50-245">若要更新搜索条件和新建帐户创建详细信息，请编辑 **[自定义] 创建或从 Dynamics 365 流中获取详细信息** ，然后转到 **创建或获取** CRM 中的客户帐户并 **创建客户帐户操作**。</span><span class="sxs-lookup"><span data-stu-id="29b50-245">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or get customer account** in the CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="29b50-246">更新环境变量</span><span class="sxs-lookup"><span data-stu-id="29b50-246">Update environment variable</span></span>

<span data-ttu-id="29b50-247">更新环境变量值：</span><span class="sxs-lookup"><span data-stu-id="29b50-247">To update an environment variable value:</span></span>

1. <span data-ttu-id="29b50-248">请在 " **解决方案** " 页上，选择 " **默认解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="29b50-248">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="29b50-249">选择 "**全部**" 以选择 **环境变量**。</span><span class="sxs-lookup"><span data-stu-id="29b50-249">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="29b50-250">选择需要更新的值的环境变量，并使用省略号图标选择 " **编辑** "。</span><span class="sxs-lookup"><span data-stu-id="29b50-250">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="29b50-251">更新 **当前值** (不要使用 "**新建值**" 选项并提供值来更新 **默认值**) 。</span><span class="sxs-lookup"><span data-stu-id="29b50-251">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="29b50-252">该值必须与变量的数据类型匹配。</span><span class="sxs-lookup"><span data-stu-id="29b50-252">The value must match the data type of the variable.</span></span> <span data-ttu-id="29b50-253">例如，"是" 或 "否" 数据类型将接受 Yes 或 No 值。</span><span class="sxs-lookup"><span data-stu-id="29b50-253">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/environment-variables-video.gif" alt-text="显示更新环境变量的屏幕截图。":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a><span data-ttu-id="29b50-255">端到端双向共同销售引用同步</span><span class="sxs-lookup"><span data-stu-id="29b50-255">End-to-end bidirectional co-sell referral synchronization</span></span>

<span data-ttu-id="29b50-256">安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。</span><span class="sxs-lookup"><span data-stu-id="29b50-256">After you've installed, configured, and customized the Power Automate solution, you can test for co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="29b50-257">先决条件</span><span class="sxs-lookup"><span data-stu-id="29b50-257">Prerequisites</span></span>

<span data-ttu-id="29b50-258">若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-258">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="29b50-259">此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。</span><span class="sxs-lookup"><span data-stu-id="29b50-259">This identification gives your seller teams the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="29b50-260">一组自定义字段和对象将作为解决方案安装的一部分添加。</span><span class="sxs-lookup"><span data-stu-id="29b50-260">A set of custom fields and objects will be added as part of the solution installation.</span></span> <span data-ttu-id="29b50-261">CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="29b50-261">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="29b50-262">以下自定义字段应为 CRM 部分的一部分：</span><span class="sxs-lookup"><span data-stu-id="29b50-262">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="29b50-263">**与合作伙伴中心同步**：是否要将此机会与合作伙伴中心同步。</span><span class="sxs-lookup"><span data-stu-id="29b50-263">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="29b50-264">默认情况下，此字段的值为 "否"，并且你的卖方需要将其显式设置为 "是"，以便与 Microsoft 共享机会。</span><span class="sxs-lookup"><span data-stu-id="29b50-264">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="29b50-265">从合作伙伴中心到 CRM 共享的新引用将此字段值设置为 "是"。</span><span class="sxs-lookup"><span data-stu-id="29b50-265">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>
- <span data-ttu-id="29b50-266">**引用标识符**：合作伙伴中心引用的只读标识符字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-266">**Referral Identifier**: A read-only identifier field for the Partner Center referral.</span></span>
- <span data-ttu-id="29b50-267">**引用链接**：指向合作伙伴中心中的引用的只读链接。</span><span class="sxs-lookup"><span data-stu-id="29b50-267">**Referral Link**: A read-only link to the referral in Partner Center.</span></span>
- <span data-ttu-id="29b50-268">**Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助。</span><span class="sxs-lookup"><span data-stu-id="29b50-268">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="29b50-269">若要创建共同销售引用，请选择 Microsoft 所需的适当帮助。</span><span class="sxs-lookup"><span data-stu-id="29b50-269">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="29b50-270">必须将客户联系人关联到创建共同销售引用的机会。</span><span class="sxs-lookup"><span data-stu-id="29b50-270">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="29b50-271">若要创建非共同销售引用，请不要选择此字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-271">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="29b50-272">通过选择适当的帮助-必需选项，可以随时将非共同销售引用转换为共同销售引用。</span><span class="sxs-lookup"><span data-stu-id="29b50-272">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>
- <span data-ttu-id="29b50-273">**Microsoft 合作伙伴中心引用可见性**：选择合作伙伴中心引用的可见性。</span><span class="sxs-lookup"><span data-stu-id="29b50-273">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="29b50-274">通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。</span><span class="sxs-lookup"><span data-stu-id="29b50-274">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="29b50-275">如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会显示该引用。</span><span class="sxs-lookup"><span data-stu-id="29b50-275">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="29b50-276">将此字段标记为可见后，将无法还原它。</span><span class="sxs-lookup"><span data-stu-id="29b50-276">After this field is marked as visible, it can't be reverted.</span></span>
- <span data-ttu-id="29b50-277">**MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。</span><span class="sxs-lookup"><span data-stu-id="29b50-277">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>
- <span data-ttu-id="29b50-278">**产品：已过时**：请勿使用此字段或将其添加到 CRM 部分。</span><span class="sxs-lookup"><span data-stu-id="29b50-278">**Products: Obsolete**: Don't use this field or add it to the CRM section.</span></span> <span data-ttu-id="29b50-279">它仅可用于向后兼容。</span><span class="sxs-lookup"><span data-stu-id="29b50-279">It's available for backward compatibility only.</span></span> <span data-ttu-id="29b50-280">请改用合作伙伴中心解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-280">Use Partner Center solutions instead.</span></span>
- <span data-ttu-id="29b50-281">**Audit**：与合作伙伴中心引用同步的只读审核记录。</span><span class="sxs-lookup"><span data-stu-id="29b50-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals.</span></span>
- <span data-ttu-id="29b50-282">**Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。</span><span class="sxs-lookup"><span data-stu-id="29b50-282">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="29b50-283">可以在商机中添加或删除一个或多个解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-283">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="29b50-284">在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-284">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="29b50-285">若要将此对象与商机关联，请在 CRM 中更新 **商机** 窗体。</span><span class="sxs-lookup"><span data-stu-id="29b50-285">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

  <span data-ttu-id="29b50-286">选择 " **机会** " 窗体上的相应选项卡，并添加子网格，如下所示。</span><span class="sxs-lookup"><span data-stu-id="29b50-286">Select the appropriate tab on the **Opportunity** form, and add a subgrid as shown here.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="显示机会窗体的屏幕截图。":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="显示 Microsoft 解决方案的屏幕截图。":::

- <span data-ttu-id="29b50-289">添加 Microsoft 解决方案后，你可以预填充联合销售就绪解决方案详细信息，以便你的卖方不必添加它们。</span><span class="sxs-lookup"><span data-stu-id="29b50-289">After you add Microsoft solutions, you can prepopulate co-sell ready solution details so that your sellers don't have to add them.</span></span> <span data-ttu-id="29b50-290">若要添加新的解决方案详细信息，请前往 CRM 中的 Microsoft 解决方案详细信息对象，然后选择 " **添加记录** " 以添加一个条目或使用 **Excel 上传** 添加多个条目。</span><span class="sxs-lookup"><span data-stu-id="29b50-290">To add a new solution detail, go to the Microsoft Solution Details object in the CRM and select **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="显示新的 Microsoft 解决方案详细信息的屏幕截图。":::

### <a name="scenarios"></a><span data-ttu-id="29b50-292">方案</span><span class="sxs-lookup"><span data-stu-id="29b50-292">Scenarios</span></span>

1. <span data-ttu-id="29b50-293">在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：</span><span class="sxs-lookup"><span data-stu-id="29b50-293">Referral synchronization when referral is created or updated in the CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="29b50-294">在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="29b50-294">Sign in to your Dynamics 365 CRM environment with the user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="29b50-295">在 Dynamics 365 环境中创建新机会时，请确保 **Microsoft 合作伙伴中心** 部分存在。</span><span class="sxs-lookup"><span data-stu-id="29b50-295">Ensure that the **Microsoft Partner Center** section is present when you create a new opportunity in the Dynamics 365 environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="显示新机会的屏幕截图。":::

   1. <span data-ttu-id="29b50-297">若要将此机会与合作伙伴中心同步，请确保在卡片视图中设置以下字段：</span><span class="sxs-lookup"><span data-stu-id="29b50-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="29b50-298">**Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。</span><span class="sxs-lookup"><span data-stu-id="29b50-298">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="显示如何在卡片视图中获取相应字段的屏幕截图。":::

      - <span data-ttu-id="29b50-300">**客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。</span><span class="sxs-lookup"><span data-stu-id="29b50-300">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="29b50-301">**与合作伙伴中心同步**：是。</span><span class="sxs-lookup"><span data-stu-id="29b50-301">**Sync With Partner Center**: Yes.</span></span>
      - <span data-ttu-id="29b50-302">**Microsoft 解决方案**：若要与 microsoft 共享引用，请向此机会添加有效的合作销售就绪或 Microsoft 解决方案。</span><span class="sxs-lookup"><span data-stu-id="29b50-302">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="显示解决方案 ID 的屏幕截图。":::

   1. <span data-ttu-id="29b50-304">在 Dynamics 365 中创建机会后，在 " **与合作伙伴中心同步** " 选项设置为 "是" 后，等待10分钟。</span><span class="sxs-lookup"><span data-stu-id="29b50-304">After the opportunity is created in Dynamics 365 with the **Sync With Partner Center** option set to Yes, wait 10 minutes.</span></span> <span data-ttu-id="29b50-305">然后登录到合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="29b50-305">Then sign in to your Partner Center account.</span></span> <span data-ttu-id="29b50-306">你的引用将与 Dynamics 365 和 **引用标识符** 同步。</span><span class="sxs-lookup"><span data-stu-id="29b50-306">Your referrals will be synchronized with Dynamics 365 and **Referral Identifier**.</span></span> <span data-ttu-id="29b50-307">将填充 **引用链接**。</span><span class="sxs-lookup"><span data-stu-id="29b50-307">**Referral Link** will get populated.</span></span> <span data-ttu-id="29b50-308">如果出现故障，则将使用错误信息填充 **审核** 字段。</span><span class="sxs-lookup"><span data-stu-id="29b50-308">If there's a failure, the **Audit** field will be populated with error information.</span></span>

      1. <span data-ttu-id="29b50-309">同样，如果将 " **与合作伙伴中心同步** " 选项设置为 "是"，则在 DYNAMICS 365 CRM 中更新该机会时，所做的更改将在你的合作伙伴中心帐户中同步。</span><span class="sxs-lookup"><span data-stu-id="29b50-309">Likewise, for an opportunity that had the **Sync With Partner Center** option set to Yes, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

      1. <span data-ttu-id="29b50-310">与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。</span><span class="sxs-lookup"><span data-stu-id="29b50-310">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

1. <span data-ttu-id="29b50-311">当在合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时，引用同步：</span><span class="sxs-lookup"><span data-stu-id="29b50-311">Referral synchronization when the referral is created or updated in Partner Center and synchronized in the Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="29b50-312">登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="29b50-312">Sign in to your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   1. <span data-ttu-id="29b50-313">从左侧菜单中选择 " **引用** "。</span><span class="sxs-lookup"><span data-stu-id="29b50-313">Select **Referrals** from the left menu.</span></span>

   1. <span data-ttu-id="29b50-314">通过选择 " **新建交易** " 选项，从合作伙伴中心创建新的共同销售引用。</span><span class="sxs-lookup"><span data-stu-id="29b50-314">Create a new co-sell referral from Partner Center by selecting the **New deal** option.</span></span>

   1. <span data-ttu-id="29b50-315">登录到 Dynamics 365 CRM 环境。</span><span class="sxs-lookup"><span data-stu-id="29b50-315">Sign in to your Dynamics 365 CRM environment.</span></span>

   1. <span data-ttu-id="29b50-316">前往 **开放机会**。</span><span class="sxs-lookup"><span data-stu-id="29b50-316">Go to **Open Opportunities**.</span></span> <span data-ttu-id="29b50-317">现在，在合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。</span><span class="sxs-lookup"><span data-stu-id="29b50-317">The referral created in Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   1. <span data-ttu-id="29b50-318">选择同步的引用时，将填充卡片视图详细信息。</span><span class="sxs-lookup"><span data-stu-id="29b50-318">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="29b50-319">后续步骤</span><span class="sxs-lookup"><span data-stu-id="29b50-319">Next steps</span></span>

- [<span data-ttu-id="29b50-320">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="29b50-320">Manage leads</span></span>](manage-leads.md)
- [<span data-ttu-id="29b50-321">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="29b50-321">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
- [<span data-ttu-id="29b50-322">有关 Microsoft Power 自动化平台的详细信息</span><span class="sxs-lookup"><span data-stu-id="29b50-322">More about Microsoft Power Automate platform</span></span>](/power-automate/)
- [<span data-ttu-id="29b50-323">合作伙伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="29b50-323">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
