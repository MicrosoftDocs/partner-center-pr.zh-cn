---
title: 2021 年 4 月公告
description: Microsoft 合作伙伴中心 2021 年 4 月公告，包括新功能、促销、产品/服务、市场或对现有产品/服务的更改。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150125"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="4beed-103">2021 年 4 月公告</span><span class="sxs-lookup"><span data-stu-id="4beed-103">April 2021 announcements</span></span>

<span data-ttu-id="4beed-104">本页提供了 Microsoft 合作伙伴中心 2021 年 4 月公告。</span><span class="sxs-lookup"><span data-stu-id="4beed-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="4beed-105">就绪情况：更新的 CSP 客户地址验证 API 将于 6 月上线；测试功能现已可用</span><span class="sxs-lookup"><span data-stu-id="4beed-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-106">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-106">Categories</span></span>

- <span data-ttu-id="4beed-107">日期：2021-04-30</span><span class="sxs-lookup"><span data-stu-id="4beed-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="4beed-108">就绪</span><span class="sxs-lookup"><span data-stu-id="4beed-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-109">总结</span><span class="sxs-lookup"><span data-stu-id="4beed-109">Summary</span></span>

<span data-ttu-id="4beed-110">为帮助合作伙伴和客户在相互信任的基础上开展其业务，我们将邀请世界各地的合作伙伴测试对验证地址 API 的更改。</span><span class="sxs-lookup"><span data-stu-id="4beed-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-111">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-111">Impacted audience</span></span>

<span data-ttu-id="4beed-112">新建客户地址详细信息或更新现有客户地址详细信息的 CSP 直接计费合作伙伴和间接提供商</span><span class="sxs-lookup"><span data-stu-id="4beed-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="4beed-113">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-113">Details</span></span>

<span data-ttu-id="4beed-114">Microsoft 值得信赖。</span><span class="sxs-lookup"><span data-stu-id="4beed-114">Microsoft runs on trust.</span></span> <span data-ttu-id="4beed-115">我们致力于在 CSP 计划中为交易客户订阅提供合规、安全且可靠的客户地址验证方法。</span><span class="sxs-lookup"><span data-stu-id="4beed-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="4beed-116">从 2021 年 3 月 31 日起，我们已向验证地址 API 中引入更改。</span><span class="sxs-lookup"><span data-stu-id="4beed-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="4beed-117">我们邀请合作伙伴在上线之前（2021 年 6 月底）测试该 API。</span><span class="sxs-lookup"><span data-stu-id="4beed-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="4beed-118">请注意，这些更改仅影响验证地址 API。</span><span class="sxs-lookup"><span data-stu-id="4beed-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="4beed-119">创建客户和更新计费配置文件 API 不受影响。</span><span class="sxs-lookup"><span data-stu-id="4beed-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="4beed-120">尽管建议的地址目前不需要与创建客户 API 结合使用，但强烈建议这样做。</span><span class="sxs-lookup"><span data-stu-id="4beed-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="4beed-121">响应将返回以下某个状态消息：</span><span class="sxs-lookup"><span data-stu-id="4beed-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="4beed-122">状态</span><span class="sxs-lookup"><span data-stu-id="4beed-122">Status</span></span>     | <span data-ttu-id="4beed-123">说明</span><span class="sxs-lookup"><span data-stu-id="4beed-123">Description</span></span> |    <span data-ttu-id="4beed-124">返回的建议地址数</span><span class="sxs-lookup"><span data-stu-id="4beed-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="4beed-125">Verified shippable</span><span class="sxs-lookup"><span data-stu-id="4beed-125">Verified shippable</span></span> | <span data-ttu-id="4beed-126">地址已经过验证且可送达。</span><span class="sxs-lookup"><span data-stu-id="4beed-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="4beed-127">Single</span><span class="sxs-lookup"><span data-stu-id="4beed-127">Single</span></span> |
|<span data-ttu-id="4beed-128">已验证</span><span class="sxs-lookup"><span data-stu-id="4beed-128">Verified</span></span> | <span data-ttu-id="4beed-129">已验证地址。</span><span class="sxs-lookup"><span data-stu-id="4beed-129">Address is verified.</span></span> | <span data-ttu-id="4beed-130">Single</span><span class="sxs-lookup"><span data-stu-id="4beed-130">Single</span></span> |
|<span data-ttu-id="4beed-131">Interaction required</span><span class="sxs-lookup"><span data-stu-id="4beed-131">Interaction required</span></span> | <span data-ttu-id="4beed-132">建议的地址发生了重大更改，需要用户确认。</span><span class="sxs-lookup"><span data-stu-id="4beed-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="4beed-133">Single</span><span class="sxs-lookup"><span data-stu-id="4beed-133">Single</span></span> |
|<span data-ttu-id="4beed-134">Street partial</span><span class="sxs-lookup"><span data-stu-id="4beed-134">Street partial</span></span> | <span data-ttu-id="4beed-135">地址中给出的街道信息不完整，需要更多信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="4beed-136">多个 - 最多 3 个</span><span class="sxs-lookup"><span data-stu-id="4beed-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="4beed-137">Premises partial</span><span class="sxs-lookup"><span data-stu-id="4beed-137">Premises partial</span></span> | <span data-ttu-id="4beed-138">给出的场所信息（楼栋号、房号等）不完整，需要更多信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="4beed-139">多个 - 最多 3 个</span><span class="sxs-lookup"><span data-stu-id="4beed-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="4beed-140">多个</span><span class="sxs-lookup"><span data-stu-id="4beed-140">Multiple</span></span> | <span data-ttu-id="4beed-141">地址中有多个字段不完整（也可能包括 street partial 和 premises partial）。</span><span class="sxs-lookup"><span data-stu-id="4beed-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="4beed-142">多个 - 最多 3 个</span><span class="sxs-lookup"><span data-stu-id="4beed-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="4beed-143">无</span><span class="sxs-lookup"><span data-stu-id="4beed-143">None</span></span> | <span data-ttu-id="4beed-144">地址错误。</span><span class="sxs-lookup"><span data-stu-id="4beed-144">Address is incorrect.</span></span> | <span data-ttu-id="4beed-145">无</span><span class="sxs-lookup"><span data-stu-id="4beed-145">None</span></span> |
|<span data-ttu-id="4beed-146">未验证</span><span class="sxs-lookup"><span data-stu-id="4beed-146">Not validated</span></span> | <span data-ttu-id="4beed-147">无法通过验证过程发送地址。</span><span class="sxs-lookup"><span data-stu-id="4beed-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="4beed-148">无</span><span class="sxs-lookup"><span data-stu-id="4beed-148">None</span></span> |

