---
title: 奖励的客户关联问题
description: 了解如何解决在使用声称的记录 (CPOR) 客户关联的合作伙伴时遇到的问题。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152165"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a><span data-ttu-id="eca4a-103"> (CPOR) 客户关联的声明合作伙伴的问题</span><span class="sxs-lookup"><span data-stu-id="eca4a-103">Issues with Claimed Partner of Record (CPOR) customer associations</span></span>

<span data-ttu-id="eca4a-104">**适当的角色**：计费管理员 |全局管理员 |奖励管理</span><span class="sxs-lookup"><span data-stu-id="eca4a-104">**Appropriate roles**: Billing admin | Global admin | Incentives admin</span></span>

<span data-ttu-id="eca4a-105">以下内容将帮助你解决在使用客户关联时可能出现的问题。</span><span class="sxs-lookup"><span data-stu-id="eca4a-105">The content below will help you solve issues that can come up when you work with customer associations.</span></span>

## <a name="domain-tenant-mismatch"></a><span data-ttu-id="eca4a-106">域-租户不匹配</span><span class="sxs-lookup"><span data-stu-id="eca4a-106">Domain-tenant mismatch</span></span>

<span data-ttu-id="eca4a-107">在请求的记录合作伙伴 (CPOR) 关联声明流中，系统将要求你提供客户租户 ID 和子域。</span><span class="sxs-lookup"><span data-stu-id="eca4a-107">In the Claimed Partner of Record (CPOR) association claim flow, you will be asked to provide the customer tenant ID and subdomain.</span></span> <span data-ttu-id="eca4a-108">如果收到指出不匹配的错误，请与客户联系以确保具有正确的详细信息。</span><span class="sxs-lookup"><span data-stu-id="eca4a-108">If you receive an error stating that they don’t match, contact your customer to ensure you have the correct details.</span></span>

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a><span data-ttu-id="eca4a-109">CPOR 关联声明流中的订阅错误</span><span class="sxs-lookup"><span data-stu-id="eca4a-109">Subscription errors in the CPOR association claim flow</span></span>

<span data-ttu-id="eca4a-110">在 CPOR 关联声明流中，系统可能会要求你通过 Business Applications (Dynamics 365) 为你试图声明的产品提供订阅。</span><span class="sxs-lookup"><span data-stu-id="eca4a-110">In the CPOR association claim flow, you may be asked to provide a subscription for a product that you're trying to claim via Business Applications (Dynamics 365).</span></span> <span data-ttu-id="eca4a-111">我们要求提供订阅，因为我们要动态检查产品和订阅是否属于所申请的租户。</span><span class="sxs-lookup"><span data-stu-id="eca4a-111">We ask for the subscription because we're dynamically checking that the product and subscription belong to the tenant being claimed for.</span></span> <span data-ttu-id="eca4a-112">我们还检查订阅是否处于活动/已宽限状态。</span><span class="sxs-lookup"><span data-stu-id="eca4a-112">We're also checking that the subscription is in active/in grace status.</span></span>

<span data-ttu-id="eca4a-113">如果收到错误，则可能是由于以下几个原因：</span><span class="sxs-lookup"><span data-stu-id="eca4a-113">If you receive the error, it could be for several reasons:</span></span>

- <span data-ttu-id="eca4a-114">客户的租户上不存在所选产品</span><span class="sxs-lookup"><span data-stu-id="eca4a-114">The product selected doesn’t exist on the customer’s tenant</span></span>
- <span data-ttu-id="eca4a-115">提供的订阅不适用于 Dynamics</span><span class="sxs-lookup"><span data-stu-id="eca4a-115">The subscription provided isn't for Dynamics</span></span>
- <span data-ttu-id="eca4a-116">提供的订阅适用于 CSP</span><span class="sxs-lookup"><span data-stu-id="eca4a-116">The subscription provided is for CSP</span></span>
- <span data-ttu-id="eca4a-117">客户尚未激活/预配该订阅的产品</span><span class="sxs-lookup"><span data-stu-id="eca4a-117">The customer hasn't yet activated/provisioned the products for that subscription</span></span>
- <span data-ttu-id="eca4a-118">已声明订阅</span><span class="sxs-lookup"><span data-stu-id="eca4a-118">The subscription has already been claimed</span></span>
- <span data-ttu-id="eca4a-119">提供的标识符不是订阅 ID</span><span class="sxs-lookup"><span data-stu-id="eca4a-119">The identifier provided isn't a subscription ID</span></span>

