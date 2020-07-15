---
title: 为客户设置 Azure 支出预算
ms.topic: article
ms.date: 06/03/2020
description: 了解如何为客户设置或删除每月 Azure 支出预算，同时查看 Azure 支出数据并设置与预算相关的通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a52fa8d490ad43cc1e4f331b1a335004a07c83bd
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377731"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="da530-103">为合作伙伴中心的客户设置、检查或删除每月 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="da530-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="da530-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="da530-104">Applies to:</span></span>

- <span data-ttu-id="da530-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="da530-105">Partner Center</span></span>
- <span data-ttu-id="da530-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="da530-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="da530-107">可以在合作伙伴中心[为客户设置每月 Azure 支出预算](#set-azure-spending-budget)。</span><span class="sxs-lookup"><span data-stu-id="da530-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="da530-108">这可以帮助客户管理其 Azure 支出。</span><span class="sxs-lookup"><span data-stu-id="da530-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="da530-109">此选项可让你将客户的 Azure 支出与当月的预算进行比较。</span><span class="sxs-lookup"><span data-stu-id="da530-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="da530-110">它还可帮助你的客户为其 Azure 支出预算，使每月帐单不会超过预期。</span><span class="sxs-lookup"><span data-stu-id="da530-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="da530-111">此功能在生产（TIP）帐户中的沙盒或测试中不可用。</span><span class="sxs-lookup"><span data-stu-id="da530-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="da530-112">[为客户设置 Azure 支出预算](#set-azure-spending-budget)后，还可以通过以下方式查看客户使用情况。</span><span class="sxs-lookup"><span data-stu-id="da530-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="da530-113">这些选项可帮助你找出配置错误的服务或可能会导致欺诈的异常趋势。</span><span class="sxs-lookup"><span data-stu-id="da530-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="da530-114">然后，你可以与客户合作来确定根本原因并管理成本。</span><span class="sxs-lookup"><span data-stu-id="da530-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="da530-115">如果需要，还可以[将客户的预算更改](#set-azure-spending-budget)为较高的金额。</span><span class="sxs-lookup"><span data-stu-id="da530-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="da530-116">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="da530-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="da530-117">当客户的支出接近预算限制时，打开电子邮件通知</span><span class="sxs-lookup"><span data-stu-id="da530-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="da530-118">查看基于使用情况的订阅的按服务列出的费用</span><span class="sxs-lookup"><span data-stu-id="da530-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="da530-119">你还可以随时删除客户的[Azure 支出预算](#remove-azure-spending-budget)。</span><span class="sxs-lookup"><span data-stu-id="da530-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="da530-120">Azure 支出数据</span><span class="sxs-lookup"><span data-stu-id="da530-120">Azure spending data</span></span>

<span data-ttu-id="da530-121">Azure 支出数据是一个*估计值*，*实际计费金额可能会有所不同*。</span><span class="sxs-lookup"><span data-stu-id="da530-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="da530-122">此数据的值*不会反映*税金、信用额度、调整或可能适用的其他费用。</span><span class="sxs-lookup"><span data-stu-id="da530-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="da530-123">支出数据*每天刷新一次*。</span><span class="sxs-lookup"><span data-stu-id="da530-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="da530-124">你的客户可以继续使用 Azure 服务和资源（并向其收费），除非你在 Azure 门户中更改其帐户设置。</span><span class="sxs-lookup"><span data-stu-id="da530-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="da530-125">设置 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="da530-125">Set Azure spending budget</span></span>

<span data-ttu-id="da530-126">可以为合作伙伴中心内的多个客户*设置每月 Azure 支出预算*：</span><span class="sxs-lookup"><span data-stu-id="da530-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="da530-127">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="da530-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="da530-128">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="da530-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da530-129">在 " **Azure 支出**" 页的 "**具有 Microsoft Azure 订阅的客户**" 下，选择要为其设置预算的客户。</span><span class="sxs-lookup"><span data-stu-id="da530-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="da530-130">为 "**月度预算**" 输入一个值。</span><span class="sxs-lookup"><span data-stu-id="da530-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="da530-131">选择 "**应用**" 保存更改。</span><span class="sxs-lookup"><span data-stu-id="da530-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="da530-132">你还可以在其订阅设置中*设置单个客户的预算*：</span><span class="sxs-lookup"><span data-stu-id="da530-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="da530-133">登录到合作伙伴中心面板。</span><span class="sxs-lookup"><span data-stu-id="da530-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="da530-134">在**CSP**下的左侧菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="da530-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="da530-135">在 "**客户**" 页上，选择客户的**公司名称**。</span><span class="sxs-lookup"><span data-stu-id="da530-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="da530-136">在客户的 "**订阅**" 页的 "**基于使用情况的订阅**" 下，选择 "**更改预算**"。</span><span class="sxs-lookup"><span data-stu-id="da530-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="da530-137">输入预算的值。</span><span class="sxs-lookup"><span data-stu-id="da530-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="da530-138">选择 "**应用**" 保存更改。</span><span class="sxs-lookup"><span data-stu-id="da530-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="da530-139">删除 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="da530-139">Remove Azure spending budget</span></span>

<span data-ttu-id="da530-140">你可以在合作伙伴中心为你的客户*删除每月 Azure 支出预算*：</span><span class="sxs-lookup"><span data-stu-id="da530-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="da530-141">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="da530-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="da530-142">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="da530-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da530-143">在 " **Azure 支出**" 页的 "**具有 Microsoft Azure 订阅的客户**" 下，选择要删除其预算的客户。</span><span class="sxs-lookup"><span data-stu-id="da530-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="da530-144">选择 "**删除预算**"。</span><span class="sxs-lookup"><span data-stu-id="da530-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="da530-145">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="da530-145">Check current Azure spending</span></span>

<span data-ttu-id="da530-146">你可以随时*跟踪客户的当前 Azure 支出和月度预算*：</span><span class="sxs-lookup"><span data-stu-id="da530-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="da530-147">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="da530-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="da530-148">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="da530-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da530-149">在 " **Azure 支出**" 页上的 "**具有 Microsoft Azure 订阅的客户**" 下，你可以看到客户的月度预算、当前支出估计和使用的预算百分比的概述。</span><span class="sxs-lookup"><span data-stu-id="da530-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="da530-150">预算限制的通知</span><span class="sxs-lookup"><span data-stu-id="da530-150">Notifications for budget limits</span></span>

<span data-ttu-id="da530-151">当你的客户的每月支出接近预算限制时，可以*打开电子邮件通知*。</span><span class="sxs-lookup"><span data-stu-id="da530-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="da530-152">当你启用此选项时，当客户使用80% 或更多月度预算时，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="da530-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="da530-153">此选项可帮助你随时了解 Azure 帐单。</span><span class="sxs-lookup"><span data-stu-id="da530-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="da530-154">配置电子邮件通知：</span><span class="sxs-lookup"><span data-stu-id="da530-154">To configure email notifications:</span></span>

1. <span data-ttu-id="da530-155">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="da530-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="da530-156">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="da530-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da530-157">在 " **Azure 支出**" 页的 "**电子邮件通知**" 下，将 "**获取电子邮件**" 设置切换为 **"开**"。</span><span class="sxs-lookup"><span data-stu-id="da530-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>

4. <span data-ttu-id="da530-158">选择 "**更改电子邮件地址**" 以查看通知的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="da530-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="da530-159">如果电子邮件地址*不正确*，请输入正确的电子邮件地址，然后选择 "**更新**"。</span><span class="sxs-lookup"><span data-stu-id="da530-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="da530-160">如果电子邮件地址*正确*，请选择 "**取消**"。</span><span class="sxs-lookup"><span data-stu-id="da530-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="da530-161">按服务列出的成本</span><span class="sxs-lookup"><span data-stu-id="da530-161">Itemized costs by service</span></span>

<span data-ttu-id="da530-162">可以*按服务查看基于使用情况的订阅的详细成本（和估计使用率）*：</span><span class="sxs-lookup"><span data-stu-id="da530-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="da530-163">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="da530-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="da530-164">在**CSP**下的左侧菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="da530-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="da530-165">在 "**客户**" 页上，选择客户的**公司名称**。</span><span class="sxs-lookup"><span data-stu-id="da530-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="da530-166">在客户的 "**订阅**" 页的 "**基于使用情况的订阅**" 下，选择**订阅**的名称。</span><span class="sxs-lookup"><span data-stu-id="da530-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="da530-167">在订阅页上，你可以查看按服务划分的**详细成本**，以及当月的**预估使用量**。</span><span class="sxs-lookup"><span data-stu-id="da530-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
