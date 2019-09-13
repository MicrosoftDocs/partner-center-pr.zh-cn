---
title: Azure Cost Management by Cloudyn（面向云解决方案提供商合作伙伴）| 合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
description: Azure Cost Management by Cloudyn 需要对合作伙伴中心 API 的访问权限进行预配。
author: Janet
ms.author: janet
Keywords: Azure 成本管理应用, 管理成本, web 应用
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 27ff91d9d42f08e44f812663f3d4409e1080d580
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820300"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="2d4e4-104">面向 Azure 云解决方案提供商合作伙伴的 Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="2d4e4-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="2d4e4-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="2d4e4-105">**Applies to**</span></span>

-  <span data-ttu-id="2d4e4-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2d4e4-106">Partner Center</span></span>

[<span data-ttu-id="2d4e4-107">获取有关 Azure 成本管理的详细信息</span><span class="sxs-lookup"><span data-stu-id="2d4e4-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="2d4e4-108">开始之前</span><span class="sxs-lookup"><span data-stu-id="2d4e4-108">Before you begin</span></span>
<span data-ttu-id="2d4e4-109">为能够使用 Azure Cost Management，请确保你满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="2d4e4-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="2d4e4-110">你是参与云解决方案提供商计划的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="2d4e4-111">你具备创建合作伙伴中心 API Web 应用的能力。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="2d4e4-112">概述</span><span class="sxs-lookup"><span data-stu-id="2d4e4-112">Overview</span></span>

<span data-ttu-id="2d4e4-113">Cloudyn 是一个 web 应用, 可用于跟踪和管理你的客户使用 Azure 的量和该使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="2d4e4-114">你可以通过合作伙伴中心 API 使用 Azure Cost Management。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="2d4e4-115">在合作伙伴中心注册你的 Web 应用</span><span class="sxs-lookup"><span data-stu-id="2d4e4-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="2d4e4-116">在合作伙伴中心注册一款 Azure Active Directory Web 应用即可获得合作伙伴中心 API 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="2d4e4-117">使用[全局管理员或管理员代理帐户](create-user-accounts-and-set-permissions.md)登录到[合作伙伴中心](https://partnercenter.microsoft.com/pcv/dashboard/overview)。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="2d4e4-118">从 "**合作伙伴中心**", 选择 "**帐户设置** &gt; " " **[应用管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** "。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="2d4e4-119">在 **Web 应用**部分中，单击**添加新的 Web 应用**。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="2d4e4-120">**注意**：如果你之前创建了 web 应用, 则可以跳过步骤3。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="2d4e4-121">复制并保存你的 Web 应用的**商业 ID** GUID 和**应用 ID** GUID。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="2d4e4-122">你必须拥有这两个 ID，才能使用为期 30 天的 Azure Cost Management 应用免费试用版。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="2d4e4-123">为应用添加密钥</span><span class="sxs-lookup"><span data-stu-id="2d4e4-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="2d4e4-124">在**添加密钥**按钮旁的下拉列表中，选择 1 年或 2 年有效期。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="2d4e4-125">单击**添加密钥**。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="2d4e4-126">复制并保存密钥值。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-126">Copy and save the secret key value.</span></span> <span data-ttu-id="2d4e4-127">你将需要借助此密钥使用为期 30 天的免费试用版。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="2d4e4-128">应用程序密钥类似于密码, 具有较长的到期日期。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="2d4e4-129">请将密钥值保存在安全的位置以供今后使用。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2d4e4-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2d4e4-130">Next steps</span></span>
<span data-ttu-id="2d4e4-131">开始使用[为期 30 天的免费试用版](https://go.microsoft.com/fwlink/?linkid=857895)。</span><span class="sxs-lookup"><span data-stu-id="2d4e4-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="2d4e4-132">你需要提供以下详细信息以开始试用：</span><span class="sxs-lookup"><span data-stu-id="2d4e4-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="2d4e4-133">合作伙伴中心登录凭据</span><span class="sxs-lookup"><span data-stu-id="2d4e4-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="2d4e4-134">商业 ID GUID</span><span class="sxs-lookup"><span data-stu-id="2d4e4-134">Commerce ID GUID</span></span>
- <span data-ttu-id="2d4e4-135">应用 ID GUID</span><span class="sxs-lookup"><span data-stu-id="2d4e4-135">App ID GUID</span></span>
- <span data-ttu-id="2d4e4-136">应用程序密钥值</span><span class="sxs-lookup"><span data-stu-id="2d4e4-136">Application secret key value</span></span>
