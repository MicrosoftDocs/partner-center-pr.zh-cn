---
title: 管理合作伙伴帐户中的位置
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005905"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="43f0b-103">管理 MPN 帐户位置并添加（删除）位置</span><span class="sxs-lookup"><span data-stu-id="43f0b-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="43f0b-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="43f0b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="43f0b-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="43f0b-105">Global admin</span></span>
- <span data-ttu-id="43f0b-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="43f0b-106">Account admin</span></span>

<span data-ttu-id="43f0b-107">位置 MPN ID 标识了公司的每一特定位置。</span><span class="sxs-lookup"><span data-stu-id="43f0b-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="43f0b-108">可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。</span><span class="sxs-lookup"><span data-stu-id="43f0b-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="43f0b-109">全局 MPN ID 用于非交易性活动，例如支持请求。</span><span class="sxs-lookup"><span data-stu-id="43f0b-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="43f0b-110">下面是一个典型方案：</span><span class="sxs-lookup"><span data-stu-id="43f0b-110">The following is a typical scenario:</span></span>

<span data-ttu-id="43f0b-111">Contoso 的合作伙伴全局帐户 (PGA) 位于英国。</span><span class="sxs-lookup"><span data-stu-id="43f0b-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="43f0b-112">这是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="43f0b-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="43f0b-113">Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="43f0b-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="43f0b-114">在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="43f0b-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="43f0b-115">PLA 用于交易性业务，例如 CSP 或奖励计划。</span><span class="sxs-lookup"><span data-stu-id="43f0b-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="43f0b-116">付款与特定位置相关。</span><span class="sxs-lookup"><span data-stu-id="43f0b-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="43f0b-117">CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。</span><span class="sxs-lookup"><span data-stu-id="43f0b-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="43f0b-119">为 CSP 业务添加新帐户的先决条件</span><span class="sxs-lookup"><span data-stu-id="43f0b-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="43f0b-120">若要添加新的 CSP 业务帐户，请先确保满足先决条件。</span><span class="sxs-lookup"><span data-stu-id="43f0b-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="43f0b-121">必须在要开展 CSP 业务的国家/地区具有 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="43f0b-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="43f0b-122">若要创建新的 MPN 位置，请阅读下面的“添加 MPN 位置”。</span><span class="sxs-lookup"><span data-stu-id="43f0b-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="43f0b-123">若要创建新的 CSP Indirect Reseller 注册，请阅读[与间接提供商合作](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="43f0b-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="43f0b-124">请记得使用新凭据登录新的 CSP 帐户 。</span><span class="sxs-lookup"><span data-stu-id="43f0b-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="43f0b-125">不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。</span><span class="sxs-lookup"><span data-stu-id="43f0b-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="43f0b-126">接受 Microsoft 合作伙伴协议并激活帐户。</span><span class="sxs-lookup"><span data-stu-id="43f0b-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="43f0b-127">如果要注册为直接计费合作伙伴，请阅读[直接计费合作伙伴要求](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="43f0b-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="43f0b-128">查看 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="43f0b-128">View your MPN locations</span></span>

1. <span data-ttu-id="43f0b-129">使用 MPN 帐户凭据登录合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="43f0b-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="43f0b-130">（MPN 凭据可能与 CSP 凭据不同）</span><span class="sxs-lookup"><span data-stu-id="43f0b-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="43f0b-131">从“设置”图标中，依次选择“帐户设置”、“组织资料”和“法务”   。</span><span class="sxs-lookup"><span data-stu-id="43f0b-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="43f0b-132">在“合作伙伴”选项卡中，验证确保没有横幅错误消息要求你修复从 PMC 迁移的位置。</span><span class="sxs-lookup"><span data-stu-id="43f0b-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="43f0b-133">如果有错误消息，请按照说明修复这些位置。</span><span class="sxs-lookup"><span data-stu-id="43f0b-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="43f0b-134">如果没有错误消息，请从“设置”中依次选择“帐户设置”、“组织资料”和“标识符”   。</span><span class="sxs-lookup"><span data-stu-id="43f0b-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="43f0b-135">找到类型为“位置”且与此 CSP 帐户所在国家/地区匹配的 MPN ID，然后用它在下面进行搜索并完成关联。</span><span class="sxs-lookup"><span data-stu-id="43f0b-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="43f0b-136">如果找不到与要使用的 CSP 帐户匹配的位置 MPN ID，可添加一个新位置，它将创建新的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="43f0b-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="43f0b-137">请查看下面的“添加 MPN 位置”。</span><span class="sxs-lookup"><span data-stu-id="43f0b-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="43f0b-138">添加 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="43f0b-138">Add an MPN location</span></span>

