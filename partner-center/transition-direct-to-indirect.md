---
title: 将直接帐单合作伙伴切换到间接经销商
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解云解决方案提供商如何 (CSP) 计划合作伙伴可以使用合作伙伴中心从直接计费合作伙伴过渡到间接经销商。
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 205451a1c42c6538936df49ba8a4314372a94082
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112490047"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="16b59-103">从云解决方案提供商 (CSP) 计划直接计费合作伙伴过渡到云解决方案提供商计划间接经销商</span><span class="sxs-lookup"><span data-stu-id="16b59-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="16b59-104">**相应的角色**：全局管理员</span><span class="sxs-lookup"><span data-stu-id="16b59-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="16b59-105">本文适用于已决定过渡到间接经销商的直销合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="16b59-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="16b59-106">但是，即使尚未做出明确的决定作为间接经销商注册，Microsoft 在其[直接帐单功能受到限制](restricted-direct-bill-capabilities.md)的情况下，如果不符合 CSP 直销合作伙伴计划的新[要求](direct-partner-new-requirements.md)，他们也会收到通知。</span><span class="sxs-lookup"><span data-stu-id="16b59-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="16b59-107">从2021年1月起，将添加新的收入要求。</span><span class="sxs-lookup"><span data-stu-id="16b59-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="16b59-108">注册为直接帐单合作伙伴的合作伙伴将需要在前12个月内，以合作伙伴全局帐户级别至少在30万个的 CSP 计划收入中进行交易。</span><span class="sxs-lookup"><span data-stu-id="16b59-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in CSP program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="16b59-109">你将能够使用现有的直属帐单租户注册间接经销商计划。</span><span class="sxs-lookup"><span data-stu-id="16b59-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="16b59-110">入门</span><span class="sxs-lookup"><span data-stu-id="16b59-110">Get started</span></span>

1. <span data-ttu-id="16b59-111">请确保合作伙伴中心的合作伙伴配置文件与 Microsoft 合作伙伴网络 (MPN) ID 是最新的。</span><span class="sxs-lookup"><span data-stu-id="16b59-111">Make sure your partner profile in Partner Center and Microsoft Partner Network (MPN) ID are current.</span></span>

2. <span data-ttu-id="16b59-112">以要过渡到间接经销商的直接帐单租户的全局管理员身份登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="16b59-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="叙述.":::

3. <span data-ttu-id="16b59-114">查看有关注册窗体的合作伙伴详细信息。</span><span class="sxs-lookup"><span data-stu-id="16b59-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="立即注册。":::

