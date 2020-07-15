---
title: 从 Microsoft 请求 SLA 信用额度
ms.topic: article
ms.date: 04/28/2020
description: 如果你的客户遇到服务中断，请了解从 Microsoft 请求服务级别协议（SLA）信用额度的好处、限制和程序。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377751"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a><span data-ttu-id="0d286-103">如何以及何时向 Microsoft 请求服务级别协议（SLA）信用额度</span><span class="sxs-lookup"><span data-stu-id="0d286-103">How and when to request a service-level agreement (SLA) credit from Microsoft</span></span>

<span data-ttu-id="0d286-104">如果你为客户提供的服务中断，你可以从 Microsoft 请求**服务级别协议（SLA）信用额度**。</span><span class="sxs-lookup"><span data-stu-id="0d286-104">You're able to request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.</span></span>

## <a name="sla-credit-calculation"></a><span data-ttu-id="0d286-105">SLA 信用计算</span><span class="sxs-lookup"><span data-stu-id="0d286-105">SLA credit calculation</span></span>

<span data-ttu-id="0d286-106">Microsoft 的 SLA 信用取决于受影响的服务。</span><span class="sxs-lookup"><span data-stu-id="0d286-106">SLA credits from Microsoft are determined based on which service(s) were impacted.</span></span> <span data-ttu-id="0d286-107">例如，如果你的客户有 Office 365 套件但仅经历了 SharePoint 中断，则 SLA 信用仅针对 SharePoint 而不是客户的整个计划。</span><span class="sxs-lookup"><span data-stu-id="0d286-107">For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.</span></span>

<span data-ttu-id="0d286-108">*信用额度基于受影响的服务和中断持续时间进行估价。*</span><span class="sxs-lookup"><span data-stu-id="0d286-108">*Credits are pro-rated based on the service affected and the duration of the outage.*</span></span> <span data-ttu-id="0d286-109">若要查看符合 SLA 信用的方案类型，请参阅[联机服务合并 SLA 文档](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)。</span><span class="sxs-lookup"><span data-stu-id="0d286-109">To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="0d286-110">此信息也适用于通过云解决方案提供商计划出售的服务。</span><span class="sxs-lookup"><span data-stu-id="0d286-110">This information applies to services sold through the Cloud Solution Provider program, too.</span></span>

## <a name="request-an-sla-credit"></a><span data-ttu-id="0d286-111">请求 SLA 信用额度</span><span class="sxs-lookup"><span data-stu-id="0d286-111">Request an SLA credit</span></span>

<span data-ttu-id="0d286-112">*云解决方案提供商（CSP）合作伙伴必须在发生事件的月份后，按日历月结束时间提交声明和所有必需的信息。*</span><span class="sxs-lookup"><span data-stu-id="0d286-112">*The Cloud Solution Provider (CSP) partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.*</span></span> <span data-ttu-id="0d286-113">例如，如果事件在2月15日发生，则 Microsoft 必须在3月31日前收到声明和所有必需的信息。</span><span class="sxs-lookup"><span data-stu-id="0d286-113">For example, if the incident occurred on February 15th, Microsoft must receive the claim and all required information by March 31st.</span></span> <span data-ttu-id="0d286-114">最终客户和间接经销商无法提交 SLA 信用索赔;间接提供商或直接帐单合作伙伴必须代表他们提交声明。</span><span class="sxs-lookup"><span data-stu-id="0d286-114">End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.</span></span>

### <a name="required-information"></a><span data-ttu-id="0d286-115">必需的信息</span><span class="sxs-lookup"><span data-stu-id="0d286-115">Required information</span></span>

