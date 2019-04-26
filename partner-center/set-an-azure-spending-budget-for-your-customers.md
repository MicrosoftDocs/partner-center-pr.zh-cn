---
title: 为客户设置 Azure 费用预算 | 合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
description: 在合作伙伴中心中，你可以设置每个客户的每月预算，以便在月末他们的 Azure 帐单不会让他们吃惊不已。
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 116fdff7c2a1ca30027dfa29bda5376fa101b089
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133947"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="753f4-103">为你的客户设置 Azure 费用预算</span><span class="sxs-lookup"><span data-stu-id="753f4-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="753f4-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="753f4-104">**Applies to**</span></span>

-  <span data-ttu-id="753f4-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="753f4-105">Partner Center</span></span>
-  <span data-ttu-id="753f4-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="753f4-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="753f4-107">为了帮助客户管理其 Azure 费用，可以设置一个每月费用预算，以使其 Azure 帐单金额不至于超出其预期。</span><span class="sxs-lookup"><span data-stu-id="753f4-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="753f4-108">设置 Azure 费用预算后，你便可以将客户的 Azure 费用与当月的预算进行比较。</span><span class="sxs-lookup"><span data-stu-id="753f4-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="753f4-109">使用此功能，你可以：</span><span class="sxs-lookup"><span data-stu-id="753f4-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="753f4-110">在客户的费用接近预算限制时收到电子邮件通知</span><span class="sxs-lookup"><span data-stu-id="753f4-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="753f4-111">查看客户每月的 Azure 费用预算</span><span class="sxs-lookup"><span data-stu-id="753f4-111">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="753f4-112">发现错误配置的服务或可能表示欺诈的异常使用情况趋势。</span><span class="sxs-lookup"><span data-stu-id="753f4-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="753f4-113">与客户携手合作以辨别根源问题所在并对费用进行管理</span><span class="sxs-lookup"><span data-stu-id="753f4-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="753f4-114">在与客户达成一致的情况下，将预算更改为更高的金额</span><span class="sxs-lookup"><span data-stu-id="753f4-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="753f4-115">Azure 费用数据是估计值，实际计费金额可能会有所不同，并且该值不反映税款、积分、调整或其他可能适用的费用。</span><span class="sxs-lookup"><span data-stu-id="753f4-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="753f4-116">费用数据每天刷新一次。</span><span class="sxs-lookup"><span data-stu-id="753f4-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="753f4-117">除非你在 Azure 门户中更改客户的帐户设置，否则你的客户将继续使用 Azure 服务和资源并需要支付相关费用。</span><span class="sxs-lookup"><span data-stu-id="753f4-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="753f4-118">此功能不可用在沙盒或测试生产 (TIP) 帐户中。</span><span class="sxs-lookup"><span data-stu-id="753f4-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="753f4-119">**启用电子邮件通知**</span><span class="sxs-lookup"><span data-stu-id="753f4-119">**Turn on email notifications**</span></span>
1.  <span data-ttu-id="753f4-120">在合作伙伴中心菜单中，选择**Azure 支出**。</span><span class="sxs-lookup"><span data-stu-id="753f4-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="753f4-121">请启用**获取电子邮件**选项，以便在客户使用了 80% 或更高预算时获取通知。</span><span class="sxs-lookup"><span data-stu-id="753f4-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="753f4-122">这将帮助你关注你的 Azure 帐单。</span><span class="sxs-lookup"><span data-stu-id="753f4-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="753f4-123">你可以将默认电子邮件地址更改为个人或其他任何电子邮件以接收通知。</span><span class="sxs-lookup"><span data-stu-id="753f4-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="753f4-124">**设置在预算**</span><span class="sxs-lookup"><span data-stu-id="753f4-124">**Set a budget**</span></span>
1.  <span data-ttu-id="753f4-125">在合作伙伴中心菜单中，选择**Azure 支出**。</span><span class="sxs-lookup"><span data-stu-id="753f4-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="753f4-126">选择你想要为其设置预算的客户。</span><span class="sxs-lookup"><span data-stu-id="753f4-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="753f4-127">在**每月预算**框中输入值，然后选择**应用**。</span><span class="sxs-lookup"><span data-stu-id="753f4-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="753f4-128">若要查看当前费用，请返回到此页面。</span><span class="sxs-lookup"><span data-stu-id="753f4-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="753f4-129">还可以在客户管理页面上的**基于使用情况的订阅**下设置个别预算。</span><span class="sxs-lookup"><span data-stu-id="753f4-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="753f4-130">**删除在预算**</span><span class="sxs-lookup"><span data-stu-id="753f4-130">**Remove a budget**</span></span>
1.  <span data-ttu-id="753f4-131">在合作伙伴中心菜单中，选择**Azure 支出**。</span><span class="sxs-lookup"><span data-stu-id="753f4-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="753f4-132">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="753f4-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="753f4-133">选择**删除预算**。</span><span class="sxs-lookup"><span data-stu-id="753f4-133">Select **Remove budget**.</span></span>

<span data-ttu-id="753f4-134">**请参阅逐项列出了成本**</span><span class="sxs-lookup"><span data-stu-id="753f4-134">**See itemized costs**</span></span>
1.  <span data-ttu-id="753f4-135">在合作伙伴中心菜单中，选择**客户**。</span><span class="sxs-lookup"><span data-stu-id="753f4-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="753f4-136">从客户列表，选择客户。</span><span class="sxs-lookup"><span data-stu-id="753f4-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="753f4-137">在其客户管理页面上的**基于使用情况的订阅**下，选择某个订阅。</span><span class="sxs-lookup"><span data-stu-id="753f4-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="753f4-138">查看其当前估计的使用情况和按服务明细化的成本列表。</span><span class="sxs-lookup"><span data-stu-id="753f4-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



