---
title: 在 marketplace 产品/服务中管理许可
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何设置和管理 ISV 商用 marketplace 产品/服务的许可。
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284867"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="1ff5d-103">在 marketplace 产品/服务中管理许可</span><span class="sxs-lookup"><span data-stu-id="1ff5d-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="1ff5d-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="1ff5d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1ff5d-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1ff5d-105">Global admin</span></span>
- <span data-ttu-id="1ff5d-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="1ff5d-106">Account admin</span></span>

<span data-ttu-id="1ff5d-107">本文将指导你完成在合作伙伴中心设置产品/服务的过程，使其可用于 Microsoft AppSource，然后管理该产品的许可证。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="1ff5d-108">本文中的功能目前为公共预览版。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1ff5d-109">开始之前</span><span class="sxs-lookup"><span data-stu-id="1ff5d-109">Before you begin</span></span>

<span data-ttu-id="1ff5d-110">开始此过程之前，应熟悉以下信息。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="1ff5d-111">查看 Azure Marketplace 文档</span><span class="sxs-lookup"><span data-stu-id="1ff5d-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="1ff5d-112">下面的文章包含您在继续操作之前应该了解的信息。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="1ff5d-113">创建 Dynamics 365 for Customer Engagement & PowerApps 套餐</span><span class="sxs-lookup"><span data-stu-id="1ff5d-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="1ff5d-114">在合作伙伴中心创建商业市场帐户</span><span class="sxs-lookup"><span data-stu-id="1ff5d-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="1ff5d-115">创建产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="1ff5d-115">Create your Offer ID</span></span>

<span data-ttu-id="1ff5d-116">在下面的过程中，系统将提示你输入产品/服务 ID。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="1ff5d-117">现在请花一些时间来提供合适的产品/服务 ID，请记住以下几点：</span><span class="sxs-lookup"><span data-stu-id="1ff5d-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="1ff5d-118">客户可以在市场产品/服务和 Azure 资源管理器模板的 Web 地址中看到此 ID（若有）。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="1ff5d-119">与发布者 ID 组合的产品 ID 的长度必须为40个字符。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="1ff5d-120">只使用小写字母和数字。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="1ff5d-121">产品/服务 ID 可以包括连字符和下划线，但不能包含空格。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="1ff5d-122">例如，如果你的发布者 ID 是 "testpublisherid"，并且你输入了 "测试/服务-1"，则 "产品/服务" 网址为 https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="1ff5d-123">选择 " **创建**" 后，不能更改此 ID。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="1ff5d-124">创建产品/服务别名</span><span class="sxs-lookup"><span data-stu-id="1ff5d-124">Create your Offer alias</span></span>

<span data-ttu-id="1ff5d-125">"产品/服务" 别名是用于 "合作伙伴中心" 中的产品/服务的名称。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="1ff5d-126">还需要遵循以下指导原则的适当提议：</span><span class="sxs-lookup"><span data-stu-id="1ff5d-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="1ff5d-127">此名称没有用于市场，与向客户显示的产品/服务名称和其他值不同。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="1ff5d-128">选择 "创建" 后，不能更改此名称。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="1ff5d-129">创建产品/服务</span><span class="sxs-lookup"><span data-stu-id="1ff5d-129">Create your offer</span></span>

<span data-ttu-id="1ff5d-130">授权过程的第一步是创建商业 marketplace 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="1ff5d-131">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1ff5d-132">在左侧导航菜单中，选择 " **商业 Marketplace/概述**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="1ff5d-133">在 "概述" 页的顶部，选择 " **新建产品/服务**"，然后选择 " **Dynamics 365 for Customer Engagement & PowerApps**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="1ff5d-134">输入先前创建的产品/服务 **ID** 和 **产品/服务别名** 。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="1ff5d-135">选择“创建”，以生成产品/服务，并继续操作。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="1ff5d-136">选择授权选项。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="1ff5d-137">若要为你的产品/服务启用许可证管理，请选择 " **通过 Microsoft 启用应用许可证管理**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="1ff5d-138">这是一次性设置，一旦发布产品/服务后，你将无法对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="1ff5d-139">您还可以让客户在没有许可证的情况下运行应用程序的基本功能，并在购买许可证后运行高级版功能。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="1ff5d-140">为此，请选择 " **允许客户安装我的应用，即使未分配许可证**。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="1ff5d-141">如果你不希望你的产品/服务启用许可证管理，请选择 " **立即获取" (免费)**、 **免费试用版** 或 " **与我联系**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="1ff5d-142">创建计划</span><span class="sxs-lookup"><span data-stu-id="1ff5d-142">Create your plan</span></span>

