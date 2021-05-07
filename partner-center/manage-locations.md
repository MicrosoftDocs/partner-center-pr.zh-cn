---
title: 管理合作伙伴帐户中的位置
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702886"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="90044-103">管理 MPN 帐户位置并添加（删除）位置</span><span class="sxs-lookup"><span data-stu-id="90044-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="90044-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="90044-104">**Appropriate roles**</span></span>

- <span data-ttu-id="90044-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="90044-105">Global admin</span></span>
- <span data-ttu-id="90044-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="90044-106">Account admin</span></span>

<span data-ttu-id="90044-107">位置 MPN ID 标识了公司的每一特定位置。</span><span class="sxs-lookup"><span data-stu-id="90044-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="90044-108">可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。</span><span class="sxs-lookup"><span data-stu-id="90044-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="90044-109">全局 MPN ID 用于非交易性活动，例如支持请求。</span><span class="sxs-lookup"><span data-stu-id="90044-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="90044-110">以下为典型场景：</span><span class="sxs-lookup"><span data-stu-id="90044-110">The following scenario is typical:</span></span>

<span data-ttu-id="90044-111">Contoso 的合作伙伴全局帐户 (PGA) 位于英国。</span><span class="sxs-lookup"><span data-stu-id="90044-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="90044-112">PGA 是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="90044-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="90044-113">Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="90044-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="90044-114">在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="90044-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="90044-115">PLA 用于交易性业务，例如 CSP 或奖励计划。</span><span class="sxs-lookup"><span data-stu-id="90044-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="90044-116">付款与特定位置相关。</span><span class="sxs-lookup"><span data-stu-id="90044-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="90044-117">CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。</span><span class="sxs-lookup"><span data-stu-id="90044-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="90044-119">为 CSP 业务添加新帐户的先决条件</span><span class="sxs-lookup"><span data-stu-id="90044-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="90044-120">若要添加新的 CSP 业务帐户，请先确保满足先决条件。</span><span class="sxs-lookup"><span data-stu-id="90044-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="90044-121">必须在要开展 CSP 业务的国家/地区具有 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="90044-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="90044-122">若要创建新的 MPN 位置，请阅读下面的“添加 MPN 位置”。</span><span class="sxs-lookup"><span data-stu-id="90044-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="90044-123">若要创建新的 CSP Indirect Reseller 注册，请阅读[与间接提供商合作](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="90044-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="90044-124">请记得使用新凭据登录新的 CSP 帐户 。</span><span class="sxs-lookup"><span data-stu-id="90044-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="90044-125">不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。</span><span class="sxs-lookup"><span data-stu-id="90044-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="90044-126">接受 Microsoft 合作伙伴协议并激活帐户。</span><span class="sxs-lookup"><span data-stu-id="90044-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="90044-127">如果要注册为直接计费合作伙伴，请阅读[直接计费合作伙伴要求](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="90044-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="90044-128">查看和更新 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="90044-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="90044-129">使用 MPN 帐户凭据登录合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="90044-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="90044-130">（MPN 凭据可能与 CSP 凭据不同）</span><span class="sxs-lookup"><span data-stu-id="90044-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="90044-131">从“设置”图标中，依次选择“帐户设置”、“组织资料”和“法务”   。</span><span class="sxs-lookup"><span data-stu-id="90044-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="90044-132">在“合作伙伴”选项卡中，验证确保没有横幅错误消息要求你修复从 PMC 迁移的位置。</span><span class="sxs-lookup"><span data-stu-id="90044-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="90044-133">如果位置未在 PMC 中正确设置，并且尚未转换为 PC，则需要更新这些位置。</span><span class="sxs-lookup"><span data-stu-id="90044-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="截图演示如何更新位置。":::
 
4.  <span data-ttu-id="90044-135">在“查看 PMC 位置”屏幕上，选择“更新” 。</span><span class="sxs-lookup"><span data-stu-id="90044-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="90044-136">更新以下字段：</span><span class="sxs-lookup"><span data-stu-id="90044-136">Update the following fields:</span></span>

