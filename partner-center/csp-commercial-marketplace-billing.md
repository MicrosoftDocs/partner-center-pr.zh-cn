---
title: 商业应用商店产品的帐单
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何针对从合作伙伴中心内的商业市场为客户购买的 ISV SaaS 产品或订阅付费。
author: LauraBrenner
ms.author: labrenne
keywords: 订阅，产品，购买，Marketplace，第三方，ISV，计费，发票，协调，侦测文件
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9672850b699a2660f646ede5250e52298f5522cd
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394158"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a><span data-ttu-id="a1666-104">适用于合作伙伴中心的商业 marketplace 产品和订阅的帐单</span><span class="sxs-lookup"><span data-stu-id="a1666-104">Billing for commercial marketplace products and subscriptions in Partner Center</span></span>

<span data-ttu-id="a1666-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="a1666-105">**Applies to**</span></span>

- <span data-ttu-id="a1666-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="a1666-106">Partner Center</span></span>
- <span data-ttu-id="a1666-107">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="a1666-107">Partners in the CSP program</span></span>

<span data-ttu-id="a1666-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="a1666-108">**Appropriate roles**</span></span>

- <span data-ttu-id="a1666-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a1666-109">Global admin</span></span>
- <span data-ttu-id="a1666-110">计费管理员</span><span class="sxs-lookup"><span data-stu-id="a1666-110">Billing admin</span></span>

<span data-ttu-id="a1666-111">作为 CSP 计划中的合作伙伴，你可以使用合作伙伴中心从商业应用商店中的 ISV 出版商那里购买基于许可证的 SaaS 产品。</span><span class="sxs-lookup"><span data-stu-id="a1666-111">As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace.</span></span> <span data-ttu-id="a1666-112">完成此操作后，你可以访问这些类型采购的帐单。</span><span class="sxs-lookup"><span data-stu-id="a1666-112">After you do so, you can access a bill for these types of purchases.</span></span> <span data-ttu-id="a1666-113">计费周期从日历月的第一天开始，到日历月的最后一天结束。</span><span class="sxs-lookup"><span data-stu-id="a1666-113">The billing period starts on the first day of the calendar month and ends on the last day of the calendar month.</span></span> <span data-ttu-id="a1666-114">发票在下个月的第8天可用。</span><span class="sxs-lookup"><span data-stu-id="a1666-114">Invoices are made available on the 8th day of the following month.</span></span>

<span data-ttu-id="a1666-115">你可以通过合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/)或使用[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/)访问发票。</span><span class="sxs-lookup"><span data-stu-id="a1666-115">You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="a1666-116">CSP 计划中的合作伙伴需要为客户购买的 ISV 商用 marketplace 解决方案收费，当他们从合作伙伴中心或从 Azure 门户购买这些产品（使用客户以前的 CSP 购买的 Azure 租户）。</span><span class="sxs-lookup"><span data-stu-id="a1666-116">Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).</span></span>

