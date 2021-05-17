---
title: 2021 年 3 月公告
description: Microsoft 合作伙伴中心 2021 年 3 月公告，包括新功能、促销、产品/服务、市场或对现有产品/服务的更改。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 3d91eb26f98005b92a48c6f242ea4439e42cde05
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702869"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="6393d-103">2021 年 3 月公告</span><span class="sxs-lookup"><span data-stu-id="6393d-103">March 2021 announcements</span></span>

<span data-ttu-id="6393d-104">本页提供了 Microsoft 合作伙伴中心 2021 年 3 月公告。</span><span class="sxs-lookup"><span data-stu-id="6393d-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a><span data-ttu-id="6393d-105">就绪情况：对云解决方案提供商 (CSP) 客户地址验证 API 的更改将于 6 月上线；测试功能现已可用</span><span class="sxs-lookup"><span data-stu-id="6393d-105">Readiness: Changes to the Cloud Solution Provider (CSP) customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-106">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-106">Categories</span></span>

- <span data-ttu-id="6393d-107">日期：2021-03-30</span><span class="sxs-lookup"><span data-stu-id="6393d-107">Date: 2021-03-30</span></span>
- <span data-ttu-id="6393d-108">就绪</span><span class="sxs-lookup"><span data-stu-id="6393d-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-109">总结</span><span class="sxs-lookup"><span data-stu-id="6393d-109">Summary</span></span>

<span data-ttu-id="6393d-110">为帮助合作伙伴和客户在相互信任的基础上开展其业务，我们将邀请世界各地的合作伙伴测试对验证地址 API 的更改。</span><span class="sxs-lookup"><span data-stu-id="6393d-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-111">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-111">Impacted audience</span></span>

<span data-ttu-id="6393d-112">新建客户地址详细信息或更新现有客户地址详细信息的 CSP 直接计费合作伙伴和间接提供商。</span><span class="sxs-lookup"><span data-stu-id="6393d-112">CSP direct bill partners and indirect providers who create new or update existing customers address details.</span></span>

### <a name="details"></a><span data-ttu-id="6393d-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-113">Details</span></span>

<span data-ttu-id="6393d-114">Microsoft 值得信赖。</span><span class="sxs-lookup"><span data-stu-id="6393d-114">Microsoft runs on trust.</span></span> <span data-ttu-id="6393d-115">我们致力于在 CSP 计划中为交易客户订阅提供合规、安全且可靠的客户地址验证方法。</span><span class="sxs-lookup"><span data-stu-id="6393d-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="6393d-116">从 2021 年 3 月 31 日开始，我们引入了对验证地址 API 的更改，我们已邀请合作伙伴在推出这些更改（2021 年 6 月）之前对其进行测试。</span><span class="sxs-lookup"><span data-stu-id="6393d-116">As of March 31, 2021, we’ve introduced changes to the Validate Address API that we invited partners to test, prior to going live with the changes in June 2021.</span></span>

<span data-ttu-id="6393d-117">更改仅影响验证地址 API。</span><span class="sxs-lookup"><span data-stu-id="6393d-117">Changes affect the Validate Address API only.</span></span> <span data-ttu-id="6393d-118">创建客户和更新计费配置文件 API 不受影响。</span><span class="sxs-lookup"><span data-stu-id="6393d-118">Create Customer and Update Billing Profile APIs aren’t impacted.</span></span>

<span data-ttu-id="6393d-119">响应将返回以下某个状态消息：</span><span class="sxs-lookup"><span data-stu-id="6393d-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="6393d-120">状态</span><span class="sxs-lookup"><span data-stu-id="6393d-120">Status</span></span>     | <span data-ttu-id="6393d-121">说明</span><span class="sxs-lookup"><span data-stu-id="6393d-121">Description</span></span> |    <span data-ttu-id="6393d-122">返回的建议地址数</span><span class="sxs-lookup"><span data-stu-id="6393d-122">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="6393d-123">Verified shippable</span><span class="sxs-lookup"><span data-stu-id="6393d-123">Verified shippable</span></span> | <span data-ttu-id="6393d-124">地址已经过验证且可送达。</span><span class="sxs-lookup"><span data-stu-id="6393d-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="6393d-125">Single</span><span class="sxs-lookup"><span data-stu-id="6393d-125">Single</span></span> |
|<span data-ttu-id="6393d-126">已验证</span><span class="sxs-lookup"><span data-stu-id="6393d-126">Verified</span></span> | <span data-ttu-id="6393d-127">已验证地址。</span><span class="sxs-lookup"><span data-stu-id="6393d-127">Address is verified.</span></span> | <span data-ttu-id="6393d-128">Single</span><span class="sxs-lookup"><span data-stu-id="6393d-128">Single</span></span> |
|<span data-ttu-id="6393d-129">Interaction required</span><span class="sxs-lookup"><span data-stu-id="6393d-129">Interaction required</span></span> | <span data-ttu-id="6393d-130">建议的地址发生了重大更改，需要用户确认。</span><span class="sxs-lookup"><span data-stu-id="6393d-130">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="6393d-131">Single</span><span class="sxs-lookup"><span data-stu-id="6393d-131">Single</span></span> |
|<span data-ttu-id="6393d-132">Street partial</span><span class="sxs-lookup"><span data-stu-id="6393d-132">Street partial</span></span> | <span data-ttu-id="6393d-133">地址中给出的街道信息不完整，需要更多信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="6393d-134">多个 - 最多 3 个</span><span class="sxs-lookup"><span data-stu-id="6393d-134">Multiple—maximum of three</span></span> |
|<span data-ttu-id="6393d-135">Premises partial</span><span class="sxs-lookup"><span data-stu-id="6393d-135">Premises partial</span></span> | <span data-ttu-id="6393d-136">给出的场所信息（楼栋号、房号等）不完整，需要更多信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-136">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="6393d-137">多个 - 最多 3 个</span><span class="sxs-lookup"><span data-stu-id="6393d-137">Multiple—maximum of three</span></span> |
|<span data-ttu-id="6393d-138">多个</span><span class="sxs-lookup"><span data-stu-id="6393d-138">Multiple</span></span> | <span data-ttu-id="6393d-139">地址中有多个字段不完整（也可能包括 street partial 和 premises partial）。</span><span class="sxs-lookup"><span data-stu-id="6393d-139">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="6393d-140">多个 - 最多 3 个</span><span class="sxs-lookup"><span data-stu-id="6393d-140">Multiple—maximum of three</span></span> |
|<span data-ttu-id="6393d-141">无</span><span class="sxs-lookup"><span data-stu-id="6393d-141">None</span></span> | <span data-ttu-id="6393d-142">地址错误。</span><span class="sxs-lookup"><span data-stu-id="6393d-142">Address is incorrect.</span></span> | <span data-ttu-id="6393d-143">无</span><span class="sxs-lookup"><span data-stu-id="6393d-143">None</span></span> |
|<span data-ttu-id="6393d-144">未验证</span><span class="sxs-lookup"><span data-stu-id="6393d-144">Not validated</span></span> | <span data-ttu-id="6393d-145">无法通过验证过程发送地址。</span><span class="sxs-lookup"><span data-stu-id="6393d-145">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="6393d-146">无</span><span class="sxs-lookup"><span data-stu-id="6393d-146">None</span></span> |

<span data-ttu-id="6393d-147">美国邮政编码将返回额外 4 个数字 + 连字符，例如 12345-6789。</span><span class="sxs-lookup"><span data-stu-id="6393d-147">US post codes will return an additional 4 digits + hyphen - for example, 12345-6789.</span></span>

<span data-ttu-id="6393d-148">提交地址供验证地址 API 验证后，会返回以下响应架构：</span><span class="sxs-lookup"><span data-stu-id="6393d-148">Once an address is submitted for validation via the Validate Address API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="6393d-149">查看此示例响应。</span><span class="sxs-lookup"><span data-stu-id="6393d-149">Take a look at this sample response.</span></span> <span data-ttu-id="6393d-150">请注意，对于美国，如果你仅输入 5 位邮政编码，响应将为邮政编码行返回额外的 4 位后缀。</span><span class="sxs-lookup"><span data-stu-id="6393d-150">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="6393d-151">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-151">Next steps</span></span>

- <span data-ttu-id="6393d-152">与行业专家 Ali Khaki 分享你的沙盒租户 ID，以加入外部测试，这样你便可以开始准备更新。</span><span class="sxs-lookup"><span data-stu-id="6393d-152">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="6393d-153">如果正在使用控制面板供应商 (CPV) 解决方案，请咨询 CPV。</span><span class="sxs-lookup"><span data-stu-id="6393d-153">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-154">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-154">Questions?</span></span>

<span data-ttu-id="6393d-155">如果在 Microsoft 运营方面需要支持，请联系你的合作伙伴 Yammer 支持组。</span><span class="sxs-lookup"><span data-stu-id="6393d-155">If you need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

### <a name="change-log"></a><span data-ttu-id="6393d-156">更改日志：</span><span class="sxs-lookup"><span data-stu-id="6393d-156">Change log:</span></span>

- <span data-ttu-id="6393d-157">2020 年 3 月 31 日：原始发布日期</span><span class="sxs-lookup"><span data-stu-id="6393d-157">March 31, 2020: Original publication</span></span>

