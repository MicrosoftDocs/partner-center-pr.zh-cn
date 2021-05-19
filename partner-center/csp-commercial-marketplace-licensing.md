---
title: 管理市场产品/服务中的许可
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何设置和管理 ISV 商用 marketplace 产品/服务的许可。
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147949"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="c2eb8-103">管理市场产品/服务中的许可</span><span class="sxs-lookup"><span data-stu-id="c2eb8-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="c2eb8-104">**适当的角色**：全局管理员 |帐户管理员</span><span class="sxs-lookup"><span data-stu-id="c2eb8-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="c2eb8-105">本文将指导你完成在合作伙伴中心设置产品/服务的过程，使其可用于 Microsoft AppSource，然后管理该产品的许可证。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-105">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="c2eb8-106">本文中的功能目前为公共预览版。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-106">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="c2eb8-107">准备阶段</span><span class="sxs-lookup"><span data-stu-id="c2eb8-107">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="c2eb8-108">商业市场基础知识</span><span class="sxs-lookup"><span data-stu-id="c2eb8-108">Commercial marketplace basics</span></span>

<span data-ttu-id="c2eb8-109">在开始此过程之前，您应熟悉商业应用商店的基本知识。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-109">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="c2eb8-110">下表中的文章将帮助你入门。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-110">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="c2eb8-111">主题</span><span class="sxs-lookup"><span data-stu-id="c2eb8-111">Topic</span></span>  | <span data-ttu-id="c2eb8-112">项目</span><span class="sxs-lookup"><span data-stu-id="c2eb8-112">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="c2eb8-113">商业市场计划</span><span class="sxs-lookup"><span data-stu-id="c2eb8-113">Commercial marketplace plans</span></span> | [<span data-ttu-id="c2eb8-114">商业市场产品/服务计划和定价</span><span class="sxs-lookup"><span data-stu-id="c2eb8-114">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="c2eb8-115">商业市场优惠</span><span class="sxs-lookup"><span data-stu-id="c2eb8-115">Commercial marketplace offers</span></span>  | [<span data-ttu-id="c2eb8-116">列表类型</span><span class="sxs-lookup"><span data-stu-id="c2eb8-116">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="c2eb8-117">商业应用商店帐户</span><span class="sxs-lookup"><span data-stu-id="c2eb8-117">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="c2eb8-118">在合作伙伴中心创建商业市场帐户</span><span class="sxs-lookup"><span data-stu-id="c2eb8-118">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="c2eb8-119">确定产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="c2eb8-119">Determine your Offer ID</span></span>

<span data-ttu-id="c2eb8-120">在下面的过程中，系统将提示你输入产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-120">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="c2eb8-121">现在请花一些时间来提供合适的产品/服务 ID，请记住以下几点：</span><span class="sxs-lookup"><span data-stu-id="c2eb8-121">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="c2eb8-122">客户可以在市场产品/服务和 Azure 资源管理器模板的 Web 地址中看到此 ID（若有）。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-122">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="c2eb8-123">产品 ID 和发布者 ID 的组合长度必须为在 40 个字符以内。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-123">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="c2eb8-124">只使用小写字母和数字。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-124">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="c2eb8-125">产品/服务 ID 可以包括连字符和下划线，但不能包含空格。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-125">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="c2eb8-126">例如，如果你的发布者 ID 为 `testpublisherid` ，并且你输入了 `test-offer-1` ，则 "产品/服务" 网址为 `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` 。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-126">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="c2eb8-127">选择“创建”后，便无法更改此 ID。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-127">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="c2eb8-128">确定提供别名</span><span class="sxs-lookup"><span data-stu-id="c2eb8-128">Determine your Offer alias</span></span>

<span data-ttu-id="c2eb8-129">"产品/服务" 别名是用于 "合作伙伴中心" 中的产品/服务的名称。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-129">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="c2eb8-130">还需要遵循以下指导原则的适当提议：</span><span class="sxs-lookup"><span data-stu-id="c2eb8-130">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="c2eb8-131">此名称没有用于市场，与向客户显示的产品/服务名称和其他值不同。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-131">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="c2eb8-132">选择“创建”后，便无法更改此名称。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-132">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="c2eb8-133">创建产品/服务</span><span class="sxs-lookup"><span data-stu-id="c2eb8-133">Create your offer</span></span>

<span data-ttu-id="c2eb8-134">授权过程的第一步是创建商业 marketplace 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-134">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="c2eb8-135">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-135">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="c2eb8-136">在左侧导航菜单中，选择"**商业市场/概述"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-136">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="c2eb8-137">在"概述"页顶部，选择"新建产品/服务"，然后选择 **"Dynamics 365 for Customer Engagement & PowerApps"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-137">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="c2eb8-138">输入之前 **创建的"产品** /服务 **ID"和** "产品/服务别名"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-138">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="c2eb8-139">选择“创建”，以生成产品/服务，并继续操作。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-139">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="c2eb8-140">选择许可选项。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-140">Choose your licensing options.</span></span>

    - <span data-ttu-id="c2eb8-141">若要为产品/服务启用许可证管理，请选择 **"通过 Microsoft 启用应用许可证管理"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-141">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="c2eb8-142">这是一次设置，发布产品/服务后，不能更改此设置。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-142">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="c2eb8-143">还可以让客户在没有许可证的情况下运行应用的基本功能，在购买许可证后运行高级功能。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-143">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="c2eb8-144">为此，请选择 **"即使未分配许可证，也允许客户安装我的应用"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-144">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="c2eb8-145">如果不希望产品/服务启用许可证管理，请选择"立即获取 (免费 **) 免费试用"** 或"**与我联系"。** </span><span class="sxs-lookup"><span data-stu-id="c2eb8-145">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="c2eb8-146">创建计划</span><span class="sxs-lookup"><span data-stu-id="c2eb8-146">Create your plan</span></span>

<span data-ttu-id="c2eb8-147">在这些步骤中，你将定义要为产品/服务启用的计划。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-147">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="c2eb8-148">在左侧导航菜单中，选择"**计划概述**"，然后选择"**创建新计划"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-148">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="c2eb8-149">输入"**计划 ID"** 和 **"计划名称"，** 然后选择"创建 **"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-149">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="c2eb8-150">在" **计划列表"** 页上，输入 **计划说明**。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-150">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="c2eb8-151">若要保存说明并稍后完成，请选择"**保存草稿"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-151">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="c2eb8-152">完成后，选择"查看并 **发布"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-152">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="c2eb8-153">计划信息现在将显示在套餐列表 appsource.microsoft.com 套餐列表 (部分下) 。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-153">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="c2eb8-154">创建此产品/服务的所有计划后，需要复制每个计划的"服务 ID"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-154">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="c2eb8-155">选择 **"计划** 列表"页顶部的"计划概述"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-155">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="c2eb8-156">将每个计划的服务 ID 复制到安全位置。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-156">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="c2eb8-157">将服务 ID 添加到解决方案</span><span class="sxs-lookup"><span data-stu-id="c2eb8-157">Add Service IDs to your solution</span></span>

<span data-ttu-id="c2eb8-158">下一步是通过为刚复制的每个计划添加服务 D 来更新解决方案。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-158">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="c2eb8-159">有关此的指导，请参阅 [为解决方案 创建 AppSource 包](/powerapps/developer/data-platform/create-package-app-appsource)。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-159">For guidance on this, see [Create an AppSource Package for your solution](/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="c2eb8-160">上传包并发布产品/服务</span><span class="sxs-lookup"><span data-stu-id="c2eb8-160">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="c2eb8-161">在左侧导航窗格中，选择"**商业市场"，** 然后选择"**技术配置"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-161">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="c2eb8-162">在"**基本许可证模型"下**，选择"**用户"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-162">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="c2eb8-163">在 **"CRM 包**"下，输入包位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-163">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="c2eb8-164">使用左侧导航窗格中的其他选项卡输入任何其他必需信息。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-164">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="c2eb8-165">完成后，选择"查看并 **发布"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-165">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="c2eb8-166">发布产品/服务后，我们将查看并验证你的信息。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-166">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="c2eb8-167">如果此过程存在任何问题，我们会通知你。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-167">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="c2eb8-168">解决所有问题后，你可收到通知，告知产品/服务在 AppSource 中可用。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-168">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="c2eb8-169">此时，可以使其上线。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-169">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="c2eb8-170">使产品/服务在 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="c2eb8-170">Make your offer live in Partner Center</span></span>

<span data-ttu-id="c2eb8-171">以下过程将指导你完成在 AppSource 中启用产品/服务的过程。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-171">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="c2eb8-172">若要了解有关此过程的详细信息，请参阅 [列出选项 简介](/azure/marketplace/determine-your-listing-type)。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-172">To learn more about this process, see [Introduction to listing options](/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="c2eb8-173">发布产品/服务后，需要 4-6 小时才能上台。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-173">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="c2eb8-174">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-174">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="c2eb8-175">在左侧导航菜单中，选择"**商业市场/概述"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-175">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="c2eb8-176">在 **"概述** "页上，找到要查找的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-176">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="c2eb8-177">已准备好发布的产品/服务的状态为"预览 **"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-177">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="c2eb8-178">选择产品/服务。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-178">Select the offer.</span></span>
4. <span data-ttu-id="c2eb8-179">在"**产品/服务概述"** 页上，选择"**上一版"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-179">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="c2eb8-180">产品/服务将在4-6 小时内推出。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-180">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="c2eb8-181">若要查看 AppSource 上的产品/服务列表，请选择 "**产品/服务概述**" 页底部的 " **AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-181">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="c2eb8-182">**对于启用许可证的产品/** 服务：如果你的产品/服务需要许可证检查，则用户将只能通过单击 " **与我联系**" 来输入潜在客户，以便可以与他们进行通信。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-182">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="c2eb8-183">**对于启用许可证的产品/服务免费安装选项**：如果产品/服务不需要许可证检查，则除了 **与我联系**，管理员用户还将看到 "**立即获取**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-183">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="c2eb8-184">如果用户想要尝试 "免费安装" 选项，则应单击 " **立即获取**"，这会使用户在 Power Platform 管理中心上安装产品/服务。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-184">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="c2eb8-185">如果用户有任何疑问，或者他们想要升级到付费计划，用户仍然可以使用 " **联系我** "。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-185">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="c2eb8-186">注册 ISV Connect 交易交易注册</span><span class="sxs-lookup"><span data-stu-id="c2eb8-186">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="c2eb8-187">在将许可证分配给客户之前，需要在合作伙伴中心注册每个销售。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-187">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="c2eb8-188">为此，请参阅 [注册交易](register-deals.md)。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-188">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="c2eb8-189">邀请客户</span><span class="sxs-lookup"><span data-stu-id="c2eb8-189">Invite the customer</span></span>

<span data-ttu-id="c2eb8-190">使用以下过程邀请客户参与此交易。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-190">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="c2eb8-191">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-191">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="c2eb8-192">在左侧导航菜单中，选择 " **商业 Marketplace/概述**"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-192">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="c2eb8-193">在左侧导航菜单中，选择 " **引用**"，然后选择 " **交易注册**"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-193">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="c2eb8-194">筛选 **提交** 的交易，选择 " **正在进行** " 选项卡，然后选择所需的交易。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-194">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="c2eb8-195">在此交易的 "概述" 页上，选择 " **管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-195">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="c2eb8-196">在 " **管理许可证** " 窗口中，从 " **客户详细信息** " 下拉列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-196">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="c2eb8-197">如果客户关系尚不存在，请选择 " **+ 邀请新客户同意**"。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-197">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="c2eb8-198">复制显示的链接。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-198">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="c2eb8-199">通过电子邮件将此链接发送到客户的帐单管理员或全局管理员，并让他们使用此链接访问 admin.microsoft.com，并接受并授权您正在建立的关系。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-199">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c2eb8-200">在客户执行此步骤之前，将不会建立关系。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-200">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="c2eb8-201">激活、管理和删除许可证</span><span class="sxs-lookup"><span data-stu-id="c2eb8-201">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="c2eb8-202">客户获得与关系的授权后，可以开始从产品/服务添加计划，并将许可证分配给每个计划。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-202">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="c2eb8-203">在"管理此交易的许可"窗口中，选择 **"+添加计划"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-203">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="c2eb8-204">完成"**此解决方案的计划"和\*\*\*\*"许可证数量**"字段，然后选择"**更新许可证"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-204">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="c2eb8-205">这些许可证将在 admin.microsoft.com 供客户管理和分配给员工。</span><span class="sxs-lookup"><span data-stu-id="c2eb8-205">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="c2eb8-206">若要更改现有计划的许可证数，请在"许可证数"字段中输入新 **编号，然后选择**"**更新许可证"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-206">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="c2eb8-207">若要停用或删除交易许可证，请在"操作"字段中选择垃圾桶图标，然后选择"更新 **许可证"。**</span><span class="sxs-lookup"><span data-stu-id="c2eb8-207">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c2eb8-208">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c2eb8-208">Next steps</span></span>

[<span data-ttu-id="c2eb8-209">许可资源</span><span class="sxs-lookup"><span data-stu-id="c2eb8-209">Licensing resources</span></span>](support-resources-licensing.md)