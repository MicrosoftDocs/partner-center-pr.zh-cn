---
title: Cloudyn for Csp 的 Azure 成本管理
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心注册 Cloudyn web 应用并使用它的密钥，以便可以使用该应用来跟踪客户的 Azure 使用情况和成本。
author: aparnagkrishnan
ms.author: aparnag
Keywords: Azure 成本管理应用，管理成本，web 应用
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 521501f9a979c0993d299ab30443168408656a44
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390444"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="0221a-104">使用适用于 CSP 合作伙伴的 Azure 成本管理应用跟踪客户的 Azure 使用情况和成本</span><span class="sxs-lookup"><span data-stu-id="0221a-104">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="0221a-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="0221a-105">**Applies to**</span></span>

- <span data-ttu-id="0221a-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="0221a-106">Partner Center</span></span>
- <span data-ttu-id="0221a-107">云解决方案提供商计划合作伙伴</span><span class="sxs-lookup"><span data-stu-id="0221a-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="0221a-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="0221a-108">**Appropriate roles**</span></span>

- <span data-ttu-id="0221a-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0221a-109">Global admin</span></span>
- <span data-ttu-id="0221a-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="0221a-110">Admin agent</span></span>

[<span data-ttu-id="0221a-111">获取有关 Azure Cost Management 的详细信息</span><span class="sxs-lookup"><span data-stu-id="0221a-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="0221a-112">开始之前</span><span class="sxs-lookup"><span data-stu-id="0221a-112">Before you begin</span></span>
<span data-ttu-id="0221a-113">为能够使用 Azure Cost Management，请确保你满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="0221a-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="0221a-114">你是参与云解决方案提供商计划的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="0221a-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="0221a-115">你具备创建合作伙伴中心 API Web 应用的能力。</span><span class="sxs-lookup"><span data-stu-id="0221a-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="0221a-116">概述</span><span class="sxs-lookup"><span data-stu-id="0221a-116">Overview</span></span>

<span data-ttu-id="0221a-117">Cloudyn 是一个 web 应用，可用于跟踪和管理你的客户使用 Azure 的量和该使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="0221a-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="0221a-118">你可以通过合作伙伴中心 API 使用 Azure Cost Management。</span><span class="sxs-lookup"><span data-stu-id="0221a-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="0221a-119">在合作伙伴中心注册你的 Web 应用</span><span class="sxs-lookup"><span data-stu-id="0221a-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="0221a-120">在合作伙伴中心注册一款 Azure Active Directory Web 应用即可获得合作伙伴中心 API 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="0221a-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="0221a-121">使用[全局管理员或管理员代理帐户](create-user-accounts-and-set-permissions.md)登录到[合作伙伴中心](https://partnercenter.microsoft.com/pcv/dashboard/overview)。</span><span class="sxs-lookup"><span data-stu-id="0221a-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="0221a-122">从 "**合作伙伴中心**"，选择 "**帐户设置**" " &gt; **[应用管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**"。</span><span class="sxs-lookup"><span data-stu-id="0221a-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="0221a-123">在 **Web 应用**部分中，单击**添加新的 Web 应用**。</span><span class="sxs-lookup"><span data-stu-id="0221a-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="0221a-124">**注意**：如果此前已创建 Web 应用，你可以跳过第 3 步。</span><span class="sxs-lookup"><span data-stu-id="0221a-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="0221a-125">复制并保存你的 Web 应用的**商业 ID** GUID 和**应用 ID** GUID。</span><span class="sxs-lookup"><span data-stu-id="0221a-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="0221a-126">你必须拥有这两个 ID，才能使用为期 30 天的 Azure Cost Management 应用免费试用版。</span><span class="sxs-lookup"><span data-stu-id="0221a-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="0221a-127">为应用添加密钥</span><span class="sxs-lookup"><span data-stu-id="0221a-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="0221a-128">在**添加密钥**按钮旁的下拉列表中，选择 1 年或 2 年有效期。</span><span class="sxs-lookup"><span data-stu-id="0221a-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="0221a-129">单击 "**添加密钥**"。</span><span class="sxs-lookup"><span data-stu-id="0221a-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="0221a-130">复制并保存密钥值。</span><span class="sxs-lookup"><span data-stu-id="0221a-130">Copy and save the secret key value.</span></span> <span data-ttu-id="0221a-131">你将需要借助此密钥使用为期 30 天的免费试用版。</span><span class="sxs-lookup"><span data-stu-id="0221a-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="0221a-132">应用程序密钥类似于密码，具有较长的到期日期。</span><span class="sxs-lookup"><span data-stu-id="0221a-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="0221a-133">请将密钥值保存在安全的位置以供今后使用。</span><span class="sxs-lookup"><span data-stu-id="0221a-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0221a-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0221a-134">Next steps</span></span>
<span data-ttu-id="0221a-135">开始使用[为期 30 天的免费试用版](https://go.microsoft.com/fwlink/?linkid=857895)。</span><span class="sxs-lookup"><span data-stu-id="0221a-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="0221a-136">你需要提供以下详细信息以开始试用：</span><span class="sxs-lookup"><span data-stu-id="0221a-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="0221a-137">合作伙伴中心登录凭据</span><span class="sxs-lookup"><span data-stu-id="0221a-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="0221a-138">商业 ID GUID</span><span class="sxs-lookup"><span data-stu-id="0221a-138">Commerce ID GUID</span></span>
- <span data-ttu-id="0221a-139">应用 ID GUID</span><span class="sxs-lookup"><span data-stu-id="0221a-139">App ID GUID</span></span>
- <span data-ttu-id="0221a-140">应用程序密钥值</span><span class="sxs-lookup"><span data-stu-id="0221a-140">Application secret key value</span></span>