- <span data-ttu-id="6393d-158">2021 年 4 月 30 日：示例响应和邮政编码详细信息更新</span><span class="sxs-lookup"><span data-stu-id="6393d-158">April 30, 2021: Updates for sample response and Zip code details</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="6393d-159">新的 Exchange 管理中心 (EAC) 体验</span><span class="sxs-lookup"><span data-stu-id="6393d-159">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-160">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-160">Categories</span></span>

- <span data-ttu-id="6393d-161">日期：2021-03-29</span><span class="sxs-lookup"><span data-stu-id="6393d-161">Date: 2021-03-29</span></span>
- <span data-ttu-id="6393d-162">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-162">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-163">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-163">Summary</span></span>

<span data-ttu-id="6393d-164">从 2021 年 4 月 27 日开始，Exchange 管理中心 (EAC) 将推出一种将提高用户日常工作效率的新体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-164">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-165">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-165">Impacted audience</span></span>

<span data-ttu-id="6393d-166">通过合作伙伴中心访问 Exchange 的委派管理员</span><span class="sxs-lookup"><span data-stu-id="6393d-166">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="6393d-167">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-167">Details</span></span>

<span data-ttu-id="6393d-168">从 2021 年 4 月 27 日起，通过合作伙伴中心导航到 Exchange 的合作伙伴会被重定向到新的 EAC。</span><span class="sxs-lookup"><span data-stu-id="6393d-168">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="6393d-169">此新体验当前以预览版的形式提供，管理员可提供选择经典 EAC 右上角的切换开关来激活此体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-169">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="6393d-170">他们还可以选择所有页面上显示的“立即试用”横幅导航到新的 EAC。</span><span class="sxs-lookup"><span data-stu-id="6393d-170">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="6393d-171">新 EAC 的优点包括：</span><span class="sxs-lookup"><span data-stu-id="6393d-171">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="6393d-172">添加了与邮件流相关的问题的见解、报告和警报机制。</span><span class="sxs-lookup"><span data-stu-id="6393d-172">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="6393d-173">个性化的面板，便于提高工作效率。</span><span class="sxs-lookup"><span data-stu-id="6393d-173">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="6393d-174">为了帮助你浏览新体验，“培训和指南”部分提供了有关新 EAC 体验的视频。</span><span class="sxs-lookup"><span data-stu-id="6393d-174">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="6393d-175">这些视频简要介绍如何最好地使用新门户。</span><span class="sxs-lookup"><span data-stu-id="6393d-175">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="6393d-176">进行此更改后，不会弃用经典 EAC 体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-176">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="6393d-177">我们在实施任何更改之前，会提前很久通知用户。</span><span class="sxs-lookup"><span data-stu-id="6393d-177">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-178">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-178">Next steps</span></span>

- <span data-ttu-id="6393d-179">查看[有关本主题的资源](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)，你可以在其中查看新体验的屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="6393d-179">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="6393d-180">请与贵组织中的相应利益干系人共享此信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-180">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="6393d-181">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-181">Questions?</span></span>

<span data-ttu-id="6393d-182">如果对这些更改有任何问题，请访问相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-182">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="6393d-183">Microsoft 运营：引入产品发布日历</span><span class="sxs-lookup"><span data-stu-id="6393d-183">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-184">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-184">Categories</span></span>

- <span data-ttu-id="6393d-185">日期：2021-03-25</span><span class="sxs-lookup"><span data-stu-id="6393d-185">Date: 2021-03-25</span></span>
- <span data-ttu-id="6393d-186">产品/服务 | 新式工作区</span><span class="sxs-lookup"><span data-stu-id="6393d-186">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-187">总结</span><span class="sxs-lookup"><span data-stu-id="6393d-187">Summary</span></span>

<span data-ttu-id="6393d-188">为了响应合作伙伴反馈，Microsoft 运营部将简化产品发布通信。</span><span class="sxs-lookup"><span data-stu-id="6393d-188">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-189">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-189">Impacted audience</span></span>

<span data-ttu-id="6393d-190">云解决方案提供商 (CSP) 合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-190">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="6393d-191">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-191">Details</span></span>

<span data-ttu-id="6393d-192">Microsoft 致力于不断改进合作伙伴体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-192">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="6393d-193">我们从你那里得到的反馈是，你已经收到了太多来自 Microsoft 的信息，包括重复的产品发布公告。</span><span class="sxs-lookup"><span data-stu-id="6393d-193">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="6393d-194">根据你的反馈，Microsoft 已简化了新产品/服务和现有产品/服务的产品发布准备体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-194">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="6393d-195">现在，我们将为你提供一个产品发布月度视图，该视图发布在运营准备资源库中。</span><span class="sxs-lookup"><span data-stu-id="6393d-195">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="6393d-196">此月度[产品发布日历视图](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)将替代运营准备资源库和合作伙伴中心公告中的各个产品发布通信。</span><span class="sxs-lookup"><span data-stu-id="6393d-196">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="6393d-197">你还可以从[社区集合](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)、[日历视图](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)和 [CSP 新闻稿](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)访问此[产品发布日历](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)。</span><span class="sxs-lookup"><span data-stu-id="6393d-197">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="6393d-198">当我们在运营准备资源库中发布每个月的产品发布日历及公告时，会向你发送通知。</span><span class="sxs-lookup"><span data-stu-id="6393d-198">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="6393d-199">你仍可以在价目表预览、价目表更改日志以及产品博客、许可指南和产品营销页中找到有关新产品/服务和现有产品/服务的信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-199">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="6393d-200">此更改将适用于以下产品的发布：</span><span class="sxs-lookup"><span data-stu-id="6393d-200">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="6393d-201">本地 Dynamics</span><span class="sxs-lookup"><span data-stu-id="6393d-201">Dynamics on-premises</span></span>
- <span data-ttu-id="6393d-202">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6393d-202">Microsoft 365</span></span>
- <span data-ttu-id="6393d-203">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="6393d-203">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="6393d-204">Windows</span><span class="sxs-lookup"><span data-stu-id="6393d-204">Windows</span></span>
- <span data-ttu-id="6393d-205">服务器</span><span class="sxs-lookup"><span data-stu-id="6393d-205">Server</span></span>  
- <span data-ttu-id="6393d-206">工具</span><span class="sxs-lookup"><span data-stu-id="6393d-206">Tools</span></span>
- <span data-ttu-id="6393d-207">Teams 和 Telco</span><span class="sxs-lookup"><span data-stu-id="6393d-207">Teams and Telco</span></span>

<span data-ttu-id="6393d-208">我们将继续为需要运营准备详细情况的产品发布发送具体公告。</span><span class="sxs-lookup"><span data-stu-id="6393d-208">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-209">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-209">Next steps</span></span>

<span data-ttu-id="6393d-210">查看有关本主题的资源，并与组织内部的相关利益干系人共享此信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-210">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-211">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-211">Questions?</span></span>

<span data-ttu-id="6393d-212">如果对这些产品/服务有任何进一步的问题，请访问相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-212">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="6393d-213">CSP 客户加入要求变更</span><span class="sxs-lookup"><span data-stu-id="6393d-213">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-214">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-214">Categories</span></span>

- <span data-ttu-id="6393d-215">日期：2021-03-25</span><span class="sxs-lookup"><span data-stu-id="6393d-215">Date: 2021-03-25</span></span>
- <span data-ttu-id="6393d-216">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-216">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-217">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-217">Summary</span></span>

<span data-ttu-id="6393d-218">我们承诺帮助合作伙伴和客户在相互信任的基础上开展其业务，在此过程中，我们将请求其他客户信息，从 2021 年 3 月 25 日生效。</span><span class="sxs-lookup"><span data-stu-id="6393d-218">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-219">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-219">Impacted audience</span></span>

<span data-ttu-id="6393d-220">云解决方案提供商 (CSP) 直接计费合作伙伴和间接提供商，他们拥有位于下一节所列国家/地区的新客户或现有客户</span><span class="sxs-lookup"><span data-stu-id="6393d-220">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="6393d-221">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-221">Details</span></span>

<span data-ttu-id="6393d-222">Microsoft 值得信赖。</span><span class="sxs-lookup"><span data-stu-id="6393d-222">Microsoft runs on trust.</span></span> <span data-ttu-id="6393d-223">我们致力于在 CSP 计划中为交易客户订阅提供合规、安全且可靠的客户验证方法。</span><span class="sxs-lookup"><span data-stu-id="6393d-223">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="6393d-224">在 2021 年 5 月 25 日，我们将引入合作伙伴中心 API 和用户界面 (UI) 增强功能，它们将影响同时满足以下两个条件的合作伙伴：</span><span class="sxs-lookup"><span data-stu-id="6393d-224">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="6393d-225">合作伙伴与 Microsoft 有直接计费关系（这意味着合作伙伴是直接计费合作伙伴或间接提供商）。</span><span class="sxs-lookup"><span data-stu-id="6393d-225">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="6393d-226">合作伙伴与以下国家/地区的新客户或现有客户开展业务：</span><span class="sxs-lookup"><span data-stu-id="6393d-226">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="6393d-227">泰国</span><span class="sxs-lookup"><span data-stu-id="6393d-227">Thailand</span></span>
    - <span data-ttu-id="6393d-228">越南</span><span class="sxs-lookup"><span data-stu-id="6393d-228">Vietnam</span></span>
    - <span data-ttu-id="6393d-229">土耳其</span><span class="sxs-lookup"><span data-stu-id="6393d-229">Turkey</span></span>
    - <span data-ttu-id="6393d-230">波兰</span><span class="sxs-lookup"><span data-stu-id="6393d-230">Poland</span></span>
    - <span data-ttu-id="6393d-231">南非</span><span class="sxs-lookup"><span data-stu-id="6393d-231">South Africa</span></span>
    - <span data-ttu-id="6393d-232">印度</span><span class="sxs-lookup"><span data-stu-id="6393d-232">India</span></span>
    - <span data-ttu-id="6393d-233">巴西</span><span class="sxs-lookup"><span data-stu-id="6393d-233">Brazil</span></span>
    - <span data-ttu-id="6393d-234">伊拉克</span><span class="sxs-lookup"><span data-stu-id="6393d-234">Iraq</span></span>
    - <span data-ttu-id="6393d-235">缅甸</span><span class="sxs-lookup"><span data-stu-id="6393d-235">Myanmar</span></span>
    - <span data-ttu-id="6393d-236">南苏丹</span><span class="sxs-lookup"><span data-stu-id="6393d-236">South Sudan</span></span>
    - <span data-ttu-id="6393d-237">沙特阿拉伯</span><span class="sxs-lookup"><span data-stu-id="6393d-237">Saudi Arabia</span></span>
    - <span data-ttu-id="6393d-238">阿拉伯联合酋长国</span><span class="sxs-lookup"><span data-stu-id="6393d-238">United Arab Emirates</span></span>
    - <span data-ttu-id="6393d-239">委内瑞拉</span><span class="sxs-lookup"><span data-stu-id="6393d-239">Venezuela</span></span>

