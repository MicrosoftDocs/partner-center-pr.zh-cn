---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Salesforce CRM 连接器，从 Microsoft 获取推荐
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825694"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="98f7a-103">Salesforce CRM 的共同销售连接器-概述</span><span class="sxs-lookup"><span data-stu-id="98f7a-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="98f7a-104">相应的角色</span><span class="sxs-lookup"><span data-stu-id="98f7a-104">Appropriate roles</span></span>

- <span data-ttu-id="98f7a-105">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="98f7a-105">Referrals admin</span></span>
- <span data-ttu-id="98f7a-106">CRM 上的系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="98f7a-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="98f7a-107">合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。</span><span class="sxs-lookup"><span data-stu-id="98f7a-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="98f7a-108">他们无需定型即可使用合作伙伴中心来管理共同销售交易。</span><span class="sxs-lookup"><span data-stu-id="98f7a-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="98f7a-109">使用共同销售连接器，你将能够创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用、接受/拒绝引用、修改交易数据（如交易价值、结算日期等），以及从 Microsoft 卖方接收有关这些共同销售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="98f7a-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="98f7a-110">您可以在所选的 CRM 内而不是在合作伙伴中心内完成所有这些工作。</span><span class="sxs-lookup"><span data-stu-id="98f7a-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="98f7a-111">此解决方案基于 Microsoft Power 自动化解决方案，并使用 Microsoft 合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="98f7a-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="98f7a-112">安装之前-必备组件</span><span class="sxs-lookup"><span data-stu-id="98f7a-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="98f7a-113">**主题**</span><span class="sxs-lookup"><span data-stu-id="98f7a-113">**Topics**</span></span>   |<span data-ttu-id="98f7a-114">**详细信息**</span><span class="sxs-lookup"><span data-stu-id="98f7a-114">**Details**</span></span>   |<span data-ttu-id="98f7a-115">**链接**</span><span class="sxs-lookup"><span data-stu-id="98f7a-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="98f7a-116">Microsoft 合作伙伴网络 ID</span><span class="sxs-lookup"><span data-stu-id="98f7a-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="98f7a-117">需要一个有效的 MPN ID</span><span class="sxs-lookup"><span data-stu-id="98f7a-117">You need a valid MPN ID</span></span>|<span data-ttu-id="98f7a-118">加入[MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="98f7a-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="98f7a-119">合作销售就绪</span><span class="sxs-lookup"><span data-stu-id="98f7a-119">Co-sell ready</span></span>|<span data-ttu-id="98f7a-120">你的 IP/服务解决方案必须共同销售。</span><span class="sxs-lookup"><span data-stu-id="98f7a-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="98f7a-121">与 Microsoft 一起销售</span><span class="sxs-lookup"><span data-stu-id="98f7a-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="98f7a-122">合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="98f7a-122">Partner Center account</span></span>|<span data-ttu-id="98f7a-123">与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。</span><span class="sxs-lookup"><span data-stu-id="98f7a-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="98f7a-124">在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。</span><span class="sxs-lookup"><span data-stu-id="98f7a-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="98f7a-125">管理帐户</span><span class="sxs-lookup"><span data-stu-id="98f7a-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="98f7a-126">合作伙伴中心用户角色</span><span class="sxs-lookup"><span data-stu-id="98f7a-126">Partner Center user roles</span></span>|<span data-ttu-id="98f7a-127">将安装和使用连接器的员工必须是推荐管理员</span><span class="sxs-lookup"><span data-stu-id="98f7a-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="98f7a-128">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="98f7a-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="98f7a-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="98f7a-129">Salesforce CRM</span></span>|<span data-ttu-id="98f7a-130">CRM 用户角色是系统管理员或系统定制员</span><span class="sxs-lookup"><span data-stu-id="98f7a-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="98f7a-131">在 Dynamics 365 中分配角色</span><span class="sxs-lookup"><span data-stu-id="98f7a-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="98f7a-132">Power 自动化 Flow 帐户</span><span class="sxs-lookup"><span data-stu-id="98f7a-132">Power Automate Flow Account</span></span>|<span data-ttu-id="98f7a-133">CRM 系统管理员或系统定制员的有效[电源自动完成](https://flow.microsoft.com)帐户。</span><span class="sxs-lookup"><span data-stu-id="98f7a-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="98f7a-134">在安装之前，该用户至少应登录到一次[电源](https://flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="98f7a-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="98f7a-135">为 Salesforce CRM 安装合作伙伴中心引用同步</span><span class="sxs-lookup"><span data-stu-id="98f7a-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="98f7a-136">请继续[执行 "电源自动](https://flow.microsoft.com)"，并选择右上角的 "**环境**"。</span><span class="sxs-lookup"><span data-stu-id="98f7a-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="98f7a-137">这会显示可用的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="98f7a-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="98f7a-138">从右上角的下拉菜单中选择相应的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="98f7a-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="98f7a-139">选择左侧导航栏上的 "**解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="98f7a-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="98f7a-140">单击顶部菜单上的 "**打开 AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="98f7a-140">Click on the **Open AppSource** link on the top menu.</span></span>

![打开 AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="98f7a-142">在弹出屏幕中搜索 Salesforce 的 "**合作伙伴中心引用连接器**"。</span><span class="sxs-lookup"><span data-stu-id="98f7a-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="98f7a-143">单击 "**立即获取**" 按钮，然后**继续**。</span><span class="sxs-lookup"><span data-stu-id="98f7a-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="98f7a-144">这将打开一个页面，可以在其中选择要安装应用程序的 CRM （Dynamics 365）环境。</span><span class="sxs-lookup"><span data-stu-id="98f7a-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="98f7a-145">同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="98f7a-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="98f7a-146">然后，你将转到 "**管理你的解决方案**" 页。</span><span class="sxs-lookup"><span data-stu-id="98f7a-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="98f7a-147">通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。</span><span class="sxs-lookup"><span data-stu-id="98f7a-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="98f7a-148">**计划的安装**应显示在合作伙伴中心引用解决方案旁边。</span><span class="sxs-lookup"><span data-stu-id="98f7a-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="98f7a-149">安装将需要10-15 分钟。</span><span class="sxs-lookup"><span data-stu-id="98f7a-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="98f7a-150">安装完成后，导航回 "[自动启动](https://flow.microsoft.com)"，并从左侧导航区域中选择 "**解决方案**"。</span><span class="sxs-lookup"><span data-stu-id="98f7a-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="98f7a-151">请注意，"解决方案" 列表中提供了**Salesforce 的合作伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="98f7a-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="98f7a-152">选择**Dynamics 365 的伙伴中心引用同步**。</span><span class="sxs-lookup"><span data-stu-id="98f7a-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="98f7a-153">可以使用以下功能自动执行流和实体：</span><span class="sxs-lookup"><span data-stu-id="98f7a-153">The following Power Automate flows and entities are available:</span></span>

![可用 CRM](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="98f7a-155">最佳做法：在上线之前进行测试</span><span class="sxs-lookup"><span data-stu-id="98f7a-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="98f7a-156">在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="98f7a-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="98f7a-157">在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。</span><span class="sxs-lookup"><span data-stu-id="98f7a-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="98f7a-158">制作解决方案的副本，并在过渡环境中执行配置和自动自动流自定义功能。</span><span class="sxs-lookup"><span data-stu-id="98f7a-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="98f7a-159">在过渡/CRM 实例上测试解决方案。</span><span class="sxs-lookup"><span data-stu-id="98f7a-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="98f7a-160">成功后，将作为托管解决方案导入到生产实例。</span><span class="sxs-lookup"><span data-stu-id="98f7a-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="98f7a-161">配置解决方案</span><span class="sxs-lookup"><span data-stu-id="98f7a-161">Configure the solution</span></span>

1. <span data-ttu-id="98f7a-162">在 CRM 实例中安装解决方案后，请导航回 "[电源自动](https://flow.microsoft.com/)"。</span><span class="sxs-lookup"><span data-stu-id="98f7a-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="98f7a-163">在右上角的 "**环境**" 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。</span><span class="sxs-lookup"><span data-stu-id="98f7a-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="98f7a-164">你将需要创建关联三个用户帐户的连接：</span><span class="sxs-lookup"><span data-stu-id="98f7a-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="98f7a-165">具有引用管理员凭据的合作伙伴中心用户</span><span class="sxs-lookup"><span data-stu-id="98f7a-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="98f7a-166">合作伙伴中心事件</span><span class="sxs-lookup"><span data-stu-id="98f7a-166">Partner Center Events</span></span>
- <span data-ttu-id="98f7a-167">CRM 管理员，并在解决方案中自动执行流处理。</span><span class="sxs-lookup"><span data-stu-id="98f7a-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="98f7a-168">a.</span><span class="sxs-lookup"><span data-stu-id="98f7a-168">a.</span></span> <span data-ttu-id="98f7a-169">从左侧导航栏中选择 "**连接**"，然后从列表中选择 "合作伙伴中心引用" 解决方案。</span><span class="sxs-lookup"><span data-stu-id="98f7a-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="98f7a-170">b.</span><span class="sxs-lookup"><span data-stu-id="98f7a-170">b.</span></span> <span data-ttu-id="98f7a-171">通过单击 "**创建连接**" 创建连接。</span><span class="sxs-lookup"><span data-stu-id="98f7a-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![创建连接](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="98f7a-173">c.</span><span class="sxs-lookup"><span data-stu-id="98f7a-173">c.</span></span> <span data-ttu-id="98f7a-174">在右上角的搜索栏中搜索 "**合作伙伴中心引用（预览版）** "。</span><span class="sxs-lookup"><span data-stu-id="98f7a-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="98f7a-175">d.</span><span class="sxs-lookup"><span data-stu-id="98f7a-175">d.</span></span> <span data-ttu-id="98f7a-176">使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。电邮.</span><span class="sxs-lookup"><span data-stu-id="98f7a-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="98f7a-177">接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。果.</span><span class="sxs-lookup"><span data-stu-id="98f7a-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="98f7a-178">为 CRM 管理员用户 Common Data Service （当前环境）创建连接。</span><span class="sxs-lookup"><span data-stu-id="98f7a-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="98f7a-179">若要将电源自动流与连接进行关联，请编辑每个电源自动流，以连接到 Common Data Service 和合作伙伴中心引用。</span><span class="sxs-lookup"><span data-stu-id="98f7a-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="98f7a-180">保存更改。</span><span class="sxs-lookup"><span data-stu-id="98f7a-180">Save the changes.</span></span>

5. <span data-ttu-id="98f7a-181">**打开**"自动执行流" 功能。</span><span class="sxs-lookup"><span data-stu-id="98f7a-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="98f7a-182">后续步骤</span><span class="sxs-lookup"><span data-stu-id="98f7a-182">Next steps</span></span>

- [<span data-ttu-id="98f7a-183">使用 Webhook 获取资源更改事件</span><span class="sxs-lookup"><span data-stu-id="98f7a-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="98f7a-184">有关 Microsoft Power 自动化平台的详细信息？</span><span class="sxs-lookup"><span data-stu-id="98f7a-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="98f7a-185">管理潜在客户</span><span class="sxs-lookup"><span data-stu-id="98f7a-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="98f7a-186">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="98f7a-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
