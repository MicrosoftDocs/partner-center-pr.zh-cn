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
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855346"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="0d561-103">为合作伙伴中心的客户设置、检查或删除每月 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="0d561-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="0d561-104">**适当的角色**：管理代理</span><span class="sxs-lookup"><span data-stu-id="0d561-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="0d561-105">可以在合作伙伴中心 [为客户设置每月 Azure 支出预算](#set-azure-spending-budget) 。</span><span class="sxs-lookup"><span data-stu-id="0d561-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="0d561-106">这可以帮助客户管理其 Azure 支出。</span><span class="sxs-lookup"><span data-stu-id="0d561-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="0d561-107">此选项可让你将客户的 Azure 支出与当月的预算进行比较。</span><span class="sxs-lookup"><span data-stu-id="0d561-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="0d561-108">它还可帮助你的客户为其 Azure 支出预算，使每月帐单不会超过预期。</span><span class="sxs-lookup"><span data-stu-id="0d561-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="0d561-109">此功能在生产 (TIP) 帐户中不提供沙盒或测试。</span><span class="sxs-lookup"><span data-stu-id="0d561-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="0d561-110">[为客户 () 设置 Azure 支出预算](#set-azure-spending-budget)后，还可以通过以下方式查看客户使用情况。</span><span class="sxs-lookup"><span data-stu-id="0d561-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="0d561-111">这些选项可帮助你找出配置错误的服务或可能会导致欺诈的异常趋势。</span><span class="sxs-lookup"><span data-stu-id="0d561-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="0d561-112">然后，你可以与客户 () ，以确定根本原因并管理成本。</span><span class="sxs-lookup"><span data-stu-id="0d561-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="0d561-113">如果需要，还可以 [将客户的预算更改](#set-azure-spending-budget) 为较高的金额。</span><span class="sxs-lookup"><span data-stu-id="0d561-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="0d561-114">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="0d561-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="0d561-115">当客户的支出接近预算限制时，打开电子邮件通知</span><span class="sxs-lookup"><span data-stu-id="0d561-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="0d561-116">查看基于使用情况的订阅的按服务列出的费用</span><span class="sxs-lookup"><span data-stu-id="0d561-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="0d561-117">你还可以随时删除客户 () 的 [Azure 支出预算](#remove-azure-spending-budget) 。</span><span class="sxs-lookup"><span data-stu-id="0d561-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="0d561-118">Azure 支出数据</span><span class="sxs-lookup"><span data-stu-id="0d561-118">Azure spending data</span></span>

<span data-ttu-id="0d561-119">Azure 支出数据是一个 *估计值* ， *实际计费金额可能会有所不同*。</span><span class="sxs-lookup"><span data-stu-id="0d561-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="0d561-120">此数据的值 *不会反映* 税金、信用额度、调整或可能适用的其他费用。</span><span class="sxs-lookup"><span data-stu-id="0d561-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="0d561-121">支出数据 *每天刷新一次*。</span><span class="sxs-lookup"><span data-stu-id="0d561-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="0d561-122">你的客户可以继续使用 (，并向) Azure 服务和资源收费，除非你在 Azure 门户中更改其帐户设置。</span><span class="sxs-lookup"><span data-stu-id="0d561-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="0d561-123">设置 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="0d561-123">Set Azure spending budget</span></span>

<span data-ttu-id="0d561-124">可以为合作伙伴中心内的多个客户 *设置每月 Azure 支出预算* ：</span><span class="sxs-lookup"><span data-stu-id="0d561-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="0d561-125">登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="0d561-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0d561-126">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="0d561-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0d561-127">在 " **Azure 支出** " 页的 " **具有 Microsoft Azure 订阅的客户**" 下，选择要为其设置预算的客户 () 。</span><span class="sxs-lookup"><span data-stu-id="0d561-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="0d561-128">为 " **月度预算**" 输入一个值。</span><span class="sxs-lookup"><span data-stu-id="0d561-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="0d561-129">选择 " **应用** " 保存更改。</span><span class="sxs-lookup"><span data-stu-id="0d561-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="0d561-130">你还可以在其订阅设置中 *设置单个客户的预算* ：</span><span class="sxs-lookup"><span data-stu-id="0d561-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="0d561-131">登录到合作伙伴中心面板。</span><span class="sxs-lookup"><span data-stu-id="0d561-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="0d561-132">在 **CSP** 下的左侧菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="0d561-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="0d561-133">在 " **客户** " 页上，选择客户的 **公司名称**。</span><span class="sxs-lookup"><span data-stu-id="0d561-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="0d561-134">在客户的 " **订阅** " 页的 " **基于使用情况的订阅**" 下，选择 " **更改预算**"。</span><span class="sxs-lookup"><span data-stu-id="0d561-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="0d561-135">输入预算的值。</span><span class="sxs-lookup"><span data-stu-id="0d561-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="0d561-136">选择 " **应用** " 保存更改。</span><span class="sxs-lookup"><span data-stu-id="0d561-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="0d561-137">删除 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="0d561-137">Remove Azure spending budget</span></span>

<span data-ttu-id="0d561-138">可以在合作伙伴中心为客户 () *删除每月 Azure 支出预算* ：</span><span class="sxs-lookup"><span data-stu-id="0d561-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="0d561-139">登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="0d561-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0d561-140">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="0d561-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0d561-141">在 " **Azure 支出** " 页的 " **具有 Microsoft Azure 订阅的客户**" 下，选择要删除其预算的客户 () 。</span><span class="sxs-lookup"><span data-stu-id="0d561-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="0d561-142">选择 " **删除预算**"。</span><span class="sxs-lookup"><span data-stu-id="0d561-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="0d561-143">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="0d561-143">Check current Azure spending</span></span>

<span data-ttu-id="0d561-144">你可以随时 *跟踪客户的当前 Azure 支出和月度预算* ：</span><span class="sxs-lookup"><span data-stu-id="0d561-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="0d561-145">登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="0d561-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0d561-146">在 CSP 下的左侧菜单中 **，选择\*\*\*\*"Azure 支出"。**</span><span class="sxs-lookup"><span data-stu-id="0d561-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0d561-147">在 **"Azure 支出** " **页上** 的"Microsoft Azure订阅"下，可以看到客户每月预算、当前支出估算和已使用预算百分比的概述。</span><span class="sxs-lookup"><span data-stu-id="0d561-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="0d561-148">预算限制通知</span><span class="sxs-lookup"><span data-stu-id="0d561-148">Notifications for budget limits</span></span>

<span data-ttu-id="0d561-149">当 *客户的每月支出接近其* 预算限制时，可以启用电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="0d561-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="0d561-150">启用此选项时，当客户使用其每月预算 80% 或更多时，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="0d561-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="0d561-151">此选项可帮助你关注 Azure 帐单。</span><span class="sxs-lookup"><span data-stu-id="0d561-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="0d561-152">配置电子邮件通知：</span><span class="sxs-lookup"><span data-stu-id="0d561-152">To configure email notifications:</span></span>

1. <span data-ttu-id="0d561-153">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0d561-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="0d561-154">转到“设置”  。</span><span class="sxs-lookup"><span data-stu-id="0d561-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="0d561-155">选择 **"我的首选项"。**</span><span class="sxs-lookup"><span data-stu-id="0d561-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="0d561-156">配置首选电子邮件地址（如果尚未配置）。</span><span class="sxs-lookup"><span data-stu-id="0d561-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="0d561-157">配置通知的首选语言。</span><span class="sxs-lookup"><span data-stu-id="0d561-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="0d561-158">选择 **"通知** 首选项 **"部分下的"CSP"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="0d561-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="0d561-159">选中"Azure 支出通知"的"**电子邮件**"选项，并"**保存"。**</span><span class="sxs-lookup"><span data-stu-id="0d561-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="0d561-160">按服务分项成本</span><span class="sxs-lookup"><span data-stu-id="0d561-160">Itemized costs by service</span></span>

<span data-ttu-id="0d561-161">可以查看 *基于使用情况的订阅 (按服务) 和估计的使用情况*：</span><span class="sxs-lookup"><span data-stu-id="0d561-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="0d561-162">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="0d561-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="0d561-163">在 CSP 下的左侧菜单中 **，选择"** 客户 **"。**</span><span class="sxs-lookup"><span data-stu-id="0d561-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="0d561-164">在" **客户** "页上，选择客户的公司 **名称**。</span><span class="sxs-lookup"><span data-stu-id="0d561-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="0d561-165">在客户的"订阅 **"** 页上的"基于 **使用情况的订阅"下**，选择"订阅 **"的名称**。</span><span class="sxs-lookup"><span data-stu-id="0d561-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="0d561-166">在订阅的页面上，你可以查看按服务分项成本，以及 **当前月份的估计** 使用量。</span><span class="sxs-lookup"><span data-stu-id="0d561-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="0d561-167">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0d561-167">Next steps</span></span>

- [<span data-ttu-id="0d561-168">CSP 中的新商务体验 - Azure 计费</span><span class="sxs-lookup"><span data-stu-id="0d561-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