<span data-ttu-id="6393d-240">满足条件的合作伙伴必须在加入新客户或修改现有客户详细信息时，提交该客户的公司注册 ID（也称为客户的组织 INN）和电话号码  。</span><span class="sxs-lookup"><span data-stu-id="6393d-240">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="6393d-241">这些合作伙伴还可以为客户输入可选的中间名。</span><span class="sxs-lookup"><span data-stu-id="6393d-241">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="6393d-242">请注意，在添加公司注册 ID 时，应使用企业纳税人标识号，而不是客户的个人 ID。</span><span class="sxs-lookup"><span data-stu-id="6393d-242">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="6393d-243">与以下国家/地区的新客户和现有客户合作的合作伙伴已加入 2020 年 11 月的以前版本中。</span><span class="sxs-lookup"><span data-stu-id="6393d-243">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="6393d-244">亚美尼亚</span><span class="sxs-lookup"><span data-stu-id="6393d-244">Armenia</span></span>
- <span data-ttu-id="6393d-245">阿塞拜疆</span><span class="sxs-lookup"><span data-stu-id="6393d-245">Azerbaijan</span></span>
- <span data-ttu-id="6393d-246">白俄罗斯</span><span class="sxs-lookup"><span data-stu-id="6393d-246">Belarus</span></span>
- <span data-ttu-id="6393d-247">匈牙利</span><span class="sxs-lookup"><span data-stu-id="6393d-247">Hungary</span></span>
- <span data-ttu-id="6393d-248">哈萨克斯坦</span><span class="sxs-lookup"><span data-stu-id="6393d-248">Kazakhstan</span></span>
- <span data-ttu-id="6393d-249">吉尔吉斯斯坦</span><span class="sxs-lookup"><span data-stu-id="6393d-249">Kyrgyzstan</span></span>
- <span data-ttu-id="6393d-250">摩尔多瓦</span><span class="sxs-lookup"><span data-stu-id="6393d-250">Moldova</span></span>
- <span data-ttu-id="6393d-251">俄罗斯</span><span class="sxs-lookup"><span data-stu-id="6393d-251">Russia</span></span>
- <span data-ttu-id="6393d-252">塔吉克斯坦</span><span class="sxs-lookup"><span data-stu-id="6393d-252">Tajikistan</span></span>
- <span data-ttu-id="6393d-253">乌克兰</span><span class="sxs-lookup"><span data-stu-id="6393d-253">Ukraine</span></span>
- <span data-ttu-id="6393d-254">乌兹别克斯坦</span><span class="sxs-lookup"><span data-stu-id="6393d-254">Uzbekistan</span></span>

<span data-ttu-id="6393d-255">与世界上其他国家/地区的客户合作的合作伙伴可以在 2021 年 3 月 25 日输入客户的公司注册 ID、电话号码和中间名（可选）详细信息  。</span><span class="sxs-lookup"><span data-stu-id="6393d-255">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-256">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-256">Next steps</span></span>

- <span data-ttu-id="6393d-257">有关更详细的指南，请查看[专门的合作伙伴集锦](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)中的技术文档和常见问题。</span><span class="sxs-lookup"><span data-stu-id="6393d-257">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="6393d-258">准备使用合作伙伴中心 API 和 Web 用户体验来整合更改。</span><span class="sxs-lookup"><span data-stu-id="6393d-258">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="6393d-259">API/SDK 将可用于测试。</span><span class="sxs-lookup"><span data-stu-id="6393d-259">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="6393d-260">请确保在加入新客户或修改现有客户详细信息时提交其他数据。</span><span class="sxs-lookup"><span data-stu-id="6393d-260">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="6393d-261">如果正在使用控制面板供应商 (CPV) 解决方案，请咨询 CPV。</span><span class="sxs-lookup"><span data-stu-id="6393d-261">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-262">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-262">Questions?</span></span>