- <span data-ttu-id="90044-137">“名称”字段：确保公司位置的名称正确。</span><span class="sxs-lookup"><span data-stu-id="90044-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="90044-138">如果显示重复错误，请尝试进行更改，例如将“Contoso”更改为“Contoso, Inc”。</span><span class="sxs-lookup"><span data-stu-id="90044-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="90044-139">“法律实体”字段：确保已选择该位置所绑定到的法律实体</span><span class="sxs-lookup"><span data-stu-id="90044-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="90044-140">“地址行 1”和“地址行 2”字段：确保地址正确</span><span class="sxs-lookup"><span data-stu-id="90044-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="90044-141">“城市和省/直辖市/自治区”字段：确保城市和省/市/自治区之间的组合是正确的。</span><span class="sxs-lookup"><span data-stu-id="90044-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="90044-142">在某些国家/地区可以应用用于选择省/直辖市/自治区的下拉菜单，在其他国家/地区则需要手动插入该字段。</span><span class="sxs-lookup"><span data-stu-id="90044-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="90044-143">“邮政编码”字段：确保“邮政编码”字段与指定的国家/地区、区域、城市或地址匹配。</span><span class="sxs-lookup"><span data-stu-id="90044-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="90044-144">“主要联系人信息”字段：确保已填写“名字”和“姓氏”字段，并且所指示的电子邮件地址是工作电子邮件地址，而不是个人电子邮件地址（例如，@outlook.com、@live.com 等）</span><span class="sxs-lookup"><span data-stu-id="90044-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="90044-145">“电话号码”字段：确保电话号码不包含特殊字符、空格或国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="90044-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="90044-146">“电话号码”字段中输入的值将始终包含最多 10 个字符。</span><span class="sxs-lookup"><span data-stu-id="90044-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="90044-147">如果没有错误消息，请从“设置”中依次选择“帐户设置”、“组织资料”和“标识符”   。</span><span class="sxs-lookup"><span data-stu-id="90044-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="90044-148">找到类型为“位置”且与此 CSP 帐户所在国家/地区匹配的 MPN ID，然后用它完成关联。</span><span class="sxs-lookup"><span data-stu-id="90044-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="90044-149">如果找不到与要使用的 CSP 帐户匹配的位置 MPN ID，可添加一个新位置，它将创建新的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="90044-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="90044-150">请查看下面的“添加 MPN 位置”。</span><span class="sxs-lookup"><span data-stu-id="90044-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="90044-151">添加 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="90044-151">Add an MPN location</span></span>

1. <span data-ttu-id="90044-152">在合作伙伴中心使用 MPN 帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="90044-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="90044-153">（你的 MPN 凭据可能与 CSP 凭据不同）。</span><span class="sxs-lookup"><span data-stu-id="90044-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="90044-154">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="90044-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="90044-155">从设置图标中，选择“帐户设置”，然后选择“组织资料”  。</span><span class="sxs-lookup"><span data-stu-id="90044-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="90044-156">选择“法务”，然后在“合作伙伴”选项卡上选择“业务位置”，然后单击“添加位置”   。</span><span class="sxs-lookup"><span data-stu-id="90044-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="90044-157">提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和联系人。</span><span class="sxs-lookup"><span data-stu-id="90044-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="90044-158">单击“添加位置”。</span><span class="sxs-lookup"><span data-stu-id="90044-158">Click **Add location**.</span></span> <span data-ttu-id="90044-159">这将为新位置创建一个新的 MPN ID，你可用它来进行 CSP 交易和激励。</span><span class="sxs-lookup"><span data-stu-id="90044-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="添加新的法定公司":::

> [!NOTE]
> <span data-ttu-id="90044-161">一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。</span><span class="sxs-lookup"><span data-stu-id="90044-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="90044-162">如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。</span><span class="sxs-lookup"><span data-stu-id="90044-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="90044-163">添加注册号 ID</span><span class="sxs-lookup"><span data-stu-id="90044-163">Add the registration number ID</span></span>

