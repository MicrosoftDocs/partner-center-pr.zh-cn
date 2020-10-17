---
title: 管理合作伙伴帐户中的位置
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "92100767"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="6d4ed-103">管理 MPN 帐户位置并添加新位置</span><span class="sxs-lookup"><span data-stu-id="6d4ed-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="6d4ed-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="6d4ed-104">**Applies to**</span></span>

- <span data-ttu-id="6d4ed-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6d4ed-105">Partner Center</span></span>

<span data-ttu-id="6d4ed-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="6d4ed-106">**Appropriate roles**</span></span>

- <span data-ttu-id="6d4ed-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="6d4ed-107">Global admin</span></span>
- <span data-ttu-id="6d4ed-108">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="6d4ed-108">Account admin</span></span>

<span data-ttu-id="6d4ed-109">位置 MPN ID 标识了公司的每一特定位置。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="6d4ed-110">可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="6d4ed-111">全局 MPN ID 用于非交易性活动，例如支持请求。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="6d4ed-112">下面是一个典型方案：</span><span class="sxs-lookup"><span data-stu-id="6d4ed-112">The following is a typical scenario:</span></span>

<span data-ttu-id="6d4ed-113">Contoso 的合作伙伴全局帐户 (PGA) 位于英国。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="6d4ed-114">这是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="6d4ed-115">Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="6d4ed-116">在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="6d4ed-117">PLA 用于交易性业务，例如 CSP 或奖励计划。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="6d4ed-118">付款与特定位置相关。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="6d4ed-119">CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="6d4ed-121">为 CSP 业务添加新位置的先决条件</span><span class="sxs-lookup"><span data-stu-id="6d4ed-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="6d4ed-122">若要添加新的 CSP 业务位置，需要满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="6d4ed-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="6d4ed-123">必须在要开展业务的国家/地区具有 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="6d4ed-124">你需要在尚未注册 CSP 的[业务区域](regional-authorization-overview.md)中具有一个新的 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="6d4ed-125">在注册 CSP 时创建此租户。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="6d4ed-126">使用新的 AAD 租户注册在该区域注册 CSP 计划。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="6d4ed-127">提供法定的公司详细信息，包括合法的公司名称、地址、主要联系人详细信息。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="6d4ed-128">此帐户将经过验证，因此请确保添加有效的信息。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="6d4ed-129">请记住，使用新的凭据登录新的 Azure AD 租户 。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="6d4ed-130">不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="6d4ed-131">接受 Microsoft 合作伙伴协议并激活帐户。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="6d4ed-132">添加 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="6d4ed-132">Add an MPN location</span></span>

1. <span data-ttu-id="6d4ed-133">使用合作伙伴中心的 MPN 帐户登录。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="6d4ed-134">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="6d4ed-135">从“设置”图标中选择“合作伙伴设置”。 </span><span class="sxs-lookup"><span data-stu-id="6d4ed-135">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="6d4ed-136">选择“位置”。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-136">Select **Locations.**</span></span>

3. <span data-ttu-id="6d4ed-137">选择“添加位置”，然后插入要添加到公司的位置的地址详细信息以及该位置的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="6d4ed-138">一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="6d4ed-139">如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="6d4ed-140">更改全局合作伙伴帐户位置</span><span class="sxs-lookup"><span data-stu-id="6d4ed-140">Change Global partner account location</span></span>

1. <span data-ttu-id="6d4ed-141">在“[位置](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)”页面上，检查位置列表，确保其中已列出你希望作为法人实体的位置。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="6d4ed-142">否则，请添加该位置。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN 位置的结构":::

2. <span data-ttu-id="6d4ed-144">选择“合作伙伴配置文件”，然后选择“更新法定公司配置文件” </span><span class="sxs-lookup"><span data-stu-id="6d4ed-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN 位置的结构":::

3. <span data-ttu-id="6d4ed-146">选择区域和法人，并“提交”。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN 位置的结构":::

## <a name="next-steps"></a><span data-ttu-id="6d4ed-148">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6d4ed-148">Next steps</span></span>

- <span data-ttu-id="6d4ed-149">了解[验证过程](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="6d4ed-149">Learn about the [verification process](verification-responses.md).</span></span>