<span data-ttu-id="6393d-263">如果你有任何与法律识别码（也称为 INN 或 TIN）相关的问题，请与你的税务顾问或当地税务局联系。</span><span class="sxs-lookup"><span data-stu-id="6393d-263">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="6393d-264">Microsoft 无法提供有关税务事宜的指导。</span><span class="sxs-lookup"><span data-stu-id="6393d-264">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="6393d-265">如果需要与 Microsoft 运营有关的支持，请[创建服务请求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。</span><span class="sxs-lookup"><span data-stu-id="6393d-265">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="6393d-266">更正了 2021 年 3 月 1 日永久性软件价目表</span><span class="sxs-lookup"><span data-stu-id="6393d-266">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-267">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-267">Categories</span></span>

- <span data-ttu-id="6393d-268">日期：2021-03-23</span><span class="sxs-lookup"><span data-stu-id="6393d-268">Date: 2021-03-23</span></span>
- <span data-ttu-id="6393d-269">产品/市场</span><span class="sxs-lookup"><span data-stu-id="6393d-269">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-270">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-270">Impacted audience</span></span>

<span data-ttu-id="6393d-271">交易永久性软件的间接提供商和直接帐单合作伙伴在云解决方案提供商计划中</span><span class="sxs-lookup"><span data-stu-id="6393d-271">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="6393d-272">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-272">Details</span></span>

<span data-ttu-id="6393d-273">2021 年 3 月 1 日发布的永久性软件的价目表包含了不应包含的市场。</span><span class="sxs-lookup"><span data-stu-id="6393d-273">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="6393d-274">已于 2021 年 3 月 17 日更正永久性软件价目表。</span><span class="sxs-lookup"><span data-stu-id="6393d-274">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="6393d-275">这些更正仅适用于：</span><span class="sxs-lookup"><span data-stu-id="6393d-275">These corrections were only applicable to:</span></span>

- <span data-ttu-id="6393d-276">产品 ID：DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="6393d-276">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="6393d-277">产品名称：Microsoft 365 商业版的 Windows 10 家庭版到专业版升级</span><span class="sxs-lookup"><span data-stu-id="6393d-277">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="6393d-278">已删除或不受支持的市场：AE、AF、AL、AM、AO、BA、BB、BD、BH、BM、BN、BO、BR、BS、BW、BY、BZ、CI、CL、CM、CO、CR、CW、DO、DZ、EC、EG、ET、FJ、FO、GE、GH、GT、HN、IL、IN、IQ、JM、JO、KE、KG、KN、KW、KY、KZ、LB、LK、LY、MA、MC、MD、ME、MN、MO、MU、NA、NG、NI、NP、OM、PA、PE、PH、PK、PR、PY、QA、RS、RU、RW、SG、SN、SV、TH、TJ、TM、TN、TT、TZ、UA、UG、UY、UZ、VE、VN、YE、ZM、ZW</span><span class="sxs-lookup"><span data-stu-id="6393d-278">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="6393d-279">这些更改仅适用于上述产品。</span><span class="sxs-lookup"><span data-stu-id="6393d-279">These changes only apply to the above product.</span></span> <span data-ttu-id="6393d-280">其他产品没有更正。</span><span class="sxs-lookup"><span data-stu-id="6393d-280">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="6393d-281">后续步骤和资源</span><span class="sxs-lookup"><span data-stu-id="6393d-281">Next steps and resources</span></span>

- <span data-ttu-id="6393d-282">交易永久性软件的合作伙伴应下载最新的永久性软件价目表。</span><span class="sxs-lookup"><span data-stu-id="6393d-282">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="6393d-283">请参阅[国家/地区代码](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)，了解两个字母的缩写到国家/地区的易懂对应关系。</span><span class="sxs-lookup"><span data-stu-id="6393d-283">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><span data-ttu-id="6393d-284"><a name="13">.NET Standard 上的 SDK 版本 (v1.17.0)</a></span><span class="sxs-lookup"><span data-stu-id="6393d-284"><a name="13"></a> SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-285">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-285">Categories</span></span>

- <span data-ttu-id="6393d-286">日期：2021-03-23</span><span class="sxs-lookup"><span data-stu-id="6393d-286">Date: 2021-03-23</span></span>

- <span data-ttu-id="6393d-287">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-287">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="6393d-288">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-288">Impacted audience</span></span>

<span data-ttu-id="6393d-289">使用合作伙伴中心 .NET SDK 且参与 CSP 计划的直接计费合作伙伴和间接提供商。</span><span class="sxs-lookup"><span data-stu-id="6393d-289">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="6393d-290">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-290">Details</span></span>

<span data-ttu-id="6393d-291">从 2021 年 3 月 23 日开始，合作伙伴便可下载最新版 [MicrosoftPartnerCenter.NETSDK（NuGet 库 | Microsoft.Store.PartnerCenter 1.17.0）](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)，还可下载更新的公共合作伙伴中心 SDK [GitHub 示例](https://github.com/Microsoft/Partner-Center-DotNet-Samples)。</span><span class="sxs-lookup"><span data-stu-id="6393d-291">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="6393d-292">此版本包括以下方法更新：</span><span class="sxs-lookup"><span data-stu-id="6393d-292">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="6393d-293">审核已更新：新操作类型</span><span class="sxs-lookup"><span data-stu-id="6393d-293">Audit Updated: New operation types</span></span>

<span data-ttu-id="6393d-294">添加了新的[操作类型](https://docs.microsoft.com/partner-center/develop/auditing-resources)，以了解客户批准和终止 DAP 的时间。</span><span class="sxs-lookup"><span data-stu-id="6393d-294">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="6393d-295">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="6393d-295">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="6393d-296">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="6393d-296">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="6393d-297">审核已更新：新资源和操作类型</span><span class="sxs-lookup"><span data-stu-id="6393d-297">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="6393d-298">添加了新的[资源和操作类型](https://docs.microsoft.com/partner-center/develop/auditing-resources)以支持客户目录角色方案。</span><span class="sxs-lookup"><span data-stu-id="6393d-298">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="6393d-299">新资源类型“CustomerDirectoryRole”</span><span class="sxs-lookup"><span data-stu-id="6393d-299">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="6393d-300">操作类型“AddUserMember”和“RemoveUserMember”</span><span class="sxs-lookup"><span data-stu-id="6393d-300">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="6393d-301">对客户帐户的 SDK 更新</span><span class="sxs-lookup"><span data-stu-id="6393d-301">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="6393d-302">对 GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus 的支持</span><span class="sxs-lookup"><span data-stu-id="6393d-302">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="6393d-303">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="6393d-303">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="6393d-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="6393d-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="6393d-305">其他更改</span><span class="sxs-lookup"><span data-stu-id="6393d-305">Additional changes</span></span>

<span data-ttu-id="6393d-306">以下更改将作为“新商业”的一部分引入，当前仅适用于已加入 M365/D365 新商业体验技术预览版的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="6393d-306">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="6393d-307">未参与新商业技术预览版的合作伙伴应该不会注意到影响，并且应向后兼容。</span><span class="sxs-lookup"><span data-stu-id="6393d-307">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="6393d-308">目录更改：</span><span class="sxs-lookup"><span data-stu-id="6393d-308">Catalog Changes:</span></span>

  - <span data-ttu-id="6393d-309">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="6393d-309">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="6393d-310">购买和管理：</span><span class="sxs-lookup"><span data-stu-id="6393d-310">Purchase and Manage:</span></span>
  - <span data-ttu-id="6393d-311">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="6393d-311">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="6393d-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="6393d-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="6393d-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="6393d-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="6393d-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="6393d-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="6393d-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="6393d-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="6393d-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="6393d-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-317">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-317">Next Steps</span></span>

- <span data-ttu-id="6393d-318">下载最新版 [MicrosoftPartnerCenter.NETSDK（NuGet 库 | Microsoft.Store.PartnerCenter 1.17.0）](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="6393d-318">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="6393d-319">下载并查看 [GitHub 示例](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="6393d-319">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="6393d-320">CSP 商业市场产品/服务以及 2021 财年 CSP 奖励措施（针对符合条件的产品/服务）</span><span class="sxs-lookup"><span data-stu-id="6393d-320">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-321">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-321">Categories</span></span>

- <span data-ttu-id="6393d-322">日期：2021-03-18</span><span class="sxs-lookup"><span data-stu-id="6393d-322">Date: 2021-03-18</span></span>
- <span data-ttu-id="6393d-323">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-323">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-324">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-324">Impacted audience</span></span>

<span data-ttu-id="6393d-325">云解决方案提供商计划中的间接提供商和直接计费合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-325">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="6393d-326">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-326">Details</span></span>

<span data-ttu-id="6393d-327">云解决方案提供商计划中的间接提供商和直接帐单合作伙伴可以销售第三方产品/服务，并就合作伙伴中心或 Azure 门户中每个符合条件的第三方产品/服务获得退款奖励。</span><span class="sxs-lookup"><span data-stu-id="6393d-327">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="6393d-328">激励采取为符合资格的产品/服务的已计费销售进行退款的形式，有效期持续到 2021 年 6 月 30 日。</span><span class="sxs-lookup"><span data-stu-id="6393d-328">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="6393d-329">在下方继续了解此云解决方案提供商商业市场产品/服务激励，并立即与客户联系，确定适当的产品/服务以便让他们能够实现持续成功和数字转换。</span><span class="sxs-lookup"><span data-stu-id="6393d-329">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="6393d-330">我们与独立软件供应商合作 (ISV) 合作，将最新的 IaaS 和 SaaS 解决方案推向市场以便 Microsoft 客户使用。</span><span class="sxs-lookup"><span data-stu-id="6393d-330">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="6393d-331">ISV 发布者可以选择允许通过 Microsoft 合作伙伴渠道销售其产品/服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-331">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="6393d-332">有资格获得激励的产品/服务分为两类：</span><span class="sxs-lookup"><span data-stu-id="6393d-332">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="6393d-333">具有 Azure IP 共同销售激励状态的 SaaS 和 IaaS 第三方产品/服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-333">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="6393d-334">与 Teams 或至少两款 Microsoft 365 生产力应用程序（如 PowerPoint、Word、Excel、Outlook 或 SharePoint）集成的 SaaS 应用程序。</span><span class="sxs-lookup"><span data-stu-id="6393d-334">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="6393d-335">后续步骤和资源</span><span class="sxs-lookup"><span data-stu-id="6393d-335">Next steps and resources</span></span>

- <span data-ttu-id="6393d-336">了解如何通过销售符合资格的市场应用（有资格获得激励的应用）获得[合作伙伴奖励](https://partner.microsoft.com/membership/partner-incentives)。</span><span class="sxs-lookup"><span data-stu-id="6393d-336">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="6393d-337">每个月都会添加新产品/服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-337">New offers are added monthly.</span></span>  
- [<span data-ttu-id="6393d-338">云解决方案提供商直接计费合作伙伴激励资源</span><span class="sxs-lookup"><span data-stu-id="6393d-338">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="6393d-339">云解决方案提供商间接提供商激励资源</span><span class="sxs-lookup"><span data-stu-id="6393d-339">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="6393d-340">查看此[演示文稿](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)，了解有关销售商业市场应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-340">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="6393d-341">可在[此处](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)查看更多资源。</span><span class="sxs-lookup"><span data-stu-id="6393d-341">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="6393d-342">可在[合作伙伴中心](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover)或 [Azure 门户](https://ms.portal.azure.com/#home)中浏览商业市场目录</span><span class="sxs-lookup"><span data-stu-id="6393d-342">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="6393d-343">使用 [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) 将应用集成到公司的市场</span><span class="sxs-lookup"><span data-stu-id="6393d-343">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="6393d-344">与你想要与之开展业务的 ISV 联系</span><span class="sxs-lookup"><span data-stu-id="6393d-344">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="6393d-345">间接提供商需要使用 API 集成，并指导经销商应销售哪些应用</span><span class="sxs-lookup"><span data-stu-id="6393d-345">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-346">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-346">Questions?</span></span>  

<span data-ttu-id="6393d-347">请参阅[这篇文章](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)，了解合作伙伴中心商业市场的概述。</span><span class="sxs-lookup"><span data-stu-id="6393d-347">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="6393d-348">如需获得更多帮助，可以在合作伙伴中心创建支持请求。</span><span class="sxs-lookup"><span data-stu-id="6393d-348">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="6393d-349">更多信息请访问 [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1)。</span><span class="sxs-lookup"><span data-stu-id="6393d-349">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="6393d-350">Power BI Premium 产品/服务命名和先决条件更新</span><span class="sxs-lookup"><span data-stu-id="6393d-350">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-351">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-351">Categories</span></span>

- <span data-ttu-id="6393d-352">日期：2021-03-18</span><span class="sxs-lookup"><span data-stu-id="6393d-352">Date: 2021-03-18</span></span>
- <span data-ttu-id="6393d-353">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-353">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-354">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-354">Summary</span></span>

<span data-ttu-id="6393d-355">2021 年 4 月 1 日的最终价目表将更新以明确 Power BI Premium Per User 产品/服务的命名和/或先决条件信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-356">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-356">Impacted audience</span></span>

<span data-ttu-id="6393d-357">云解决方案提供商 (CSP) 直接和间接合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-357">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="6393d-358">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-358">Details</span></span>

<span data-ttu-id="6393d-359">2021 年 4 月 1 日的最终价目表将更新以明确 Power BI Premium Per User 产品/服务的命名和/或先决条件信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-359">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="6393d-360">在更新最终价目表之前，请使用此部分中的信息来确保订购适当的产品。</span><span class="sxs-lookup"><span data-stu-id="6393d-360">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="6393d-361">以下详细信息显示受影响的 SKU 和先决条件的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-361">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="6393d-362">3 月 1 日价目表预览中的的产品/服务显示名称</span><span class="sxs-lookup"><span data-stu-id="6393d-362">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="6393d-363">4 月 1 日最终价目表上更新的产品/服务显示名称</span><span class="sxs-lookup"><span data-stu-id="6393d-363">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="6393d-364">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-364">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="6393d-365">Power BI Premium Per User 加载项（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-365">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="6393d-366">Power BI Premium Per User 加载项 (Office)（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-366">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="6393d-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="6393d-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="6393d-368">客户需要满足以下任一先决条件才能购买此产品/服务：</span><span class="sxs-lookup"><span data-stu-id="6393d-368">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="6393d-369">产品/服务显示名称</span><span class="sxs-lookup"><span data-stu-id="6393d-369">Offer display name</span></span> | <span data-ttu-id="6393d-370">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-370">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6393d-371">Microsoft 365 E5（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-371">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="6393d-372">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="6393d-372">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="6393d-373">不带音频会议的 Microsoft 365 E5（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-373">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6393d-374">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="6393d-374">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="6393d-375">Office 365 E5（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-375">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="6393d-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="6393d-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="6393d-377">Office 365 E5（非营利组织员工定价）试用版</span><span class="sxs-lookup"><span data-stu-id="6393d-377">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="6393d-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="6393d-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="6393d-379">不带音频会议的 Office 365 E5（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-379">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6393d-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="6393d-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="6393d-381">需要满足先决条件才能购买以下 Power BI Premium 产品/服务：</span><span class="sxs-lookup"><span data-stu-id="6393d-381">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="6393d-382">产品/服务显示名称</span><span class="sxs-lookup"><span data-stu-id="6393d-382">Offer display name</span></span> | <span data-ttu-id="6393d-383">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-383">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="6393d-384">Power BI Premium Per User 加载项（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-384">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6393d-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="6393d-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="6393d-386">客户需要具有此先决条件才能购买此产品/服务：</span><span class="sxs-lookup"><span data-stu-id="6393d-386">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="6393d-387">产品/服务显示名称</span><span class="sxs-lookup"><span data-stu-id="6393d-387">Offer display name</span></span> | <span data-ttu-id="6393d-388">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-388">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="6393d-389">Power BI Pro（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-389">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="6393d-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="6393d-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="6393d-391">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-391">Next steps</span></span>

<span data-ttu-id="6393d-392">查看有关本主题的资源，并与组织内部的相关利益干系人共享此信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-392">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="6393d-393">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-393">Questions?</span></span>

<span data-ttu-id="6393d-394">如果对这些产品/服务有任何疑问，请查看相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-394">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a><span data-ttu-id="6393d-395">Microsoft 365 F3 的 3 月价格更新</span><span class="sxs-lookup"><span data-stu-id="6393d-395">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-396">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-396">Categories</span></span>

- <span data-ttu-id="6393d-397">日期：2021-03-16</span><span class="sxs-lookup"><span data-stu-id="6393d-397">Date: 2021-03-16</span></span>
- <span data-ttu-id="6393d-398">产品/市场</span><span class="sxs-lookup"><span data-stu-id="6393d-398">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-399">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-399">Summary</span></span>

<span data-ttu-id="6393d-400">已更正 2021 年 3 月定价，以反映正确的 Microsoft 365 F3 英镑 (GBP) 和欧元 (EUR) 价格。</span><span class="sxs-lookup"><span data-stu-id="6393d-400">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-401">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-401">Impacted audience</span></span>

<span data-ttu-id="6393d-402">在 2021 年 3 月 1 日到 3月 17 日之间通过云解决方案提供商 (CSP) 程序以英镑或欧元购买 Microsoft 365 F3 的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="6393d-402">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="6393d-403">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-403">Details</span></span>

<span data-ttu-id="6393d-404">Microsoft 已更正 Microsoft 365 F3 的错误定价。</span><span class="sxs-lookup"><span data-stu-id="6393d-404">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="6393d-405">只有英镑和欧元的价格不正确，并且只有 2021 年 3 月 1 日到 3 月 17 日之间购买的产品/服务受到影响。</span><span class="sxs-lookup"><span data-stu-id="6393d-405">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="6393d-406">下方列出了受影响的产品/服务和货币。</span><span class="sxs-lookup"><span data-stu-id="6393d-406">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="6393d-407">产品名称</span><span class="sxs-lookup"><span data-stu-id="6393d-407">Offer name</span></span> | <span data-ttu-id="6393d-408">货币</span><span class="sxs-lookup"><span data-stu-id="6393d-408">Currency</span></span> | <span data-ttu-id="6393d-409">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-409">Offer ID</span></span> | <span data-ttu-id="6393d-410">材料 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-410">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="6393d-411">Microsoft 365 F3（慈善）</span><span class="sxs-lookup"><span data-stu-id="6393d-411">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="6393d-412">GBP</span><span class="sxs-lookup"><span data-stu-id="6393d-412">GBP</span></span> | <span data-ttu-id="6393d-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="6393d-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="6393d-414">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="6393d-414">AAD-11626</span></span> |
| <span data-ttu-id="6393d-415">Microsoft 365 F3（商业）</span><span class="sxs-lookup"><span data-stu-id="6393d-415">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="6393d-416">EUR</span><span class="sxs-lookup"><span data-stu-id="6393d-416">EUR</span></span>| <span data-ttu-id="6393d-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="6393d-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="6393d-418">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="6393d-418">AAA-89898</span></span> |
 
<span data-ttu-id="6393d-419">太平洋标准时间 3 月 16 日下午 5 点更新了 3 月和 4 月预览版基于许可证的价目表。</span><span class="sxs-lookup"><span data-stu-id="6393d-419">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-420">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-420">Next steps</span></span>

- <span data-ttu-id="6393d-421">合作伙伴应将重新下载当前基于许可证的价目表（3 月和 4 月预览版），其中包含相应的这些价格更正。</span><span class="sxs-lookup"><span data-stu-id="6393d-421">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="6393d-422">Microsoft 将在未来几周内通过电子邮件联系受影响的合作伙伴，告知他们与更正受影响的交易相关的后续步骤。</span><span class="sxs-lookup"><span data-stu-id="6393d-422">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-423">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-423">Questions?</span></span>

<span data-ttu-id="6393d-424">如果有任何进一步的问题，请访问相关的 CSP Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-424">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a><span data-ttu-id="6393d-425">通过合作伙伴中心更新法定公司名称</span><span class="sxs-lookup"><span data-stu-id="6393d-425">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-426">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-426">Categories</span></span>

- <span data-ttu-id="6393d-427">日期：2021-03-16</span><span class="sxs-lookup"><span data-stu-id="6393d-427">Date: 2021-03-16</span></span>
- <span data-ttu-id="6393d-428">促使提高效率和规模</span><span class="sxs-lookup"><span data-stu-id="6393d-428">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-429">总结</span><span class="sxs-lookup"><span data-stu-id="6393d-429">Summary</span></span>

<span data-ttu-id="6393d-430">从 2021 年 3 月起，Microsoft 合作伙伴网络 (MPN) 合作伙伴和云解决方案提供商 (CSP) 间接经销商可通过合作伙伴中心更新其法定公司名称。</span><span class="sxs-lookup"><span data-stu-id="6393d-430">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-431">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-431">Impacted audience</span></span>

<span data-ttu-id="6393d-432">MPN 合作伙伴和 CSP 间接经销商（不适用于 CSP 直接计费合作伙伴）</span><span class="sxs-lookup"><span data-stu-id="6393d-432">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="6393d-433">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-433">Details</span></span>

<span data-ttu-id="6393d-434">从 2021 年 3 月起，MPN 合作伙伴和 CSP 间接经销商可在合作伙伴中心通过兼容的自助服务方式更新其法定公司名称。</span><span class="sxs-lookup"><span data-stu-id="6393d-434">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="6393d-435">借助这项新功能，合作伙伴将无需再提交合作伙伴中心支持票证来更新其公司名称。</span><span class="sxs-lookup"><span data-stu-id="6393d-435">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="6393d-436">这样可以在合作伙伴执行这些活动时节省大量时间。</span><span class="sxs-lookup"><span data-stu-id="6393d-436">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="6393d-437">若要了解详细信息，请参阅[更新法定公司资料](../update-your-partner-profile.md#update-your-legal-business-profile)。</span><span class="sxs-lookup"><span data-stu-id="6393d-437">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="6393d-438">请确保法定公司资料中的公司名称没有拼写错误和缩写，并且与正式的公司商业注册记录完全一致。</span><span class="sxs-lookup"><span data-stu-id="6393d-438">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="6393d-439">若要详细了解如何更新组织资料，请查看[验证组织资料](../update-your-partner-profile.md#update-your-legal-business-profile)。</span><span class="sxs-lookup"><span data-stu-id="6393d-439">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-440">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-440">Next steps</span></span>

<span data-ttu-id="6393d-441">在组织中分享此信息，以便相应团队可查看和更新其流程。</span><span class="sxs-lookup"><span data-stu-id="6393d-441">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-442">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-442">Questions?</span></span>

<span data-ttu-id="6393d-443">如果有任何进一步的问题，请访问相关的 CSP Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-443">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a><span data-ttu-id="6393d-444">云解决方案提供商 (CSP) 计划演进和开放式许可计划变更更新</span><span class="sxs-lookup"><span data-stu-id="6393d-444">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-445">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-445">Categories</span></span>

- <span data-ttu-id="6393d-446">日期：2021-03-15</span><span class="sxs-lookup"><span data-stu-id="6393d-446">Date: 2021-03-15</span></span>
- <span data-ttu-id="6393d-447">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-447">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-448">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-448">Summary</span></span>

<span data-ttu-id="6393d-449">除了开放式许可计划出现变更，云解决方案提供商 (CSP) 也将增添新的商业和公共领域永久性软件产品。</span><span class="sxs-lookup"><span data-stu-id="6393d-449">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-450">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-450">Impacted audience</span></span>

<span data-ttu-id="6393d-451">通过开放式许可计划销售的商业分销商和托管经销商，以及交易永久性软件的所有 CSP 合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-451">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="6393d-452">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-452">Details</span></span>

<span data-ttu-id="6393d-453">在 2020 年 9 月，Microsoft 就其数字转型之旅[宣布了](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)一系列的措施，目的是将机会扩大给已加入 CSP 计划的合作伙伴，这些机会包括合作伙伴本地软件的可用性。</span><span class="sxs-lookup"><span data-stu-id="6393d-453">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="6393d-454">借助这些变更，合作伙伴可利用 CSP 中的软件许可证发展自身业务并扩大触达范围，在如今以云为先的世界里摆正自己的定位来争取成功。</span><span class="sxs-lookup"><span data-stu-id="6393d-454">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="6393d-455">它们还帮助客户过渡到云中，并为合作伙伴提供客户混合云环境所需的灵活性。</span><span class="sxs-lookup"><span data-stu-id="6393d-455">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="6393d-456">在这次数字转型的延续中，我们宣布进行以下变更：</span><span class="sxs-lookup"><span data-stu-id="6393d-456">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="6393d-457">2021 年 7 月 1 日：不向开放式许可计划价目表添加任何新的 SKU、产品或促销。</span><span class="sxs-lookup"><span data-stu-id="6393d-457">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="6393d-458">2021 年 7 月 7 日：将向 CSP 永久性软件价目表添加两款商业产品/服务（Get Genuine Windows 和 Visual Studio Professional）和公共领域产品/服务（政府、教育和非营利性组织 - 具体查看[公告](./2020-december.md#9)）。</span><span class="sxs-lookup"><span data-stu-id="6393d-458">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="6393d-459">可在合作伙伴中心的[“销售”>“定价与产品”](https://partnercenter.microsoft.com/pcv/sales)的“软件”部分找到价目表，且该表格将在该日期重新发布。</span><span class="sxs-lookup"><span data-stu-id="6393d-459">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="6393d-460">有关 CSP 计划演进和开放式许可计划变更的完整详细信息，请查看下面的后续步骤。</span><span class="sxs-lookup"><span data-stu-id="6393d-460">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-461">后续步骤：</span><span class="sxs-lookup"><span data-stu-id="6393d-461">Next Steps:</span></span>

- <span data-ttu-id="6393d-462">CSP 计划演进：请查看[云解决方案提供商计划中的永久性软件](https://partner.microsoft.com/resources/collection/software-in-csp#/)就绪性资料。</span><span class="sxs-lookup"><span data-stu-id="6393d-462">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="6393d-463">请使用此[就绪性地图](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)快速找到适合你的角色的信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-463">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="6393d-464">开放式许可计划变更：请查看 [CSP 计划演进和开放式许可计划变更](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)就绪性资料。</span><span class="sxs-lookup"><span data-stu-id="6393d-464">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="6393d-465">请使用此[就绪性地图](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)快速找到适合你的角色的信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-465">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-466">问题</span><span class="sxs-lookup"><span data-stu-id="6393d-466">Questions</span></span>

<span data-ttu-id="6393d-467">如果有任何进一步的问题，请访问相关的 CSP Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-467">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="6393d-468">对上一公告的更新：高级评估，合规性管理器加载项</span><span class="sxs-lookup"><span data-stu-id="6393d-468">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-469">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-469">Categories</span></span>

- <span data-ttu-id="6393d-470">日期：2021-03-15</span><span class="sxs-lookup"><span data-stu-id="6393d-470">Date: 2021-03-15</span></span>
- <span data-ttu-id="6393d-471">拓展业务</span><span class="sxs-lookup"><span data-stu-id="6393d-471">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-472">总结</span><span class="sxs-lookup"><span data-stu-id="6393d-472">Summary</span></span>

<span data-ttu-id="6393d-473">不得在价目表中列出试用版产品/服务，这些内容将被删除。</span><span class="sxs-lookup"><span data-stu-id="6393d-473">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-474">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-474">Impacted audience</span></span>

<span data-ttu-id="6393d-475">通过云解决方案提供商交易的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-475">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="6393d-476">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-476">Details</span></span>

<span data-ttu-id="6393d-477">价目表中不得包含试用版产品/服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-477">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="6393d-478">这些内容将从 2021 年 5 月 1 日的价目表中删除。</span><span class="sxs-lookup"><span data-stu-id="6393d-478">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="6393d-479">如需最初公告，请查看[此处](./2021-february.md#4)。</span><span class="sxs-lookup"><span data-stu-id="6393d-479">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="6393d-480">其他资源</span><span class="sxs-lookup"><span data-stu-id="6393d-480">Additional resources</span></span>

- [<span data-ttu-id="6393d-481">Microsoft 365 E5 安全性和合规性</span><span class="sxs-lookup"><span data-stu-id="6393d-481">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="6393d-482">在 Microsoft 合规性管理器中生成和管理评估 - Microsoft 365 合规性</span><span class="sxs-lookup"><span data-stu-id="6393d-482">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="6393d-483">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-483">Next steps</span></span>

<span data-ttu-id="6393d-484">查看有关本主题的资源，并与组织内部的相关利益干系人共享此信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-484">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-485">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-485">Questions?</span></span>

<span data-ttu-id="6393d-486">如果对这些产品/服务有疑问，请查看相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-486">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a><span data-ttu-id="6393d-487">将解决方案从 One Commercial Partner (OCP) 进入市场 (GTM) 迁移到 Microsoft 商业市场</span><span class="sxs-lookup"><span data-stu-id="6393d-487">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-488">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-488">Categories</span></span>

- <span data-ttu-id="6393d-489">日期：2021-03-12</span><span class="sxs-lookup"><span data-stu-id="6393d-489">Date: 2021-03-12</span></span>
- <span data-ttu-id="6393d-490">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-490">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-491">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-491">Summary</span></span>

<span data-ttu-id="6393d-492">从 2021 年 3 月 29 日开始，你将开始体验功能受限的 One Commercial Partner (OCP) 进入市场 (GTM) 功能。</span><span class="sxs-lookup"><span data-stu-id="6393d-492">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="6393d-493">建议你将解决方案迁移到合作伙伴中心的商业市场。</span><span class="sxs-lookup"><span data-stu-id="6393d-493">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-494">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-494">Impacted audience</span></span>

<span data-ttu-id="6393d-495">在 OCP GTM 中联合销售解决方案的组织</span><span class="sxs-lookup"><span data-stu-id="6393d-495">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="6393d-496">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-496">Details</span></span>

<span data-ttu-id="6393d-497">在 2020 年 12 月，我们开始了从 Microsoft OCP GTM 工具迁移到合作伙伴中心的 Microsoft 商业市场的旅程。</span><span class="sxs-lookup"><span data-stu-id="6393d-497">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="6393d-498">这次过渡扩展了商业市场的能力，你可在这里向数百万名客户展示你的解决方案、与其他 Microsoft 和合作伙伴卖方相互分享销售机会，并联手销售创新的解决方案。</span><span class="sxs-lookup"><span data-stu-id="6393d-498">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="6393d-499">本次过渡的下一里程碑举措将在 2021 年 3 月 29 日实施。</span><span class="sxs-lookup"><span data-stu-id="6393d-499">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="6393d-500">届时，你将开始体验功能受限的 OCP GTM 功能，其中某些方面变为只供查看。</span><span class="sxs-lookup"><span data-stu-id="6393d-500">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="6393d-501">如果你当前正在 OCP GTM 中联合销售解决方案，建议你将解决方案迁移到商业市场来利用该市场中的功能并简化你的发布体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-501">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="6393d-502">移到商业市场后，合作伙伴中心就成为了获取联合销售发布体验的主要位置。</span><span class="sxs-lookup"><span data-stu-id="6393d-502">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="6393d-503">在这里，你可通过与我们对 Microsoft 产品使用的一样的通道和产品内体验将你的解决方案推广给我们共同的客户，从而继续发展你的业务。</span><span class="sxs-lookup"><span data-stu-id="6393d-503">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="6393d-504">[详细了解商业市场](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)。</span><span class="sxs-lookup"><span data-stu-id="6393d-504">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-505">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-505">Next steps</span></span>

- <span data-ttu-id="6393d-506">如果你尚未移动解决方案，请按照[过渡指南](/azure/marketplace/co-sell-solution-migration)中详述的说明或查看[视频分步教程](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)，来完成各项迁移活动并开始在商业市场发布你的解决方案。</span><span class="sxs-lookup"><span data-stu-id="6393d-506">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="6393d-507">如果对 OCP GTM 中的受限功能体验存有疑问，请查看[在 Microsoft 商业市场中发布内容的联合销售要求常见问题解答](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)。</span><span class="sxs-lookup"><span data-stu-id="6393d-507">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="6393d-508">（请查看“从 2021 年 3 月 29 日起推出 OCP GTM 受限功能”部分。）</span><span class="sxs-lookup"><span data-stu-id="6393d-508">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-509">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-509">Questions?</span></span>

<span data-ttu-id="6393d-510">如有任何疑问或需要更多信息，请联系[支持人员](https://partner.microsoft.com/support/?stage=1) 。</span><span class="sxs-lookup"><span data-stu-id="6393d-510">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="6393d-511">将 Azure 的云解决方案提供商 (CSP) 计划中新推出的商业体验扩展到俄罗斯</span><span class="sxs-lookup"><span data-stu-id="6393d-511">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-512">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-512">Categories</span></span>

- <span data-ttu-id="6393d-513">日期：2021-03-10</span><span class="sxs-lookup"><span data-stu-id="6393d-513">Date: 2021-03-10</span></span>
- <span data-ttu-id="6393d-514">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-514">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-515">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-515">Impacted audience</span></span>

<span data-ttu-id="6393d-516">参与云解决方案提供商 (CSP) 计划的所有俄罗斯的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="6393d-516">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="6393d-517">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-517">Details</span></span>

<span data-ttu-id="6393d-518">我们很高兴宣布，从 2021 年 3 月 10 日起在俄罗斯的 CSP for Azure 中推出新的商业体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-518">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="6393d-519">此体验将简化和改进客户购买及使用 Azure 服务的方式。</span><span class="sxs-lookup"><span data-stu-id="6393d-519">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="6393d-520">通过它，已加入 CSP 计划的合作伙伴可查看各销售活动中 Azure 定价的一致视图、获取美元定价（它可确保全球价格一致）、确保计费日期一致并访问 Azure 成本管理功能。</span><span class="sxs-lookup"><span data-stu-id="6393d-520">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-521">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-521">Next steps</span></span>

<span data-ttu-id="6393d-522">提供了有多项资源，它们引入了新的 Azure 商业体验并提供其他信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-522">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="6393d-523">有关最新的常见问题解答、宣传资料和视频等内容，可查看 [CSP 计划更新资源库](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).。</span><span class="sxs-lookup"><span data-stu-id="6393d-523">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="6393d-524">合作伙伴中心软件许可证密钥和下载履行</span><span class="sxs-lookup"><span data-stu-id="6393d-524">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-525">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-525">Categories</span></span>

- <span data-ttu-id="6393d-526">日期：2021-03-04</span><span class="sxs-lookup"><span data-stu-id="6393d-526">Date: 2021-03-04</span></span>
- <span data-ttu-id="6393d-527">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-527">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-528">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-528">Summary</span></span>

<span data-ttu-id="6393d-529">现已恢复合作伙伴中心软件下载和许可证密钥履行功能。</span><span class="sxs-lookup"><span data-stu-id="6393d-529">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-530">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-530">Impacted audience</span></span>

<span data-ttu-id="6393d-531">通过合作伙伴中心处理永久性和服务器订阅软件订单的所有云解决方案提供商 (CSP) 合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-531">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="6393d-532">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-532">Details</span></span>

<span data-ttu-id="6393d-533">为了回应合作伙伴反馈，我们将恢复合作伙伴中心履行功能，你可为永久性和服务器订阅软件订单获取软件和许可证密钥。</span><span class="sxs-lookup"><span data-stu-id="6393d-533">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="6393d-534">此功能会还原到其之前的状态，然后在 2021 年 1 月 19 日被移除。</span><span class="sxs-lookup"><span data-stu-id="6393d-534">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="6393d-535">（请查看[公告](2020-september.md#17)。）</span><span class="sxs-lookup"><span data-stu-id="6393d-535">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="6393d-536">请注意，软件许可证密钥和下载链接是宝贵且受到热烈追捧的知识产权资产。</span><span class="sxs-lookup"><span data-stu-id="6393d-536">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="6393d-537">如果遭到泄露，其激活限制可能很快就被会耗尽，导致出现负面的客户和合作伙伴体验。</span><span class="sxs-lookup"><span data-stu-id="6393d-537">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-538">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-538">Next steps</span></span>

<span data-ttu-id="6393d-539">请查看下列资源，了解有关软件密钥分发的使用说明和重要指导：</span><span class="sxs-lookup"><span data-stu-id="6393d-539">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="6393d-540">通过 CSP 计划出售本地软件</span><span class="sxs-lookup"><span data-stu-id="6393d-540">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="6393d-541">[合作伙伴中心新版商业操作指南](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)（请查看“软件密钥分发指导”部分。）</span><span class="sxs-lookup"><span data-stu-id="6393d-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-542">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-542">Questions?</span></span>

<span data-ttu-id="6393d-543">如果对此通知还有其他疑问，请访问相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-543">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="6393d-544">将交易从 Partner Sales Connect (PSC) 迁移到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6393d-544">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-545">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-545">Categories</span></span>

- <span data-ttu-id="6393d-546">日期：2021-03-04</span><span class="sxs-lookup"><span data-stu-id="6393d-546">Date: 2021-03-04</span></span>
- <span data-ttu-id="6393d-547">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-547">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-548">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-548">Summary</span></span>

<span data-ttu-id="6393d-549">自 2021 年 3 月 31 日起，将只能以只读方式访问 Partner Sales Connect (PSC)，因此请开始将你在 PSC 中的交易迁移到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="6393d-549">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-550">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-550">Impacted audience</span></span>

<span data-ttu-id="6393d-551">在 PSC 中具有交易的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-551">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="6393d-552">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-552">Details</span></span>

<span data-ttu-id="6393d-553">作为我们共同的发展承诺的一部分，与 Microsoft 联合销售让你能够被发现、表现你的专业知识并扩大客户群体来获得积极的客户成果 。</span><span class="sxs-lookup"><span data-stu-id="6393d-553">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="6393d-554">在合作伙伴中心管理你的联合销售体验将使平均交易时间比平时快 3.5 倍，让你能够跨直接客户、合作伙伴和 Microsoft 卖家渠道进行销售，并在一个位置管理你的整个推荐管道。</span><span class="sxs-lookup"><span data-stu-id="6393d-554">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="6393d-555">自 2021 年 3 月 31 日起，将只能以只读方式访问 PSC，因此请开始迁移到合作伙伴中心，获取下列功能改进  ：</span><span class="sxs-lookup"><span data-stu-id="6393d-555">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="6393d-556">根据你需要的协助类型，更准确地将你与 Microsoft 共享的交易引导给适当的卖家。</span><span class="sxs-lookup"><span data-stu-id="6393d-556">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="6393d-557">对符合激励计划的解决方案的前期交易资格验证，目的是满足 ISV Connect 计划标准，从而简化审批过程和最终的执行证明 (POE)。</span><span class="sxs-lookup"><span data-stu-id="6393d-557">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="6393d-558">无缝的用户体验，可在一个位置管理你的联合销售机会和销售合格潜在客户。</span><span class="sxs-lookup"><span data-stu-id="6393d-558">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="6393d-559">我们最近还在合作伙伴中心增添了新的功能来帮助你进行迁移：</span><span class="sxs-lookup"><span data-stu-id="6393d-559">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="6393d-560">针对联合销售机会的批量操作</span><span class="sxs-lookup"><span data-stu-id="6393d-560">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="6393d-561">[交易迁移功能](../psc-to-pc.md)（请查看“PSC 交易迁移”部分。）</span><span class="sxs-lookup"><span data-stu-id="6393d-561">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="6393d-562">借助合作伙伴中心的联合销售体验，你的销售团队将有更多时间专注于培养潜在客户、创造机会、达成交易和建立持久的客户关系。</span><span class="sxs-lookup"><span data-stu-id="6393d-562">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6393d-563">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-563">Next steps</span></span>

<span data-ttu-id="6393d-564">使用合作伙伴中心[过渡指南](../psc-to-pc.md)引导自己完成将交易从 PSC 迁移到合作伙伴中心的步骤。</span><span class="sxs-lookup"><span data-stu-id="6393d-564">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-565">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-565">Questions?</span></span>

<span data-ttu-id="6393d-566">如果还有其他疑问，请联系[支持部门](https://partner.microsoft.com/support/?stage=1)。</span><span class="sxs-lookup"><span data-stu-id="6393d-566">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="6393d-567">将于 2021 年 4 月 1 日推出的新增 Microsoft Dynamics 365 产品和服务</span><span class="sxs-lookup"><span data-stu-id="6393d-567">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-568">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-568">Categories</span></span>

- <span data-ttu-id="6393d-569">日期：2021-03-04</span><span class="sxs-lookup"><span data-stu-id="6393d-569">Date: 2021-03-04</span></span>
- <span data-ttu-id="6393d-570">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-570">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-571">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-571">Summary</span></span>

<span data-ttu-id="6393d-572">在 2021 年 4 月 1 日，Microsoft 将对云解决方案提供商 (CSP) 计划推出几项新的产品和服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-572">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-573">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-573">Impacted audience</span></span>

<span data-ttu-id="6393d-574">参与云解决方案提供商 (CSP) 计划的所有合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-574">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="6393d-575">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-575">Details</span></span>

<span data-ttu-id="6393d-576">在 2021 年 4 月 1 日，Microsoft 将推出下列新产品和服务：</span><span class="sxs-lookup"><span data-stu-id="6393d-576">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="6393d-577">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="6393d-577">Power BI Premium Per User</span></span>
- <span data-ttu-id="6393d-578">Customer Voice 和 Marketing USL 地域和细分市场拓展</span><span class="sxs-lookup"><span data-stu-id="6393d-578">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="6393d-579">**Power BI Premium Per User**</span><span class="sxs-lookup"><span data-stu-id="6393d-579">**Power BI Premium Per User**</span></span>

<span data-ttu-id="6393d-580">Microsoft 将引入首批 Power BI Premium 每用户产品/服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-580">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="6393d-581">目前仅在容量构造中出售 Power BI Premium。</span><span class="sxs-lookup"><span data-stu-id="6393d-581">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="6393d-582">通过 Power BI Premium Per User，可访问企业商业智能 (BI) 和分析功能。</span><span class="sxs-lookup"><span data-stu-id="6393d-582">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="6393d-583">其灵活的个人席位许可很适合中小型企业。</span><span class="sxs-lookup"><span data-stu-id="6393d-583">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="6393d-584">若要详细了解此产品/服务，请查看 [Power BI 发布详细信息](/power-platform-release-plan/2020wave2/power-bi/planned-features)。</span><span class="sxs-lookup"><span data-stu-id="6393d-584">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="6393d-585">**产品/服务详细信息**</span><span class="sxs-lookup"><span data-stu-id="6393d-585">**Offer details**</span></span>

<span data-ttu-id="6393d-586">请注意，产品/服务名称与价目表预览中的略有不同。</span><span class="sxs-lookup"><span data-stu-id="6393d-586">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="6393d-587">产品名称</span><span class="sxs-lookup"><span data-stu-id="6393d-587">Offer name</span></span> | <span data-ttu-id="6393d-588">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-588">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="6393d-589">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="6393d-589">Power BI Premium Per User</span></span> | <span data-ttu-id="6393d-590">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="6393d-590">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="6393d-591">Power BI Premium Per User 教职员工版</span><span class="sxs-lookup"><span data-stu-id="6393d-591">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="6393d-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="6393d-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="6393d-593">Power BI Premium Per User 学生版</span><span class="sxs-lookup"><span data-stu-id="6393d-593">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="6393d-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="6393d-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="6393d-595">Power BI Premium Per User（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-595">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6393d-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="6393d-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="6393d-597">Power BI Premium Per User 加载项</span><span class="sxs-lookup"><span data-stu-id="6393d-597">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="6393d-598">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="6393d-598">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="6393d-599">Power BI Premium Per User 加载项教职员工版</span><span class="sxs-lookup"><span data-stu-id="6393d-599">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="6393d-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="6393d-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="6393d-601">Power BI Premium Per User 加载项学生版</span><span class="sxs-lookup"><span data-stu-id="6393d-601">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="6393d-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="6393d-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="6393d-603">Power BI Premium Per User 加载项（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-603">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6393d-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="6393d-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="6393d-605">**Customer Voice 和 Marketing USL 地域和细分市场拓展**</span><span class="sxs-lookup"><span data-stu-id="6393d-605">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="6393d-606">作为 2020 年 12 月发布的后续，Dynamics 365 Customer Voice 和 Marketing USL 产品/服务进行了更改，现增添新的国家/地区和更多非营利及教育 SKU。</span><span class="sxs-lookup"><span data-stu-id="6393d-606">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="6393d-607">产品名称</span><span class="sxs-lookup"><span data-stu-id="6393d-607">Offer name</span></span> | <span data-ttu-id="6393d-608">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-608">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="6393d-609">Dynamics 365 Customer Voice USL（非营利组织员工定价）</span><span class="sxs-lookup"><span data-stu-id="6393d-609">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6393d-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="6393d-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="6393d-611">Dynamics 365 Customer Voice USL 教职员工版</span><span class="sxs-lookup"><span data-stu-id="6393d-611">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="6393d-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="6393d-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="6393d-613">请访问以下页面，详细了解这些产品/服务：</span><span class="sxs-lookup"><span data-stu-id="6393d-613">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="6393d-614">Dynamics 365 Customer Service Voice 主页</span><span class="sxs-lookup"><span data-stu-id="6393d-614">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="6393d-615">Dynamics 365 Marketing 主页</span><span class="sxs-lookup"><span data-stu-id="6393d-615">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="6393d-616">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-616">Next steps</span></span>

<span data-ttu-id="6393d-617">请查看此主题的相关资源，与组织中的适当利益干系人分享此信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-617">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="6393d-618">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="6393d-618">Questions?</span></span>

<span data-ttu-id="6393d-619">如果对这些产品/服务有任何疑问，请查看相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-619">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a><span data-ttu-id="6393d-620">现已在部分套件中提供 Microsoft 通用打印服务</span><span class="sxs-lookup"><span data-stu-id="6393d-620">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="6393d-621">类别</span><span class="sxs-lookup"><span data-stu-id="6393d-621">Categories</span></span>

- <span data-ttu-id="6393d-622">日期：2021-03-03</span><span class="sxs-lookup"><span data-stu-id="6393d-622">Date: 2021-03-03</span></span>
- <span data-ttu-id="6393d-623">功能</span><span class="sxs-lookup"><span data-stu-id="6393d-623">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6393d-624">摘要</span><span class="sxs-lookup"><span data-stu-id="6393d-624">Summary</span></span>

<span data-ttu-id="6393d-625">从 2021 年 3 月 1 日起，可在特选 Microsoft 365 套件中或以独立加载项的形式办理 Microsoft 通用打印服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-625">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6393d-626">影响受众</span><span class="sxs-lookup"><span data-stu-id="6393d-626">Impacted audience</span></span>

<span data-ttu-id="6393d-627">参与云解决方案提供商 (CSP) 计划的所有合作伙伴</span><span class="sxs-lookup"><span data-stu-id="6393d-627">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="6393d-628">详细信息</span><span class="sxs-lookup"><span data-stu-id="6393d-628">Details</span></span>

<span data-ttu-id="6393d-629">[通用打印](https://aka.ms/universalprint)是一项 Microsoft 365 打印服务，它让你不再需要本地打印服务器，还使 Windows 设备能够打印到注册了 Azure 的打印机。</span><span class="sxs-lookup"><span data-stu-id="6393d-629">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="6393d-630">自 2021 年 3 月 1 日起可办理此功能。</span><span class="sxs-lookup"><span data-stu-id="6393d-630">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="6393d-631">免用驱动程序的打印、基于位置轻松发现打印机，以及无需累积学习的直观打印体验，这些都使员工受益匪浅。</span><span class="sxs-lookup"><span data-stu-id="6393d-631">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="6393d-632">已加入 Azure Active Directory (Azure AD) 的设备使用现有的 Azure AD 凭据安全地进行打印。</span><span class="sxs-lookup"><span data-stu-id="6393d-632">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="6393d-633">管理员通过 Azure 门户管理打印，并可借助对通用打印的本机支持轻松连接打印机。</span><span class="sxs-lookup"><span data-stu-id="6393d-633">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="6393d-634">可使用通用打印连接器软件在不简单的打印机上部署通用打印服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-634">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="6393d-635">在通用打印发布时，Windows E3、A3、E5 和 A5 以及 Microsoft 365 BP、F3、E3、A3、E5 和 A5 上将恢复该项服务。</span><span class="sxs-lookup"><span data-stu-id="6393d-635">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="6393d-636">**产品/服务详细信息**</span><span class="sxs-lookup"><span data-stu-id="6393d-636">**Offer details**</span></span>

<span data-ttu-id="6393d-637">请注意，产品/服务名称与价目表预览中的略有不同。</span><span class="sxs-lookup"><span data-stu-id="6393d-637">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="6393d-638">产品名称</span><span class="sxs-lookup"><span data-stu-id="6393d-638">Offer name</span></span> | <span data-ttu-id="6393d-639">产品/服务 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-639">Offer ID</span></span> | <span data-ttu-id="6393d-640">材料 ID</span><span class="sxs-lookup"><span data-stu-id="6393d-640">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="6393d-641">通用打印卷加载项（500 个作业）- Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6393d-641">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="6393d-642">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="6393d-642">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="6393d-643">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="6393d-643">9BI-00004</span></span>   |
| <span data-ttu-id="6393d-644">通用打印卷加载项（500 个作业）教职员工版 - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6393d-644">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="6393d-645">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="6393d-645">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="6393d-646">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="6393d-646">9BK-00004</span></span>   |
| <span data-ttu-id="6393d-647">通用打印卷加载项（500 个作业）- Windows</span><span class="sxs-lookup"><span data-stu-id="6393d-647">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="6393d-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="6393d-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="6393d-649">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="6393d-649">9BI-00002</span></span>   |
| <span data-ttu-id="6393d-650">通用打印卷加载项（500 个作业）教职员工版 - Windows</span><span class="sxs-lookup"><span data-stu-id="6393d-650">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="6393d-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="6393d-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="6393d-652">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="6393d-652">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="6393d-653">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6393d-653">Next steps</span></span>

<span data-ttu-id="6393d-654">熟悉价目表和[通用打印概述](/universal-print/fundamentals/universal-print-whatis)。</span><span class="sxs-lookup"><span data-stu-id="6393d-654">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="6393d-655">请与贵组织中的相应联系人共享这些信息。</span><span class="sxs-lookup"><span data-stu-id="6393d-655">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6393d-656">有疑问？</span><span class="sxs-lookup"><span data-stu-id="6393d-656">Questions?</span></span>

<span data-ttu-id="6393d-657">如果对这些产品/服务有任何疑问，请查看相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="6393d-657">For any questions about these offers, check your relevant Yammer communities.</span></span>