4. <span data-ttu-id="16b59-116">选择“立即注册”。</span><span class="sxs-lookup"><span data-stu-id="16b59-116">Select Enroll now.</span></span> <span data-ttu-id="16b59-117">你的间接经销商企业将使用与你用于直接业务的) 租户相同的 Microsoft Azure Active Directory (Azure AD。</span><span class="sxs-lookup"><span data-stu-id="16b59-117">Your indirect reseller business will use the same Microsoft Azure Active Directory (Azure AD) tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="16b59-118">最初，这一新的转换功能将在9月1日至12月1日的合作伙伴提供。</span><span class="sxs-lookup"><span data-stu-id="16b59-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="16b59-119">如果你在9月到12月之间没有周年纪念日期，此时你将看不到此功能。</span><span class="sxs-lookup"><span data-stu-id="16b59-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="16b59-120">如果为合作伙伴启用了该功能，则将在以后收到包含周年纪念2018的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="16b59-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="16b59-121">批准注册后，再次登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="16b59-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="16b59-122">尽管批准通常是即时的，但最多可能需要五个工作日内。</span><span class="sxs-lookup"><span data-stu-id="16b59-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="16b59-123">批准后，你将收到一个通知，告知你已在 "注册" 表单中的 "主要联系人" 下指定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="16b59-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="16b59-124">你还可以在 "设置" "   >  **帐户设置**" "  >  **合作伙伴配置文件**> 程序信息" 下查看你的注册状态。</span><span class="sxs-lookup"><span data-stu-id="16b59-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="16b59-125">在 " **概述** " 页上，你将看到间接经销商协议。</span><span class="sxs-lookup"><span data-stu-id="16b59-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="16b59-126">选择 **接受并继续操作**。</span><span class="sxs-lookup"><span data-stu-id="16b59-126">Select **Accept and continue**.</span></span> <span data-ttu-id="16b59-127">此操作启用间接分销商功能。</span><span class="sxs-lookup"><span data-stu-id="16b59-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="16b59-128">当你接受间接经销商协议后，你会注意到你的合作伙伴配置文件 **将你标识为直接** 帐单和间接经销商。</span><span class="sxs-lookup"><span data-stu-id="16b59-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="间接分销商协议。":::

> [!IMPORTANT]
> <span data-ttu-id="16b59-130">使用新功能将注册为间接经销商后，就不会将任何选项回滚到仅限帐单的租户。</span><span class="sxs-lookup"><span data-stu-id="16b59-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="16b59-131">注册为间接经销商之前，请确保完全评估你的业务需求。</span><span class="sxs-lookup"><span data-stu-id="16b59-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="16b59-132">从直接过渡到间接经销商时</span><span class="sxs-lookup"><span data-stu-id="16b59-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="16b59-133">在此阶段，你将继续管理直接客户的订阅需求，包括计费过程。</span><span class="sxs-lookup"><span data-stu-id="16b59-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="16b59-134">你还可以开始接受来自间接提供商的客户，并以间接经销商的身份运行。</span><span class="sxs-lookup"><span data-stu-id="16b59-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="你既是直接帐单也是间接经销商。":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="16b59-136">查找间接提供商</span><span class="sxs-lookup"><span data-stu-id="16b59-136">Find an indirect provider</span></span>

<span data-ttu-id="16b59-137">注册后，指向间接提供程序的链接将显示在左侧导航栏中。</span><span class="sxs-lookup"><span data-stu-id="16b59-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="16b59-138">作为间接经销商，您将建立与间接提供商的关系，然后可以处理您的帐单、为客户购买产品并支持基础结构。</span><span class="sxs-lookup"><span data-stu-id="16b59-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="16b59-139">不同的间接提供商会提供不同的支持和服务，因此你应该评估所在地区的提供商，确定哪些提供商最能够满足你的需求。</span><span class="sxs-lookup"><span data-stu-id="16b59-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="16b59-140">通常，大多数提供商将：</span><span class="sxs-lookup"><span data-stu-id="16b59-140">Generally, most providers will:</span></span>

- <span data-ttu-id="16b59-141">为你提供技术培训和援助</span><span class="sxs-lookup"><span data-stu-id="16b59-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="16b59-142">帮助你推销产品和服务</span><span class="sxs-lookup"><span data-stu-id="16b59-142">Help you market your products and services</span></span>
- <span data-ttu-id="16b59-143">管理你的融资和信贷条款</span><span class="sxs-lookup"><span data-stu-id="16b59-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="16b59-144">搜索官方 [Microsoft 间接提供程序](https://partnercenter.microsoft.com/partner/find-a-provider)列表。</span><span class="sxs-lookup"><span data-stu-id="16b59-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="16b59-145">了解更多，  [通过间接提供商阅读合作伙伴](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="16b59-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="16b59-146">接受来自间接提供商的合作邀请邀请</span><span class="sxs-lookup"><span data-stu-id="16b59-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="16b59-147">查找与合作伙伴合作的间接提供程序时，与合作伙伴中心的间接提供商建立合作关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="16b59-148">你选择的间接提供程序会向你发送电子邮件合作伙伴邀请链接，该链接会将你带到合作伙伴中心的邀请。</span><span class="sxs-lookup"><span data-stu-id="16b59-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="16b59-149">请确保你的全局管理员登录到合作伙伴中心并按照邀请链接进行。</span><span class="sxs-lookup"><span data-stu-id="16b59-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="16b59-150">接受邀请后，提供者的名称将出现在间接提供程序列表中。</span><span class="sxs-lookup"><span data-stu-id="16b59-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="16b59-151">作为间接经销商购买新客户</span><span class="sxs-lookup"><span data-stu-id="16b59-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="16b59-152">你和你的间接提供商都需要与客户建立分销商关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="16b59-153">利用这些分销商关系，你可以代表客户管理客户的订阅和服务。</span><span class="sxs-lookup"><span data-stu-id="16b59-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="16b59-154">若要获取现有 Azure AD 租户的新客户，可以邀请客户同时与您和您的提供商建立分销商关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="16b59-155">若要创建间接经销商邀请：</span><span class="sxs-lookup"><span data-stu-id="16b59-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="16b59-156">从合作伙伴中心左侧导航栏中选择 " **间接提供程序** "。</span><span class="sxs-lookup"><span data-stu-id="16b59-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="16b59-157">选择“邀请新客户”以邀请客户同时与你和间接提供商建立经销商关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="16b59-158">提供商需要与客户建立分销商关系，因此，当客户想要购买新订阅或向现有订阅添加新许可证时，他们可以代表客户提交订单。</span><span class="sxs-lookup"><span data-stu-id="16b59-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="16b59-159">在下一页上，查看草稿电子邮件。</span><span class="sxs-lookup"><span data-stu-id="16b59-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="16b59-160">可以通过电子邮件打开草稿邮件，也可以将邮件复制到剪贴板，然后将其粘贴到电子邮件中。</span><span class="sxs-lookup"><span data-stu-id="16b59-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="16b59-161">编辑电子邮件中的文本以说明所需内容，但请确保在个性化的同时将该链接连接到帐户和提供商的帐户。</span><span class="sxs-lookup"><span data-stu-id="16b59-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="16b59-162">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="16b59-162">Then select **Done**.</span></span>

5. <span data-ttu-id="16b59-163">客户准许你和你的提供商成为其备案经销商后，你将拥有管理员权限，可以代表他们管理其订阅、许可证和用户，并且你的间接提供商将能够代表他们提交订单。</span><span class="sxs-lookup"><span data-stu-id="16b59-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="16b59-164">若要管理客户的帐户、服务、用户和许可证，请选择客户名称旁边的向下箭头，展开客户的记录。</span><span class="sxs-lookup"><span data-stu-id="16b59-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="16b59-165">与直属合作方不同，间接经销商无法为合作伙伴中心的新客户创建 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="16b59-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="16b59-166">你的提供程序将创建租户，并将你指定为此客户的间接分销商。</span><span class="sxs-lookup"><span data-stu-id="16b59-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="16b59-167">这可确保客户将显示在合作伙伴中心的客户列表中。</span><span class="sxs-lookup"><span data-stu-id="16b59-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="16b59-168">你将不能使用直接帐单功能为你作为间接经销商购买的客户创建采购。</span><span class="sxs-lookup"><span data-stu-id="16b59-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="16b59-169">管理直接帐单客户和间接经销商客户</span><span class="sxs-lookup"><span data-stu-id="16b59-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="16b59-170">你可以用不同的方式管理直接帐单客户和间接经销商客户。</span><span class="sxs-lookup"><span data-stu-id="16b59-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="16b59-171">直接向客户收费 (你不会作为间接经销商) </span><span class="sxs-lookup"><span data-stu-id="16b59-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="16b59-172">为产品创建订单</span><span class="sxs-lookup"><span data-stu-id="16b59-172">Create orders for products</span></span>
- <span data-ttu-id="16b59-173">管理 Azure 预留项</span><span class="sxs-lookup"><span data-stu-id="16b59-173">Manage Azure reservations</span></span>
- <span data-ttu-id="16b59-174">管理其订单历史记录</span><span class="sxs-lookup"><span data-stu-id="16b59-174">Manage their order history</span></span>
- <span data-ttu-id="16b59-175">购买软件</span><span class="sxs-lookup"><span data-stu-id="16b59-175">Purchase software</span></span>
- <span data-ttu-id="16b59-176">直接向客户收费</span><span class="sxs-lookup"><span data-stu-id="16b59-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="16b59-177">间接经销商客户</span><span class="sxs-lookup"><span data-stu-id="16b59-177">Indirect reseller customers</span></span>

- <span data-ttu-id="16b59-178">你的间接提供商为你的客户订购产品</span><span class="sxs-lookup"><span data-stu-id="16b59-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="16b59-179">管理客户的许可证和用户</span><span class="sxs-lookup"><span data-stu-id="16b59-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="16b59-180">处理订阅续订</span><span class="sxs-lookup"><span data-stu-id="16b59-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="16b59-181">确定作为直销合作伙伴获得的客户</span><span class="sxs-lookup"><span data-stu-id="16b59-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="16b59-182">选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="16b59-182">Select **Customers**.</span></span>

2. <span data-ttu-id="16b59-183">选择要查看其详细信息的客户。</span><span class="sxs-lookup"><span data-stu-id="16b59-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="16b59-184">如果此客户是你作为直销合作伙伴获得的客户，你将看到 **添加** 或 **查看产品** 的选项，你将看到其订阅。</span><span class="sxs-lookup"><span data-stu-id="16b59-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="16b59-185">如果客户与你有间接的分销商关系，这些选项将不可用。</span><span class="sxs-lookup"><span data-stu-id="16b59-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="16b59-186">将直接帐单客户移动到间接提供商</span><span class="sxs-lookup"><span data-stu-id="16b59-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="16b59-187">你的间接提供商不能提交订单或现有直销客户的现有订阅转移，直到他们与他们建立了分销商关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="16b59-188">若要建立间接提供商与现有直销客户之间的分销商关系，可以使用以下方法之一：</span><span class="sxs-lookup"><span data-stu-id="16b59-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="16b59-189">分销商关系扩展</span><span class="sxs-lookup"><span data-stu-id="16b59-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="16b59-190">向客户发送间接经销商邀请</span><span class="sxs-lookup"><span data-stu-id="16b59-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="16b59-191">可以在 "[直接到间接转换" 文档](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)中找到循序渐进过程的详细概述</span><span class="sxs-lookup"><span data-stu-id="16b59-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="16b59-192">分销商关系扩展</span><span class="sxs-lookup"><span data-stu-id="16b59-192">Reseller relationship extension</span></span>

<span data-ttu-id="16b59-193">你可以使用分销商关系扩展功能，通过合作伙伴中心仪表板建立现有直销客户和间接提供商之间的分销商关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="16b59-194">使用此功能之前，请注意以下事项：</span><span class="sxs-lookup"><span data-stu-id="16b59-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="16b59-195">此功能仅适用于正在转换为间接经销商完成 [间接经销商注册](#get-started)的直接帐单合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="16b59-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="16b59-196">只能将此功能应用于现有的直属帐单客户。</span><span class="sxs-lookup"><span data-stu-id="16b59-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="16b59-197">它不适用于 [间接经销商客户](#acquire-new-customers-as-indirect-reseller)。</span><span class="sxs-lookup"><span data-stu-id="16b59-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="16b59-198">你只能选择已 [接受间接提供商提供的合作伙伴邀请](#accept-a-partnership-invitation-from-your-indirect-provider)的间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="16b59-199">您对此客户的帐单信息的副本将提供给间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="16b59-200">你可以通过访问合作伙伴中心仪表板中此客户的帐户页来访问帐单信息。</span><span class="sxs-lookup"><span data-stu-id="16b59-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="16b59-201">通过使用经销商关系扩展功能，即表示你同意与间接提供商共享此客户的计费方式信息。</span><span class="sxs-lookup"><span data-stu-id="16b59-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="16b59-202">不会向间接提供商提供 [客户租户的](customers-revoke-admin-privileges.md) 委派管理权限。</span><span class="sxs-lookup"><span data-stu-id="16b59-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="16b59-203">如果间接提供商需要委派的管理权限，则必须改为向客户发送间接经销商邀请。</span><span class="sxs-lookup"><span data-stu-id="16b59-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="16b59-204">建立经销商关系后，间接提供商将在 Microsoft 365[管理](https://admin.microsoft.com/AdminPortal/Home#/partners)中心的"合作伙伴关系"页下显示为客户的 CSP[适用于企业的 Microsoft Store。](/microsoft-store/work-with-partner-microsoft-store-business)</span><span class="sxs-lookup"><span data-stu-id="16b59-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="16b59-205">为了避免混淆和误解，在使用关系扩展功能在现有的直接计费客户和间接提供商之间建立经销商关系之前，合作伙伴协议会要求你通知并获取直接计费客户的同意。</span><span class="sxs-lookup"><span data-stu-id="16b59-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="16b59-206">若要在现有的客户租户上使用此功能，请：</span><span class="sxs-lookup"><span data-stu-id="16b59-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="16b59-207">以管理员合作伙伴中心登录到 **。**</span><span class="sxs-lookup"><span data-stu-id="16b59-207">Sign in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="16b59-208">在" **客户"** 页中，选择现有客户并选择其" **快速链接** "图标以展开客户的摘要视图。</span><span class="sxs-lookup"><span data-stu-id="16b59-208">In the **Customers page**, select an existing customer and select its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="16b59-209">在 **"间接提供商 (") "，** 选择"在间接 **提供商上转移客户"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-209">Under **Indirect provider(s)**, select **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="将客户转移到间接提供商。":::

4. <span data-ttu-id="16b59-211">在弹出对话框中，选择要与客户建立经销商关系的间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="16b59-212">选择“保存并继续”。 </span><span class="sxs-lookup"><span data-stu-id="16b59-212">Select **Save and continue**.</span></span>

6. <span data-ttu-id="16b59-213">验证所选间接提供商是否显示在"间接提供商" (**下) 。**</span><span class="sxs-lookup"><span data-stu-id="16b59-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="列出的间接提供商。":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="16b59-215">向客户发送间接经销商邀请</span><span class="sxs-lookup"><span data-stu-id="16b59-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="16b59-216">在间接提供商与现有的直接计费客户建立经销商关系之前，他们无法提交订单。</span><span class="sxs-lookup"><span data-stu-id="16b59-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="16b59-217">若要在现有客户与间接提供商之间建立经销商关系，请通过间接经销商邀请邀请客户。</span><span class="sxs-lookup"><span data-stu-id="16b59-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="16b59-218">从 **左侧导航导航** 合作伙伴中心间接提供商"。</span><span class="sxs-lookup"><span data-stu-id="16b59-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="16b59-219">选择“邀请新客户”以邀请客户同时与你和间接提供商建立经销商关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="16b59-220">提供商需要与客户建立经销商关系，以便客户想要购买新订阅或将新许可证添加到现有订阅时，可以代表客户提交订单。</span><span class="sxs-lookup"><span data-stu-id="16b59-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="邀请新客户。":::

3. <span data-ttu-id="16b59-222">在下一页上，查看草稿电子邮件。</span><span class="sxs-lookup"><span data-stu-id="16b59-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="16b59-223">可以在电子邮件中打开草稿消息，也可以将邮件复制到剪贴板并将其粘贴到电子邮件中。</span><span class="sxs-lookup"><span data-stu-id="16b59-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="16b59-224">编辑电子邮件中的文本，以说明所需的内容，但请务必包含该链接，因为它已个性化，可将客户直接连接到帐户和提供商的帐户。</span><span class="sxs-lookup"><span data-stu-id="16b59-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="16b59-225">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="16b59-225">Then select **Done**.</span></span>

5. <span data-ttu-id="16b59-226">客户准许你和你的提供商成为其备案经销商后，你将拥有管理员权限，可以代表他们管理其订阅、许可证和用户，并且你的间接提供商将能够代表他们提交订单。</span><span class="sxs-lookup"><span data-stu-id="16b59-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="16b59-227">若要管理客户的帐户、服务、用户和许可证，请选择客户名称旁边的向下箭头，展开客户的记录。</span><span class="sxs-lookup"><span data-stu-id="16b59-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="16b59-228">Microsoft 客户协议接受</span><span class="sxs-lookup"><span data-stu-id="16b59-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="16b59-229">Microsoft 云协议有效期至 2020 年 1 月 31 日。</span><span class="sxs-lookup"><span data-stu-id="16b59-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="16b59-230">在此日期之后，所有现有客户和新客户都必须对新的[Microsoft 客户协议。](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="16b59-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="16b59-231">对于过渡客户，如果：</span><span class="sxs-lookup"><span data-stu-id="16b59-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="16b59-232">**客户尚未接受Microsoft 客户协议**</span><span class="sxs-lookup"><span data-stu-id="16b59-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="16b59-233">请与间接提供商合作，使[客户接受Microsoft 客户协议。](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="16b59-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="16b59-234">**客户已Microsoft 客户协议管理中心Microsoft 365你**</span><span class="sxs-lookup"><span data-stu-id="16b59-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="16b59-235">与间接提供商建立经销商关系后，将保留接受。</span><span class="sxs-lookup"><span data-stu-id="16b59-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="16b59-236">无需执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="16b59-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="16b59-237">**客户已Microsoft 客户协议合作伙伴证明与用户联系**</span><span class="sxs-lookup"><span data-stu-id="16b59-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="16b59-238">不会保留接受。</span><span class="sxs-lookup"><span data-stu-id="16b59-238">The acceptance will not be retained.</span></span> <span data-ttu-id="16b59-239">请与间接提供商合作[，在 中更新客户的合作伙伴中心。](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)</span><span class="sxs-lookup"><span data-stu-id="16b59-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="16b59-240">将现有的直接计费订阅转移到间接提供商</span><span class="sxs-lookup"><span data-stu-id="16b59-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="16b59-241">在 CSP 间接模型中，间接经销商与 Microsoft 没有计费关系。</span><span class="sxs-lookup"><span data-stu-id="16b59-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="16b59-242">相反，间接经销商通过间接提供商获取客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="16b59-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="16b59-243">从直接计费合作伙伴过渡到间接经销商时，需要将作为直接计费合作伙伴的现有订阅转移到间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="16b59-244">可以使用仪表板中的自助服务订阅合作伙伴中心功能。</span><span class="sxs-lookup"><span data-stu-id="16b59-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="16b59-245">先决条件</span><span class="sxs-lookup"><span data-stu-id="16b59-245">Prerequisites</span></span>

- <span data-ttu-id="16b59-246">此功能仅适用于已使用其现有直接计费合作伙伴租户完成间接经销商注册的过渡合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="16b59-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="16b59-247">在转移与给定客户关联的订阅之前，过渡合作伙伴必须将客户转移到间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="16b59-248">客户必须已 [Microsoft 客户协议间接提供商 接受该请求](#microsoft-customer-agreement-acceptance)。</span><span class="sxs-lookup"><span data-stu-id="16b59-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="16b59-249">如何过渡到间接经销商状态</span><span class="sxs-lookup"><span data-stu-id="16b59-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="16b59-250">此功能是一个四步过程，其中：</span><span class="sxs-lookup"><span data-stu-id="16b59-250">The feature is a four-step process, where:</span></span>

- <span data-ttu-id="16b59-251">过渡合作伙伴创建订阅转移请求。</span><span class="sxs-lookup"><span data-stu-id="16b59-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="16b59-252">该请求包含一个或多个与同一客户关联的现有订阅，并针对间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="16b59-253">间接提供商审核并接受 (或拒绝) 请求。</span><span class="sxs-lookup"><span data-stu-id="16b59-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="16b59-254">间接提供商验证转移请求是否已完成。</span><span class="sxs-lookup"><span data-stu-id="16b59-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="16b59-255">转换伙伴将验证传输请求是否已完成。</span><span class="sxs-lookup"><span data-stu-id="16b59-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="16b59-256">过渡合作伙伴</span><span class="sxs-lookup"><span data-stu-id="16b59-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="16b59-257">还可使用 合作伙伴中心 [API/SDK](/partner-center/develop/manage-customers) 将现有订阅转移到间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="16b59-258">获取客户的订阅转让资格</span><span class="sxs-lookup"><span data-stu-id="16b59-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="16b59-259">创建客户的转让</span><span class="sxs-lookup"><span data-stu-id="16b59-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="16b59-260">撤消客户的转让</span><span class="sxs-lookup"><span data-stu-id="16b59-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="16b59-261">接受客户的转让</span><span class="sxs-lookup"><span data-stu-id="16b59-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="16b59-262">拒绝客户的转让</span><span class="sxs-lookup"><span data-stu-id="16b59-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="16b59-263">获取客户的转让</span><span class="sxs-lookup"><span data-stu-id="16b59-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="16b59-264">按 ID 获取传输详细信息</span><span class="sxs-lookup"><span data-stu-id="16b59-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="16b59-265">转换合作伙伴 - 创建转移请求</span><span class="sxs-lookup"><span data-stu-id="16b59-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="16b59-266">若要创建转移请求作为转换伙伴，请完成以下过程：</span><span class="sxs-lookup"><span data-stu-id="16b59-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="16b59-267">以管理员合作伙伴中心登录到 **。**</span><span class="sxs-lookup"><span data-stu-id="16b59-267">Sign in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="16b59-268">在 **"客户** "页中，选择目标客户，然后选择"快速链接"图标以展开客户的摘要视图。</span><span class="sxs-lookup"><span data-stu-id="16b59-268">In the **Customers** page, select the intended customer and select the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="16b59-269">在 **"间接 (") "** 下，确认已列出预期的间接提供商。</span><span class="sxs-lookup"><span data-stu-id="16b59-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="16b59-270">选择 **"查看订阅"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-270">Select **View Subscriptions**.</span></span>

5. <span data-ttu-id="16b59-271">在"**订阅"** 页中，查找"**订阅转移"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="16b59-272">在"**订阅转移"** 下，选择 **"请求订阅转移"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-272">Under **Subscription Transfer**, select **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="请求订阅转移。":::

7. <span data-ttu-id="16b59-274">在"转移请求"对话框中，选择要转移的一个或多个订阅。</span><span class="sxs-lookup"><span data-stu-id="16b59-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="创建传输请求。":::

8. <span data-ttu-id="16b59-276">选择“创建”  。</span><span class="sxs-lookup"><span data-stu-id="16b59-276">Select **Create**.</span></span>

9. <span data-ttu-id="16b59-277">活动订阅转移请求将显示在"订阅转移 **"下**。</span><span class="sxs-lookup"><span data-stu-id="16b59-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="传输请求列表。":::

10. <span data-ttu-id="16b59-279">告知间接提供商你已创建其订阅转移请求。</span><span class="sxs-lookup"><span data-stu-id="16b59-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="16b59-280">间接提供商 - 接受转移请求</span><span class="sxs-lookup"><span data-stu-id="16b59-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="16b59-281">查看并接受作为间接提供商的转移请求：</span><span class="sxs-lookup"><span data-stu-id="16b59-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="16b59-282">以管理员合作伙伴中心 **或销售\*\*\*\*代理登录**。</span><span class="sxs-lookup"><span data-stu-id="16b59-282">Sign in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="16b59-283">在" **客户** "页中，选择目标客户并选择其"快速链接"图标以展开客户的摘要视图。</span><span class="sxs-lookup"><span data-stu-id="16b59-283">In the **Customers** page, select the intended customer and select its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="16b59-284">在 **"间接 () "** 下，确认已列出过渡合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="16b59-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="16b59-285">选择 **"查看订阅"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-285">Select **View Subscriptions**.</span></span>

5. <span data-ttu-id="16b59-286">在"**订阅"** 页中，查找"**订阅转移"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="查看传输请求。":::

6. <span data-ttu-id="16b59-288">在 **"订阅转移**"下，选择要审阅的转移请求。</span><span class="sxs-lookup"><span data-stu-id="16b59-288">Under **Subscription Transfer**, select the transfer request to review.</span></span>

7. <span data-ttu-id="16b59-289">选择" ("，) 选择"拒绝"。</span><span class="sxs-lookup"><span data-stu-id="16b59-289">Select **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="接受转移请求。":::

8. <span data-ttu-id="16b59-291">等待传输请求完成。</span><span class="sxs-lookup"><span data-stu-id="16b59-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="16b59-292">间接提供商 - 验证转移请求是否已完成</span><span class="sxs-lookup"><span data-stu-id="16b59-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="16b59-293">成功完成转移请求后，验证订阅是否显示在"订阅 **"下**。</span><span class="sxs-lookup"><span data-stu-id="16b59-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="16b59-294">通知过渡合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="16b59-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="16b59-295">转换合作伙伴 - 验证转移请求是否已完成</span><span class="sxs-lookup"><span data-stu-id="16b59-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="16b59-296">过渡伙伴应执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="16b59-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="16b59-297">以管理员合作伙伴中心 **或销售代理\*\*\*\*登录**。</span><span class="sxs-lookup"><span data-stu-id="16b59-297">Sign in to Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="16b59-298">在 **"客户** "页中，选择目标客户，然后选择" **快速** 链接"图标以展开客户的摘要视图。</span><span class="sxs-lookup"><span data-stu-id="16b59-298">In the **Customers** page, select the intended customer and select the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="16b59-299">选择 **"查看订阅"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-299">Select **View Subscriptions**.</span></span>

4. <span data-ttu-id="16b59-300">在"**订阅"** 页中，查找"**订阅转移"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="16b59-301">验证传输请求是否标记为"完成 **"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="16b59-302">验证订阅 () 在"订阅"页中是否 **不再** 显示为活动状态：</span><span class="sxs-lookup"><span data-stu-id="16b59-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="16b59-303">如果这是 MS-AZR-0145P (Azure 订阅，) 将不再列出。</span><span class="sxs-lookup"><span data-stu-id="16b59-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="16b59-304">如果这是 Office 365、 (Dynamics、Intune) 的基于许可证的订阅，则其状态将列为"已 **挂起"。**</span><span class="sxs-lookup"><span data-stu-id="16b59-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="订阅已挂起。":::

### <a name="considerations"></a><span data-ttu-id="16b59-306">注意事项</span><span class="sxs-lookup"><span data-stu-id="16b59-306">Considerations</span></span>

- <span data-ttu-id="16b59-307">**转移后，订阅 ID 会有所不同。**</span><span class="sxs-lookup"><span data-stu-id="16b59-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="16b59-308">如果它是 Azure 订阅 (MS-AZR-0145P) ，则它将具有 Azure 订阅 ID，该 ID 保留自以前的所有者，并且将显示在 Azure 管理门户中。</span><span class="sxs-lookup"><span data-stu-id="16b59-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="16b59-309">**多个转移请求不能引用同一订阅。**</span><span class="sxs-lookup"><span data-stu-id="16b59-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="16b59-310">创建包含现有订阅的转移请求后，在取消第一个转移请求之前，无法创建包含同一订阅的其他转移请求。</span><span class="sxs-lookup"><span data-stu-id="16b59-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="16b59-311">**基于许可证的订阅的加载项必须连同其基本订阅一起转移。**</span><span class="sxs-lookup"><span data-stu-id="16b59-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="16b59-312">创建转移请求时，如果选取具有一个或多个加载项的现有订阅，则加载项将自动包含在转移请求中。</span><span class="sxs-lookup"><span data-stu-id="16b59-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="16b59-313">**订阅的许可证计数更改不会反映在现有转移请求中。**</span><span class="sxs-lookup"><span data-stu-id="16b59-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="16b59-314">创建包含现有订阅的转移请求后，应避免更新订阅的许可证数量 (或关联的加载项) 。</span><span class="sxs-lookup"><span data-stu-id="16b59-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="16b59-315">如果这样做，新数量将不会反映在转移请求中。</span><span class="sxs-lookup"><span data-stu-id="16b59-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="16b59-316">间接提供商接受转移请求后，最终的订阅将具有旧数量。</span><span class="sxs-lookup"><span data-stu-id="16b59-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="16b59-317">如果希望将新数量转移到间接提供商，则必须取消现有转移请求并重新创建一个新请求。</span><span class="sxs-lookup"><span data-stu-id="16b59-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="16b59-318">**并非所有购买都可以使用自助订阅转让进行转移。**</span><span class="sxs-lookup"><span data-stu-id="16b59-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="16b59-319">目前，只能使用此功能将 O365 订阅和 Azure PAYG (MS-AZR-0145P) 转移。</span><span class="sxs-lookup"><span data-stu-id="16b59-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="16b59-320">不支持其他购买，包括 Azure 计划、Azure 预留实例、基于期限的订阅和适用于 Azure 市场 SaaS 订阅。</span><span class="sxs-lookup"><span data-stu-id="16b59-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="16b59-321">你将在提交转移请求页中看到无法转移订阅的原因。</span><span class="sxs-lookup"><span data-stu-id="16b59-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="16b59-322">若要转移这些订阅，需要取消现有订阅，[](create-a-new-subscription.md#suspend-or-cancel-a-subscription)并通过间接提供商为客户购买新产品/服务。</span><span class="sxs-lookup"><span data-stu-id="16b59-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="16b59-323">**无法使用沙盒环境进行测试。**</span><span class="sxs-lookup"><span data-stu-id="16b59-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="16b59-324">注册间接经销商奖励</span><span class="sxs-lookup"><span data-stu-id="16b59-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="16b59-325">在现有的直接计费合作伙伴租户上成功注册为间接经销商后，你将收到在 30 天内注册间接经销商奖励的邀请。</span><span class="sxs-lookup"><span data-stu-id="16b59-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="16b59-326">邀请基于当前与 CSP 合作伙伴租户关联的合作伙伴 MPN 帐户。</span><span class="sxs-lookup"><span data-stu-id="16b59-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="16b59-327">邀请将发送到与合作伙伴 MPN 帐户关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="16b59-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="16b59-328">你还有资格注册同一合作伙伴租户的直接帐单奖励计划。</span><span class="sxs-lookup"><span data-stu-id="16b59-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="16b59-329">必须单独管理程序。</span><span class="sxs-lookup"><span data-stu-id="16b59-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="16b59-330">后续步骤</span><span class="sxs-lookup"><span data-stu-id="16b59-330">Next steps</span></span>

- [<span data-ttu-id="16b59-331">成为间接经销商的其他信息</span><span class="sxs-lookup"><span data-stu-id="16b59-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="16b59-332">云解决方案提供商计划直接合作伙伴新要求</span><span class="sxs-lookup"><span data-stu-id="16b59-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="16b59-333">受限的直接计费功能</span><span class="sxs-lookup"><span data-stu-id="16b59-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