1. <span data-ttu-id="43f0b-139">在合作伙伴中心使用 MPN 帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="43f0b-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="43f0b-140">（你的 MPN 凭据可能与 CSP 凭据不同）。</span><span class="sxs-lookup"><span data-stu-id="43f0b-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="43f0b-141">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="43f0b-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="43f0b-142">从设置图标中，选择“帐户设置”，然后选择“组织资料”  。</span><span class="sxs-lookup"><span data-stu-id="43f0b-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="43f0b-143">选择“法务”，然后在“合作伙伴”选项卡上选择“业务位置”，然后单击“添加位置”   。</span><span class="sxs-lookup"><span data-stu-id="43f0b-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="43f0b-144">提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和联系人。</span><span class="sxs-lookup"><span data-stu-id="43f0b-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="43f0b-145">单击“添加位置”。</span><span class="sxs-lookup"><span data-stu-id="43f0b-145">Click **Add location**.</span></span> <span data-ttu-id="43f0b-146">这将为新位置创建一个新的 MPN ID，你可用它来进行 CSP 交易和激励。</span><span class="sxs-lookup"><span data-stu-id="43f0b-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="添加新的法定公司":::

> [!NOTE]
> <span data-ttu-id="43f0b-148">一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。</span><span class="sxs-lookup"><span data-stu-id="43f0b-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="43f0b-149">如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。</span><span class="sxs-lookup"><span data-stu-id="43f0b-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="43f0b-150">删除位置</span><span class="sxs-lookup"><span data-stu-id="43f0b-150">Delete a location</span></span>

<span data-ttu-id="43f0b-151">若要从帐户中删除某个位置，需要联系[合作伙伴支持](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)人员。</span><span class="sxs-lookup"><span data-stu-id="43f0b-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="43f0b-152">请确保了解此操作的影响。</span><span class="sxs-lookup"><span data-stu-id="43f0b-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="43f0b-153">无法检索已删除的位置，并且将不再为你的公司识别或激活任何绑定到该特定 MPN id 的内容。</span><span class="sxs-lookup"><span data-stu-id="43f0b-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="43f0b-154">更改合作伙伴全球帐户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="43f0b-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="43f0b-155">在合作伙伴中心使用 MPN 帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="43f0b-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="43f0b-156">（你的 MPN 凭据可能与 CSP 凭据不同）。</span><span class="sxs-lookup"><span data-stu-id="43f0b-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="43f0b-157">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="43f0b-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="43f0b-158">在“合作伙伴”选项卡上，转到“业务位置”，然后检查位置列表，确保已列出你想用作法律实体的位置 。</span><span class="sxs-lookup"><span data-stu-id="43f0b-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="43f0b-159">若要添加位置，请单击“添加位置”，然后在弹出窗口中，提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和主要联系人。</span><span class="sxs-lookup"><span data-stu-id="43f0b-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="43f0b-160">选择“国家/地区”下拉列表旁边的“更改国家/地区”，然后按照步骤操作 。</span><span class="sxs-lookup"><span data-stu-id="43f0b-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法定公司资料数据弹出窗口":::

5. <span data-ttu-id="43f0b-162">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="43f0b-162">Click **Save**.</span></span>

6. <span data-ttu-id="43f0b-163">MPN 全球帐户所在国家/地区将更改为新的法定国家/地区。</span><span class="sxs-lookup"><span data-stu-id="43f0b-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="43f0b-164">后续步骤</span><span class="sxs-lookup"><span data-stu-id="43f0b-164">Next steps</span></span>

- <span data-ttu-id="43f0b-165">了解[验证过程](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="43f0b-165">Learn about the [verification process](verification-responses.md).</span></span>