<span data-ttu-id="4beed-149">美国邮政编码将返回额外 4 个数字 + 连字符，例如 12345-6789。</span><span class="sxs-lookup"><span data-stu-id="4beed-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-150">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-150">Next steps</span></span>

- <span data-ttu-id="4beed-151">有关更详细的指南，请查看[专门的合作伙伴集锦](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)中的技术文档和常见问题。</span><span class="sxs-lookup"><span data-stu-id="4beed-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="4beed-152">准备使用合作伙伴中心 API 和 Web 用户体验来整合更改。</span><span class="sxs-lookup"><span data-stu-id="4beed-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="4beed-153">与行业专家 Ali Khaki 分享你的沙盒租户 ID，以加入外部测试，这样你便可以开始准备更新。</span><span class="sxs-lookup"><span data-stu-id="4beed-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="4beed-154">如果正在使用控制面板供应商 (CPV) 解决方案，请咨询 CPV。</span><span class="sxs-lookup"><span data-stu-id="4beed-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-155">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-155">Questions?</span></span>

<span data-ttu-id="4beed-156">如果在 Microsoft 运营方面需要支持，请联系你的合作伙伴 Yammer 支持组或创建[服务请求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。</span><span class="sxs-lookup"><span data-stu-id="4beed-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="4beed-157">合作伙伴中心 API Swagger 文档的新位置</span><span class="sxs-lookup"><span data-stu-id="4beed-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-158">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-158">Categories</span></span>

- <span data-ttu-id="4beed-159">日期：2021-04-26</span><span class="sxs-lookup"><span data-stu-id="4beed-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="4beed-160">功能</span><span class="sxs-lookup"><span data-stu-id="4beed-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-161">摘要</span><span class="sxs-lookup"><span data-stu-id="4beed-161">Summary</span></span>

<span data-ttu-id="4beed-162">合作伙伴中心 API Swagger 文档已从[以前的 Swagger 文档网站](https://apidocs.microsoft.com/services/partnercenter)迁移到[新 Swagger 文档网站](/rest/api/partner-center-rest/)。</span><span class="sxs-lookup"><span data-stu-id="4beed-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-163">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-163">Impacted audience</span></span>

<span data-ttu-id="4beed-164">使用合作伙伴中心 API 且参与云解决方案提供商 (CSP) 计划的直接计费合作伙伴和间接提供商</span><span class="sxs-lookup"><span data-stu-id="4beed-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="4beed-165">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-165">Details</span></span>

<span data-ttu-id="4beed-166">从 2021 年 4 月 26 日起，合作伙伴中心 API Swagger 文档（包括 Rest API 内容）在[新站点](/rest/api/partner-center-rest/)提供。</span><span class="sxs-lookup"><span data-stu-id="4beed-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="4beed-167">几周后，旧站点将无法访问。</span><span class="sxs-lookup"><span data-stu-id="4beed-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="4beed-168">好处</span><span class="sxs-lookup"><span data-stu-id="4beed-168">Benefits</span></span>

<span data-ttu-id="4beed-169">合作伙伴中心 API Swagger 文档将提供“试看”功能。</span><span class="sxs-lookup"><span data-stu-id="4beed-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="4beed-170">使用此功能需要拥有持有者令牌，可以按照[合作伙伴中心身份验证](/partner-center/develop/partner-center-authentication#app--user-authentication)中列出的步骤生成该令牌。</span><span class="sxs-lookup"><span data-stu-id="4beed-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-171">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-171">Next steps</span></span>

<span data-ttu-id="4beed-172">在组织中分享此信息，以便相应团队可查看和更新其流程。</span><span class="sxs-lookup"><span data-stu-id="4beed-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-173">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-173">Questions?</span></span>

<span data-ttu-id="4beed-174">如果对这些产品/服务有疑问，请查看相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="4beed-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="4beed-175">云解决方案提供商 (CSP) 软件退货期政策和下载链接有效期通知</span><span class="sxs-lookup"><span data-stu-id="4beed-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-176">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-176">Categories</span></span>

- <span data-ttu-id="4beed-177">日期：2021-04-21</span><span class="sxs-lookup"><span data-stu-id="4beed-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="4beed-178">功能</span><span class="sxs-lookup"><span data-stu-id="4beed-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-179">摘要</span><span class="sxs-lookup"><span data-stu-id="4beed-179">Summary</span></span>

<span data-ttu-id="4beed-180">CSP 软件退货期政策和下载链接有效期发生了更改。</span><span class="sxs-lookup"><span data-stu-id="4beed-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-181">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-181">Impacted audience</span></span>

<span data-ttu-id="4beed-182">在 CSP 中购买永久性软件或软件订阅产品/服务的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="4beed-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="4beed-183">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-183">Details</span></span>

<span data-ttu-id="4beed-184">请注意以下关于通过合作伙伴中心购买永久性软件和软件订阅的重要通知：</span><span class="sxs-lookup"><span data-stu-id="4beed-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="4beed-185">软件退货期政策</span><span class="sxs-lookup"><span data-stu-id="4beed-185">Software return period policy</span></span>

<span data-ttu-id="4beed-186">按照 Microsoft 合作伙伴协议 (MPA) 的规定，从 2021 年 6 月 1 日起，CSP 中的软件产品/服务的退货期将从下单日期后的 60 天更改下单日期后的 30 天。</span><span class="sxs-lookup"><span data-stu-id="4beed-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="4beed-187">在提交软件产品/服务的订单后，合作伙伴将有 30 天的时间来提交对该订单的任何修改：</span><span class="sxs-lookup"><span data-stu-id="4beed-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="4beed-188">任何在 30 天退货期内退回的永久性软件许可证将获得已付购买价格的全额退款。</span><span class="sxs-lookup"><span data-stu-id="4beed-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="4beed-189">任何在 30 天退货期内退回的软件订购产品将获得已付购买价格的相应比例的退款。</span><span class="sxs-lookup"><span data-stu-id="4beed-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="4beed-190">为了跟进我们在 2020 年 12 月和 2021 年 4 月向所有 CSP 合作伙伴发出的关于退货期和其他 MPA 更新的电子邮件，我们发布了此消息。</span><span class="sxs-lookup"><span data-stu-id="4beed-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="4beed-191">请参考这些通知，全面详细地了解有关影响 MPA 的更改。</span><span class="sxs-lookup"><span data-stu-id="4beed-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="4beed-192">软件下载链接有效期</span><span class="sxs-lookup"><span data-stu-id="4beed-192">Software download link expiry</span></span>

<span data-ttu-id="4beed-193">从 2021 年 6 月 3 日起，通过合作伙伴中心购买的永久性软件和软件订阅产品的软件下载链接将有一个有效期，从首次下载后的 5 天内有效。</span><span class="sxs-lookup"><span data-stu-id="4beed-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="4beed-194">在 2021 年 6 月 3 日之前购买，以及在 2021 年 6 月 3 日当天或以后购买均可适用此有效期。</span><span class="sxs-lookup"><span data-stu-id="4beed-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-195">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-195">Next steps</span></span>

<span data-ttu-id="4beed-196">查看 [CSP 退货期和下载链接有效期常见问题解答](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)，并向组织中的所有相应团队通知这些更改：</span><span class="sxs-lookup"><span data-stu-id="4beed-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-197">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-197">Questions?</span></span>

<span data-ttu-id="4beed-198">如果对这些产品/服务有疑问，请查看相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="4beed-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="4beed-199">开放许可计划：将经销商转换到云解决方案提供商 (CSP) 计划</span><span class="sxs-lookup"><span data-stu-id="4beed-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-200">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-200">Categories</span></span>

- <span data-ttu-id="4beed-201">日期：2021-04-19</span><span class="sxs-lookup"><span data-stu-id="4beed-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="4beed-202">发展你的业务</span><span class="sxs-lookup"><span data-stu-id="4beed-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-203">总结</span><span class="sxs-lookup"><span data-stu-id="4beed-203">Summary</span></span>

<span data-ttu-id="4beed-204">此通知详细说明了如何准备好应对开放许可计划即将出现的变更。</span><span class="sxs-lookup"><span data-stu-id="4beed-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-205">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-205">Impacted audience</span></span>

<span data-ttu-id="4beed-206">CSP 和开放许可合作伙伴</span><span class="sxs-lookup"><span data-stu-id="4beed-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="4beed-207">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-207">Details</span></span>

<span data-ttu-id="4beed-208">2020 年，Microsoft [宣布](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/)将通过云解决方案提供商 (CSP) 计划向合作伙伴和客户广泛提供永久性软件许可证。</span><span class="sxs-lookup"><span data-stu-id="4beed-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="4beed-209">第一个里程碑已在 2021 年 1 月达成，当时提供了商用永久性软件产品/服务。</span><span class="sxs-lookup"><span data-stu-id="4beed-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="4beed-210">下一个关键的里程碑将在 2021 年 7 月发生，当时将提供[公共部门](https://aka.ms/openlicensepublicsector)产品/服务。</span><span class="sxs-lookup"><span data-stu-id="4beed-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="4beed-211">我们还[宣布](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)自 2022 年 1 月 1 日起，不可通过开放许可计划针对软件保障或联机服务进行新的软件许可证购买或续订。</span><span class="sxs-lookup"><span data-stu-id="4beed-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="4beed-212">在新的商业体验中将永久性软件过渡到 CSP 计划将帮助合作伙伴拓展机遇来提供多种解决方案和托管服务。</span><span class="sxs-lookup"><span data-stu-id="4beed-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="4beed-213">这也将加速客户过渡到云端的速度。</span><span class="sxs-lookup"><span data-stu-id="4beed-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="4beed-214">为了帮助确保合作伙伴和客户顺利过渡，我们作出了这些调整和资料来加速这一数字转型：</span><span class="sxs-lookup"><span data-stu-id="4beed-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="4beed-215">2021 年 4 月</span><span class="sxs-lookup"><span data-stu-id="4beed-215">April 2021</span></span>

<span data-ttu-id="4beed-216">[现已推出](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)：面向经销商的“开放许可到 CSP 过渡”资料</span><span class="sxs-lookup"><span data-stu-id="4beed-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="4beed-217">2021 年 7 月</span><span class="sxs-lookup"><span data-stu-id="4beed-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="4beed-218">CSP</span><span class="sxs-lookup"><span data-stu-id="4beed-218">CSP</span></span>

- <span data-ttu-id="4beed-219">7 月 1 日：向公共部门客户提供永久性软件许可证</span><span class="sxs-lookup"><span data-stu-id="4beed-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="4beed-220">7 月 7 日：向所有细分领域提供 Visual Studio Pro 和 Get Genuine Windows Agreement 永久性软件许可证</span><span class="sxs-lookup"><span data-stu-id="4beed-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="4beed-221">开发价值</span><span class="sxs-lookup"><span data-stu-id="4beed-221">Open Value</span></span>

- <span data-ttu-id="4beed-222">7 月1 日：在开发价值计划中向教育领域和非营利领域提供额外的 SKU，从而向开放许可计划提供类似的产品/服务</span><span class="sxs-lookup"><span data-stu-id="4beed-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="4beed-223">开放许可</span><span class="sxs-lookup"><span data-stu-id="4beed-223">Open License</span></span>

- <span data-ttu-id="4beed-224">7 月 1 日：Microsoft 将不再在开放许可计划中发布新的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="4beed-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="4beed-225">2022 年 1 月</span><span class="sxs-lookup"><span data-stu-id="4beed-225">January 2022</span></span>

- <span data-ttu-id="4beed-226">1 月 1 日：不可通过开放许可计划进行新的购买或续订</span><span class="sxs-lookup"><span data-stu-id="4beed-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-227">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="4beed-228">CSP 间接提供商</span><span class="sxs-lookup"><span data-stu-id="4beed-228">CSP indirect providers</span></span>

<span data-ttu-id="4beed-229">在未来几个月中，参加合作伙伴社区活动并采用面向经销商的“开放许可到 CSP 过渡”资料，帮助开放许可经销商适应 CSP 计划：</span><span class="sxs-lookup"><span data-stu-id="4beed-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="4beed-230">[面向经销商的“开放许可到 CSP 过渡”资料](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/) - 可自定义的概述演示文稿、电子邮件模板、CSP 间接经销商培训指南等等，可帮助你推动经销商大规模采用。</span><span class="sxs-lookup"><span data-stu-id="4beed-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="4beed-231">由 Microsoft 业务运营部主持的 [CSP 合作伙伴社区活动](https://globalpbocomm.eventbuilder.com/GlobalCSP)。</span><span class="sxs-lookup"><span data-stu-id="4beed-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="4beed-232">加入各种研讨会来学习 CSP 基础（CSP 基本知识）或跟进最新动向，还可就 CSP 中的软件提问求解（问答研讨会）。</span><span class="sxs-lookup"><span data-stu-id="4beed-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="4beed-233">（即将推出）Microsoft 业务运营部主持的聚焦 CSP 间接经销商的培训研讨会。</span><span class="sxs-lookup"><span data-stu-id="4beed-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="4beed-234">开放许可经销商</span><span class="sxs-lookup"><span data-stu-id="4beed-234">Open License resellers</span></span>

- <span data-ttu-id="4beed-235">如果你的组织目前未注册加入 CSP 计划，请联系分销商了解如何开始操作。</span><span class="sxs-lookup"><span data-stu-id="4beed-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="4beed-236">请在[此处](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)与间接提供商联系。</span><span class="sxs-lookup"><span data-stu-id="4beed-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="4beed-237">如果你的组织已注册加入 CSP 计划，请在[此处](https://partner.microsoft.com/resources/collection/software-in-csp)详细了解永久性软件。</span><span class="sxs-lookup"><span data-stu-id="4beed-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-238">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-238">Questions?</span></span>

<span data-ttu-id="4beed-239">如果对这些产品/服务有进一步的问题，请访问相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="4beed-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="4beed-240">现已推出：全球促销就绪指南</span><span class="sxs-lookup"><span data-stu-id="4beed-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-241">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-241">Categories</span></span>

- <span data-ttu-id="4beed-242">日期：2021-04-16</span><span class="sxs-lookup"><span data-stu-id="4beed-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="4beed-243">功能</span><span class="sxs-lookup"><span data-stu-id="4beed-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-244">摘要</span><span class="sxs-lookup"><span data-stu-id="4beed-244">Summary</span></span>

<span data-ttu-id="4beed-245">发布准备部已针对运营就绪性资源库发布了新的[全球促销就绪指南](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)。</span><span class="sxs-lookup"><span data-stu-id="4beed-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="4beed-246">本指南综合显示了所有现行[全球促销](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)。</span><span class="sxs-lookup"><span data-stu-id="4beed-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-247">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-247">Impacted audience</span></span>

<span data-ttu-id="4beed-248">所有批量许可 (VL)、动态价目表 (DPL) 和云解决方案提供商 (CSP) 合作伙伴</span><span class="sxs-lookup"><span data-stu-id="4beed-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="4beed-249">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-249">Details</span></span>

<span data-ttu-id="4beed-250">Microsoft 合作伙伴和我们有同一个需求，那就是提供各项全球促销的综合视图并附上辅助详细信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="4beed-251">你希望此综合指南可帮助你运用促销，确信所有可用信息都将在一个集中便利的位置随时可供访问。</span><span class="sxs-lookup"><span data-stu-id="4beed-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="4beed-252">从 2021 年 4 月开始，Microsoft 将每月更新一次本指南，它将在运营就绪性资源库中的专用“全球促销就绪指南”集合中提供。</span><span class="sxs-lookup"><span data-stu-id="4beed-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="4beed-253">本指南的链接还将包含在下列集合中：</span><span class="sxs-lookup"><span data-stu-id="4beed-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="4beed-254">[发布日历集合](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)，它将集中显示即将发生的变更和发布。</span><span class="sxs-lookup"><span data-stu-id="4beed-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="4beed-255">[社区集合](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)它包含我们每月合作伙伴通话的辅助资料，重点突出即将发生的变更和及时的热门运营主题。</span><span class="sxs-lookup"><span data-stu-id="4beed-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="4beed-256">[合作伙伴新闻稿](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)，例如 CSP 每月更新</span><span class="sxs-lookup"><span data-stu-id="4beed-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="4beed-257">在每月提醒中，我们还将发布合作伙伴中心公告，其中包含全球促销就绪指南的每项新问题。</span><span class="sxs-lookup"><span data-stu-id="4beed-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-258">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-258">Next steps</span></span>

<span data-ttu-id="4beed-259">在每月初，你将在[运营就绪性资源库](https://partner.microsoft.com/resources)中找到最新的[全球促销就绪指南](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)。</span><span class="sxs-lookup"><span data-stu-id="4beed-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="4beed-260">请与组织中适当的联系人分享此信息，并通过每页底部的“此页面有帮助吗？”按钮告诉我们指南</span><span class="sxs-lookup"><span data-stu-id="4beed-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="4beed-261">在多大程度上有所帮助。</span><span class="sxs-lookup"><span data-stu-id="4beed-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="4beed-262">4 月云解决方案提供商 (CSP) 社区更新和提醒</span><span class="sxs-lookup"><span data-stu-id="4beed-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-263">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-263">Categories</span></span>

- <span data-ttu-id="4beed-264">日期：2021-04-16</span><span class="sxs-lookup"><span data-stu-id="4beed-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="4beed-265">社区 | 邀请和提醒</span><span class="sxs-lookup"><span data-stu-id="4beed-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-266">总结</span><span class="sxs-lookup"><span data-stu-id="4beed-266">Summary</span></span>

<span data-ttu-id="4beed-267">CSP 社区资源按需提供且每月更新，便于你保持知情且准备好应对 CSP 计划中的变更。</span><span class="sxs-lookup"><span data-stu-id="4beed-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-268">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-268">Impacted audience</span></span>

<span data-ttu-id="4beed-269">CSP 直接计费合作伙伴和间接提供商</span><span class="sxs-lookup"><span data-stu-id="4beed-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="4beed-270">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-270">Details</span></span>

<span data-ttu-id="4beed-271">在本月，资源将纳入下列重要主题：</span><span class="sxs-lookup"><span data-stu-id="4beed-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="4beed-272">关于 CSP 计划演进和开放许可计划变更的新信息</span><span class="sxs-lookup"><span data-stu-id="4beed-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="4beed-273">对某些区域的 CSP 客户加入要求的变更</span><span class="sxs-lookup"><span data-stu-id="4beed-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="4beed-274">对 CSP 计划中新的商务 PDF 发票使用新格式</span><span class="sxs-lookup"><span data-stu-id="4beed-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="4beed-275">在 [CSP 社区集合](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)中，你将找到：</span><span class="sxs-lookup"><span data-stu-id="4beed-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="4beed-276">可下载的 [CSP 每月更新新闻稿](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)，它在易于阅读的文档中汇总了最新的 CSP 公告、更新、活动和提醒。</span><span class="sxs-lookup"><span data-stu-id="4beed-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="4beed-277">[CSP 公告日历](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)，它就即将发生的会影响计划的变更提供时间线视图。</span><span class="sxs-lookup"><span data-stu-id="4beed-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="4beed-278">新的[产品发布日历](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)，你可在此查看即将进行的产品发布和套餐。</span><span class="sxs-lookup"><span data-stu-id="4beed-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="4beed-279">[CSP 发布更新资源](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/)，它包含关于关键运营变更的易用内容。</span><span class="sxs-lookup"><span data-stu-id="4beed-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="4beed-280">[新资讯和提醒](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf)，介绍人们感兴趣和询问的关键 CSP 主题。</span><span class="sxs-lookup"><span data-stu-id="4beed-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="4beed-281">CSP 社区通话问答</span><span class="sxs-lookup"><span data-stu-id="4beed-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="4beed-282">提供了社区通话问答来帮助你解答有关即将发生的变更的问题。</span><span class="sxs-lookup"><span data-stu-id="4beed-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="4beed-283">请立即注册参加 4 月、5 月和 6 月举行的 CSP 社区通话问答活动。</span><span class="sxs-lookup"><span data-stu-id="4beed-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="4beed-284">这些活动将聚焦于最新的发布、重要新资讯和提醒。</span><span class="sxs-lookup"><span data-stu-id="4beed-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="4beed-285">[在此处注册](https://globalpbocomm.eventbuilder.com/GlobalCSP)。</span><span class="sxs-lookup"><span data-stu-id="4beed-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-286">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-286">Next steps</span></span>

<span data-ttu-id="4beed-287">查看社区资源并注册参加社区通话问答活动。</span><span class="sxs-lookup"><span data-stu-id="4beed-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="4beed-288">为了确保你从社区通话问答活动中获得最大收益，请查看按需社区内容，并在通话前 48 小时内提交你的问题。</span><span class="sxs-lookup"><span data-stu-id="4beed-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-289">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-289">Questions?</span></span>

<span data-ttu-id="4beed-290">如有关于 CSP 计划变更的问题，最适合提问的地方就是每月的 CSP 社区通话问答活动。</span><span class="sxs-lookup"><span data-stu-id="4beed-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="4beed-291">在每月，请查看资料并提前提交问题，以便我们可在研讨会上聚焦对你来说最重要的主题。</span><span class="sxs-lookup"><span data-stu-id="4beed-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="4beed-292">有关详细信息，请联系[支持人员](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)。</span><span class="sxs-lookup"><span data-stu-id="4beed-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="4beed-293">最后提醒：于 2021 年 5 月 6 日弃用 GET 资格</span><span class="sxs-lookup"><span data-stu-id="4beed-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-294">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-294">Categories</span></span>

- <span data-ttu-id="4beed-295">日期：2021-05-04</span><span class="sxs-lookup"><span data-stu-id="4beed-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="4beed-296">功能</span><span class="sxs-lookup"><span data-stu-id="4beed-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-297">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-297">Impacted audience</span></span>

<span data-ttu-id="4beed-298">使用合作伙伴中心 API，通过云解决方案提供商计划销售学术、非盈利和政府社区云 (GCC) 产品/服务的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="4beed-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="4beed-299">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-299">Details</span></span>

<span data-ttu-id="4beed-300">本公告是对 [12 月发布的合作伙伴中心增强功能](./2020-december.md#1)的跟进。</span><span class="sxs-lookup"><span data-stu-id="4beed-300">This announcement is a follow-up to the Partner Center [enhancements released in December](./2020-december.md#1).</span></span> <span data-ttu-id="4beed-301">此版本部署了新的 GET 和 POST 资格 API，因此现有 GET 资格将于 2021 年 5 月 6 日停用。</span><span class="sxs-lookup"><span data-stu-id="4beed-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="4beed-302">届时，你需要已经过渡到使用新的 POST 合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="4beed-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="4beed-303">可使用新的 POST API 购买教育版产品/服务，同时将可使用新的 GET API 购买预获资格的非营利组织’和 GCC 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="4beed-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-304">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-304">Next steps</span></span>

- <span data-ttu-id="4beed-305">请更新到新的 API，以便及时成功转换。</span><span class="sxs-lookup"><span data-stu-id="4beed-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="4beed-306">请访问运营准备资源 - [合作伙伴中心教育客户验证过程增强](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)，查看新的合作伙伴中心 API 更改和指南。</span><span class="sxs-lookup"><span data-stu-id="4beed-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="4beed-307">请与经销商和组织中的相应团队分享此信息，帮助他们为这些更改做好准备。</span><span class="sxs-lookup"><span data-stu-id="4beed-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-308">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-308">Questions?</span></span>

<span data-ttu-id="4beed-309">若有与此通知相关的任何问题，请联系[合作伙伴中心支持部门](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)。</span><span class="sxs-lookup"><span data-stu-id="4beed-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="4beed-310">更改日志</span><span class="sxs-lookup"><span data-stu-id="4beed-310">Change log</span></span>

- <span data-ttu-id="4beed-311">2021 年 4 月 4 日：最后提醒即将弃用 GET 资格</span><span class="sxs-lookup"><span data-stu-id="4beed-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="4beed-312">2021 年 4 月 9 日：提醒即将弃用 GET 资格</span><span class="sxs-lookup"><span data-stu-id="4beed-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="4beed-313">二月：更新了停用 GET 和 PUT 资格的时间线</span><span class="sxs-lookup"><span data-stu-id="4beed-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="4beed-314">一月：提醒即将开始弃用 GET 和 PUT 资格</span><span class="sxs-lookup"><span data-stu-id="4beed-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="4beed-315">对 CSP 中新的商务 PDF 发票使用新格式</span><span class="sxs-lookup"><span data-stu-id="4beed-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-316">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-316">Categories</span></span>

- <span data-ttu-id="4beed-317">日期：2021-04-05</span><span class="sxs-lookup"><span data-stu-id="4beed-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="4beed-318">功能</span><span class="sxs-lookup"><span data-stu-id="4beed-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-319">摘要</span><span class="sxs-lookup"><span data-stu-id="4beed-319">Summary</span></span>

<span data-ttu-id="4beed-320">Microsoft 在云解决方案提供商 (CSP) 计划中为新的商务 PDF 发票引入一种新格式，以按产品详细信息而不是按 SKU 说明显示账单详细信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-321">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-321">Impacted audience</span></span>

<span data-ttu-id="4beed-322">通过 CSP 计划进行交易的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="4beed-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="4beed-323">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-323">Details</span></span>

<span data-ttu-id="4beed-324">Microsoft 将从 2021 年 5 月起在 CSP 计划中为新的商务 PDF 发票引入一种新格式，即按产品详细信息（而不是 SKU 说明）显示账单详细信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="4beed-325">通过此更新，我们将按产品类型聚合行项，同时在单独的行上显示每个产品。</span><span class="sxs-lookup"><span data-stu-id="4beed-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="4beed-326">合作伙伴请注意，此更改将在 5 月的发票中（计费周期为 2021 年 4 月 1 日到 2021 年 4 月 30 日）开始生效。</span><span class="sxs-lookup"><span data-stu-id="4beed-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="4beed-327">受影响的产品/服务包括 Microsoft Azure 预留实例、Azure 订阅（Azure 计划）和市场。</span><span class="sxs-lookup"><span data-stu-id="4beed-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="4beed-328">发票格式更新后提出的任何额度重计请求都会采用新格式。</span><span class="sxs-lookup"><span data-stu-id="4beed-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="4beed-329">合作伙伴权益</span><span class="sxs-lookup"><span data-stu-id="4beed-329">Partner benefits</span></span>

<span data-ttu-id="4beed-330">此更新在合作伙伴开票体验方面提供以下改进：</span><span class="sxs-lookup"><span data-stu-id="4beed-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="4beed-331">减小了发票大小，同时保留了关键数据</span><span class="sxs-lookup"><span data-stu-id="4beed-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="4beed-332">使格式与行业标准保持一致，以生成精简且便于用户使用的发票</span><span class="sxs-lookup"><span data-stu-id="4beed-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="4beed-333">以下元素不会受到影响：</span><span class="sxs-lookup"><span data-stu-id="4beed-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="4beed-334">发票 PDF 中的“账单摘要”页</span><span class="sxs-lookup"><span data-stu-id="4beed-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="4beed-335">现有开票 API</span><span class="sxs-lookup"><span data-stu-id="4beed-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="4beed-336">对帐文件（对帐文件可用于检索精细数据。）</span><span class="sxs-lookup"><span data-stu-id="4beed-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="4beed-337">基于使用量和许可证的费用发票</span><span class="sxs-lookup"><span data-stu-id="4beed-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-338">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-338">Next steps</span></span>

<span data-ttu-id="4beed-339">在 Microsoft 合作伙伴网站上的[运营准备资源库](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)中查看有关此主题的信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="4beed-340">有关计费和税务主题（包括计费资源、发票、CSP 计费和税务）的详细信息，请访问合作伙伴中心的[计费部分](../billing.md)。</span><span class="sxs-lookup"><span data-stu-id="4beed-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](../billing.md) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="4beed-341">对云解决方案提供商 (CSP) 客户加入要求的更改</span><span class="sxs-lookup"><span data-stu-id="4beed-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-342">Categories</span><span class="sxs-lookup"><span data-stu-id="4beed-342">Categories</span></span>

- <span data-ttu-id="4beed-343">日期：2021-04-02</span><span class="sxs-lookup"><span data-stu-id="4beed-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="4beed-344">产品/市场</span><span class="sxs-lookup"><span data-stu-id="4beed-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="4beed-345">摘要</span><span class="sxs-lookup"><span data-stu-id="4beed-345">Summary</span></span>

<span data-ttu-id="4beed-346">我们承诺帮助合作伙伴和客户在相互信任的基础上开展其业务，在此过程中，我们将请求其他客户信息，从 2021 年 3 月 25 日生效。</span><span class="sxs-lookup"><span data-stu-id="4beed-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-347">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-347">Impacted audience</span></span>

<span data-ttu-id="4beed-348">CSP 商直接计费合作伙伴和间接提供商，他们在下一节中列出的国家/地区具有新客户或现有客户</span><span class="sxs-lookup"><span data-stu-id="4beed-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="4beed-349">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-349">Details</span></span>

<span data-ttu-id="4beed-350">Microsoft 值得信赖。</span><span class="sxs-lookup"><span data-stu-id="4beed-350">Microsoft runs on trust.</span></span> <span data-ttu-id="4beed-351">我们致力于在 CSP 计划中为交易客户订阅提供合规、安全且可靠的客户验证方法。</span><span class="sxs-lookup"><span data-stu-id="4beed-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="4beed-352">在 2021 年 5 月 25 日，我们将引入合作伙伴中心 API 和用户界面 (UI) 增强功能，它们将影响同时满足以下两个条件的合作伙伴：</span><span class="sxs-lookup"><span data-stu-id="4beed-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="4beed-353">合作伙伴与 Microsoft 有直接计费关系（这意味着合作伙伴是直接计费合作伙伴或间接提供商）。</span><span class="sxs-lookup"><span data-stu-id="4beed-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="4beed-354">合作伙伴与以下国家/地区的新客户或现有客户开展业务：</span><span class="sxs-lookup"><span data-stu-id="4beed-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="4beed-355">泰国</span><span class="sxs-lookup"><span data-stu-id="4beed-355">Thailand</span></span>
    - <span data-ttu-id="4beed-356">越南</span><span class="sxs-lookup"><span data-stu-id="4beed-356">Vietnam</span></span>
    - <span data-ttu-id="4beed-357">土耳其</span><span class="sxs-lookup"><span data-stu-id="4beed-357">Turkey</span></span>
    - <span data-ttu-id="4beed-358">波兰</span><span class="sxs-lookup"><span data-stu-id="4beed-358">Poland</span></span>
    - <span data-ttu-id="4beed-359">南非</span><span class="sxs-lookup"><span data-stu-id="4beed-359">South Africa</span></span>
    - <span data-ttu-id="4beed-360">印度</span><span class="sxs-lookup"><span data-stu-id="4beed-360">India</span></span>
    - <span data-ttu-id="4beed-361">巴西</span><span class="sxs-lookup"><span data-stu-id="4beed-361">Brazil</span></span>
    - <span data-ttu-id="4beed-362">伊拉克</span><span class="sxs-lookup"><span data-stu-id="4beed-362">Iraq</span></span>
    - <span data-ttu-id="4beed-363">缅甸</span><span class="sxs-lookup"><span data-stu-id="4beed-363">Myanmar</span></span>
    - <span data-ttu-id="4beed-364">南苏丹</span><span class="sxs-lookup"><span data-stu-id="4beed-364">South Sudan</span></span>
    - <span data-ttu-id="4beed-365">沙特阿拉伯</span><span class="sxs-lookup"><span data-stu-id="4beed-365">Saudi Arabia</span></span>
    - <span data-ttu-id="4beed-366">阿拉伯联合酋长国</span><span class="sxs-lookup"><span data-stu-id="4beed-366">United Arab Emirates</span></span>
    - <span data-ttu-id="4beed-367">委内瑞拉</span><span class="sxs-lookup"><span data-stu-id="4beed-367">Venezuela</span></span>

<span data-ttu-id="4beed-368">满足条件的合作伙伴必须在其下一次更新或为客户创建订阅时提交该客户的公司注册 ID（也称为客户的组织 INN）和电话号码。</span><span class="sxs-lookup"><span data-stu-id="4beed-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="4beed-369">这些合作伙伴还可以为客户输入可选的中间名。</span><span class="sxs-lookup"><span data-stu-id="4beed-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="4beed-370">请注意，在添加公司注册 ID 时，应使用企业纳税人标识号，而不是客户的个人 ID。</span><span class="sxs-lookup"><span data-stu-id="4beed-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="4beed-371">与以下国家/地区的新客户和现有客户合作的合作伙伴已加入 2020 年 11 月的以前版本中。</span><span class="sxs-lookup"><span data-stu-id="4beed-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="4beed-372">亚美尼亚</span><span class="sxs-lookup"><span data-stu-id="4beed-372">Armenia</span></span>
- <span data-ttu-id="4beed-373">阿塞拜疆</span><span class="sxs-lookup"><span data-stu-id="4beed-373">Azerbaijan</span></span>
- <span data-ttu-id="4beed-374">白俄罗斯</span><span class="sxs-lookup"><span data-stu-id="4beed-374">Belarus</span></span>
- <span data-ttu-id="4beed-375">匈牙利</span><span class="sxs-lookup"><span data-stu-id="4beed-375">Hungary</span></span>
- <span data-ttu-id="4beed-376">哈萨克斯坦</span><span class="sxs-lookup"><span data-stu-id="4beed-376">Kazakhstan</span></span>
- <span data-ttu-id="4beed-377">吉尔吉斯斯坦</span><span class="sxs-lookup"><span data-stu-id="4beed-377">Kyrgyzstan</span></span>
- <span data-ttu-id="4beed-378">摩尔多瓦</span><span class="sxs-lookup"><span data-stu-id="4beed-378">Moldova</span></span>
- <span data-ttu-id="4beed-379">俄罗斯</span><span class="sxs-lookup"><span data-stu-id="4beed-379">Russia</span></span>
- <span data-ttu-id="4beed-380">塔吉克斯坦</span><span class="sxs-lookup"><span data-stu-id="4beed-380">Tajikistan</span></span>
- <span data-ttu-id="4beed-381">乌克兰</span><span class="sxs-lookup"><span data-stu-id="4beed-381">Ukraine</span></span>
- <span data-ttu-id="4beed-382">乌兹别克斯坦</span><span class="sxs-lookup"><span data-stu-id="4beed-382">Uzbekistan</span></span>

<span data-ttu-id="4beed-383">与世界上其他国家/地区的客户合作的合作伙伴可以在 2021 年 3 月底输入客户的公司注册 ID、电话号码和中间名（可选）详细信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-384">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-384">Next steps</span></span>

- <span data-ttu-id="4beed-385">有关更详细的指南，请查看专门的[合作伙伴集锦](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)中的技术文档和常见问题。</span><span class="sxs-lookup"><span data-stu-id="4beed-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="4beed-386">准备使用合作伙伴中心 API 和 Web 用户体验来整合更改。</span><span class="sxs-lookup"><span data-stu-id="4beed-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="4beed-387">API/SDK 将可用于测试。</span><span class="sxs-lookup"><span data-stu-id="4beed-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="4beed-388">请确保在加入新客户或修改现有客户详细信息时提交其他数据。</span><span class="sxs-lookup"><span data-stu-id="4beed-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="4beed-389">如果正在使用控制面板供应商 (CPV) 解决方案，请咨询 CPV。</span><span class="sxs-lookup"><span data-stu-id="4beed-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="4beed-390">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-390">Questions?</span></span>

<span data-ttu-id="4beed-391">如果你有任何与公司注册 ID（也称为 INN 或 TIN）相关的问题，请与你的税务顾问或当地税务局联系。</span><span class="sxs-lookup"><span data-stu-id="4beed-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="4beed-392">Microsoft 无法提供有关税务事宜的指导。</span><span class="sxs-lookup"><span data-stu-id="4beed-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="4beed-393">如果需要 Microsoft 运营方面的支持，请创建[服务请求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。</span><span class="sxs-lookup"><span data-stu-id="4beed-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="4beed-394">查看本月的产品发布以及产品/服务</span><span class="sxs-lookup"><span data-stu-id="4beed-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="4beed-395">类别</span><span class="sxs-lookup"><span data-stu-id="4beed-395">Categories</span></span>

- <span data-ttu-id="4beed-396">日期：2021-04-01</span><span class="sxs-lookup"><span data-stu-id="4beed-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="4beed-397">功能</span><span class="sxs-lookup"><span data-stu-id="4beed-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="4beed-398">摘要</span><span class="sxs-lookup"><span data-stu-id="4beed-398">Summary</span></span>

<span data-ttu-id="4beed-399">2021 年 4 月的产品发布日历现已发布。</span><span class="sxs-lookup"><span data-stu-id="4beed-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="4beed-400">影响受众</span><span class="sxs-lookup"><span data-stu-id="4beed-400">Impacted audience</span></span>

<span data-ttu-id="4beed-401">参与云解决方案提供商 (CSP) 计划的所有合作伙伴</span><span class="sxs-lookup"><span data-stu-id="4beed-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="4beed-402">详细信息</span><span class="sxs-lookup"><span data-stu-id="4beed-402">Details</span></span>

<span data-ttu-id="4beed-403">现已在运营准备资源库中提供 2021 年 4 月的[产品发布日历](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)。</span><span class="sxs-lookup"><span data-stu-id="4beed-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="4beed-404">在此处查看即将进行的产品发布和将推出的产品/服务。</span><span class="sxs-lookup"><span data-stu-id="4beed-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="4beed-405">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4beed-405">Next steps</span></span>

<span data-ttu-id="4beed-406">请查看[产品发布日历](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)，与组织中的相应利益干系人分享此信息。</span><span class="sxs-lookup"><span data-stu-id="4beed-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="4beed-407">是否有任何问题?</span><span class="sxs-lookup"><span data-stu-id="4beed-407">Questions?</span></span>

<span data-ttu-id="4beed-408">如果对这些产品/服务有任何进一步的问题，请访问相关的 Yammer 社区。</span><span class="sxs-lookup"><span data-stu-id="4beed-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>