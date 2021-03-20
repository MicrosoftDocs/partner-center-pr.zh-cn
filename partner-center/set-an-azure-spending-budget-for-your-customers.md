---
title: 为客户设置 Azure 支出预算
ms.topic: how-to
ms.date: 03/17/2021
description: 了解如何为客户设置或删除每月 Azure 支出预算，同时查看 Azure 支出数据并设置与预算相关的通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712743"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="5c822-103">为合作伙伴中心的客户设置、检查或删除每月 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="5c822-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="5c822-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="5c822-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5c822-105">管理员代理</span><span class="sxs-lookup"><span data-stu-id="5c822-105">Admin agent</span></span>

<span data-ttu-id="5c822-106">可以在合作伙伴中心 [为客户设置每月 Azure 支出预算](#set-azure-spending-budget) 。</span><span class="sxs-lookup"><span data-stu-id="5c822-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="5c822-107">这可以帮助客户管理其 Azure 支出。</span><span class="sxs-lookup"><span data-stu-id="5c822-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="5c822-108">此选项可让你将客户的 Azure 支出与当月的预算进行比较。</span><span class="sxs-lookup"><span data-stu-id="5c822-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="5c822-109">它还可帮助你的客户为其 Azure 支出预算，使每月帐单不会超过预期。</span><span class="sxs-lookup"><span data-stu-id="5c822-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="5c822-110">此功能在生产 (TIP) 帐户中不提供沙盒或测试。</span><span class="sxs-lookup"><span data-stu-id="5c822-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="5c822-111">[为客户 () 设置 Azure 支出预算](#set-azure-spending-budget)后，还可以通过以下方式查看客户使用情况。</span><span class="sxs-lookup"><span data-stu-id="5c822-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="5c822-112">这些选项可帮助你找出配置错误的服务或可能会导致欺诈的异常趋势。</span><span class="sxs-lookup"><span data-stu-id="5c822-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="5c822-113">然后，你可以与客户 () ，以确定根本原因并管理成本。</span><span class="sxs-lookup"><span data-stu-id="5c822-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="5c822-114">如果需要，还可以 [将客户的预算更改](#set-azure-spending-budget) 为较高的金额。</span><span class="sxs-lookup"><span data-stu-id="5c822-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="5c822-115">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="5c822-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="5c822-116">当客户的支出接近预算限制时，打开电子邮件通知</span><span class="sxs-lookup"><span data-stu-id="5c822-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="5c822-117">查看基于使用情况的订阅的按服务列出的费用</span><span class="sxs-lookup"><span data-stu-id="5c822-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="5c822-118">你还可以随时删除客户 () 的 [Azure 支出预算](#remove-azure-spending-budget) 。</span><span class="sxs-lookup"><span data-stu-id="5c822-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="5c822-119">Azure 支出数据</span><span class="sxs-lookup"><span data-stu-id="5c822-119">Azure spending data</span></span>

<span data-ttu-id="5c822-120">Azure 支出数据是一个 *估计值* ， *实际计费金额可能会有所不同*。</span><span class="sxs-lookup"><span data-stu-id="5c822-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="5c822-121">此数据的值 *不会反映* 税金、信用额度、调整或可能适用的其他费用。</span><span class="sxs-lookup"><span data-stu-id="5c822-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="5c822-122">支出数据 *每天刷新一次*。</span><span class="sxs-lookup"><span data-stu-id="5c822-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="5c822-123">你的客户可以继续使用 (，并向) Azure 服务和资源收费，除非你在 Azure 门户中更改其帐户设置。</span><span class="sxs-lookup"><span data-stu-id="5c822-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="5c822-124">设置 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="5c822-124">Set Azure spending budget</span></span>

<span data-ttu-id="5c822-125">可以为合作伙伴中心内的多个客户 *设置每月 Azure 支出预算* ：</span><span class="sxs-lookup"><span data-stu-id="5c822-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="5c822-126">登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="5c822-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5c822-127">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="5c822-128">在 " **Azure 支出** " 页的 " **具有 Microsoft Azure 订阅的客户**" 下，选择要为其设置预算的客户 () 。</span><span class="sxs-lookup"><span data-stu-id="5c822-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="5c822-129">为 " **月度预算**" 输入一个值。</span><span class="sxs-lookup"><span data-stu-id="5c822-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="5c822-130">选择 " **应用** " 保存更改。</span><span class="sxs-lookup"><span data-stu-id="5c822-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="5c822-131">你还可以在其订阅设置中 *设置单个客户的预算* ：</span><span class="sxs-lookup"><span data-stu-id="5c822-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="5c822-132">登录到合作伙伴中心面板。</span><span class="sxs-lookup"><span data-stu-id="5c822-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="5c822-133">在 **CSP** 下的左侧菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="5c822-134">在 " **客户** " 页上，选择客户的 **公司名称**。</span><span class="sxs-lookup"><span data-stu-id="5c822-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="5c822-135">在客户的 " **订阅** " 页的 " **基于使用情况的订阅**" 下，选择 " **更改预算**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="5c822-136">输入预算的值。</span><span class="sxs-lookup"><span data-stu-id="5c822-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="5c822-137">选择 " **应用** " 保存更改。</span><span class="sxs-lookup"><span data-stu-id="5c822-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="5c822-138">删除 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="5c822-138">Remove Azure spending budget</span></span>

<span data-ttu-id="5c822-139">可以在合作伙伴中心为客户 () *删除每月 Azure 支出预算* ：</span><span class="sxs-lookup"><span data-stu-id="5c822-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="5c822-140">登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="5c822-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5c822-141">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="5c822-142">在 " **Azure 支出** " 页的 " **具有 Microsoft Azure 订阅的客户**" 下，选择要删除其预算的客户 () 。</span><span class="sxs-lookup"><span data-stu-id="5c822-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="5c822-143">选择 " **删除预算**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="5c822-144">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="5c822-144">Check current Azure spending</span></span>

<span data-ttu-id="5c822-145">你可以随时 *跟踪客户的当前 Azure 支出和月度预算* ：</span><span class="sxs-lookup"><span data-stu-id="5c822-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="5c822-146">登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="5c822-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5c822-147">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="5c822-148">在 " **Azure 支出** " 页上的 " **具有 Microsoft Azure 订阅的客户**" 下，你可以看到客户的月度预算、当前支出估计和使用的预算百分比的概述。</span><span class="sxs-lookup"><span data-stu-id="5c822-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="5c822-149">预算限制的通知</span><span class="sxs-lookup"><span data-stu-id="5c822-149">Notifications for budget limits</span></span>

<span data-ttu-id="5c822-150">当你的客户的每月支出接近预算限制时，可以 *打开电子邮件通知* 。</span><span class="sxs-lookup"><span data-stu-id="5c822-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="5c822-151">当你启用此选项时，当客户使用80% 或更多月度预算时，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="5c822-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="5c822-152">此选项可帮助你随时了解 Azure 帐单。</span><span class="sxs-lookup"><span data-stu-id="5c822-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="5c822-153">配置电子邮件通知：</span><span class="sxs-lookup"><span data-stu-id="5c822-153">To configure email notifications:</span></span>

1. <span data-ttu-id="5c822-154">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="5c822-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="5c822-155">转到“设置”  。</span><span class="sxs-lookup"><span data-stu-id="5c822-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="5c822-156">选择 **"我的首选项"**。</span><span class="sxs-lookup"><span data-stu-id="5c822-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="5c822-157">配置首选电子邮件地址（如果尚未这样做）。</span><span class="sxs-lookup"><span data-stu-id="5c822-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="5c822-158">配置通知的首选语言。</span><span class="sxs-lookup"><span data-stu-id="5c822-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="5c822-159">选择 "**通知首** 选项" 部分下的 " **CSP** "。</span><span class="sxs-lookup"><span data-stu-id="5c822-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="5c822-160">查看 **Azure 支出** 通知的电子邮件选项，并 **保存**。</span><span class="sxs-lookup"><span data-stu-id="5c822-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="5c822-161">按服务列出的成本</span><span class="sxs-lookup"><span data-stu-id="5c822-161">Itemized costs by service</span></span>

<span data-ttu-id="5c822-162">你可以 *查看 (和估计使用情况) 按服务使用基于使用情况的订阅的详细成本*：</span><span class="sxs-lookup"><span data-stu-id="5c822-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="5c822-163">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="5c822-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="5c822-164">在 **CSP** 下的左侧菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="5c822-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="5c822-165">在 " **客户** " 页上，选择客户的 **公司名称**。</span><span class="sxs-lookup"><span data-stu-id="5c822-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="5c822-166">在客户的 " **订阅** " 页的 " **基于使用情况的订阅**" 下，选择 **订阅** 的名称。</span><span class="sxs-lookup"><span data-stu-id="5c822-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="5c822-167">在订阅页上，你可以查看按服务划分的 **详细成本** ，以及当月的 **预估使用量** 。</span><span class="sxs-lookup"><span data-stu-id="5c822-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="5c822-168">后续步骤</span><span class="sxs-lookup"><span data-stu-id="5c822-168">Next steps</span></span>

- [<span data-ttu-id="5c822-169">CSP 中的新商务体验 - Azure 计费</span><span class="sxs-lookup"><span data-stu-id="5c822-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