<span data-ttu-id="1ff5d-143">在这些步骤中，你将定义你要为产品/服务启用的计划或计划。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="1ff5d-144">在左侧导航菜单中，选择 " **计划概述**"，然后选择 " **创建新计划**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="1ff5d-145">输入 **计划 ID** 和 **计划名称**，然后选择 " **创建**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="1ff5d-146">在 " **计划列表** " 页上，输入 **计划说明**。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="1ff5d-147">若要保存说明并稍后完成，请选择 " **保存草稿**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="1ff5d-148">完成后，请选择 " **查看并发布**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="1ff5d-149">计划信息现在会显示在 appsource.microsoft.com 下的 "产品/服务列表 (计划" 部分) 。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="1ff5d-150">创建了此产品/服务的所有计划后，需要复制每个计划的服务 ID。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="1ff5d-151">选择计划列表页顶部的 " **计划概述** "。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="1ff5d-152">将每个计划的服务 ID 复制到一个安全的位置。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="1ff5d-153">向解决方案添加服务 Id</span><span class="sxs-lookup"><span data-stu-id="1ff5d-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="1ff5d-154">下一步是通过为刚复制的每个计划添加服务 Id 来更新解决方案。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="1ff5d-155">有关此内容的指导，请参阅为 [解决方案创建 AppSource 包](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="1ff5d-156">上传包并发布产品/服务</span><span class="sxs-lookup"><span data-stu-id="1ff5d-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="1ff5d-157">在左侧导航窗格中，选择 " **商用 Marketplace**"，然后选择 " **技术配置**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="1ff5d-158">在 " **基本许可证模型**" 下，选择 " **用户**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="1ff5d-159">在 " **CRM 包**" 下，输入包位置的 URL。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="1ff5d-160">使用左侧导航窗格中的 "其他" 选项卡输入任何其他所需的信息。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="1ff5d-161">完成后，请选择 " **查看并发布**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="1ff5d-162">发布产品/服务后，我们将查看并验证你的信息。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="1ff5d-163">如果此过程有任何问题，我们会通知你。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="1ff5d-164">解决所有问题后，你会收到通知，告知你的产品/服务在 AppSource 中可用。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="1ff5d-165">此时，你可以使其生效。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="1ff5d-166">在合作伙伴中心提供产品/服务</span><span class="sxs-lookup"><span data-stu-id="1ff5d-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="1ff5d-167">以下过程将指导你完成产品/服务的 AppSource。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="1ff5d-168">若要了解有关此过程的详细信息，请参阅 [列表选项简介](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="1ff5d-169">发布产品/服务后，将需要4-6 小时才能投入使用。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="1ff5d-170">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1ff5d-171">在左侧导航菜单中，选择 " **商业 Marketplace/概述**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="1ff5d-172">在 " **概述** " 页上，找到你要查找的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="1ff5d-173">"产品/服务" 的状态为 " **预览**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="1ff5d-174">选择产品/服务。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-174">Select the offer.</span></span>
4. <span data-ttu-id="1ff5d-175">在 **产品/服务概述** 页上 **，选择 "上线"**。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="1ff5d-176">产品/服务将在4-6 小时内推出。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="1ff5d-177">若要查看 AppSource 上的产品/服务列表，请选择 "**产品/服务概述**" 页底部的 " **AppSource** " 链接。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="1ff5d-178">**对于启用许可证的产品/** 服务：如果你的产品/服务需要许可证检查，则用户将只能通过单击 " **与我联系**" 来输入潜在客户，以便可以与他们进行通信。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="1ff5d-179">**对于启用许可证的产品/服务免费安装选项**：如果产品/服务不需要许可证检查，则除了 **与我联系**，管理员用户还将看到 "**立即获取**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="1ff5d-180">如果用户想要尝试 "免费安装" 选项，则应单击 " **立即获取**"，这会使用户在 Power Platform 管理中心上安装产品/服务。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="1ff5d-181">如果用户有任何疑问，或者他们想要升级到付费计划，用户仍然可以使用 " **联系我** "。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="1ff5d-182">注册 DealReg 中的 ISV Connect 交易</span><span class="sxs-lookup"><span data-stu-id="1ff5d-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="1ff5d-183">下一步是注册交易。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-183">The next step is to register your deal.</span></span> <span data-ttu-id="1ff5d-184">为此，请参阅 [注册交易](https://docs.microsoft.com/partner-center/register-deals)。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="1ff5d-185">邀请客户</span><span class="sxs-lookup"><span data-stu-id="1ff5d-185">Invite the customer</span></span>

<span data-ttu-id="1ff5d-186">使用以下过程邀请客户参与此交易。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="1ff5d-187">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1ff5d-188">在左侧导航菜单中，选择 " **商业 Marketplace/概述**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="1ff5d-189">筛选 **提交** 的交易，选择 " **正在进行** " 选项卡，然后选择所需的交易。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="1ff5d-190">在此交易的 "概述" 页上，选择 " **管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="1ff5d-191">在 " **管理许可证** " 窗口中，从 " **客户详细信息** " 下拉列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="1ff5d-192">如果客户关系尚不存在，请选择 " **+ 邀请新客户同意**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="1ff5d-193">复制显示的链接。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="1ff5d-194">通过电子邮件将此链接发送到客户的帐单管理员或全局管理员，并让他们使用此链接访问 admin.microsoft.com，并接受并授权您正在建立的关系。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="1ff5d-195">在客户执行此步骤之前，将不会建立关系。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="1ff5d-196">激活、管理和删除你的许可证</span><span class="sxs-lookup"><span data-stu-id="1ff5d-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="1ff5d-197">建立客户后，可以开始从产品/服务添加计划并将许可证分配给每个计划。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="1ff5d-198">在此交易的 "管理许可证" 窗口中，选择 " **+ 添加计划**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="1ff5d-199">完成 **此解决方案的计划** 和 **许可证字段数量** ，然后选择 " **更新许可证**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="1ff5d-200">许可证将在 admin.microsoft.com 上提供，供客户管理并分配给员工。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="1ff5d-201">若要更改现有计划的许可证数量，请在 " **许可证数** " 字段中输入新编号，然后选择 " **更新许可证**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="1ff5d-202">若要停用或删除交易的许可证，请在 " **操作** " 字段中选择垃圾桶图标，然后选择 " **更新许可证**"。</span><span class="sxs-lookup"><span data-stu-id="1ff5d-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>