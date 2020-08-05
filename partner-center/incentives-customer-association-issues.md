---
title: 客户关联问题
description: 了解如何解决在使用声称的记录 (CPOR) 客户关联的合作伙伴时遇到的问题。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: 69c0eb822ed8bf2ff09d7fc4a37e920dc123133a
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/04/2020
ms.locfileid: "87546008"
---
# <a name="customer-association-issues"></a><span data-ttu-id="d962a-103">客户关联问题</span><span class="sxs-lookup"><span data-stu-id="d962a-103">Customer association issues</span></span>

<span data-ttu-id="d962a-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="d962a-104">Applies to:</span></span>

- <span data-ttu-id="d962a-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="d962a-105">Partner Center</span></span>

<span data-ttu-id="d962a-106">以下内容将帮助你解决在使用客户关联时可能出现的问题。</span><span class="sxs-lookup"><span data-stu-id="d962a-106">The content below will help you solve issues that can come up when you work with customer associations.</span></span>

<span data-ttu-id="d962a-107">适当的角色：</span><span class="sxs-lookup"><span data-stu-id="d962a-107">Appropriate roles:</span></span>

- <span data-ttu-id="d962a-108">计费管理员</span><span class="sxs-lookup"><span data-stu-id="d962a-108">Billing admin</span></span>
- <span data-ttu-id="d962a-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d962a-109">Global admin</span></span>
- <span data-ttu-id="d962a-110">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="d962a-110">Incentives admin</span></span>

## <a name="domain-tenant-mismatch"></a><span data-ttu-id="d962a-111">域-租户不匹配</span><span class="sxs-lookup"><span data-stu-id="d962a-111">Domain-tenant mismatch</span></span>

<span data-ttu-id="d962a-112">在请求的记录合作伙伴 (CPOR) 关联声明流中，系统将要求你提供客户租户 ID 和子域。</span><span class="sxs-lookup"><span data-stu-id="d962a-112">In the Claimed Partner of Record (CPOR) association claim flow, you will be asked to provide the customer tenant ID and subdomain.</span></span> <span data-ttu-id="d962a-113">如果收到指出不匹配的错误，请与客户联系以确保具有正确的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d962a-113">If you receive an error stating that they don’t match, contact your customer to ensure you have the correct details.</span></span>

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a><span data-ttu-id="d962a-114">CPOR 关联声明流中的订阅错误</span><span class="sxs-lookup"><span data-stu-id="d962a-114">Subscription errors in the CPOR association claim flow</span></span>

<span data-ttu-id="d962a-115">在 CPOR 关联声明流中，系统可能会要求你通过 Business Applications (Dynamics 365) 为你试图声明的产品提供订阅。</span><span class="sxs-lookup"><span data-stu-id="d962a-115">In the CPOR association claim flow, you may be asked to provide a subscription for a product that you're trying to claim via Business Applications (Dynamics 365).</span></span> <span data-ttu-id="d962a-116">我们要求提供订阅，因为我们要动态检查产品和订阅是否属于所申请的租户。</span><span class="sxs-lookup"><span data-stu-id="d962a-116">We ask for the subscription because we're dynamically checking that the product and subscription belong to the tenant being claimed for.</span></span> <span data-ttu-id="d962a-117">我们还检查订阅是否处于活动/已宽限状态。</span><span class="sxs-lookup"><span data-stu-id="d962a-117">We're also checking that the subscription is in active/in grace status.</span></span>

<span data-ttu-id="d962a-118">如果收到错误，则可能是由于以下几个原因：</span><span class="sxs-lookup"><span data-stu-id="d962a-118">If you receive the error, it could be for several reasons:</span></span>

- <span data-ttu-id="d962a-119">客户的租户上不存在所选产品</span><span class="sxs-lookup"><span data-stu-id="d962a-119">The product selected doesn’t exist on the customer’s tenant</span></span>
- <span data-ttu-id="d962a-120">提供的订阅不适用于 Dynamics</span><span class="sxs-lookup"><span data-stu-id="d962a-120">The subscription provided isn't for Dynamics</span></span>
- <span data-ttu-id="d962a-121">提供的订阅适用于 CSP</span><span class="sxs-lookup"><span data-stu-id="d962a-121">The subscription provided is for CSP</span></span>
- <span data-ttu-id="d962a-122">客户尚未激活/预配该订阅的产品</span><span class="sxs-lookup"><span data-stu-id="d962a-122">The customer hasn't yet activated/provisioned the products for that subscription</span></span>
- <span data-ttu-id="d962a-123">已声明订阅</span><span class="sxs-lookup"><span data-stu-id="d962a-123">The subscription has already been claimed</span></span>
- <span data-ttu-id="d962a-124">提供的标识符不是订阅 ID</span><span class="sxs-lookup"><span data-stu-id="d962a-124">The identifier provided isn't a subscription ID</span></span>