<span data-ttu-id="eca4a-120">如果对订阅准确性有疑问，请与客户合作，确保订阅正确并使用正确的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="eca4a-120">If you have a question about the accuracy of your subscription, work with your customer to ensure the subscription is correct and that you're using the correct tenant ID.</span></span>

<span data-ttu-id="eca4a-121">如果此路由尚未解决你的问题，请联系 [支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。</span><span class="sxs-lookup"><span data-stu-id="eca4a-121">If this route hasn't resolved your issue, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="when-subscriptions-will-be-available-to-claim"></a><span data-ttu-id="eca4a-122">订阅将可用于声明</span><span class="sxs-lookup"><span data-stu-id="eca4a-122">When subscriptions will be available to claim</span></span>

<span data-ttu-id="eca4a-123">在为订阅申报时，如果尚未预配订阅，你将会收到错误。</span><span class="sxs-lookup"><span data-stu-id="eca4a-123">When claiming for a subscription, you will receive an error if the subscription hasn't been provisioned yet.</span></span> <span data-ttu-id="eca4a-124">客户需要执行几个步骤，以便 CPOR 平台可以选择订阅并使其可供声明使用。</span><span class="sxs-lookup"><span data-stu-id="eca4a-124">There are several steps the customer needs to take for the subscription to become available for the CPOR platform to pick it up and make it available to claim.</span></span> <span data-ttu-id="eca4a-125">如果在尝试申请订阅时收到错误，请联系客户，确保已预配该订阅，并且所声明的订阅正确无误。</span><span class="sxs-lookup"><span data-stu-id="eca4a-125">If you're receiving an error when trying to claim a subscription, contact your customer to ensure that it has been provisioned and the subscription you're claiming is correct.</span></span> <span data-ttu-id="eca4a-126">如果已采取此路由，请联系 [支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。</span><span class="sxs-lookup"><span data-stu-id="eca4a-126">If you have taken this route already, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="which-activity-do-i-choose"></a><span data-ttu-id="eca4a-127">我选择哪种活动？</span><span class="sxs-lookup"><span data-stu-id="eca4a-127">Which activity do I choose?</span></span>

<span data-ttu-id="eca4a-128">CPOR 声明平台允许 CPOR 关联声明，这些声明Business Applications和Microsoft 365方面。</span><span class="sxs-lookup"><span data-stu-id="eca4a-128">The CPOR claiming platform allows for CPOR association claims related to Business Applications and Microsoft 365 solution areas.</span></span> <span data-ttu-id="eca4a-129">下面列出了适用于每个解决方案领域的活动。</span><span class="sxs-lookup"><span data-stu-id="eca4a-129">The activities that are applicable to each solution area are below.</span></span> <span data-ttu-id="eca4a-130">根据说明选择正确的活动，以避免将来必须回收。</span><span class="sxs-lookup"><span data-stu-id="eca4a-130">Select the correct activity based on the descriptions to avoid having to reclaim in the future.</span></span> <span data-ttu-id="eca4a-131">使用不正确的活动进行声明可能会导致错过资格和奖励收益。</span><span class="sxs-lookup"><span data-stu-id="eca4a-131">Claiming with an incorrect activity may result in missed eligibility and incentive earnings.</span></span>


| <span data-ttu-id="eca4a-132">解决方案领域</span><span class="sxs-lookup"><span data-stu-id="eca4a-132">Solution area</span></span> | <span data-ttu-id="eca4a-133">活动</span><span class="sxs-lookup"><span data-stu-id="eca4a-133">Activity</span></span> | <span data-ttu-id="eca4a-134">适用于</span><span class="sxs-lookup"><span data-stu-id="eca4a-134">Applicable for</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="eca4a-135">业务应用程序</span><span class="sxs-lookup"><span data-stu-id="eca4a-135">Business applications</span></span>      | <span data-ttu-id="eca4a-136">售前</span><span class="sxs-lookup"><span data-stu-id="eca4a-136">Presales</span></span>   | <span data-ttu-id="eca4a-137">选择是否影响他们购买符合条件的产品，并想要申请预售奖励。</span><span class="sxs-lookup"><span data-stu-id="eca4a-137">Select if you influenced their purchase of an eligible product, and want to apply for pre-sale incentives.</span></span> <span data-ttu-id="eca4a-138">只有在客户通过批量许可协议或 Web-Direct 购买这些产品时，此选项才适用。</span><span class="sxs-lookup"><span data-stu-id="eca4a-138">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    |  <span data-ttu-id="eca4a-139">使用情况</span><span class="sxs-lookup"><span data-stu-id="eca4a-139">Usage</span></span>  | <span data-ttu-id="eca4a-140">选择是否推动其采用和使用符合条件的工作负载，并想要申请使用奖励。</span><span class="sxs-lookup"><span data-stu-id="eca4a-140">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> <span data-ttu-id="eca4a-141">只有在客户通过批量许可协议或 Web-Direct 购买这些产品时，此选项才适用。</span><span class="sxs-lookup"><span data-stu-id="eca4a-141">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    | <span data-ttu-id="eca4a-142">收入关联</span><span class="sxs-lookup"><span data-stu-id="eca4a-142">Revenue association</span></span>   | <span data-ttu-id="eca4a-143">选择是否影响他们选择符合条件的产品作为业务影响因素。</span><span class="sxs-lookup"><span data-stu-id="eca4a-143">Select if you influenced their selection of an eligible product as a Business Influencer.</span></span> <span data-ttu-id="eca4a-144">此选项仅适用于收入关联，不用于奖励付款。</span><span class="sxs-lookup"><span data-stu-id="eca4a-144">This option is for revenue association only, not for incentive payments.</span></span> <span data-ttu-id="eca4a-145">只有在客户通过批量许可协议或 Web-Direct 购买这些产品时，此选项才适用。</span><span class="sxs-lookup"><span data-stu-id="eca4a-145">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span>   |
| <span data-ttu-id="eca4a-146">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="eca4a-146">Microsoft 365</span></span>   | <span data-ttu-id="eca4a-147">使用情况</span><span class="sxs-lookup"><span data-stu-id="eca4a-147">Usage</span></span>   | <span data-ttu-id="eca4a-148">选择是否推动其采用和使用符合条件的工作负载，并想要申请使用奖励。</span><span class="sxs-lookup"><span data-stu-id="eca4a-148">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> |

## <a name="which-mpn-do-i-choose"></a><span data-ttu-id="eca4a-149">我选择哪个 MPN？</span><span class="sxs-lookup"><span data-stu-id="eca4a-149">Which MPN do I choose?</span></span>

<span data-ttu-id="eca4a-150">在 CPOR 关联声明流中，将要求你选择一个公司 MPN，该 MPN 应关联到最终客户要申请的工作。</span><span class="sxs-lookup"><span data-stu-id="eca4a-150">In the CPOR association claim flow, you will be asked to choose a company MPN that should be associated to the work you're claiming for at the end customer.</span></span> <span data-ttu-id="eca4a-151">你的公司可能有许多 MPNs，其中一些可能在激励计划中注册，另一些则与合作伙伴类型（如 FRP FastTrack）相关联。</span><span class="sxs-lookup"><span data-stu-id="eca4a-151">Your company may have many MPNs, some of which may be enrolled in incentive programs, and others associated with a partner type such as FRP FastTrack.</span></span> <span data-ttu-id="eca4a-152">CPOR 关联声明流将确定哪些 MPNs 在激励计划中注册，但它不会告诉您它是否为特定的合作伙伴类型 MPN。</span><span class="sxs-lookup"><span data-stu-id="eca4a-152">The CPOR association claim flow will identify which MPNs are enrolled in an incentive program, but it will not tell you if it is a specific partner type MPN.</span></span> <span data-ttu-id="eca4a-153">选择正确的 MPN，以避免将来不得不回收，这一点很重要。</span><span class="sxs-lookup"><span data-stu-id="eca4a-153">It’s important to select the correct MPN, to avoid having to reclaim in the future.</span></span> <span data-ttu-id="eca4a-154">如果申报的 MPN 不正确，可能会导致缺少资格和激励收益。</span><span class="sxs-lookup"><span data-stu-id="eca4a-154">Claiming with an incorrect MPN may result in missed eligibility and incentive earnings.</span></span>

<span data-ttu-id="eca4a-155">如果你不知道要使用哪种 MPN，请联系你的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="eca4a-155">If you do not know which MPN to use, contact your global admin.</span></span>

<span data-ttu-id="eca4a-156">如果要使用的 MPN 未注册，可以在 " [激励概述" 选项卡](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) 中进行管理， (登录所需) 。</span><span class="sxs-lookup"><span data-stu-id="eca4a-156">If the MPN you're wanting to use isn't enrolled, you can manage that in the [Incentives overview tab](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (sign-in required).</span></span>

## <a name="choosing-a-product-vs-entering-a-subscription"></a><span data-ttu-id="eca4a-157">选择产品与输入订阅</span><span class="sxs-lookup"><span data-stu-id="eca4a-157">Choosing a product vs entering a subscription</span></span>

<span data-ttu-id="eca4a-158">当要求和批准 Dynamics 产品时，合作伙伴可以在 CPOR 关联声明自身中查看订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="eca4a-158">When a Dynamics product is claimed and approved, the partner can view the subscription ID in the CPOR association claim itself.</span></span> <span data-ttu-id="eca4a-159">当声明此订阅时，该订阅处于活动状态或处于宽限状态，但可能会有时间结束，并且需要在单独的 CPOR 关联声明中声明新的订阅。</span><span class="sxs-lookup"><span data-stu-id="eca4a-159">When this subscription is claimed, it is in active or in grace status, but there may be a time when the subscription ends, and the new subscriptions will need to be claimed in a separate CPOR association claim.</span></span>

## <a name="competing-claims"></a><span data-ttu-id="eca4a-160">竞争声明</span><span class="sxs-lookup"><span data-stu-id="eca4a-160">Competing claims</span></span>

<span data-ttu-id="eca4a-161">如果要为客户创建 CPOR 关联声明，并为已与另一个合作伙伴关联的产品 () ，则声明将通过仲裁：</span><span class="sxs-lookup"><span data-stu-id="eca4a-161">If you're creating a CPOR association claim for a customer and their product(s) that is already associated with another partner, your claim will go through arbitration:</span></span>

1. <span data-ttu-id="eca4a-162">创建新的客户关联后，Microsoft 将验证关联的详细信息以及提供的执行证明，以确保其准确性。</span><span class="sxs-lookup"><span data-stu-id="eca4a-162">After you create a new customer association, Microsoft will verify the details of the association and proof of execution provided to ensure its accuracy.</span></span>

2. <span data-ttu-id="eca4a-163">如果你和其他合作伙伴声称了相同的客户和产品/工作负荷，Microsoft 将查看每个合作伙伴的执行证明文档，以确定要批准的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="eca4a-163">If you and another partner claim the same customer and product/workload, Microsoft will review each partner's proof of execution documentation to determine which partner to approve.</span></span>

3. <span data-ttu-id="eca4a-164">可能会从两个伙伴请求其他信息，这可能会导致延迟处理您的关联请求。</span><span class="sxs-lookup"><span data-stu-id="eca4a-164">Additional information might be requested from both partners, which could cause delays in processing your association request.</span></span>

4. <span data-ttu-id="eca4a-165">你 _的 CPOR_ 关联声明仍将在五个工作日内查看，但其状态可能会持续很长一段时间。</span><span class="sxs-lookup"><span data-stu-id="eca4a-165">Your CPOR association claim will still be reviewed within five business days, although its status may stay as _Under Review_ for a longer period of time.</span></span> <span data-ttu-id="eca4a-166">当 Microsoft 与当前拥有产品/工作负载的合作伙伴合作时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="eca4a-166">This scenario can happen when Microsoft works with the partner currently owning the product/workload.</span></span> <span data-ttu-id="eca4a-167">如果出现这种情况，你将在声明的 "评论" 部分中收到通知。</span><span class="sxs-lookup"><span data-stu-id="eca4a-167">You will be notified within the comments section of your claim if that is the case.</span></span> 

>[!IMPORTANT]
><span data-ttu-id="eca4a-168">如果我们需要其他信息来验证你的 CPOR 关联执行证明 (PoE) ，我们将通过 CPOR 关联声明注释部分联系你。</span><span class="sxs-lookup"><span data-stu-id="eca4a-168">If we require additional information to verify your CPOR association proof of execution (PoE), we'll contact you via the CPOR association claim comments section.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eca4a-169">后续步骤</span><span class="sxs-lookup"><span data-stu-id="eca4a-169">Next steps</span></span>

- [<span data-ttu-id="eca4a-170">即刻体验奖励</span><span class="sxs-lookup"><span data-stu-id="eca4a-170">Getting started with incentives</span></span>](incentives-get-started-intro.md)
