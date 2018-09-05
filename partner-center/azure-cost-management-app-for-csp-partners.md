---
title: Azure Cost Management by Cloudyn（面向云解决方案提供商合作伙伴）| 合作伙伴中心
description: Azure Cost Management by Cloudyn 需要对合作伙伴中心 API 的访问权限进行预配。
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 6ab388f9a178a0bfd3b3d3133da855bcddee9d4f
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877447"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="70e84-103">面向 Azure 云解决方案提供商合作伙伴的 Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="70e84-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="70e84-104">适用范围</span><span class="sxs-lookup"><span data-stu-id="70e84-104">Applies to</span></span>**

-  <span data-ttu-id="70e84-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="70e84-105">Partner Center</span></span>

[<span data-ttu-id="70e84-106">获取有关 Azure Cost Management 的详细信息</span><span class="sxs-lookup"><span data-stu-id="70e84-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="70e84-107">开始之前</span><span class="sxs-lookup"><span data-stu-id="70e84-107">Before you begin</span></span>
<span data-ttu-id="70e84-108">为能够使用 Azure Cost Management，请确保你满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="70e84-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="70e84-109">你是参与云解决方案提供商计划的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="70e84-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="70e84-110">你具备创建合作伙伴中心 API Web 应用的能力。</span><span class="sxs-lookup"><span data-stu-id="70e84-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="70e84-111">概述</span><span class="sxs-lookup"><span data-stu-id="70e84-111">Overview</span></span>

<span data-ttu-id="70e84-112">Azure Cost Management by Cloudyn 是一款 Web 应用，用于跟踪和管理客户使用 Azure 的程度以及该使用情况所产生的成本。</span><span class="sxs-lookup"><span data-stu-id="70e84-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="70e84-113">你可以通过合作伙伴中心 API 使用 Azure Cost Management。</span><span class="sxs-lookup"><span data-stu-id="70e84-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="70e84-114">在合作伙伴中心注册你的 Web 应用</span><span class="sxs-lookup"><span data-stu-id="70e84-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="70e84-115">在合作伙伴中心注册一款 Azure Active Directory Web 应用即可获得合作伙伴中心 API 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="70e84-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="70e84-116">使用[全局管理员或管理员代理帐户](create-user-accounts-and-set-permissions.md)登录到[合作伙伴中心](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)。</span><span class="sxs-lookup"><span data-stu-id="70e84-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="70e84-117">在**仪表板**中，选择**帐户设置** &gt; **[应用管理](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**。</span><span class="sxs-lookup"><span data-stu-id="70e84-117">From the **Dashboard**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="70e84-118">在 **Web 应用**部分中，单击**添加新的 Web 应用**。</span><span class="sxs-lookup"><span data-stu-id="70e84-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="70e84-119">**注意**：如果此前已创建 Web 应用，你可以跳过第 3 步。</span><span class="sxs-lookup"><span data-stu-id="70e84-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="70e84-120">复制并保存你的 Web 应用的**商业 ID** GUID 和**应用 ID** GUID。</span><span class="sxs-lookup"><span data-stu-id="70e84-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="70e84-121">你必须拥有这两个 ID，才能使用为期 30 天的 Azure Cost Management 应用免费试用版。</span><span class="sxs-lookup"><span data-stu-id="70e84-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="70e84-122">为应用添加密钥</span><span class="sxs-lookup"><span data-stu-id="70e84-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="70e84-123">在**添加密钥**按钮旁的下拉列表中，选择 1 年或 2 年有效期。</span><span class="sxs-lookup"><span data-stu-id="70e84-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="70e84-124">单击**添加密钥**。</span><span class="sxs-lookup"><span data-stu-id="70e84-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="70e84-125">复制并保存密钥值。</span><span class="sxs-lookup"><span data-stu-id="70e84-125">Copy and save the secret key value.</span></span> <span data-ttu-id="70e84-126">你将需要借助此密钥使用为期 30 天的免费试用版。</span><span class="sxs-lookup"><span data-stu-id="70e84-126">You will need this for the 30-day free trial.</span></span>
<br><span data-ttu-id="70e84-127">**注意**：应用程序密钥类似于密码，不过有效期更久。</span><span class="sxs-lookup"><span data-stu-id="70e84-127">**Note**: The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="70e84-128">请将密钥值保存在安全的位置以供今后使用。</span><span class="sxs-lookup"><span data-stu-id="70e84-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="70e84-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="70e84-129">Next steps</span></span>
<span data-ttu-id="70e84-130">开始使用[为期 30 天的免费试用版](https://go.microsoft.com/fwlink/?linkid=857895)。</span><span class="sxs-lookup"><span data-stu-id="70e84-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="70e84-131">你需要提供以下详细信息以开始试用：</span><span class="sxs-lookup"><span data-stu-id="70e84-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="70e84-132">合作伙伴中心登录凭据</span><span class="sxs-lookup"><span data-stu-id="70e84-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="70e84-133">商业 ID GUID</span><span class="sxs-lookup"><span data-stu-id="70e84-133">Commerce ID GUID</span></span>
- <span data-ttu-id="70e84-134">应用 ID GUID</span><span class="sxs-lookup"><span data-stu-id="70e84-134">App ID GUID</span></span>
- <span data-ttu-id="70e84-135">应用程序密钥值</span><span class="sxs-lookup"><span data-stu-id="70e84-135">Application secret key value</span></span>
