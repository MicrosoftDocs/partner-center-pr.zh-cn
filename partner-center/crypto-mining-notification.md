---
title: 加密挖掘活动的通知
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解在一个或多个 Azure 订阅上出现有关潜在的加密货币挖掘（或加密挖掘）的通知时，这意味着什么。
author: aarzh-AaronZhang
ms.author: v-aarzh
robots: noindex, nofollow
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05da3ae93a43b1e9977d5b6646a73750b30b4415
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943494"
---
# <a name="partner-center-notification-for-cryptocurrency-mining-activity"></a><span data-ttu-id="93411-103">加密货币挖掘活动的合作伙伴中心通知</span><span class="sxs-lookup"><span data-stu-id="93411-103">Partner Center notification for cryptocurrency mining activity</span></span>

<span data-ttu-id="93411-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="93411-104">**Applies to**</span></span>

-  <span data-ttu-id="93411-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="93411-105">Partner Center</span></span>
-  <span data-ttu-id="93411-106">云解决方案提供商合作伙伴</span><span class="sxs-lookup"><span data-stu-id="93411-106">CSP partners</span></span>

<span data-ttu-id="93411-107">你可能已收到有关加密货币挖掘的以下合作伙伴中心通知：</span><span class="sxs-lookup"><span data-stu-id="93411-107">You may have received the following Partner Center notification about cryptocurrency mining:</span></span>

:::image type="content" source="images/crypto1.png" alt-text="合作伙伴中心的安全通知图像":::

<span data-ttu-id="93411-109">此通知的目的是通知你我们在过去一周内检测到针对一个或多个 Azure 订阅的加密货币挖掘活动。</span><span class="sxs-lookup"><span data-stu-id="93411-109">The purpose of this notification is to inform you that we've detected cryptocurrency mining on one or more of your Azure subscriptions within the past week.</span></span> <span data-ttu-id="93411-110">加密货币挖掘不一定是欺诈活动。</span><span class="sxs-lookup"><span data-stu-id="93411-110">Cryptocurrency mining does not necessarily equal fraudulent activity.</span></span> <span data-ttu-id="93411-111">然而，这是不同寻常的活动，因为在 Azure 中运行加密货币挖掘的成本往往超过了任何潜在的经济回报。</span><span class="sxs-lookup"><span data-stu-id="93411-111">However, it's unusual because the cost of running cryptocurrency mining in Azure tends to outweigh any potential financial rewards.</span></span>

## <a name="checklist"></a><span data-ttu-id="93411-112">清单</span><span class="sxs-lookup"><span data-stu-id="93411-112">Checklist</span></span>

<span data-ttu-id="93411-113">为防止可能影响你或你的客户的财务欺诈，请考虑执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="93411-113">To protect against financial fraud that may impact you or your customer, consider the following steps:</span></span>

1. <span data-ttu-id="93411-114">查看并确认客户帐户信誉良好。</span><span class="sxs-lookup"><span data-stu-id="93411-114">Review and confirm that the customer account is in good standing.</span></span> <span data-ttu-id="93411-115">你可以通过单击通知直接访问订阅。</span><span class="sxs-lookup"><span data-stu-id="93411-115">You can access the subscription directly by clicking on the notification.</span></span>

2. <span data-ttu-id="93411-116">查看订阅的 Azure 使用模式。</span><span class="sxs-lookup"><span data-stu-id="93411-116">Review Azure usage patterns for the subscription.</span></span> <span data-ttu-id="93411-117">突然激增可能暗示有异常活动。</span><span class="sxs-lookup"><span data-stu-id="93411-117">Sudden spikes may suggest unexpected activity.</span></span>

3. <span data-ttu-id="93411-118">联系客户以确认活动为预期活动。</span><span class="sxs-lookup"><span data-stu-id="93411-118">Contact the customer to confirm that the activity is expected.</span></span>

   <span data-ttu-id="93411-119">如果是预期活动，请返回到客户的 Azure 订阅详细信息页面，然后确认加密货币挖掘是合法的。</span><span class="sxs-lookup"><span data-stu-id="93411-119">If the activity is expected, return to the customer's Azure subscription detail page and confirm that the cryptocurrency mining is legitimate.</span></span>

   :::image type="content" source="images/crypto2.png" alt-text="客户的 Azure 订阅详细信息页的图像":::

## <a name="steps-for-unexpected-activity"></a><span data-ttu-id="93411-121">意外活动的步骤</span><span class="sxs-lookup"><span data-stu-id="93411-121">Steps for unexpected activity</span></span>

