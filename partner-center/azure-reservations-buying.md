---
title: 代表客户购买 Microsoft Azure 预订 | 合作伙伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何代表你的客户在合作伙伴中心购买或购买 Azure 预订。
author: LauraBrenner
ms.author: labrenne
keywords: azure, 预订, 管理, 计费, 购买
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 1ed6e84a931c609fefb70dbc1081309b244d8e63
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722009"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a><span data-ttu-id="b286d-104">在合作伙伴中心代表客户购买 Microsoft Azure 预订</span><span class="sxs-lookup"><span data-stu-id="b286d-104">Buy Microsoft Azure reservations on behalf of your customers in Partner Center</span></span> 

<span data-ttu-id="b286d-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="b286d-105">**Applies to**</span></span>

- <span data-ttu-id="b286d-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="b286d-106">Partner Center</span></span>
- <span data-ttu-id="b286d-107">Microsoft Azure 门户</span><span class="sxs-lookup"><span data-stu-id="b286d-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="b286d-108">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b286d-108">Partners in CSP</span></span>

<span data-ttu-id="b286d-109">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="b286d-109">**Appropriate roles**</span></span>

- <span data-ttu-id="b286d-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="b286d-110">Admin agent</span></span>
- <span data-ttu-id="b286d-111">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b286d-111">Global admin</span></span>
- <span data-ttu-id="b286d-112">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="b286d-112">Helpdesk agent</span></span>
- <span data-ttu-id="b286d-113">销售代理</span><span class="sxs-lookup"><span data-stu-id="b286d-113">Sales agent</span></span>
- <span data-ttu-id="b286d-114">用户管理管理员</span><span class="sxs-lookup"><span data-stu-id="b286d-114">User management admin</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="b286d-115">开始之前</span><span class="sxs-lookup"><span data-stu-id="b286d-115">Before you begin</span></span>

<span data-ttu-id="b286d-116">请先查看下面的重要信息，再代表客户购买 Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="b286d-116">Review the important information below before you buy Azure reservations on behalf of your customers.</span></span>

