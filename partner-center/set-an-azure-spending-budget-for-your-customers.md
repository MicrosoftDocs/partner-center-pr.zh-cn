---
title: 为客户设置 Azure 费用预算 | 合作伙伴中心
ms.topic: article
ms.date: 11/21/2019
description: 为 "合作伙伴中心" 中的每个客户设置每月预算。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 05212746e1ccbcc5081c68ca97ced6a99e20bb8c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384894"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="6f56b-103">为你的客户设置 Azure 费用预算</span><span class="sxs-lookup"><span data-stu-id="6f56b-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="6f56b-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="6f56b-104">Applies to:</span></span>

- <span data-ttu-id="6f56b-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6f56b-105">Partner Center</span></span>
- <span data-ttu-id="6f56b-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6f56b-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6f56b-107">可以在合作伙伴中心[为客户设置每月 Azure 支出预算](#set-azure-spending-budget)。</span><span class="sxs-lookup"><span data-stu-id="6f56b-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="6f56b-108">这可以帮助客户管理其 Azure 支出。</span><span class="sxs-lookup"><span data-stu-id="6f56b-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="6f56b-109">此选项可让你将客户的 Azure 支出与当月的预算进行比较。</span><span class="sxs-lookup"><span data-stu-id="6f56b-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="6f56b-110">它还可帮助客户预算其 Azure 支出，使每月帐单不会超过预期。</span><span class="sxs-lookup"><span data-stu-id="6f56b-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>


> [!NOTE]  
> <span data-ttu-id="6f56b-111">此功能在生产（TIP）帐户中的沙盒或测试中不可用。</span><span class="sxs-lookup"><span data-stu-id="6f56b-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="6f56b-112">[为客户设置 Azure 支出预算](#set-azure-spending-budget)后，还可以通过以下方式查看客户使用情况。</span><span class="sxs-lookup"><span data-stu-id="6f56b-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="6f56b-113">这些选项可帮助你找出配置错误的服务或可能会导致欺诈的异常趋势。</span><span class="sxs-lookup"><span data-stu-id="6f56b-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="6f56b-114">然后，你可以与客户合作来确定根本原因并管理成本。</span><span class="sxs-lookup"><span data-stu-id="6f56b-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="6f56b-115">如果需要，还可以[将客户的预算更改](#set-azure-spending-budget)为较高的金额。</span><span class="sxs-lookup"><span data-stu-id="6f56b-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="6f56b-116">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="6f56b-116">Check current Azure spending</span></span>](#check-current-azure-spending)
- [<span data-ttu-id="6f56b-117">当客户的支出接近预算限制时，打开电子邮件通知</span><span class="sxs-lookup"><span data-stu-id="6f56b-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)
- [<span data-ttu-id="6f56b-118">查看基于使用情况的订阅的按服务列出的费用</span><span class="sxs-lookup"><span data-stu-id="6f56b-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="6f56b-119">你还可以随时删除客户的[Azure 支出预算](#remove-azure-spending-budget)。</span><span class="sxs-lookup"><span data-stu-id="6f56b-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="6f56b-120">Azure 支出数据</span><span class="sxs-lookup"><span data-stu-id="6f56b-120">Azure spending data</span></span>

<span data-ttu-id="6f56b-121">Azure 支出数据是一个*估计值*，*实际计费金额可能会有所不同*。</span><span class="sxs-lookup"><span data-stu-id="6f56b-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="6f56b-122">此数据的值*不会反映*税金、信用额度、调整或可能适用的其他费用。</span><span class="sxs-lookup"><span data-stu-id="6f56b-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="6f56b-123">支出数据*每天刷新一次*。</span><span class="sxs-lookup"><span data-stu-id="6f56b-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="6f56b-124">你的客户可以继续使用 Azure 服务和资源（并向其收费），除非你在 Azure 门户中更改其帐户设置。</span><span class="sxs-lookup"><span data-stu-id="6f56b-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="6f56b-125">设置 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="6f56b-125">Set Azure spending budget</span></span>

<span data-ttu-id="6f56b-126">可以为合作伙伴中心内的多个客户*设置每月 Azure 支出预算*：</span><span class="sxs-lookup"><span data-stu-id="6f56b-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="6f56b-127">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="6f56b-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6f56b-128">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="6f56b-129">在 " **Azure 支出**" 页的 "**具有 Microsoft Azure 订阅的客户**" 下，选择要为其设置预算的客户。</span><span class="sxs-lookup"><span data-stu-id="6f56b-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>
4. <span data-ttu-id="6f56b-130">为 "**月度预算**" 输入一个值。</span><span class="sxs-lookup"><span data-stu-id="6f56b-130">Enter a value for **Monthly budget**.</span></span>
5. <span data-ttu-id="6f56b-131">选择 "**应用**" 保存更改。</span><span class="sxs-lookup"><span data-stu-id="6f56b-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="6f56b-132">你还可以在其订阅设置中*设置单个客户的预算*：</span><span class="sxs-lookup"><span data-stu-id="6f56b-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="6f56b-133">登录到合作伙伴中心仪表板。</span><span class="sxs-lookup"><span data-stu-id="6f56b-133">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="6f56b-134">在**CSP**下的左侧菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="6f56b-135">在 "**客户**" 页上，选择客户的**公司名称**。</span><span class="sxs-lookup"><span data-stu-id="6f56b-135">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="6f56b-136">在客户的 "**订阅**" 页的 "**基于使用情况的订阅**" 下，选择 "**更改预算**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>
5. <span data-ttu-id="6f56b-137">输入预算的值。</span><span class="sxs-lookup"><span data-stu-id="6f56b-137">Enter a value for the budget.</span></span>
6. <span data-ttu-id="6f56b-138">选择 "**应用**" 保存更改。</span><span class="sxs-lookup"><span data-stu-id="6f56b-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="6f56b-139">删除 Azure 支出预算</span><span class="sxs-lookup"><span data-stu-id="6f56b-139">Remove Azure spending budget</span></span>

<span data-ttu-id="6f56b-140">你可以在合作伙伴中心为你的客户*删除每月 Azure 支出预算*：</span><span class="sxs-lookup"><span data-stu-id="6f56b-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="6f56b-141">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="6f56b-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6f56b-142">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="6f56b-143">在 " **Azure 支出**" 页的 "**具有 Microsoft Azure 订阅的客户**" 下，选择要删除其预算的客户。</span><span class="sxs-lookup"><span data-stu-id="6f56b-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>
4. <span data-ttu-id="6f56b-144">选择 "**删除预算**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="6f56b-145">检查当前 Azure 支出</span><span class="sxs-lookup"><span data-stu-id="6f56b-145">Check current Azure spending</span></span>

<span data-ttu-id="6f56b-146">你可以随时*跟踪客户的当前 Azure 支出和月度预算*：</span><span class="sxs-lookup"><span data-stu-id="6f56b-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="6f56b-147">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="6f56b-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="6f56b-148">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="6f56b-149">在 " **Azure 支出**" 页上的 "**具有 Microsoft Azure 订阅的客户**" 下，你可以看到客户的月度预算、当前支出估计和使用的预算百分比的概述。</span><span class="sxs-lookup"><span data-stu-id="6f56b-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="6f56b-150">预算限制的通知</span><span class="sxs-lookup"><span data-stu-id="6f56b-150">Notifications for budget limits</span></span>

<span data-ttu-id="6f56b-151">当你的客户的每月支出接近预算限制时，可以*打开电子邮件通知*。</span><span class="sxs-lookup"><span data-stu-id="6f56b-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="6f56b-152">当你启用此选项时，当客户使用80% 或更多月度预算时，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="6f56b-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="6f56b-153">此选项可帮助你随时了解 Azure 帐单。</span><span class="sxs-lookup"><span data-stu-id="6f56b-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="6f56b-154">配置电子邮件通知：</span><span class="sxs-lookup"><span data-stu-id="6f56b-154">To configure email notifications:</span></span>

1. <span data-ttu-id="6f56b-155">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="6f56b-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6f56b-156">在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="6f56b-157">在 " **Azure 支出**" 页的 "**电子邮件通知**" 下，将 "**获取电子邮件**" 设置切换为 **"开**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>
4. <span data-ttu-id="6f56b-158">选择 "**更改电子邮件地址**" 以查看通知的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6f56b-158">Choose **Change email address** to see the email address for notifications.</span></span>
5. <span data-ttu-id="6f56b-159">如果电子邮件地址*不正确*，请输入正确的电子邮件地址，然后选择 "**更新**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="6f56b-160">如果电子邮件地址*正确*，请选择 "**取消**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="6f56b-161">按服务列出的成本</span><span class="sxs-lookup"><span data-stu-id="6f56b-161">Itemized costs by service</span></span>

<span data-ttu-id="6f56b-162">可以*按服务查看基于使用情况的订阅的详细成本（和估计使用率）* ：</span><span class="sxs-lookup"><span data-stu-id="6f56b-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="6f56b-163">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="6f56b-163">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6f56b-164">在**CSP**下的左侧菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="6f56b-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="6f56b-165">在 "**客户**" 页上，选择客户的**公司名称**。</span><span class="sxs-lookup"><span data-stu-id="6f56b-165">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="6f56b-166">在客户的 "**订阅**" 页的 "**基于使用情况的订阅**" 下，选择**订阅**的名称。</span><span class="sxs-lookup"><span data-stu-id="6f56b-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>
5. <span data-ttu-id="6f56b-167">在订阅页上，你可以查看按服务划分的**详细成本**，以及当月的**预估使用量**。</span><span class="sxs-lookup"><span data-stu-id="6f56b-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