<span data-ttu-id="90044-164">如果你是间接提供商、直接计费合作伙伴或间接经销商，并且与以下国家/地区的新客户和现有客户开展业务，则需要为你的企业提供注册 ID 号。</span><span class="sxs-lookup"><span data-stu-id="90044-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="90044-165">如果你开展业务的国家/地区未在下面列出，则不必提供注册 ID。</span><span class="sxs-lookup"><span data-stu-id="90044-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="90044-166">亚美尼亚</span><span class="sxs-lookup"><span data-stu-id="90044-166">Armenia</span></span> 
- <span data-ttu-id="90044-167">阿塞拜疆</span><span class="sxs-lookup"><span data-stu-id="90044-167">Azerbaijan</span></span> 
- <span data-ttu-id="90044-168">白俄罗斯</span><span class="sxs-lookup"><span data-stu-id="90044-168">Belarus</span></span> 
- <span data-ttu-id="90044-169">巴西</span><span class="sxs-lookup"><span data-stu-id="90044-169">Brazil</span></span> 
- <span data-ttu-id="90044-170">匈牙利</span><span class="sxs-lookup"><span data-stu-id="90044-170">Hungary</span></span> 
- <span data-ttu-id="90044-171">印度</span><span class="sxs-lookup"><span data-stu-id="90044-171">India</span></span> 
- <span data-ttu-id="90044-172">伊拉克</span><span class="sxs-lookup"><span data-stu-id="90044-172">Iraq</span></span> 
- <span data-ttu-id="90044-173">哈萨克斯坦</span><span class="sxs-lookup"><span data-stu-id="90044-173">Kazakhstan</span></span> 
- <span data-ttu-id="90044-174">吉尔吉斯斯坦</span><span class="sxs-lookup"><span data-stu-id="90044-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="90044-175">摩尔多瓦</span><span class="sxs-lookup"><span data-stu-id="90044-175">Moldova</span></span> 
- <span data-ttu-id="90044-176">缅甸</span><span class="sxs-lookup"><span data-stu-id="90044-176">Myanmar</span></span> 
- <span data-ttu-id="90044-177">波兰</span><span class="sxs-lookup"><span data-stu-id="90044-177">Poland</span></span> 
- <span data-ttu-id="90044-178">俄罗斯</span><span class="sxs-lookup"><span data-stu-id="90044-178">Russia</span></span> 
- <span data-ttu-id="90044-179">沙特阿拉伯</span><span class="sxs-lookup"><span data-stu-id="90044-179">Saudi Arabia</span></span> 
- <span data-ttu-id="90044-180">南非</span><span class="sxs-lookup"><span data-stu-id="90044-180">South Africa</span></span> 
- <span data-ttu-id="90044-181">南苏丹</span><span class="sxs-lookup"><span data-stu-id="90044-181">South Sudan</span></span>  
- <span data-ttu-id="90044-182">塔吉克斯坦</span><span class="sxs-lookup"><span data-stu-id="90044-182">Tajikistan</span></span> 
- <span data-ttu-id="90044-183">泰国</span><span class="sxs-lookup"><span data-stu-id="90044-183">Thailand</span></span>
- <span data-ttu-id="90044-184">土耳其</span><span class="sxs-lookup"><span data-stu-id="90044-184">Turkey</span></span> 
- <span data-ttu-id="90044-185">乌克兰</span><span class="sxs-lookup"><span data-stu-id="90044-185">Ukraine</span></span> 
- <span data-ttu-id="90044-186">阿拉伯联合酋长国</span><span class="sxs-lookup"><span data-stu-id="90044-186">United Arab Emirates</span></span> 
- <span data-ttu-id="90044-187">乌兹别克斯坦</span><span class="sxs-lookup"><span data-stu-id="90044-187">Uzbekistan</span></span> 
- <span data-ttu-id="90044-188">委内瑞拉</span><span class="sxs-lookup"><span data-stu-id="90044-188">Venezuela</span></span>
- <span data-ttu-id="90044-189">越南</span><span class="sxs-lookup"><span data-stu-id="90044-189">Vietnam</span></span> 


<span data-ttu-id="90044-190">有关详细信息，请参阅[注册 ID 号信息](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="90044-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="90044-191">删除位置</span><span class="sxs-lookup"><span data-stu-id="90044-191">Delete a location</span></span>

<span data-ttu-id="90044-192">若要从帐户中删除某个位置，需要联系[合作伙伴支持人员](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)。</span><span class="sxs-lookup"><span data-stu-id="90044-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="90044-193">请确保了解此操作的影响。</span><span class="sxs-lookup"><span data-stu-id="90044-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="90044-194">无法检索已删除的位置，并且将不再为你的公司识别或激活任何绑定到该特定 MPN id 的内容。</span><span class="sxs-lookup"><span data-stu-id="90044-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="90044-195">更改合作伙伴全球帐户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="90044-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="90044-196">在合作伙伴中心使用 MPN 帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="90044-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="90044-197">（你的 MPN 凭据可能与 CSP 凭据不同）。</span><span class="sxs-lookup"><span data-stu-id="90044-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="90044-198">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="90044-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="90044-199">在“合作伙伴”选项卡上，转到“业务位置”，然后检查位置列表，确保已列出你想用作法律实体的位置 。</span><span class="sxs-lookup"><span data-stu-id="90044-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="90044-200">若要添加位置，请单击“添加位置”，然后在弹出窗口中，提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和主要联系人。</span><span class="sxs-lookup"><span data-stu-id="90044-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="90044-201">选择“国家/地区”下拉列表旁边的“更改国家/地区”，然后按照步骤操作 。</span><span class="sxs-lookup"><span data-stu-id="90044-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法定公司资料数据弹出窗口":::

5. <span data-ttu-id="90044-203">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="90044-203">Click **Save**.</span></span>

6. <span data-ttu-id="90044-204">MPN 全球帐户所在国家/地区将更改为新的法定国家/地区。</span><span class="sxs-lookup"><span data-stu-id="90044-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="90044-205">后续步骤</span><span class="sxs-lookup"><span data-stu-id="90044-205">Next steps</span></span>

- <span data-ttu-id="90044-206">了解[验证过程](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="90044-206">Learn about the [verification process](verification-responses.md).</span></span>