<span data-ttu-id="d962a-125">如果对订阅准确性有疑问，请与客户合作，确保订阅正确并使用正确的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="d962a-125">If you have a question about the accuracy of your subscription, work with your customer to ensure the subscription is correct and that you're using the correct tenant ID.</span></span>

<span data-ttu-id="d962a-126">如果此路由尚未解决你的问题，请联系[支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。</span><span class="sxs-lookup"><span data-stu-id="d962a-126">If this route hasn't resolved your issue, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="when-subscriptions-will-be-available-to-claim"></a><span data-ttu-id="d962a-127">订阅将可用于声明</span><span class="sxs-lookup"><span data-stu-id="d962a-127">When subscriptions will be available to claim</span></span>

<span data-ttu-id="d962a-128">在为订阅申报时，如果尚未预配订阅，你将会收到错误。</span><span class="sxs-lookup"><span data-stu-id="d962a-128">When claiming for a subscription, you will receive an error if the subscription hasn't been provisioned yet.</span></span> <span data-ttu-id="d962a-129">客户需要执行几个步骤，以便 CPOR 平台可以选择订阅并使其可供声明使用。</span><span class="sxs-lookup"><span data-stu-id="d962a-129">There are several steps the customer needs to take for the subscription to become available for the CPOR platform to pick it up and make it available to claim.</span></span> <span data-ttu-id="d962a-130">如果你在尝试声明订阅时收到错误，请与你的客户联系，以确保它已预配，并且你所申报的订阅是正确的。</span><span class="sxs-lookup"><span data-stu-id="d962a-130">If you're receiving an error when trying to claim a subscription, contact your customer to ensure that it has been provisioned and the subscription you're claiming is correct.</span></span> <span data-ttu-id="d962a-131">如果已创建此路由，请联系[支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。</span><span class="sxs-lookup"><span data-stu-id="d962a-131">If you have taken this route already, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="which-activity-do-i-choose"></a><span data-ttu-id="d962a-132">我应选择哪种活动？</span><span class="sxs-lookup"><span data-stu-id="d962a-132">Which activity do I choose?</span></span>

<span data-ttu-id="d962a-133">CPOR 声明平台允许与 Business Applications 和 Microsoft 365 解决方案区域相关的 CPOR 关联声明。</span><span class="sxs-lookup"><span data-stu-id="d962a-133">The CPOR claiming platform allows for CPOR association claims related to Business Applications and Microsoft 365 solution areas.</span></span> <span data-ttu-id="d962a-134">下面是适用于每个解决方案区域的活动。</span><span class="sxs-lookup"><span data-stu-id="d962a-134">The activities that are applicable to each solution area are below.</span></span> <span data-ttu-id="d962a-135">根据说明选择正确的活动，以避免将来需要回收。</span><span class="sxs-lookup"><span data-stu-id="d962a-135">Select the correct activity based on the descriptions to avoid having to reclaim in the future.</span></span> <span data-ttu-id="d962a-136">如果申报的活动不正确，可能会导致缺少合格和激励收益。</span><span class="sxs-lookup"><span data-stu-id="d962a-136">Claiming with an incorrect activity may result in missed eligibility and incentive earnings.</span></span>


| <span data-ttu-id="d962a-137">解决方案领域</span><span class="sxs-lookup"><span data-stu-id="d962a-137">Solution area</span></span> | <span data-ttu-id="d962a-138">活动</span><span class="sxs-lookup"><span data-stu-id="d962a-138">Activity</span></span> | <span data-ttu-id="d962a-139">适用于</span><span class="sxs-lookup"><span data-stu-id="d962a-139">Applicable for</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="d962a-140">业务应用程序</span><span class="sxs-lookup"><span data-stu-id="d962a-140">Business applications</span></span>      | <span data-ttu-id="d962a-141">前</span><span class="sxs-lookup"><span data-stu-id="d962a-141">Presales</span></span>   | <span data-ttu-id="d962a-142">如果你影响其对符合条件的产品的购买，并想要申请售前奖励，请选择此项。</span><span class="sxs-lookup"><span data-stu-id="d962a-142">Select if you influenced their purchase of an eligible product, and want to apply for pre-sale incentives.</span></span> <span data-ttu-id="d962a-143">仅当客户通过批量许可协议或 Web 直接购买这些产品时，此选项才适用。</span><span class="sxs-lookup"><span data-stu-id="d962a-143">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    |  <span data-ttu-id="d962a-144">使用情况</span><span class="sxs-lookup"><span data-stu-id="d962a-144">Usage</span></span>  | <span data-ttu-id="d962a-145">如果你推动其采用和使用符合条件的工作负荷，并想要应用以实现使用奖励，请选择。</span><span class="sxs-lookup"><span data-stu-id="d962a-145">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> <span data-ttu-id="d962a-146">仅当客户通过批量许可协议或 Web 直接购买这些产品时，此选项才适用。</span><span class="sxs-lookup"><span data-stu-id="d962a-146">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    | <span data-ttu-id="d962a-147">收入关联</span><span class="sxs-lookup"><span data-stu-id="d962a-147">Revenue association</span></span>   | <span data-ttu-id="d962a-148">如果影响其对符合业务影响的产品，请选择此项。</span><span class="sxs-lookup"><span data-stu-id="d962a-148">Select if you influenced their selection of an eligible product as a Business Influencer.</span></span> <span data-ttu-id="d962a-149">此选项仅适用于收入协会，不适用于激励支付。</span><span class="sxs-lookup"><span data-stu-id="d962a-149">This option is for revenue association only, not for incentive payments.</span></span> <span data-ttu-id="d962a-150">仅当客户通过批量许可协议或 Web 直接购买这些产品时，此选项才适用。</span><span class="sxs-lookup"><span data-stu-id="d962a-150">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span>   |
| <span data-ttu-id="d962a-151">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d962a-151">Microsoft 365</span></span>   | <span data-ttu-id="d962a-152">使用情况</span><span class="sxs-lookup"><span data-stu-id="d962a-152">Usage</span></span>   | <span data-ttu-id="d962a-153">如果你推动其采用和使用符合条件的工作负荷，并想要应用以实现使用奖励，请选择。</span><span class="sxs-lookup"><span data-stu-id="d962a-153">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> |

## <a name="which-mpn-do-i-choose"></a><span data-ttu-id="d962a-154">我 MPN 选择哪一种？</span><span class="sxs-lookup"><span data-stu-id="d962a-154">Which MPN do I choose?</span></span>

<span data-ttu-id="d962a-155">在 CPOR 关联声明流中，系统将要求你选择一个公司 MPN，该公司应该与你在最终客户申报的工作相关联。</span><span class="sxs-lookup"><span data-stu-id="d962a-155">In the CPOR association claim flow, you will be asked to choose a company MPN that should be associated to the work you're claiming for at the end customer.</span></span> <span data-ttu-id="d962a-156">你的公司可能有许多 MPNs，其中一些可能在激励计划中注册，另一些则与合作伙伴类型（如 FRP FastTrack）相关联。</span><span class="sxs-lookup"><span data-stu-id="d962a-156">Your company may have many MPNs, some of which may be enrolled in incentive programs, and others associated with a partner type such as FRP FastTrack.</span></span> <span data-ttu-id="d962a-157">CPOR 关联声明流将确定哪些 MPNs 在激励计划中注册，但它不会告诉您它是否为特定的合作伙伴类型 MPN。</span><span class="sxs-lookup"><span data-stu-id="d962a-157">The CPOR association claim flow will identify which MPNs are enrolled in an incentive program, but it will not tell you if it is a specific partner type MPN.</span></span> <span data-ttu-id="d962a-158">选择正确的 MPN，以避免将来不得不回收，这一点很重要。</span><span class="sxs-lookup"><span data-stu-id="d962a-158">It’s important to select the correct MPN, to avoid having to reclaim in the future.</span></span> <span data-ttu-id="d962a-159">如果申报的 MPN 不正确，可能会导致缺少资格和激励收益。</span><span class="sxs-lookup"><span data-stu-id="d962a-159">Claiming with an incorrect MPN may result in missed eligibility and incentive earnings.</span></span>

<span data-ttu-id="d962a-160">如果你不知道要使用哪种 MPN，请联系你的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="d962a-160">If you do not know which MPN to use, contact your global admin.</span></span>

<span data-ttu-id="d962a-161">如果你想要使用的 MPN 未注册，你可以在[激励概述选项卡](https://partner.microsoft.com/dashboard/incentives/enrollment/summary)中对其进行管理。</span><span class="sxs-lookup"><span data-stu-id="d962a-161">If the MPN you're wanting to use isn't enrolled, you can manage that in the [Incentives overview tab](https://partner.microsoft.com/dashboard/incentives/enrollment/summary).</span></span>

## <a name="choosing-a-product-vs-entering-a-subscription"></a><span data-ttu-id="d962a-162">选择产品与输入订阅</span><span class="sxs-lookup"><span data-stu-id="d962a-162">Choosing a product vs entering a subscription</span></span>

<span data-ttu-id="d962a-163">当要求和批准 Dynamics 产品时，合作伙伴可以在 CPOR 关联声明自身中查看订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="d962a-163">When a Dynamics product is claimed and approved, the partner can view the subscription ID in the CPOR association claim itself.</span></span> <span data-ttu-id="d962a-164">当声明此订阅时，该订阅处于活动状态或处于宽限状态，但可能会有时间结束，并且需要在单独的 CPOR 关联声明中声明新的订阅。</span><span class="sxs-lookup"><span data-stu-id="d962a-164">When this subscription is claimed, it is in active or in grace status, but there may be a time when the subscription ends, and the new subscriptions will need to be claimed in a separate CPOR association claim.</span></span>

## <a name="competing-claims"></a><span data-ttu-id="d962a-165">竞争声明</span><span class="sxs-lookup"><span data-stu-id="d962a-165">Competing claims</span></span>

<span data-ttu-id="d962a-166">如果要为客户创建 CPOR 关联声明，并为已与另一个合作伙伴关联的产品 () ，则声明将通过仲裁：</span><span class="sxs-lookup"><span data-stu-id="d962a-166">If you're creating a CPOR association claim for a customer and their product(s) that is already associated with another partner, your claim will go through arbitration:</span></span>

1. <span data-ttu-id="d962a-167">创建新的客户关联后，Microsoft 将验证关联的详细信息以及提供的执行证明，以确保其准确性。</span><span class="sxs-lookup"><span data-stu-id="d962a-167">After you create a new customer association, Microsoft will verify the details of the association and proof of execution provided to ensure its accuracy.</span></span>

2. <span data-ttu-id="d962a-168">如果你和其他合作伙伴声称了相同的客户和产品/工作负荷，Microsoft 将查看每个合作伙伴的执行证明文档，以确定要批准的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="d962a-168">If you and another partner claim the same customer and product/workload, Microsoft will review each partner's proof of execution documentation to determine which partner to approve.</span></span>

3. <span data-ttu-id="d962a-169">可能会从两个伙伴请求其他信息，这可能会导致延迟处理您的关联请求。</span><span class="sxs-lookup"><span data-stu-id="d962a-169">Additional information might be requested from both partners, which could cause delays in processing your association request.</span></span>

4. <span data-ttu-id="d962a-170">你_的 CPOR_关联声明仍将在五个工作日内查看，但其状态可能会持续很长一段时间。</span><span class="sxs-lookup"><span data-stu-id="d962a-170">Your CPOR association claim will still be reviewed within five business days, although its status may stay as _Under Review_ for a longer period of time.</span></span> <span data-ttu-id="d962a-171">当 Microsoft 与当前拥有产品/工作负载的合作伙伴合作时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="d962a-171">This scenario can happen when Microsoft works with the partner currently owning the product/workload.</span></span> <span data-ttu-id="d962a-172">如果出现这种情况，你将在声明的 "评论" 部分中收到通知。</span><span class="sxs-lookup"><span data-stu-id="d962a-172">You will be notified within the comments section of your claim if that is the case.</span></span> 

>[!IMPORTANT]
><span data-ttu-id="d962a-173">如果我们需要其他信息来验证你的 CPOR 关联 PoE，我们将通过 CPOR 关联声明评论部分与你联系。</span><span class="sxs-lookup"><span data-stu-id="d962a-173">If we require additional information to verify your CPOR association PoE, we'll contact you via CPOR association claim comments section.</span></span>