- <span data-ttu-id="b286d-117">如果客户签署新的 Microsoft 客户协议，[确认客户接受 Microsoft 客户协议](confirm-customer-agreement.md)，则必须在 azure 计划下购买 azure 预订。</span><span class="sxs-lookup"><span data-stu-id="b286d-117">If and when your customer signs the new Microsoft Customer Agreement [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md), you must purchase Azure reservations under the Azure plan.</span></span> <span data-ttu-id="b286d-118">有关详细信息，请参阅[购买 Azure 计划](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="b286d-118">For more information, read [Purchase Azure Plan](purchase-azure-plan.md).</span></span>

- <span data-ttu-id="b286d-119">客户必须已经拥有有效的 Azure 订阅，然后你才能代表他们购买预订</span><span class="sxs-lookup"><span data-stu-id="b286d-119">Customers must already have an active Azure subscription before you can purchase reservations on their behalf</span></span>
  
- <span data-ttu-id="b286d-120">Azure 保留价格中不包括软件订阅费用，如 SQL 数据库或 SUSE Linux 软件</span><span class="sxs-lookup"><span data-stu-id="b286d-120">Software subscription costs such as SQL Database or SUSE Linux software are not included in Azure reservation prices</span></span>

- <span data-ttu-id="b286d-121">Microsoft 的商业定价不包括税款，除非你所在地为巴西。</span><span class="sxs-lookup"><span data-stu-id="b286d-121">Microsoft's commercial pricing to you does not include taxes, unless your location is Brazil.</span></span> <span data-ttu-id="b286d-122">如果你的所在地是巴西，你的商业价格将包含相应的税</span><span class="sxs-lookup"><span data-stu-id="b286d-122">If your location is Brazil, the commercial price to you includes the appropriate taxes</span></span>

- <span data-ttu-id="b286d-123">销售和支持人员代理需要显式访问 Azure 订阅，以便他们可以代表客户在 Azure 门户中购买或管理订阅，以及提出支持请求，包括进行兑换和退款</span><span class="sxs-lookup"><span data-stu-id="b286d-123">Sales and help desk agents need explicit access to the Azure subscription so they can buy or manage it in the Azure portal and file support requests, including for exchanges and refunds, on behalf of the customer</span></span>  

- <span data-ttu-id="b286d-124">如果你是一个间接提供商，并通过 Azure 门户购买 Azure 预订，则 "记录" （间接经销商）的合作伙伴将从你选择的 Azure CSP 订阅继承。</span><span class="sxs-lookup"><span data-stu-id="b286d-124">If you're an indirect provider and you buy Azure reservations through the Azure portal, the Partner on Record (indirect reseller) is inherited from the Azure CSP subscription you select.</span></span>

- <span data-ttu-id="b286d-125">无法在购买后更改 Azure 预订的记录合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="b286d-125">The Partner of Record for Azure reservations cannot be changed post-purchase.</span></span> <span data-ttu-id="b286d-126">你可以通过新记录合作伙伴取消现有预订并购买新预订。</span><span class="sxs-lookup"><span data-stu-id="b286d-126">You can cancel the existing reservation and purchase a new one with the new Partner on Record.</span></span>

- <span data-ttu-id="b286d-127">如果客户需要将 Azure 订阅从直接方式或 EA 转移至云解决方案提供商计划，预订不会转移。</span><span class="sxs-lookup"><span data-stu-id="b286d-127">If a customer wants to transfer an Azure subscription from Direct or EA to CSP, reservations do not get transferred.</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="b286d-128">Azure 预订不可用市场</span><span class="sxs-lookup"><span data-stu-id="b286d-128">Azure reservations unavailable markets</span></span>

>[!IMPORTANT] 
><span data-ttu-id="b286d-129">Azure 保留项在以下市场*中不可用*：</span><span class="sxs-lookup"><span data-stu-id="b286d-129">Azure reservations *are not* available in the following markets:</span></span>  
>  
> | <span data-ttu-id="b286d-130">不可用市场</span><span class="sxs-lookup"><span data-stu-id="b286d-130">Unavailable markets</span></span> | &nbsp; | &nbsp; |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="b286d-131">奥兰群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-131">Åland Islands</span></span>     | <span data-ttu-id="b286d-132">格陵兰</span><span class="sxs-lookup"><span data-stu-id="b286d-132">Greenland</span></span>     | <span data-ttu-id="b286d-133">巴布亚新几内亚</span><span class="sxs-lookup"><span data-stu-id="b286d-133">Papua New Guinea</span></span>     |
> | <span data-ttu-id="b286d-134">美属萨摩亚</span><span class="sxs-lookup"><span data-stu-id="b286d-134">American Samoa</span></span>     | <span data-ttu-id="b286d-135">格林纳达</span><span class="sxs-lookup"><span data-stu-id="b286d-135">Grenada</span></span>     | <span data-ttu-id="b286d-136">皮特凯恩群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-136">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="b286d-137">安道尔</span><span class="sxs-lookup"><span data-stu-id="b286d-137">Andorra</span></span>     | <span data-ttu-id="b286d-138">瓜德罗普岛</span><span class="sxs-lookup"><span data-stu-id="b286d-138">Guadeloupe</span></span>     | <span data-ttu-id="b286d-139">留尼汪</span><span class="sxs-lookup"><span data-stu-id="b286d-139">Reunion</span></span>     |
> | <span data-ttu-id="b286d-140">安圭拉岛</span><span class="sxs-lookup"><span data-stu-id="b286d-140">Anguilla</span></span>     | <span data-ttu-id="b286d-141">关岛</span><span class="sxs-lookup"><span data-stu-id="b286d-141">Guam</span></span>     | <span data-ttu-id="b286d-142">萨巴岛</span><span class="sxs-lookup"><span data-stu-id="b286d-142">Saba</span></span>   |
> | <span data-ttu-id="b286d-143">南极洲</span><span class="sxs-lookup"><span data-stu-id="b286d-143">Antarctica</span></span>     | <span data-ttu-id="b286d-144">格恩西岛</span><span class="sxs-lookup"><span data-stu-id="b286d-144">Guernsey</span></span>     | <span data-ttu-id="b286d-145">圣巴泰勒米岛</span><span class="sxs-lookup"><span data-stu-id="b286d-145">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="b286d-146">安提瓜和巴布达</span><span class="sxs-lookup"><span data-stu-id="b286d-146">Antigua and Barbuda</span></span>       | <span data-ttu-id="b286d-147">几内亚</span><span class="sxs-lookup"><span data-stu-id="b286d-147">Guinea</span></span>     | <span data-ttu-id="b286d-148">圣卢西亚</span><span class="sxs-lookup"><span data-stu-id="b286d-148">Saint Lucia</span></span>   |
> | <span data-ttu-id="b286d-149">阿鲁巴岛</span><span class="sxs-lookup"><span data-stu-id="b286d-149">Aruba</span></span>       | <span data-ttu-id="b286d-150">几内亚比绍</span><span class="sxs-lookup"><span data-stu-id="b286d-150">Guinea-Bissau</span></span>     | <span data-ttu-id="b286d-151">法属圣马丁</span><span class="sxs-lookup"><span data-stu-id="b286d-151">Saint Martin</span></span>   |
> | <span data-ttu-id="b286d-152">阿塞拜疆</span><span class="sxs-lookup"><span data-stu-id="b286d-152">Azerbaijan</span></span>       | <span data-ttu-id="b286d-153">圭亚那</span><span class="sxs-lookup"><span data-stu-id="b286d-153">Guyana</span></span>     | <span data-ttu-id="b286d-154">圣皮埃尔和密克隆岛</span><span class="sxs-lookup"><span data-stu-id="b286d-154">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="b286d-155">贝宁</span><span class="sxs-lookup"><span data-stu-id="b286d-155">Benin</span></span>     | <span data-ttu-id="b286d-156">海地</span><span class="sxs-lookup"><span data-stu-id="b286d-156">Haiti</span></span>       | <span data-ttu-id="b286d-157">圣文森特和格林纳丁斯</span><span class="sxs-lookup"><span data-stu-id="b286d-157">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="b286d-158">不丹</span><span class="sxs-lookup"><span data-stu-id="b286d-158">Bhutan</span></span>     | <span data-ttu-id="b286d-159">赫德岛和麦克唐纳群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-159">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="b286d-160">萨摩亚</span><span class="sxs-lookup"><span data-stu-id="b286d-160">Samoa</span></span>     |
> | <span data-ttu-id="b286d-161">博内尔岛</span><span class="sxs-lookup"><span data-stu-id="b286d-161">Bonaire</span></span>     | <span data-ttu-id="b286d-162">曼岛</span><span class="sxs-lookup"><span data-stu-id="b286d-162">Isle of Man</span></span>     | <span data-ttu-id="b286d-163">圣马力诺</span><span class="sxs-lookup"><span data-stu-id="b286d-163">San Marino</span></span>     |
> | <span data-ttu-id="b286d-164">布韦岛</span><span class="sxs-lookup"><span data-stu-id="b286d-164">Bouvet Island</span></span>     | <span data-ttu-id="b286d-165">扬马延</span><span class="sxs-lookup"><span data-stu-id="b286d-165">Jan Mayen</span></span>     | <span data-ttu-id="b286d-166">圣多美和普林西比</span><span class="sxs-lookup"><span data-stu-id="b286d-166">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="b286d-167">英属印度洋领地</span><span class="sxs-lookup"><span data-stu-id="b286d-167">British Indian Ocean Territory</span></span>       | <span data-ttu-id="b286d-168">泽西</span><span class="sxs-lookup"><span data-stu-id="b286d-168">Jersey</span></span>     | <span data-ttu-id="b286d-169">塞舌尔</span><span class="sxs-lookup"><span data-stu-id="b286d-169">Seychelles</span></span>   |
> | <span data-ttu-id="b286d-170">英属维尔京群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-170">British Virgin Islands</span></span>     | <span data-ttu-id="b286d-171">基里巴斯</span><span class="sxs-lookup"><span data-stu-id="b286d-171">Kiribati</span></span>       | <span data-ttu-id="b286d-172">塞拉利昂</span><span class="sxs-lookup"><span data-stu-id="b286d-172">Sierra Leone</span></span>   |
> | <span data-ttu-id="b286d-173">布基纳法索</span><span class="sxs-lookup"><span data-stu-id="b286d-173">Burkina Faso</span></span>     | <span data-ttu-id="b286d-174">科索沃</span><span class="sxs-lookup"><span data-stu-id="b286d-174">Kosovo</span></span>     | <span data-ttu-id="b286d-175">圣尤斯特歇斯</span><span class="sxs-lookup"><span data-stu-id="b286d-175">Sint Eustatius</span></span>     |
> | <span data-ttu-id="b286d-176">布隆迪</span><span class="sxs-lookup"><span data-stu-id="b286d-176">Burundi</span></span>     | <span data-ttu-id="b286d-177">老挝</span><span class="sxs-lookup"><span data-stu-id="b286d-177">Laos</span></span>     | <span data-ttu-id="b286d-178">荷属圣马丁</span><span class="sxs-lookup"><span data-stu-id="b286d-178">Sint Maarten</span></span>     |
> | <span data-ttu-id="b286d-179">柬埔寨</span><span class="sxs-lookup"><span data-stu-id="b286d-179">Cambodia</span></span>     | <span data-ttu-id="b286d-180">莱索托</span><span class="sxs-lookup"><span data-stu-id="b286d-180">Lesotho</span></span>     | <span data-ttu-id="b286d-181">所罗门群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-181">Solomon Islands</span></span>     |
> | <span data-ttu-id="b286d-182">中非共和国</span><span class="sxs-lookup"><span data-stu-id="b286d-182">Central African Republic</span></span>     | <span data-ttu-id="b286d-183">利比里亚</span><span class="sxs-lookup"><span data-stu-id="b286d-183">Liberia</span></span>     | <span data-ttu-id="b286d-184">索马里</span><span class="sxs-lookup"><span data-stu-id="b286d-184">Somalia</span></span>     |
> | <span data-ttu-id="b286d-185">乍得</span><span class="sxs-lookup"><span data-stu-id="b286d-185">Chad</span></span>     | <span data-ttu-id="b286d-186">马达加斯加</span><span class="sxs-lookup"><span data-stu-id="b286d-186">Madagascar</span></span>     | <span data-ttu-id="b286d-187">南乔治亚和南桑威奇群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-187">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="b286d-188">中国</span><span class="sxs-lookup"><span data-stu-id="b286d-188">China</span></span>     | <span data-ttu-id="b286d-189">马拉维</span><span class="sxs-lookup"><span data-stu-id="b286d-189">Malawi</span></span>     | <span data-ttu-id="b286d-190">南苏丹</span><span class="sxs-lookup"><span data-stu-id="b286d-190">South Sudan</span></span>     |
> | <span data-ttu-id="b286d-191">圣延岛</span><span class="sxs-lookup"><span data-stu-id="b286d-191">Christmas Island</span></span>     | <span data-ttu-id="b286d-192">马尔代夫</span><span class="sxs-lookup"><span data-stu-id="b286d-192">Maldives</span></span>     | <span data-ttu-id="b286d-193">圣赫勒拿、阿森松与特里斯坦达库尼亚</span><span class="sxs-lookup"><span data-stu-id="b286d-193">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="b286d-194">科科斯（基林）群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-194">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="b286d-195">马里</span><span class="sxs-lookup"><span data-stu-id="b286d-195">Mali</span></span>     | <span data-ttu-id="b286d-196">苏里南</span><span class="sxs-lookup"><span data-stu-id="b286d-196">Suriname</span></span>     |
> | <span data-ttu-id="b286d-197">科摩罗</span><span class="sxs-lookup"><span data-stu-id="b286d-197">Comoros</span></span>     | <span data-ttu-id="b286d-198">马绍尔群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-198">Marshall Islands</span></span>     | <span data-ttu-id="b286d-199">群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-199">Svalbard</span></span>     |
> | <span data-ttu-id="b286d-200">刚果（布）</span><span class="sxs-lookup"><span data-stu-id="b286d-200">Congo</span></span>     | <span data-ttu-id="b286d-201">马提尼克</span><span class="sxs-lookup"><span data-stu-id="b286d-201">Martinique</span></span>     | <span data-ttu-id="b286d-202">斯威士兰</span><span class="sxs-lookup"><span data-stu-id="b286d-202">Swaziland</span></span>     |
> | <span data-ttu-id="b286d-203">刚果（民主共和国）</span><span class="sxs-lookup"><span data-stu-id="b286d-203">Congo (DRC)</span></span>     | <span data-ttu-id="b286d-204">毛里塔尼亚</span><span class="sxs-lookup"><span data-stu-id="b286d-204">Mauritania</span></span>     | <span data-ttu-id="b286d-205">东帝汶</span><span class="sxs-lookup"><span data-stu-id="b286d-205">Timor-Leste</span></span>   |
> | <span data-ttu-id="b286d-206">库克群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-206">Cook Islands</span></span>     | <span data-ttu-id="b286d-207">马约特</span><span class="sxs-lookup"><span data-stu-id="b286d-207">Mayotte</span></span>     | <span data-ttu-id="b286d-208">多哥</span><span class="sxs-lookup"><span data-stu-id="b286d-208">Togo</span></span>   |
> | <span data-ttu-id="b286d-209">吉布提</span><span class="sxs-lookup"><span data-stu-id="b286d-209">Djibouti</span></span>     | <span data-ttu-id="b286d-210">密克罗尼西亚</span><span class="sxs-lookup"><span data-stu-id="b286d-210">Micronesia</span></span>     | <span data-ttu-id="b286d-211">托克劳</span><span class="sxs-lookup"><span data-stu-id="b286d-211">Tokelau</span></span>   |
> | <span data-ttu-id="b286d-212">多米尼克</span><span class="sxs-lookup"><span data-stu-id="b286d-212">Dominica</span></span>     | <span data-ttu-id="b286d-213">蒙特塞拉特</span><span class="sxs-lookup"><span data-stu-id="b286d-213">Montserrat</span></span>     | <span data-ttu-id="b286d-214">汤加</span><span class="sxs-lookup"><span data-stu-id="b286d-214">Tonga</span></span>   |
> | <span data-ttu-id="b286d-215">赤道几内亚</span><span class="sxs-lookup"><span data-stu-id="b286d-215">Equatorial Guinea</span></span>     | <span data-ttu-id="b286d-216">莫桑比克</span><span class="sxs-lookup"><span data-stu-id="b286d-216">Mozambique</span></span>     | <span data-ttu-id="b286d-217">特克斯和凯科斯群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-217">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="b286d-218">厄立特里亚国</span><span class="sxs-lookup"><span data-stu-id="b286d-218">Eritrea</span></span>     | <span data-ttu-id="b286d-219">缅甸语</span><span class="sxs-lookup"><span data-stu-id="b286d-219">Myanmar</span></span>     | <span data-ttu-id="b286d-220">图瓦卢</span><span class="sxs-lookup"><span data-stu-id="b286d-220">Tuvalu</span></span>   |
> | <span data-ttu-id="b286d-221">福克兰群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-221">Falkland Islands</span></span>     | <span data-ttu-id="b286d-222">瑙鲁</span><span class="sxs-lookup"><span data-stu-id="b286d-222">Nauru</span></span>     | <span data-ttu-id="b286d-223">美属外岛</span><span class="sxs-lookup"><span data-stu-id="b286d-223">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="b286d-224">法属圭亚那</span><span class="sxs-lookup"><span data-stu-id="b286d-224">French Guiana</span></span>     | <span data-ttu-id="b286d-225">新喀里多尼亚</span><span class="sxs-lookup"><span data-stu-id="b286d-225">New Caledonia</span></span>     | <span data-ttu-id="b286d-226">瓦努阿图</span><span class="sxs-lookup"><span data-stu-id="b286d-226">Vanuatu</span></span>   |
> | <span data-ttu-id="b286d-227">法属玻里尼西亚</span><span class="sxs-lookup"><span data-stu-id="b286d-227">French Polynesia</span></span>     | <span data-ttu-id="b286d-228">尼日尔</span><span class="sxs-lookup"><span data-stu-id="b286d-228">Niger</span></span>     | <span data-ttu-id="b286d-229">梵蒂冈</span><span class="sxs-lookup"><span data-stu-id="b286d-229">Vatican City</span></span>   |
> | <span data-ttu-id="b286d-230">法属南部领地</span><span class="sxs-lookup"><span data-stu-id="b286d-230">French Southern Territories</span></span>     | <span data-ttu-id="b286d-231">纽埃</span><span class="sxs-lookup"><span data-stu-id="b286d-231">Niue</span></span>     | <span data-ttu-id="b286d-232">瓦利斯和富图纳</span><span class="sxs-lookup"><span data-stu-id="b286d-232">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="b286d-233">加蓬</span><span class="sxs-lookup"><span data-stu-id="b286d-233">Gabon</span></span>     | <span data-ttu-id="b286d-234">诺福克岛</span><span class="sxs-lookup"><span data-stu-id="b286d-234">Norfolk Island</span></span>     | <span data-ttu-id="b286d-235">也门</span><span class="sxs-lookup"><span data-stu-id="b286d-235">Yemen</span></span>   |
> | <span data-ttu-id="b286d-236">冈比亚</span><span class="sxs-lookup"><span data-stu-id="b286d-236">Gambia</span></span>     | <span data-ttu-id="b286d-237">北马里亚纳群岛</span><span class="sxs-lookup"><span data-stu-id="b286d-237">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="b286d-238">直布罗陀</span><span class="sxs-lookup"><span data-stu-id="b286d-238">Gibraltar</span></span>     | <span data-ttu-id="b286d-239">帕劳</span><span class="sxs-lookup"><span data-stu-id="b286d-239">Palau</span></span>       |    |

## <a name="purchase-azure-reservations"></a><span data-ttu-id="b286d-240">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="b286d-240">Purchase Azure reservations</span></span>

<span data-ttu-id="b286d-241">按照以下步骤在合作伙伴中心购买 Microsoft Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="b286d-241">Follow the steps below to buy Microsoft Azure reservations on behalf of your customers in Partner Center.</span></span>

1. <span data-ttu-id="b286d-242">从 "合作伙伴中心" 菜单中选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="b286d-242">Select **Customers** from the Partner Center menu.</span></span>  

2. <span data-ttu-id="b286d-243">在 "**客户**" 页上，找到想要购买 Azure 预订的客户，然后选择向下箭头以展开客户的行。</span><span class="sxs-lookup"><span data-stu-id="b286d-243">On your **Customers** page, find the customer who wants to purchase Azure reservations and then select the down arrow to expand the customer's row.</span></span>  

3. <span data-ttu-id="b286d-244">依次选择“添加产品”、“Azure”。</span><span class="sxs-lookup"><span data-stu-id="b286d-244">Select **Add products** and then select **Azure**.</span></span> 

    <span data-ttu-id="b286d-245">a.</span><span class="sxs-lookup"><span data-stu-id="b286d-245">a.</span></span> <span data-ttu-id="b286d-246">从“细分市场”列表中选择该客户的细分市场。</span><span class="sxs-lookup"><span data-stu-id="b286d-246">Choose the customer's market segment from the **Segment** list.</span></span>

    <span data-ttu-id="b286d-247">b.</span><span class="sxs-lookup"><span data-stu-id="b286d-247">b.</span></span> <span data-ttu-id="b286d-248">从 "产品**类型**" 列表中选择 "**保留**"。</span><span class="sxs-lookup"><span data-stu-id="b286d-248">Choose **Reservations** from the product **Type** list.</span></span>

    <span data-ttu-id="b286d-249">c.</span><span class="sxs-lookup"><span data-stu-id="b286d-249">c.</span></span> <span data-ttu-id="b286d-250">从“预留项类型”列表中选择客户所需的预留项类型。</span><span class="sxs-lookup"><span data-stu-id="b286d-250">Choose the type of reservation the customer wants from the **Reservations type** list.</span></span>

4. <span data-ttu-id="b286d-251">Azure 预订必须与有效的 Azure 订阅相关联。</span><span class="sxs-lookup"><span data-stu-id="b286d-251">Azure reservations must be associated with an active Azure subscription.</span></span> <span data-ttu-id="b286d-252">从 "**客户订阅**" 列表中选择要向其添加 Azure 预订的客户的订阅。</span><span class="sxs-lookup"><span data-stu-id="b286d-252">Choose the customer's subscription you want to add Azure reservations to from the **Customer subscription** list.</span></span> 

   >[!IMPORTANT]
   ><span data-ttu-id="b286d-253">如果客户还没有有效的 Azure 订阅，请选择 " **azure** " 立即添加一个。</span><span class="sxs-lookup"><span data-stu-id="b286d-253">If the customer doesn't already have an active Azure subscription, select **Azure** to add one now.</span></span> 

5. <span data-ttu-id="b286d-254">使用筛选器查找满足客户要求的虚拟机上的 Azure 保留项。</span><span class="sxs-lookup"><span data-stu-id="b286d-254">Use the filters to find Azure reservations on virtual machines that meet your customer's requirements.</span></span>  

6. <span data-ttu-id="b286d-255">找到要购买的预订后，输入客户将在 "**数量**" 中所需的保留实例数，然后选择 "**添加到购物车**"。</span><span class="sxs-lookup"><span data-stu-id="b286d-255">After you find the reservation(s) you want to buy, enter the number of reserved instances the customer will need in **Quantity** and then select **Add to cart**.</span></span>  

7. <span data-ttu-id="b286d-256">重复步骤5和步骤6，直到将所有必需的项添加到订单中。</span><span class="sxs-lookup"><span data-stu-id="b286d-256">Repeat steps 5 and 6 until you've added all the necessary items to the order.</span></span> <span data-ttu-id="b286d-257">选择“查看”以确认订单是否正确无误。</span><span class="sxs-lookup"><span data-stu-id="b286d-257">Select **Review** to verify that your order is correct.</span></span>  

8. <span data-ttu-id="b286d-258">在**查看订单**页面上，可以：</span><span class="sxs-lookup"><span data-stu-id="b286d-258">On the **Review your orders** page, you can:</span></span> 

    - <span data-ttu-id="b286d-259">验证或更改预留实例数量。</span><span class="sxs-lookup"><span data-stu-id="b286d-259">Verify or change the reserved instances quantity.</span></span>

    - <span data-ttu-id="b286d-260">选择预订的作用域。</span><span class="sxs-lookup"><span data-stu-id="b286d-260">Select the reservation's scope.</span></span> <span data-ttu-id="b286d-261">预订的范围可以包含一个订阅或多个订阅（共享范围）。</span><span class="sxs-lookup"><span data-stu-id="b286d-261">The reservation's scope can cover one subscription or multiple subscriptions (shared scope).</span></span> <span data-ttu-id="b286d-262">如果将预留范围限定于单个订阅，则预订折扣仅应用于此订阅。</span><span class="sxs-lookup"><span data-stu-id="b286d-262">If you scope the reservation to a single subscription, the reservation discount is applied to this subscription only.</span></span> <span data-ttu-id="b286d-263">如果选择 "共享"，则预订折扣将应用到客户的计费上下文内的任何订阅。</span><span class="sxs-lookup"><span data-stu-id="b286d-263">If you select shared, the reservation discount is applied to any subscriptions within the customer's billing context.</span></span> 

      >[!NOTE] 
      ><span data-ttu-id="b286d-264">如果选择将预订的范围限制为单个 Azure 订阅，可能需要增加订阅的 vCPU 配额。</span><span class="sxs-lookup"><span data-stu-id="b286d-264">If you opt to limit the reservation's scope to a single Azure subscription, you may need to increase the subscription's vCPU quota.</span></span> <span data-ttu-id="b286d-265">若要增加订阅的 vCPU 配额，需要在 Azure 门户中创建支持请求。</span><span class="sxs-lookup"><span data-stu-id="b286d-265">To increase the subscription's vCPU quota, you'll need to create a support request in the Azure portal.</span></span> <span data-ttu-id="b286d-266">按照[本主题中](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request)的说明创建请求。</span><span class="sxs-lookup"><span data-stu-id="b286d-266">Follow the instructions [in this topic](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request) to create the request.</span></span> 

      >[!NOTE]   
      ><span data-ttu-id="b286d-267">如果客户位于 Azure 计划下，则**范围**将设置为 "**共享**"。</span><span class="sxs-lookup"><span data-stu-id="b286d-267">If your customer is under the Azure plan, **Scope**  will be set to **Shared**.</span></span> 

    - <span data-ttu-id="b286d-268">如果是提供商合作伙伴，请选择要与产品关联的经销商。</span><span class="sxs-lookup"><span data-stu-id="b286d-268">If you're a provider partner, select the reseller you want to associate with the product.</span></span>
    
    - <span data-ttu-id="b286d-269">如果 Azure 保留项支持计费计划选项，则可以从下拉菜单中选择 "按月计费频率"。</span><span class="sxs-lookup"><span data-stu-id="b286d-269">If your Azure reservation supports the Billing plan option, you can select the billing frequency as monthly from the dropdown menu.</span></span> 
    - <span data-ttu-id="b286d-270">如果你的 Azure 保留不支持计费计划选项，则计费频率默认为一次性计费。</span><span class="sxs-lookup"><span data-stu-id="b286d-270">If your Azure reservation does not support the Billing plan option, your billing frequency defaults to one time billing.</span></span> 

9. <span data-ttu-id="b286d-271">选择**确认购买**以购买订购的商品。</span><span class="sxs-lookup"><span data-stu-id="b286d-271">Select **Buy** to purchase the order.</span></span> <span data-ttu-id="b286d-272">订单的详细信息（包括订单号）将显示在 "**确认**" 页上。</span><span class="sxs-lookup"><span data-stu-id="b286d-272">The details of your order, including your order number, are displayed on the **Confirm** page.</span></span> <span data-ttu-id="b286d-273">选择“完成”转到“订单历史记录”页。</span><span class="sxs-lookup"><span data-stu-id="b286d-273">Select **Done** to go to your **Order history** page.</span></span> 

10. <span data-ttu-id="b286d-274">若要在 Azure 门户中管理客户的预订，请在 "**客户**" 页上找到 "客户"，然后选择向下箭头以展开客户的行。</span><span class="sxs-lookup"><span data-stu-id="b286d-274">To manage the customer's reservation in the Azure portal, find the customer on your **Customers** page and then select the down arrow to expand the customer's row.</span></span> <span data-ttu-id="b286d-275">选择 " **Microsoft Azure 管理门户**" 以打开 Azure 门户中的客户记录。</span><span class="sxs-lookup"><span data-stu-id="b286d-275">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="b286d-276">Azure 预订资源</span><span class="sxs-lookup"><span data-stu-id="b286d-276">Azure reservations resources</span></span>
|<span data-ttu-id="b286d-277">**有关**</span><span class="sxs-lookup"><span data-stu-id="b286d-277">**For information about**</span></span>   |<span data-ttu-id="b286d-278">**阅读此文**</span><span class="sxs-lookup"><span data-stu-id="b286d-278">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="b286d-279">云解决方案提供商计划中的 Azure 预订概述</span><span class="sxs-lookup"><span data-stu-id="b286d-279">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="b286d-280">出售 Microsoft Azure 预订实例</span><span class="sxs-lookup"><span data-stu-id="b286d-280">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="b286d-281">管理合作伙伴中心的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="b286d-281">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="b286d-282">管理合作伙伴中心的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="b286d-282">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="b286d-283">确定正确的虚拟机大小，然后确认客户虚拟机使用情况</span><span class="sxs-lookup"><span data-stu-id="b286d-283">Determine the correct VM size and verify customer VM usage</span></span>   |[<span data-ttu-id="b286d-284">最大 Azure 预订使用情况的 VM 大小调整</span><span class="sxs-lookup"><span data-stu-id="b286d-284">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="b286d-285">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="b286d-285">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="b286d-286">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="b286d-286">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
|

 


 
