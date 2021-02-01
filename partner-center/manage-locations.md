---
title: 管理合作伙伴帐户中的位置
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098884"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="94827-103">管理 MPN 帐户位置并添加新位置</span><span class="sxs-lookup"><span data-stu-id="94827-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="94827-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="94827-104">**Appropriate roles**</span></span>

- <span data-ttu-id="94827-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="94827-105">Global admin</span></span>
- <span data-ttu-id="94827-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="94827-106">Account admin</span></span>

<span data-ttu-id="94827-107">位置 MPN ID 标识了公司的每一特定位置。</span><span class="sxs-lookup"><span data-stu-id="94827-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="94827-108">可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。</span><span class="sxs-lookup"><span data-stu-id="94827-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="94827-109">全局 MPN ID 用于非交易性活动，例如支持请求。</span><span class="sxs-lookup"><span data-stu-id="94827-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="94827-110">下面是一个典型方案：</span><span class="sxs-lookup"><span data-stu-id="94827-110">The following is a typical scenario:</span></span>

<span data-ttu-id="94827-111">Contoso 的合作伙伴全局帐户 (PGA) 位于英国。</span><span class="sxs-lookup"><span data-stu-id="94827-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="94827-112">这是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="94827-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="94827-113">Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="94827-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="94827-114">在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="94827-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="94827-115">PLA 用于交易性业务，例如 CSP 或奖励计划。</span><span class="sxs-lookup"><span data-stu-id="94827-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="94827-116">付款与特定位置相关。</span><span class="sxs-lookup"><span data-stu-id="94827-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="94827-117">CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。</span><span class="sxs-lookup"><span data-stu-id="94827-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="94827-119">为 CSP 业务添加新帐户的先决条件</span><span class="sxs-lookup"><span data-stu-id="94827-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="94827-120">若要添加新的 CSP 业务帐户，请先确保满足先决条件。</span><span class="sxs-lookup"><span data-stu-id="94827-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="94827-121">必须在要开展 CSP 业务的国家/地区具有 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="94827-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="94827-122">若要创建新的 MPN 位置，请阅读下面的“添加 MPN 位置”。</span><span class="sxs-lookup"><span data-stu-id="94827-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="94827-123">若要创建新的 CSP Indirect Reseller 注册，请阅读[与间接提供商合作](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="94827-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="94827-124">请记得使用新凭据登录新的 CSP 帐户 。</span><span class="sxs-lookup"><span data-stu-id="94827-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="94827-125">不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。</span><span class="sxs-lookup"><span data-stu-id="94827-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="94827-126">接受 Microsoft 合作伙伴协议并激活帐户。</span><span class="sxs-lookup"><span data-stu-id="94827-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="94827-127">查看 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="94827-127">View your MPN locations</span></span>

1. <span data-ttu-id="94827-128">使用 MPN 帐户凭据登录合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="94827-128">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="94827-129">（MPN 凭据可能与 CSP 凭据不同）</span><span class="sxs-lookup"><span data-stu-id="94827-129">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="94827-130">从“设置”图标中，依次选择“帐户设置”、“组织资料”和“法务”   。</span><span class="sxs-lookup"><span data-stu-id="94827-130">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="94827-131">在“合作伙伴”选项卡中，验证确保没有横幅错误消息要求你修复从 PMC 迁移的位置。</span><span class="sxs-lookup"><span data-stu-id="94827-131">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="94827-132">如果有错误消息，请按照说明修复这些位置。</span><span class="sxs-lookup"><span data-stu-id="94827-132">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="94827-133">如果没有错误消息，请从“设置”中依次选择“帐户设置”、“组织资料”和“标识符”   。</span><span class="sxs-lookup"><span data-stu-id="94827-133">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="94827-134">找到类型为“位置”且与此 CSP 帐户所在国家/地区匹配的 MPN ID，然后用它在下面进行搜索并完成关联。</span><span class="sxs-lookup"><span data-stu-id="94827-134">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="94827-135">如果找不到与要使用的 CSP 帐户匹配的位置 MPN ID，可添加一个新位置，它将创建新的 MPN ID。</span><span class="sxs-lookup"><span data-stu-id="94827-135">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="94827-136">请查看下面的“添加 MPN 位置”。</span><span class="sxs-lookup"><span data-stu-id="94827-136">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="94827-137">添加 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="94827-137">Add an MPN location</span></span>

1. <span data-ttu-id="94827-138">在合作伙伴中心使用 MPN 帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="94827-138">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="94827-139">（你的 MPN 凭据可能与 CSP 凭据不同）。</span><span class="sxs-lookup"><span data-stu-id="94827-139">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="94827-140">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="94827-140">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="94827-141">从设置图标中，选择“帐户设置”，然后选择“组织资料”  。</span><span class="sxs-lookup"><span data-stu-id="94827-141">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="94827-142">选择“法务”，然后在“合作伙伴”选项卡上选择“业务位置”，然后单击“添加位置”   。</span><span class="sxs-lookup"><span data-stu-id="94827-142">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="94827-143">提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和联系人。</span><span class="sxs-lookup"><span data-stu-id="94827-143">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="94827-144">单击“添加位置”。</span><span class="sxs-lookup"><span data-stu-id="94827-144">Click **Add location**.</span></span> <span data-ttu-id="94827-145">这将为新位置创建一个新的 MPN ID，你可用它来进行 CSP 交易和激励。</span><span class="sxs-lookup"><span data-stu-id="94827-145">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="添加新的法定公司":::

> [!NOTE]
> <span data-ttu-id="94827-147">一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。</span><span class="sxs-lookup"><span data-stu-id="94827-147">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="94827-148">如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。</span><span class="sxs-lookup"><span data-stu-id="94827-148">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="94827-149">更改合作伙伴全球帐户所在国家/地区</span><span class="sxs-lookup"><span data-stu-id="94827-149">Change country of Partner global account</span></span> 

1. <span data-ttu-id="94827-150">在合作伙伴中心使用 MPN 帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="94827-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="94827-151">（你的 MPN 凭据可能与 CSP 凭据不同）。</span><span class="sxs-lookup"><span data-stu-id="94827-151">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="94827-152">MPN 帐户应具有全局管理员或帐户管理员权限。</span><span class="sxs-lookup"><span data-stu-id="94827-152">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="94827-153">在“合作伙伴”选项卡上，转到“业务位置”，然后检查位置列表，确保已列出你想用作法律实体的位置 。</span><span class="sxs-lookup"><span data-stu-id="94827-153">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="94827-154">若要添加位置，请单击“添加位置”，然后在弹出窗口中，提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和主要联系人。</span><span class="sxs-lookup"><span data-stu-id="94827-154">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="94827-155">选择“国家/地区”下拉列表旁边的“更改国家/地区”，然后按照步骤操作 。</span><span class="sxs-lookup"><span data-stu-id="94827-155">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法定公司资料数据弹出窗口":::

5. <span data-ttu-id="94827-157">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="94827-157">Click **Save**.</span></span>

6. <span data-ttu-id="94827-158">MPN 全球帐户所在国家/地区将更改为新的法定国家/地区。</span><span class="sxs-lookup"><span data-stu-id="94827-158">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="94827-159">后续步骤</span><span class="sxs-lookup"><span data-stu-id="94827-159">Next steps</span></span>

- <span data-ttu-id="94827-160">了解[验证过程](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="94827-160">Learn about the [verification process](verification-responses.md).</span></span>
