---
title: 移动运营商计费 - Microsoft Store
description: 该Microsoft Store为支持此功能的移动运营商提供移动运营商计费作为付款方式。
ms.date: 04/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.topic: article
ms.author: hickeys
author: hickeys
keywords: windows 10, uwp, 移动运营商, 移动结算, 移动运营商结算
ms.localizationpriority: medium
ms.openlocfilehash: 70d1d05911c927832ae82a402b0c17be52e39cfa
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151536"
---
# <a name="mobile-operator-billing"></a><span data-ttu-id="2bad7-104">移动运营商结算</span><span class="sxs-lookup"><span data-stu-id="2bad7-104">Mobile operator billing</span></span>

<span data-ttu-id="2bad7-105">**相应的角色**：全局管理员</span><span class="sxs-lookup"><span data-stu-id="2bad7-105">**Appropriate roles**: Global admin</span></span>

> [!NOTE]
> <span data-ttu-id="2bad7-106">若要寻求付款方面的支持（包括配置付款帐户、付款丢失、暂停付款或其他任何方面），请单击[此处](https://developer.microsoft.com/windows/support)联系支持人员。</span><span class="sxs-lookup"><span data-stu-id="2bad7-106">If you're looking for support regarding payouts, including configuring payout accounts, missing payouts, putting payouts on hold, or anything else, contact support [here](https://developer.microsoft.com/windows/support).</span></span>

<span data-ttu-id="2bad7-107">该Microsoft Store为运行 Windows 10、运行 Windows 10 移动版 和 Xbox One 控制台的设备提供移动运营商计费。</span><span class="sxs-lookup"><span data-stu-id="2bad7-107">The Microsoft Store offers mobile operator billing as a payment method for devices running Windows 10, phones running Windows 10 Mobile, and Xbox One consoles.</span></span> <span data-ttu-id="2bad7-108">如果客户的移动运营商支持此功能，则客户可以添加移动运营商计费作为付款方式，并使用它通过其移动帐户进行应用商店购买。</span><span class="sxs-lookup"><span data-stu-id="2bad7-108">If a customer’s mobile operator supports this capability, the customer can add mobile operator billing as a payment method and use it to make Store purchases using their mobile account.</span></span>

> [!TIP]
> <span data-ttu-id="2bad7-109">如果客户的移动运营商提供移动运营商计费，但客户在设备上找不到此选项，请查看 [以下步骤](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f)。</span><span class="sxs-lookup"><span data-stu-id="2bad7-109">If a customer’s mobile operator offers mobile operator billing, but the customer can't find this option on their device, review these [steps](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f).</span></span>

<span data-ttu-id="2bad7-110">我们定期与移动运营商合作以扩展此付款方式的可用性。</span><span class="sxs-lookup"><span data-stu-id="2bad7-110">We are regularly working with mobile operators to expand the availability of this payment method.</span></span> <span data-ttu-id="2bad7-111">如果要建议下面未列出的移动运营商，请联系该移动运营商，并请求他们添加此付款方式。</span><span class="sxs-lookup"><span data-stu-id="2bad7-111">If you’d like to suggest a mobile operator that you don’t see listed below, contact that mobile operator and request that they add this payment method.</span></span>

## <a name="operators-that-support-mobile-operator-billing"></a><span data-ttu-id="2bad7-112">支持移动运营商计费的操作员</span><span class="sxs-lookup"><span data-stu-id="2bad7-112">Operators that support mobile operator billing</span></span>

<span data-ttu-id="2bad7-113">以下移动运营商目前支持移动运营商计费。</span><span class="sxs-lookup"><span data-stu-id="2bad7-113">The following mobile operators currently support mobile operator billing.</span></span>

| <span data-ttu-id="2bad7-114">国家/地区</span><span class="sxs-lookup"><span data-stu-id="2bad7-114">Country/region</span></span>       | <span data-ttu-id="2bad7-115">移动运营商</span><span class="sxs-lookup"><span data-stu-id="2bad7-115">Mobile operators</span></span>                                        |
|----------------------|---------------------------------------------------------|
| <span data-ttu-id="2bad7-116">澳大利亚</span><span class="sxs-lookup"><span data-stu-id="2bad7-116">Australia</span></span>            | <span data-ttu-id="2bad7-117">Optus</span><span class="sxs-lookup"><span data-stu-id="2bad7-117">Optus</span></span>                                                   |
| <span data-ttu-id="2bad7-118">奥地利</span><span class="sxs-lookup"><span data-stu-id="2bad7-118">Austria</span></span>              | <span data-ttu-id="2bad7-119">A1 Telekom、Telechison 3G 匈牙利、T-Mobile/tele.ring</span><span class="sxs-lookup"><span data-stu-id="2bad7-119">A1 Telekom, Hutchison 3G Austria, T-Mobile / tele.ring</span></span>  |
| <span data-ttu-id="2bad7-120">比利时</span><span class="sxs-lookup"><span data-stu-id="2bad7-120">Belgium</span></span>              | <span data-ttu-id="2bad7-121">Base、Proximus</span><span class="sxs-lookup"><span data-stu-id="2bad7-121">Base, Proximus</span></span>                                          |
| <span data-ttu-id="2bad7-122">加拿大</span><span class="sxs-lookup"><span data-stu-id="2bad7-122">Canada</span></span>               | <span data-ttu-id="2bad7-123">Telus</span><span class="sxs-lookup"><span data-stu-id="2bad7-123">Telus</span></span>                                                   |
| <span data-ttu-id="2bad7-124">捷克</span><span class="sxs-lookup"><span data-stu-id="2bad7-124">Czechia</span></span>              | <span data-ttu-id="2bad7-125">T-Mobile、Vodafone、O2</span><span class="sxs-lookup"><span data-stu-id="2bad7-125">T-Mobile, Vodafone, O2</span></span>                                  |
| <span data-ttu-id="2bad7-126">丹麦</span><span class="sxs-lookup"><span data-stu-id="2bad7-126">Denmark</span></span>              | <span data-ttu-id="2bad7-127">3、TDC / YouSee、Telenor、Telia</span><span class="sxs-lookup"><span data-stu-id="2bad7-127">3, TDC / YouSee, Telenor, Telia</span></span>                         |
| <span data-ttu-id="2bad7-128">芬兰</span><span class="sxs-lookup"><span data-stu-id="2bad7-128">Finland</span></span>              | <span data-ttu-id="2bad7-129">DNA、Elisa</span><span class="sxs-lookup"><span data-stu-id="2bad7-129">DNA, Elisa</span></span>                                              |
| <span data-ttu-id="2bad7-130">法国</span><span class="sxs-lookup"><span data-stu-id="2bad7-130">France</span></span>               | <span data-ttu-id="2bad7-131">橙色</span><span class="sxs-lookup"><span data-stu-id="2bad7-131">Orange</span></span>                                                  |
| <span data-ttu-id="2bad7-132">德国</span><span class="sxs-lookup"><span data-stu-id="2bad7-132">Germany</span></span>              | <span data-ttu-id="2bad7-133">O2、Telekom Deutschland、Vodafone</span><span class="sxs-lookup"><span data-stu-id="2bad7-133">O2, Telekom Deutschland, Vodafone</span></span>                       |
| <span data-ttu-id="2bad7-134">匈牙利</span><span class="sxs-lookup"><span data-stu-id="2bad7-134">Hungary</span></span>              | <span data-ttu-id="2bad7-135">Telenor</span><span class="sxs-lookup"><span data-stu-id="2bad7-135">Telenor</span></span>                                                 |
| <span data-ttu-id="2bad7-136">意大利</span><span class="sxs-lookup"><span data-stu-id="2bad7-136">Italy</span></span>                | <span data-ttu-id="2bad7-137">Tre、Wind、Vodafone</span><span class="sxs-lookup"><span data-stu-id="2bad7-137">Tre, Wind, Vodafone</span></span>                                     |
| <span data-ttu-id="2bad7-138">韩国</span><span class="sxs-lookup"><span data-stu-id="2bad7-138">Korea</span></span>                | <span data-ttu-id="2bad7-139">SK Telecom</span><span class="sxs-lookup"><span data-stu-id="2bad7-139">SK Telecom</span></span>                                              |
| <span data-ttu-id="2bad7-140">马来西亚</span><span class="sxs-lookup"><span data-stu-id="2bad7-140">Malaysia</span></span>             | <span data-ttu-id="2bad7-141">Digi</span><span class="sxs-lookup"><span data-stu-id="2bad7-141">Digi</span></span>                                                    |
| <span data-ttu-id="2bad7-142">荷兰</span><span class="sxs-lookup"><span data-stu-id="2bad7-142">Netherlands</span></span>          | <span data-ttu-id="2bad7-143">KPN/Telfort、Vodafone</span><span class="sxs-lookup"><span data-stu-id="2bad7-143">KPN / Telfort, Vodafone</span></span>                                 |
| <span data-ttu-id="2bad7-144">挪威</span><span class="sxs-lookup"><span data-stu-id="2bad7-144">Norway</span></span>               | <span data-ttu-id="2bad7-145">Telenor / Talkmore、 Telia / OneCall</span><span class="sxs-lookup"><span data-stu-id="2bad7-145">Telenor / Talkmore, Telia / OneCall</span></span>                     |
| <span data-ttu-id="2bad7-146">波兰</span><span class="sxs-lookup"><span data-stu-id="2bad7-146">Poland</span></span>               | <span data-ttu-id="2bad7-147">Orange、Play、T-Mobile</span><span class="sxs-lookup"><span data-stu-id="2bad7-147">Orange, Play, T-Mobile</span></span>                                  |
| <span data-ttu-id="2bad7-148">沙特阿拉伯</span><span class="sxs-lookup"><span data-stu-id="2bad7-148">Saudi Arabia</span></span>         | <span data-ttu-id="2bad7-149">Stc</span><span class="sxs-lookup"><span data-stu-id="2bad7-149">STC</span></span>                                                     |
| <span data-ttu-id="2bad7-150">新加坡</span><span class="sxs-lookup"><span data-stu-id="2bad7-150">Singapore</span></span>            | <span data-ttu-id="2bad7-151">M1 Limited、StarHub</span><span class="sxs-lookup"><span data-stu-id="2bad7-151">M1 Limited, StarHub</span></span>                                     |
| <span data-ttu-id="2bad7-152">斯洛伐克</span><span class="sxs-lookup"><span data-stu-id="2bad7-152">Slovakia</span></span>             | <span data-ttu-id="2bad7-153">Slovak Telekom</span><span class="sxs-lookup"><span data-stu-id="2bad7-153">Slovak Telekom</span></span>                                          |
| <span data-ttu-id="2bad7-154">南非</span><span class="sxs-lookup"><span data-stu-id="2bad7-154">South Africa</span></span>         | <span data-ttu-id="2bad7-155">Vodacom</span><span class="sxs-lookup"><span data-stu-id="2bad7-155">Vodacom</span></span>                                                 |
| <span data-ttu-id="2bad7-156">西班牙</span><span class="sxs-lookup"><span data-stu-id="2bad7-156">Spain</span></span>                | <span data-ttu-id="2bad7-157">橙色</span><span class="sxs-lookup"><span data-stu-id="2bad7-157">Orange</span></span>                                                  |
| <span data-ttu-id="2bad7-158">瑞典</span><span class="sxs-lookup"><span data-stu-id="2bad7-158">Sweden</span></span>               | <span data-ttu-id="2bad7-159">3、Telenor</span><span class="sxs-lookup"><span data-stu-id="2bad7-159">3, Telenor</span></span>                                              |
| <span data-ttu-id="2bad7-160">瑞士</span><span class="sxs-lookup"><span data-stu-id="2bad7-160">Switzerland</span></span>          | <span data-ttu-id="2bad7-161">中国、瑞士</span><span class="sxs-lookup"><span data-stu-id="2bad7-161">Sunrise, Swisscom</span></span>                                       |
| <span data-ttu-id="2bad7-162">台湾</span><span class="sxs-lookup"><span data-stu-id="2bad7-162">Taiwan</span></span>               | <span data-ttu-id="2bad7-163">FarEasTone</span><span class="sxs-lookup"><span data-stu-id="2bad7-163">FarEasTone</span></span>                                              |
| <span data-ttu-id="2bad7-164">土耳其</span><span class="sxs-lookup"><span data-stu-id="2bad7-164">Turkey</span></span>               | <span data-ttu-id="2bad7-165">Turkcell</span><span class="sxs-lookup"><span data-stu-id="2bad7-165">Turkcell</span></span>                                                |
| <span data-ttu-id="2bad7-166">阿拉伯联合酋长国</span><span class="sxs-lookup"><span data-stu-id="2bad7-166">United Arab Emirates</span></span> | <span data-ttu-id="2bad7-167">Etisalat</span><span class="sxs-lookup"><span data-stu-id="2bad7-167">Etisalat</span></span>                                                |
| <span data-ttu-id="2bad7-168">美国</span><span class="sxs-lookup"><span data-stu-id="2bad7-168">United States</span></span>        | <span data-ttu-id="2bad7-169">Sprint、Verizon</span><span class="sxs-lookup"><span data-stu-id="2bad7-169">Sprint, Verizon</span></span>                                         |
| <span data-ttu-id="2bad7-170">英国</span><span class="sxs-lookup"><span data-stu-id="2bad7-170">United Kingdom</span></span>       | <span data-ttu-id="2bad7-171">3 UK，EE，O2，Vodafone</span><span class="sxs-lookup"><span data-stu-id="2bad7-171">3 UK, EE, O2, Vodafone</span></span>                                 |
