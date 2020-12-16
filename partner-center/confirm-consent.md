---
title: 确认客户接受 Microsoft 客户协议
description: 了解如何确认客户接受 Microsoft 客户协议。 为客户订购 Microsoft 产品和服务时，可能需要这样做。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354604"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="1bcfc-104">确认客户已接受 Microsoft 客户协议的已更新方法</span><span class="sxs-lookup"><span data-stu-id="1bcfc-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="1bcfc-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="1bcfc-105">**Appropriate roles**</span></span>

- <span data-ttu-id="1bcfc-106">管理员代理</span><span class="sxs-lookup"><span data-stu-id="1bcfc-106">Admin agent</span></span>
- <span data-ttu-id="1bcfc-107">销售代理</span><span class="sxs-lookup"><span data-stu-id="1bcfc-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="1bcfc-108">目前，协议资源仅受 Microsoft 公有云中合作伙伴中心的支持。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="1bcfc-109">它不适用于：</span><span class="sxs-lookup"><span data-stu-id="1bcfc-109">It is not applicable to:</span></span>
> * <span data-ttu-id="1bcfc-110">由世纪互联运营的合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1bcfc-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="1bcfc-111">德国 Microsoft 云合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1bcfc-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="1bcfc-112">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1bcfc-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="1bcfc-113">从 2020 年 1 月 31 日起，所有客户（无论是现有客户还是新客户）都必须签署新的 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="1bcfc-114">若要了解详细信息，请参阅[确认客户接受 Microsoft 客户协议](confirm-customer-agreement.md)。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="1bcfc-115">作为合作伙伴，你需要在为客户订购 Microsoft 产品和服务之前确认该客户接受了 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="1bcfc-116">为了更好地帮助合作伙伴满足合规性要求，Microsoft 要求合作伙伴通过提供有关接受协议人员的以下详细信息来确认接受协议：</span><span class="sxs-lookup"><span data-stu-id="1bcfc-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="1bcfc-117">名字</span><span class="sxs-lookup"><span data-stu-id="1bcfc-117">First name</span></span>

- <span data-ttu-id="1bcfc-118">姓氏</span><span class="sxs-lookup"><span data-stu-id="1bcfc-118">Last name</span></span>

- <span data-ttu-id="1bcfc-119">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="1bcfc-119">Email address</span></span>

- <span data-ttu-id="1bcfc-120">电话号码（可选）</span><span class="sxs-lookup"><span data-stu-id="1bcfc-120">Phone number (optional)</span></span>

- <span data-ttu-id="1bcfc-121">接受日期</span><span class="sxs-lookup"><span data-stu-id="1bcfc-121">Date of acceptance</span></span>

<span data-ttu-id="1bcfc-122">直接计费合作伙伴和间接提供商在通过合作伙伴中心或合作伙伴中心 API 进行交易时必须确认客户接受了 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="1bcfc-123">“确认”为必选项。 </span><span class="sxs-lookup"><span data-stu-id="1bcfc-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="1bcfc-124">如果没有为给定客户提供确认：</span><span class="sxs-lookup"><span data-stu-id="1bcfc-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="1bcfc-125">你将无法为此客户创建新订单。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="1bcfc-126">你无法为此客户更改现有基于许可证的订阅的许可证计数。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="1bcfc-127">可以通过合作伙伴中心或合作伙伴中心 API 确认客户接受。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="1bcfc-128">若要通过合作伙伴中心 API 执行此操作，请参阅以下主题：</span><span class="sxs-lookup"><span data-stu-id="1bcfc-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="1bcfc-129">获取客户同意的确认</span><span class="sxs-lookup"><span data-stu-id="1bcfc-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="1bcfc-130">获取协议元数据</span><span class="sxs-lookup"><span data-stu-id="1bcfc-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="1bcfc-131">确认客户同意</span><span class="sxs-lookup"><span data-stu-id="1bcfc-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="1bcfc-132">这适用于生产环境和沙盒环境。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="1bcfc-133">确认新客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="1bcfc-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="1bcfc-134">在合作伙伴中心中创建新客户租户时，可使用下面的过程来确认客户接受了协议。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="1bcfc-135">必须是管理员代理或销售代理才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1bcfc-136">依次选择“客户”、“新客户”、“帐户信息”。   </span><span class="sxs-lookup"><span data-stu-id="1bcfc-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="1bcfc-137">输入“公司”和“主要联系人”的信息。  </span><span class="sxs-lookup"><span data-stu-id="1bcfc-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="公司信息":::