>[!NOTE]
><span data-ttu-id="a1666-117">如果客户使用其自己的 Azure AD 租户（不是从 CSP 计划中的合作伙伴购买的租户），则客户还可以选择直接从（[Microsoft AppSource](https://appsource.microsoft.com/)或[Azure Marketplace](https://azuremarketplace.microsoft.com/)）购买自己的 ISV SaaS 解决方案。</span><span class="sxs-lookup"><span data-stu-id="a1666-117">If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)).</span></span> <span data-ttu-id="a1666-118">如果他们这样做，他们将直接从 Microsoft 接收自己的帐单。</span><span class="sxs-lookup"><span data-stu-id="a1666-118">If they do so, they will receive their own bill directly from Microsoft.</span></span> <span data-ttu-id="a1666-119">同样，如果 CSP 计划中的合作伙伴向客户销售 Azure 订阅或新的 Azure 计划，并向客户（或间接经销商）授予对该租户的[基于角色的访问权限](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)（向除**读者**以外的客户分配任何角色），则该客户（或间接经销商）还可以购买商业 marketplace 产品/服务，而不需要事先批准或通知 CSP 合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="a1666-119">Likewise, if a partner in the CSP program sells an Azure subscription or the new Azure plan to the customer and grants the customer (or indirect reseller) [role-based access](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer (or indirect reseller) can also purchase commercial marketplace offers without prior approval or notification to the CSP partner.</span></span> <span data-ttu-id="a1666-120">在这种情况下，Microsoft 不会直接在 CSP 计划中向合作伙伴通知客户的购买情况。</span><span class="sxs-lookup"><span data-stu-id="a1666-120">In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers.</span></span> <span data-ttu-id="a1666-121">但是，Microsoft 提供了一个可选的[Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)机制，可用于设置有关 Azure 订阅上的活动的警报或通知。</span><span class="sxs-lookup"><span data-stu-id="a1666-121">However, Microsoft does offer an optional [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.</span></span>

## <a name="access-billing-information-for-commercial-marketplace-products"></a><span data-ttu-id="a1666-122">访问商业 marketplace 产品的计费信息</span><span class="sxs-lookup"><span data-stu-id="a1666-122">Access billing information for commercial marketplace products</span></span>

<span data-ttu-id="a1666-123">当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a1666-123">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> <span data-ttu-id="a1666-124">若要访问商业 marketplace 产品购买的最新发票和对帐文件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a1666-124">To access the latest invoice and reconciliation file for commercial marketplace product purchases:</span></span>

1. <span data-ttu-id="a1666-125">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="a1666-125">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="a1666-126">在“合作伙伴中心”菜单中，选择“计费”。 </span><span class="sxs-lookup"><span data-stu-id="a1666-126">From the Partner Center menu, select **Billing**.</span></span> 

    <span data-ttu-id="a1666-127">你将在帐单页的顶部看到两个选项卡：**定期**、**定期和一次性购买**。</span><span class="sxs-lookup"><span data-stu-id="a1666-127">You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**.</span></span> <span data-ttu-id="a1666-128">每个选项卡允许您访问不同 marketplace 产品的发票和对帐（侦测）文件：</span><span class="sxs-lookup"><span data-stu-id="a1666-128">Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:</span></span>

    - <span data-ttu-id="a1666-129">"**定期**" 选项卡：显示与 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、PowerBI Pro 和 Microsoft Azure 相关的订阅的发票和对帐文件。</span><span class="sxs-lookup"><span data-stu-id="a1666-129">**Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro, and Microsoft Azure.</span></span>

    - <span data-ttu-id="a1666-130">**定期和一次性购买**选项卡：显示 azure 计划、azure 预订、软件和商业应用商店产品的发票和对帐文件。</span><span class="sxs-lookup"><span data-stu-id="a1666-130">**Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.</span></span>
  
3. <span data-ttu-id="a1666-131">选择 "**定期购买" 和 "一次性购买**" 选项卡。如果为客户购买了不同货币的订阅，则会看到每个货币的选项卡。</span><span class="sxs-lookup"><span data-stu-id="a1666-131">Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency.</span></span> <span data-ttu-id="a1666-132">你可以执行以下操作： om 此页：</span><span class="sxs-lookup"><span data-stu-id="a1666-132">You can do a few things fr:om this page:</span></span>

    - <span data-ttu-id="a1666-133">若要查看最新的发票和协调文件，请选择 "**发票**" 或 "**对帐文件**"。</span><span class="sxs-lookup"><span data-stu-id="a1666-133">To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**.</span></span> <span data-ttu-id="a1666-134">（如果需要，还可以使用[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/)访问最新的发票和侦测文件数据。</span><span class="sxs-lookup"><span data-stu-id="a1666-134">(If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

    - <span data-ttu-id="a1666-135">若要查看以前的发票和侦测文件，请展开下面的 "**帐单历史记录**" 行。</span><span class="sxs-lookup"><span data-stu-id="a1666-135">To see earlier invoices and recon files, expand the **Billing history** row below.</span></span>

    - <span data-ttu-id="a1666-136">若要根据最新的帐户活动，随时查看估计的帐户余额或帐单，请在 "**估计**" 标题下选择一个链接。</span><span class="sxs-lookup"><span data-stu-id="a1666-136">To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.</span></span>  

    >[!NOTE]
    > <span data-ttu-id="a1666-137">当我们在每月的第8天发布帐单时，它将包含税金以及任何其他适用的费用和信用额度。</span><span class="sxs-lookup"><span data-stu-id="a1666-137">When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits.</span></span> <span data-ttu-id="a1666-138">这意味着最终的应付金额可能不同于计费期间的显示内容。</span><span class="sxs-lookup"><span data-stu-id="a1666-138">This means the final amount due might differ from what you see during the billing period.</span></span>

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a><span data-ttu-id="a1666-139">有关商业 marketplace 产品的发票和侦测文件的详细信息</span><span class="sxs-lookup"><span data-stu-id="a1666-139">More about invoices and recon files for commercial marketplace products</span></span>

<span data-ttu-id="a1666-140">本部分提供了有关为第三方 ISV 发布者购买的商业 marketplace SaaS 订阅的发票和对帐文件的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1666-140">This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.</span></span>

<span data-ttu-id="a1666-141">当你从 "合作伙伴中心" 菜单中的 "**计费**" 选项中选择 "**定期购买" 和 "一次性购买**" 时，你将获得对与 Microsoft （第一方）和 ISV （第三方）购买相关的费用的发票和协调文件的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a1666-141">When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases.</span></span> <span data-ttu-id="a1666-142">这些购买可能会与相关联：</span><span class="sxs-lookup"><span data-stu-id="a1666-142">These purchases may be associated with:</span></span>

- <span data-ttu-id="a1666-143">SaaS 订阅（来自 Microsoft 或 ISV 发布者）</span><span class="sxs-lookup"><span data-stu-id="a1666-143">SaaS subscriptions (from either Microsoft or ISV publishers)</span></span>

- <span data-ttu-id="a1666-144">Azure 计划</span><span class="sxs-lookup"><span data-stu-id="a1666-144">Azure plan</span></span>

- <span data-ttu-id="a1666-145">Azure 预订</span><span class="sxs-lookup"><span data-stu-id="a1666-145">Azure reservations</span></span>

- <span data-ttu-id="a1666-146">其他基于订阅的软件（来自 Microsoft 或 ISV 发布者）</span><span class="sxs-lookup"><span data-stu-id="a1666-146">Other subscription-based software (from either Microsoft or ISV publishers)</span></span>

<span data-ttu-id="a1666-147">这些购买的示例可能包括 SUSE Linux 软件（软件订阅）或 Azure ISV SaaS 产品订阅。</span><span class="sxs-lookup"><span data-stu-id="a1666-147">Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.</span></span>

>[!NOTE]
> <span data-ttu-id="a1666-148">有关如何读取发票和侦测文件的详细信息，请参阅[帐单概述](billing.md)。</span><span class="sxs-lookup"><span data-stu-id="a1666-148">For more information about how to read invoice and recon files, see also [Billing overview](billing.md).</span></span>

### <a name="tips-on-reading-your-invoice"></a><span data-ttu-id="a1666-149">阅读发票提示</span><span class="sxs-lookup"><span data-stu-id="a1666-149">Tips on reading your invoice</span></span>

<span data-ttu-id="a1666-150">从第三方 ISV 发布商处购买基于许可证的 SaaS 产品时，你只会看到发票上的许可费用收费。</span><span class="sxs-lookup"><span data-stu-id="a1666-150">When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice.</span></span> <span data-ttu-id="a1666-151">即使 ISV 的 SaaS 产品使用（或使用）底层 Azure 基础结构资源，也是如此。</span><span class="sxs-lookup"><span data-stu-id="a1666-151">This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources.</span></span> <span data-ttu-id="a1666-152">这是因为，对 isv 的 SaaS 产品的客户的 Azure 基础结构用量收费直接向 ISV 收费。</span><span class="sxs-lookup"><span data-stu-id="a1666-152">That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV.</span></span> <span data-ttu-id="a1666-153">（Isv 会在其自己的 Azure 使用情况-每日级别的发票对帐文件中看到关联的 Azure 消耗收费。）</span><span class="sxs-lookup"><span data-stu-id="a1666-153">(ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)</span></span>

<span data-ttu-id="a1666-154">你的发票将包含多个页面：</span><span class="sxs-lookup"><span data-stu-id="a1666-154">Your invoice will contain several pages:</span></span>

- <span data-ttu-id="a1666-155">**发票第1页：** 包含 CSP 计划合作伙伴的计费详细信息的摘要概述。</span><span class="sxs-lookup"><span data-stu-id="a1666-155">**Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details.</span></span> <span data-ttu-id="a1666-156">这包括计费周期的费用摘要、发票编号、支付条款（净60天）以及通过线路或支票支付的帐单支付方法。</span><span class="sxs-lookup"><span data-stu-id="a1666-156">This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.</span></span>

- <span data-ttu-id="a1666-157">**发票的第2页（以及所有后续页面）：** 从商业性 marketplace 购买第一方 Microsoft 购买和第三方 ISV （基于许可证）的费用。</span><span class="sxs-lookup"><span data-stu-id="a1666-157">**Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace.</span></span> <span data-ttu-id="a1666-158">可以通过每个产品名称下的**发布者**行标识基于 ISV 许可证的购买。</span><span class="sxs-lookup"><span data-stu-id="a1666-158">You can identify ISV license-based purchases by the **Publisher** line beneath each product name.</span></span> <span data-ttu-id="a1666-159">关联的对帐文件为特定发票费用提供更多计费详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1666-159">The associated reconciliation file offers more billing details for specific invoice charges.</span></span>

- <span data-ttu-id="a1666-160">**发票的最后一页：** 如果你使用 ISV 提供的基于许可证的 marketplace 产品收费，此最后一页将显示有关 ISV 发布者的姓名和地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1666-160">**Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.</span></span>

### <a name="tips-on-reading-your-reconciliation-file"></a><span data-ttu-id="a1666-161">有关读取对帐文件的提示</span><span class="sxs-lookup"><span data-stu-id="a1666-161">Tips on reading your reconciliation file</span></span>

<span data-ttu-id="a1666-162">**定期和一次性采购**对帐文件包含多个列，其中包含映射到发票中的费用的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1666-162">The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice.</span></span> <span data-ttu-id="a1666-163">**PublisherName**列显示购买是来自 Microsoft 还是第三方 ISV 发布者。</span><span class="sxs-lookup"><span data-stu-id="a1666-163">The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.</span></span>

<span data-ttu-id="a1666-164">对帐文件的某些费用可能会显示为 $0。</span><span class="sxs-lookup"><span data-stu-id="a1666-164">Some charges in your reconciliation file may appear with a cost of $0.</span></span> <span data-ttu-id="a1666-165">这可能是由于 ISV "免费试用版" 产品/服务（通常为30或60天）或自带许可提供。</span><span class="sxs-lookup"><span data-stu-id="a1666-165">This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.</span></span>

<span data-ttu-id="a1666-166">对于免费试用版 ISV，请提供：</span><span class="sxs-lookup"><span data-stu-id="a1666-166">In the case of free trial ISV offers:</span></span>

- <span data-ttu-id="a1666-167">免费试用期涵盖了在此期间 ISV 基于许可证的 SaaS 产品的成本。</span><span class="sxs-lookup"><span data-stu-id="a1666-167">The free trial period covers the cost of the ISV's license-based SaaS product during that time.</span></span> <span data-ttu-id="a1666-168">对于关联的 Azure 基础结构使用该 SaaS 产品，还不会向你收费。</span><span class="sxs-lookup"><span data-stu-id="a1666-168">You will also not be charged for associated Azure infrastructure use of that SaaS product.</span></span>  <span data-ttu-id="a1666-169">但是，如果使用基于使用情况的 ISV 产品/服务，则免费试用版不包括基础 Azure 基础结构的使用成本。</span><span class="sxs-lookup"><span data-stu-id="a1666-169">If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage.</span></span> <span data-ttu-id="a1666-170">在这种情况下，Azure 基础结构使用费用将显示在单独的 Azure 对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="a1666-170">In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.</span></span>

- <span data-ttu-id="a1666-171">当你为客户购买并部署 ISV 的免费试用版产品时，客户将自动注册到 ISV 发布者的免费试用版。</span><span class="sxs-lookup"><span data-stu-id="a1666-171">When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher.</span></span> <span data-ttu-id="a1666-172">免费试用期将在 ISV 发布者定义的时间段后自动结束。</span><span class="sxs-lookup"><span data-stu-id="a1666-172">The free trial period ends automatically after the period defined by the ISV publisher.</span></span> <span data-ttu-id="a1666-173">该时间段结束后，将向客户收费。</span><span class="sxs-lookup"><span data-stu-id="a1666-173">After the period ends, the customer will be charged.</span></span> <span data-ttu-id="a1666-174">这意味着，对等认证的产品可能会显示两行：一个跟踪试用期的行和一个跟踪付费产品/服务的行（在试用期结束之前，将显示成本为 $0）。</span><span class="sxs-lookup"><span data-stu-id="a1666-174">This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends).</span></span> <span data-ttu-id="a1666-175">试用期结束后，显示付费产品/服务的行将开始显示费用。</span><span class="sxs-lookup"><span data-stu-id="a1666-175">Once the trial ends, the row showing the paid offer will start to show charges.</span></span> 

<span data-ttu-id="a1666-176">有关每个列代表的内容的详细信息，请参阅[使用对帐文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="a1666-176">For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md).</span></span> <span data-ttu-id="a1666-177">另请参阅[合作伙伴中心的计费类型](billing-different-types.md)</span><span class="sxs-lookup"><span data-stu-id="a1666-177">See also [Types of billing in Partner Center](billing-different-types.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="a1666-178">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a1666-178">Next steps</span></span>

- [<span data-ttu-id="a1666-179">为客户管理商业 marketplace 产品</span><span class="sxs-lookup"><span data-stu-id="a1666-179">Manage commercial marketplace products for customers</span></span>](csp-commercial-marketplace-manage.md)
- [<span data-ttu-id="a1666-180">了解对商业 marketplace 产品的支持</span><span class="sxs-lookup"><span data-stu-id="a1666-180">Learn about support for commercial marketplace products</span></span>](csp-commercial-marketplace-support.md)