<span data-ttu-id="93411-122">如果是异常活动，请考虑以下各项：</span><span class="sxs-lookup"><span data-stu-id="93411-122">If the activity is unexpected, consider the following:</span></span>

1. <span data-ttu-id="93411-123">确认不需要加密货币挖掘的 Azure 资源并删除它们以避免产生其他 Azure 费用。</span><span class="sxs-lookup"><span data-stu-id="93411-123">Confirm that the Azure resources for cryptocurrency mining are not needed and delete them to avoid further Azure charges.</span></span>

2. <span data-ttu-id="93411-124">首先了解如何创建资源。</span><span class="sxs-lookup"><span data-stu-id="93411-124">Understand how the resources were created in the first place.</span></span> <span data-ttu-id="93411-125">这可能要求你查看 Azure 资源管理日志以了解资源预配活动。</span><span class="sxs-lookup"><span data-stu-id="93411-125">This may require you to review the Azure Resource Management logs for resource provisioning activities.</span></span>

3. <span data-ttu-id="93411-126">如果需要找出创建订阅的人员，请查看合作伙伴中心活动日志。</span><span class="sxs-lookup"><span data-stu-id="93411-126">If you need to find out who created the subscription, review Partner Center activity logs.</span></span>

<span data-ttu-id="93411-127">加密货币挖掘活动的检测基于试探法，可能不是 100% 准确。</span><span class="sxs-lookup"><span data-stu-id="93411-127">Detection of cryptocurrency mining activities is based on heuristics and may not be 100% accurate.</span></span> <span data-ttu-id="93411-128">请确保部署管理和监控系统，以防止欺诈或其他不允许的活动。</span><span class="sxs-lookup"><span data-stu-id="93411-128">Be sure to have governance and monitoring systems in place to protect against fraudulent or other unpermitted activities.</span></span> <span data-ttu-id="93411-129">有关详细信息，请参阅[拒不付款、欺诈或滥用](non-payment--fraud--or-misuse.md)。</span><span class="sxs-lookup"><span data-stu-id="93411-129">For more information, see [Non-payment, fraud, or misuse](non-payment--fraud--or-misuse.md).</span></span>

## <a name="contact-support-if-needed"></a><span data-ttu-id="93411-130">如果需要，请联系支持人员</span><span class="sxs-lookup"><span data-stu-id="93411-130">Contact support if needed</span></span>

<span data-ttu-id="93411-131">如果对通知有任何疑问或疑虑，你可以使用以下步骤打开支持请求。</span><span class="sxs-lookup"><span data-stu-id="93411-131">If you have questions or concerns about the notification, you can use the following procedure to open a support request.</span></span>

1. <span data-ttu-id="93411-132">在合作伙伴中心中，选择 "**支持**"，然后选择 "**合作伙伴中心请求**"。</span><span class="sxs-lookup"><span data-stu-id="93411-132">In the Partner Center, select **Support** and then select **Partner Center requests**.</span></span>

2. <span data-ttu-id="93411-133">选择 "**新建请求**"。</span><span class="sxs-lookup"><span data-stu-id="93411-133">Select **New Request**.</span></span> 

3. <span data-ttu-id="93411-134">在**问题类型**下拉菜单中，选择**添加或管理客户**。</span><span class="sxs-lookup"><span data-stu-id="93411-134">In the **Type of problems** dropdown menu, select **Adding or managing customers**.</span></span>

4. <span data-ttu-id="93411-135">在**影响**下拉菜单中，选择**中等**。</span><span class="sxs-lookup"><span data-stu-id="93411-135">In the **Impact** dropdown menu, select **Moderate**.</span></span>

5. <span data-ttu-id="93411-136">在**标题**字段中，输入**加密挖掘通知**。</span><span class="sxs-lookup"><span data-stu-id="93411-136">In the **Title** field, enter **Crypto-mining notification**.</span></span>

6. <span data-ttu-id="93411-137">在**描述**字段中，输入受影响订阅的名称以及其他问题或疑虑。</span><span class="sxs-lookup"><span data-stu-id="93411-137">In the **Description** field, enter the name of the affected subscription along with your other questions or concerns.</span></span>

7. <span data-ttu-id="93411-138">输入联系信息。</span><span class="sxs-lookup"><span data-stu-id="93411-138">Enter your contact information.</span></span>

8. <span data-ttu-id="93411-139">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="93411-139">Select **Submit**.</span></span>