<span data-ttu-id="0d286-116">向 Microsoft[提交 SLA 信用请求](#submit-sla-credit-request)之前，必须收集下列信息，以将其包括在支持票证中：</span><span class="sxs-lookup"><span data-stu-id="0d286-116">Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather the following information to include in your support ticket:</span></span>

- <span data-ttu-id="0d286-117">客户租户的 GUID</span><span class="sxs-lookup"><span data-stu-id="0d286-117">The customer tenant's GUID</span></span>
- <span data-ttu-id="0d286-118">[中断事件标识符](#outage-incident-identifier)？</span><span class="sxs-lookup"><span data-stu-id="0d286-118">The [outage incident identifier](#outage-incident-identifier)?</span></span>
- <span data-ttu-id="0d286-119">受影响的订阅是否通过 CSP 购买？</span><span class="sxs-lookup"><span data-stu-id="0d286-119">Were the impacted subscriptions purchased through CSP?</span></span> <span data-ttu-id="0d286-120">（*是*或*否*）</span><span class="sxs-lookup"><span data-stu-id="0d286-120">(*yes* or *no*)</span></span>

#### <a name="outage-incident-identifier"></a><span data-ttu-id="0d286-121">停机事件标识符</span><span class="sxs-lookup"><span data-stu-id="0d286-121">Outage incident identifier</span></span>

<span data-ttu-id="0d286-122">可以在 "**服务运行状况**" 页上的 "Microsoft 365 管理中心" 中找到中断事件的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d286-122">You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="0d286-123">"**中断事件 ID** " 前面有两个字母的缩写，它指示受影响的服务（例如，Exchange Online 中断的*EX25194* ）。</span><span class="sxs-lookup"><span data-stu-id="0d286-123">The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage).</span></span> <span data-ttu-id="0d286-124">下面的表介绍了常见的服务缩写：</span><span class="sxs-lookup"><span data-stu-id="0d286-124">The follow table describes common service abbreviations:</span></span>

| <span data-ttu-id="0d286-125">两字母缩写</span><span class="sxs-lookup"><span data-stu-id="0d286-125">Two-letter abbreviation</span></span> | <span data-ttu-id="0d286-126">Microsoft 服务</span><span class="sxs-lookup"><span data-stu-id="0d286-126">Microsoft service</span></span> |
| ----------------------- | ----------------- |
| <span data-ttu-id="0d286-127">EX</span><span class="sxs-lookup"><span data-stu-id="0d286-127">EX</span></span> | <span data-ttu-id="0d286-128">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="0d286-128">Exchange Online</span></span> |
| <span data-ttu-id="0d286-129">FO</span><span class="sxs-lookup"><span data-stu-id="0d286-129">FO</span></span> | <span data-ttu-id="0d286-130">Exchange Online 保护</span><span class="sxs-lookup"><span data-stu-id="0d286-130">Exchange Online Protection</span></span> |
| <span data-ttu-id="0d286-131">SB</span><span class="sxs-lookup"><span data-stu-id="0d286-131">SB</span></span> | <span data-ttu-id="0d286-132">Skype for Business Online （以前称为 Lync Online）</span><span class="sxs-lookup"><span data-stu-id="0d286-132">Skype for Business Online (formerly Lync Online)</span></span> |
| <span data-ttu-id="0d286-133">OS</span><span class="sxs-lookup"><span data-stu-id="0d286-133">OS</span></span> | <span data-ttu-id="0d286-134">Office 订阅</span><span class="sxs-lookup"><span data-stu-id="0d286-134">Office Subscription</span></span> |
| <span data-ttu-id="0d286-135">PB</span><span class="sxs-lookup"><span data-stu-id="0d286-135">PB</span></span> | <span data-ttu-id="0d286-136">Power BI for Office 365</span><span class="sxs-lookup"><span data-stu-id="0d286-136">Power BI for Office 365</span></span> |
| <span data-ttu-id="0d286-137">SP</span><span class="sxs-lookup"><span data-stu-id="0d286-137">SP</span></span> | <span data-ttu-id="0d286-138">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0d286-138">SharePoint Online</span></span> |
| <span data-ttu-id="0d286-139">4EN-YA-P0U</span><span class="sxs-lookup"><span data-stu-id="0d286-139">YA</span></span> | <span data-ttu-id="0d286-140">Yammer 企业</span><span class="sxs-lookup"><span data-stu-id="0d286-140">Yammer Enterprise</span></span> |
| <span data-ttu-id="0d286-141">MO</span><span class="sxs-lookup"><span data-stu-id="0d286-141">MO</span></span> | <span data-ttu-id="0d286-142">门户错误</span><span class="sxs-lookup"><span data-stu-id="0d286-142">Portal error</span></span> |

### <a name="submit-sla-credit-request"></a><span data-ttu-id="0d286-143">提交 SLA 信用请求</span><span class="sxs-lookup"><span data-stu-id="0d286-143">Submit SLA credit request</span></span>

<span data-ttu-id="0d286-144">若要通过合作伙伴中心仪表板将 SLA 信用请求提交给 Microsoft，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0d286-144">To submit your SLA credit request to Microsoft through the Partner Center dashboard:</span></span>

1. <span data-ttu-id="0d286-145">登录到合作伙伴中心面板。</span><span class="sxs-lookup"><span data-stu-id="0d286-145">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="0d286-146">在左侧菜单中，选择 "**服务请求**"，然后选择 "**合作伙伴支持请求**"。</span><span class="sxs-lookup"><span data-stu-id="0d286-146">In the left-hand menu, choose **Service requests**, then select **Partner support requests**.</span></span>
3. <span data-ttu-id="0d286-147">在 "**合作伙伴请求**" 页上，选择 "**新建请求**"。</span><span class="sxs-lookup"><span data-stu-id="0d286-147">On the **Partner request** page, choose **New request**.</span></span>
4. <span data-ttu-id="0d286-148">在 "**启动请求**" 页上，找到 " **CSP-客户、订单和订阅**" 一节。</span><span class="sxs-lookup"><span data-stu-id="0d286-148">On the **Start the request** page, find the section **CSP - customers, orders and subscriptions**.</span></span> <span data-ttu-id="0d286-149">在此部分中，选择 "**选择问题类型**"，然后选择 "**客户服务信用请求**"。</span><span class="sxs-lookup"><span data-stu-id="0d286-149">In this section, choose **Select an issue type**, then select **Customer services credit requests**.</span></span>
5. <span data-ttu-id="0d286-150">在 "**推荐的解决方案**" 页的 "**是否需要更多帮助？**" 下，选择 **"是"**。</span><span class="sxs-lookup"><span data-stu-id="0d286-150">On the **Recommended solutions** page, under **Do you need more help?**, choose **Yes**.</span></span>
6. <span data-ttu-id="0d286-151">在 "**详细信息**" 页上，填写 "**问题详细信息**" 部分。</span><span class="sxs-lookup"><span data-stu-id="0d286-151">On the **Details** page, fill out the **Issue details** section.</span></span> <span data-ttu-id="0d286-152">在 "**详细信息**" 文本框中，确保输入先前收集的[所需信息](#required-information)。</span><span class="sxs-lookup"><span data-stu-id="0d286-152">In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.</span></span>
7. <span data-ttu-id="0d286-153">选择 "**提交**" 以在 SLA 信用请求中发送。</span><span class="sxs-lookup"><span data-stu-id="0d286-153">Choose **Submit** to send in your SLA credit request.</span></span>