3. <span data-ttu-id="1bcfc-139">在“Microsoft 客户协议”下，选择“客户已接受最新的 Microsoft 客户协议”。  </span><span class="sxs-lookup"><span data-stu-id="1bcfc-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="1bcfc-140">在“协议接受日期”  下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="1bcfc-141">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="1bcfc-142">输入提供接受的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="添加接受日期":::

   <span data-ttu-id="1bcfc-144">默认情况下，将显示主要联系人用户信息。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="1bcfc-145">如果此信息不正确，请选择“更新”，然后输入接受协议的人员的“名字”、“姓氏”、“电子邮件地址”和\*“电话号码”（可选）。     </span><span class="sxs-lookup"><span data-stu-id="1bcfc-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="1bcfc-146">选择“下一步”  ，继续执行创建客户租户的其余步骤。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="1bcfc-147">确认现有客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="1bcfc-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="1bcfc-148">必须是管理员代理或销售代理才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1bcfc-149">选择“客户”，然后找到并选择要查看的客户。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="1bcfc-150">选择“帐户信息”。 </span><span class="sxs-lookup"><span data-stu-id="1bcfc-150">Select **Account info**.</span></span>

3. <span data-ttu-id="1bcfc-151">在“Microsoft 客户协议”下，选择“更新”。  </span><span class="sxs-lookup"><span data-stu-id="1bcfc-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Update":::

4. <span data-ttu-id="1bcfc-153">输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    </span><span class="sxs-lookup"><span data-stu-id="1bcfc-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="1bcfc-154">在“协议接受日期”  下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="1bcfc-155">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="1bcfc-156">选择“保存并继续”。 </span><span class="sxs-lookup"><span data-stu-id="1bcfc-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="1bcfc-157">在为现有客户创建新订单时确认客户接受了协议</span><span class="sxs-lookup"><span data-stu-id="1bcfc-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="1bcfc-158">如果为之前未确认过是否接受了协议的现有客户创建新订单，你将收到完成确认的提示。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="1bcfc-159">请使用下面的过程执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="1bcfc-160">输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    </span><span class="sxs-lookup"><span data-stu-id="1bcfc-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="1bcfc-161">在“协议接受日期”  下，输入相应的日期。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="1bcfc-162">不能将此日期设置为未来日期。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="1bcfc-163">选择“保存并继续”。 </span><span class="sxs-lookup"><span data-stu-id="1bcfc-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="1bcfc-164">为现有客户检索客户接受了协议的确认</span><span class="sxs-lookup"><span data-stu-id="1bcfc-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="1bcfc-165">可以使用下面的过程为之前提供过确认的现有客户检索客户接受了协议的确认。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="1bcfc-166">必须是管理员代理或销售代理才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1bcfc-167">选择“客户”，然后找到并选择要查看的客户。</span><span class="sxs-lookup"><span data-stu-id="1bcfc-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="1bcfc-168">选择“帐户信息”。 </span><span class="sxs-lookup"><span data-stu-id="1bcfc-168">Select **Account info**.</span></span>

3. <span data-ttu-id="1bcfc-169">在“Microsoft 客户协议”下，可以看到是否已为此客户提供过确认。 </span><span class="sxs-lookup"><span data-stu-id="1bcfc-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1bcfc-170">后续步骤</span><span class="sxs-lookup"><span data-stu-id="1bcfc-170">Next steps</span></span>

- [<span data-ttu-id="1bcfc-171">确认客户接受云解决方案提供商合作伙伴计划中的 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="1bcfc-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="1bcfc-172">代表客户证明接受 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="1bcfc-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)