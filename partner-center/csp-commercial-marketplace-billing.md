---
title: 商业应用商店产品的帐单
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何针对从合作伙伴中心内的商业市场为客户购买的 ISV SaaS 产品或订阅付费。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148017"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a><span data-ttu-id="2debe-103">适用于合作伙伴中心的商业 marketplace 产品和订阅的帐单</span><span class="sxs-lookup"><span data-stu-id="2debe-103">Billing for commercial marketplace products and subscriptions in Partner Center</span></span>


<span data-ttu-id="2debe-104">**适当的角色**：全局管理员 |计费管理员</span><span class="sxs-lookup"><span data-stu-id="2debe-104">**Appropriate roles**: Global admin | Billing admin</span></span>

<span data-ttu-id="2debe-105">作为 CSP 计划中的合作伙伴，你可以使用合作伙伴中心从商业应用商店中的 ISV 出版商那里购买基于许可证的 SaaS 产品。</span><span class="sxs-lookup"><span data-stu-id="2debe-105">As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace.</span></span> <span data-ttu-id="2debe-106">完成此操作后，你可以访问这些类型采购的帐单。</span><span class="sxs-lookup"><span data-stu-id="2debe-106">After you do so, you can access a bill for these types of purchases.</span></span> <span data-ttu-id="2debe-107">计费周期从日历月的第一天开始，到日历月的最后一天结束。</span><span class="sxs-lookup"><span data-stu-id="2debe-107">The billing period starts on the first day of the calendar month and ends on the last day of the calendar month.</span></span> <span data-ttu-id="2debe-108">发票在下个月的第8天可用。</span><span class="sxs-lookup"><span data-stu-id="2debe-108">Invoices are made available on the 8th day of the following month.</span></span>

<span data-ttu-id="2debe-109">你可以通过合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/) 或使用 [合作伙伴中心 api](/partner-center/develop/)访问发票。</span><span class="sxs-lookup"><span data-stu-id="2debe-109">You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](/partner-center/develop/).</span></span>

<span data-ttu-id="2debe-110">CSP 计划中的合作伙伴需要为客户购买的 ISV 商用 marketplace 解决方案收费，当他们从合作伙伴中心或从 Azure 门户 (使用客户以前购买的 Azure 租户) 购买这些产品。</span><span class="sxs-lookup"><span data-stu-id="2debe-110">Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).</span></span>

>[!NOTE]
><span data-ttu-id="2debe-111">如果客户使用他们自己的 Azure AD 租户 (不是从 CSP 计划中的合作伙伴那里购买的) ，则客户还可以选择直接从 ([Microsoft AppSource](https://appsource.microsoft.com/) 或 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) 购买自己的 ISV SaaS 解决方案。</span><span class="sxs-lookup"><span data-stu-id="2debe-111">If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)).</span></span> <span data-ttu-id="2debe-112">如果他们这样做，他们将直接从 Microsoft 接收自己的帐单。</span><span class="sxs-lookup"><span data-stu-id="2debe-112">If they do so, they will receive their own bill directly from Microsoft.</span></span> <span data-ttu-id="2debe-113">同样，如果 CSP 计划中的合作伙伴向客户销售 Azure 订阅或新的 Azure 计划，并授予客户 (或间接分销商) 对该租户的 [基于角色的访问权限](/azure/role-based-access-control/built-in-roles) (向客户分配除 **读者**) 以外的任何角色，则该客户 (或间接经销商) 还可以购买商业 marketplace 产品/服务，而不需要事先批准或通知 CSP 合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="2debe-113">Likewise, if a partner in the CSP program sells an Azure subscription or the new Azure plan to the customer and grants the customer (or indirect reseller) [role-based access](/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer (or indirect reseller) can also purchase commercial marketplace offers without prior approval or notification to the CSP partner.</span></span> <span data-ttu-id="2debe-114">在这种情况下，Microsoft 不会直接在 CSP 计划中向合作伙伴通知客户的购买情况。</span><span class="sxs-lookup"><span data-stu-id="2debe-114">In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers.</span></span> <span data-ttu-id="2debe-115">但是，Microsoft 确实 [提供了](/azure/azure-monitor/platform/alerts-activity-log) Azure Monitor，可用于设置有关 Azure 订阅上的活动的警报或通知。</span><span class="sxs-lookup"><span data-stu-id="2debe-115">However, Microsoft does offer an optional [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.</span></span>

## <a name="access-billing-information-for-commercial-marketplace-products"></a><span data-ttu-id="2debe-116">访问商业市场产品的计费信息</span><span class="sxs-lookup"><span data-stu-id="2debe-116">Access billing information for commercial marketplace products</span></span>

<span data-ttu-id="2debe-117">当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2debe-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> <span data-ttu-id="2debe-118">访问商业市场产品购买的最新发票和对帐文件：</span><span class="sxs-lookup"><span data-stu-id="2debe-118">To access the latest invoice and reconciliation file for commercial marketplace product purchases:</span></span>

1. <span data-ttu-id="2debe-119">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="2debe-119">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="2debe-120">在“合作伙伴中心”菜单中，选择“计费”。</span><span class="sxs-lookup"><span data-stu-id="2debe-120">From the Partner Center menu, select **Billing**.</span></span> 

    <span data-ttu-id="2debe-121">"计费"页顶部有两个选项卡："定期"和"定期"和 **"一次性购买"。**</span><span class="sxs-lookup"><span data-stu-id="2debe-121">You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**.</span></span> <span data-ttu-id="2debe-122">通过每个选项卡，可以访问发票 (对帐) 不同市场产品的对帐文件：</span><span class="sxs-lookup"><span data-stu-id="2debe-122">Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:</span></span>

    - <span data-ttu-id="2debe-123">**"** 定期"选项卡：显示与 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、Power BI Pro 和 Microsoft Azure 相关的订阅的发票和对帐文件。</span><span class="sxs-lookup"><span data-stu-id="2debe-123">**Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro, and Microsoft Azure.</span></span>

    - <span data-ttu-id="2debe-124">**定期和一次性购买** 选项卡：显示 Azure 计划、Azure 预留、软件和商业市场产品的发票和对帐文件。</span><span class="sxs-lookup"><span data-stu-id="2debe-124">**Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.</span></span>
  
3. <span data-ttu-id="2debe-125">选择" **定期和一次性购买"** 选项卡。如果以其他货币为客户购买了订阅，则会看到每种货币的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2debe-125">Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency.</span></span> <span data-ttu-id="2debe-126">可以从此页面执行一些操作：</span><span class="sxs-lookup"><span data-stu-id="2debe-126">You can do a few things from this page:</span></span>

    - <span data-ttu-id="2debe-127">若要查看最新的发票和对帐文件，请选择"**发票或\*\*\*\*对帐文件"。**</span><span class="sxs-lookup"><span data-stu-id="2debe-127">To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**.</span></span> <span data-ttu-id="2debe-128"> (如果需要，还可使用 API 访问最新的发票 [和合作伙伴中心数据](/partner-center/develop/)。</span><span class="sxs-lookup"><span data-stu-id="2debe-128">(If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](/partner-center/develop/).</span></span>

    - <span data-ttu-id="2debe-129">若要查看较早的发票和对帐文件，请展开下面的 **"计费历史记录"** 行。</span><span class="sxs-lookup"><span data-stu-id="2debe-129">To see earlier invoices and recon files, expand the **Billing history** row below.</span></span>

    - <span data-ttu-id="2debe-130">若要随时根据最新的帐户活动检查估计的帐户余额或帐单，请在"估计"标题下 **选择一个** 链接。</span><span class="sxs-lookup"><span data-stu-id="2debe-130">To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.</span></span>  

    >[!NOTE]
    > <span data-ttu-id="2debe-131">当我们在当月的第 8 天发布帐单时，它将包括税款以及任何其他适用的费用与额度。</span><span class="sxs-lookup"><span data-stu-id="2debe-131">When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits.</span></span> <span data-ttu-id="2debe-132">这意味着最终到期金额可能与计费周期内看到的金额不同。</span><span class="sxs-lookup"><span data-stu-id="2debe-132">This means the final amount due might differ from what you see during the billing period.</span></span>

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a><span data-ttu-id="2debe-133">详细了解商业市场产品的发票和重新确认文件</span><span class="sxs-lookup"><span data-stu-id="2debe-133">More about invoices and recon files for commercial marketplace products</span></span>

<span data-ttu-id="2debe-134">本部分提供了有关为第三方 ISV 发布者购买的商业 marketplace SaaS 订阅的发票和对帐文件的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2debe-134">This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.</span></span>

<span data-ttu-id="2debe-135">当你从 "合作伙伴中心" 菜单中的 "**计费**" 选项中选择 "**定期购买" 和 "一次性购买**" 时，你将获得对发票和协调文件的访问权限，以获取与 Microsoft (第一方) 和 ISV (第三方) 购买相关的费用。</span><span class="sxs-lookup"><span data-stu-id="2debe-135">When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases.</span></span> <span data-ttu-id="2debe-136">这些购买可能会与相关联：</span><span class="sxs-lookup"><span data-stu-id="2debe-136">These purchases may be associated with:</span></span>

- <span data-ttu-id="2debe-137">Microsoft 或 ISV 发布者 (的 SaaS 订阅) </span><span class="sxs-lookup"><span data-stu-id="2debe-137">SaaS subscriptions (from either Microsoft or ISV publishers)</span></span>

- <span data-ttu-id="2debe-138">Azure 计划</span><span class="sxs-lookup"><span data-stu-id="2debe-138">Azure plan</span></span>

- <span data-ttu-id="2debe-139">Azure 预留项</span><span class="sxs-lookup"><span data-stu-id="2debe-139">Azure reservations</span></span>

- <span data-ttu-id="2debe-140">来自 Microsoft 或 ISV 发布者的其他基于订阅的软件 () </span><span class="sxs-lookup"><span data-stu-id="2debe-140">Other subscription-based software (from either Microsoft or ISV publishers)</span></span>

<span data-ttu-id="2debe-141">这些购买的示例可能包括 SUSE Linux 软件 (软件订阅) 或 Azure ISV SaaS 产品订阅。</span><span class="sxs-lookup"><span data-stu-id="2debe-141">Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.</span></span>

>[!NOTE]
> <span data-ttu-id="2debe-142">有关如何读取发票和侦测文件的详细信息，请参阅 [帐单概述](billing.md)。</span><span class="sxs-lookup"><span data-stu-id="2debe-142">For more information about how to read invoice and recon files, see also [Billing overview](billing.md).</span></span>

### <a name="tips-on-reading-your-invoice"></a><span data-ttu-id="2debe-143">阅读发票提示</span><span class="sxs-lookup"><span data-stu-id="2debe-143">Tips on reading your invoice</span></span>

<span data-ttu-id="2debe-144">从第三方 ISV 发布商处购买基于许可证的 SaaS 产品时，你只会看到发票上的许可费用收费。</span><span class="sxs-lookup"><span data-stu-id="2debe-144">When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice.</span></span> <span data-ttu-id="2debe-145">即使 ISV 的 SaaS 产品使用 (或使用) 底层 Azure 基础结构资源，也是如此。</span><span class="sxs-lookup"><span data-stu-id="2debe-145">This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources.</span></span> <span data-ttu-id="2debe-146">这是因为，对 isv 的 SaaS 产品的客户的 Azure 基础结构用量收费直接向 ISV 收费。</span><span class="sxs-lookup"><span data-stu-id="2debe-146">That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV.</span></span> <span data-ttu-id="2debe-147"> (Isv 会在其自己的 Azure 使用情况的每日评级发票对帐文件中看到关联的 Azure 消耗费用。 ) </span><span class="sxs-lookup"><span data-stu-id="2debe-147">(ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)</span></span>

<span data-ttu-id="2debe-148">你的发票将包含多个页面：</span><span class="sxs-lookup"><span data-stu-id="2debe-148">Your invoice will contain several pages:</span></span>

- <span data-ttu-id="2debe-149">**发票第1页：** 包含 CSP 计划合作伙伴的计费详细信息的摘要概述。</span><span class="sxs-lookup"><span data-stu-id="2debe-149">**Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details.</span></span> <span data-ttu-id="2debe-150">这包括计费周期的费用摘要、发票编号、 (Net 60 days) 的付款条款，以及通过线路或支票支付的帐单支付方法。</span><span class="sxs-lookup"><span data-stu-id="2debe-150">This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.</span></span>

- <span data-ttu-id="2debe-151">**第2页 () 发票的所有后续页面：** 第一方 Microsoft 购买和第三方 ISV (基于许可证的) 从商业应用商店购买的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2debe-151">**Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace.</span></span> <span data-ttu-id="2debe-152">可以通过发布者行在每个产品名称下标识基于 ISV许可证的购买。</span><span class="sxs-lookup"><span data-stu-id="2debe-152">You can identify ISV license-based purchases by the **Publisher** line beneath each product name.</span></span> <span data-ttu-id="2debe-153">关联的对帐文件提供特定发票费用的更多计费详细信息。</span><span class="sxs-lookup"><span data-stu-id="2debe-153">The associated reconciliation file offers more billing details for specific invoice charges.</span></span>

- <span data-ttu-id="2debe-154">**发票的最后一页：** 如果从 ISV 对基于许可证的市场产品收费，此最终页面将显示有关 ISV 发布者名称和地址的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="2debe-154">**Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.</span></span>

### <a name="tips-on-reading-your-reconciliation-file"></a><span data-ttu-id="2debe-155">有关读取对帐文件的提示</span><span class="sxs-lookup"><span data-stu-id="2debe-155">Tips on reading your reconciliation file</span></span>

<span data-ttu-id="2debe-156">定期 **和一次性购买** 对帐文件包含多个列，其中包含映射到发票中费用的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="2debe-156">The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice.</span></span> <span data-ttu-id="2debe-157">**PublisherName** 列显示购买内容是 Microsoft 还是第三方 ISV 发布者。</span><span class="sxs-lookup"><span data-stu-id="2debe-157">The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.</span></span>

<span data-ttu-id="2debe-158">对帐文件中可能会出现一些费用，费用为 0 美元。</span><span class="sxs-lookup"><span data-stu-id="2debe-158">Some charges in your reconciliation file may appear with a cost of $0.</span></span> <span data-ttu-id="2debe-159">这可能是由于 ISV"免费试用"产品/服务 (30 或 60 天) 自带许可产品/服务。</span><span class="sxs-lookup"><span data-stu-id="2debe-159">This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.</span></span>

<span data-ttu-id="2debe-160">对于免费试用版 ISV 产品/服务：</span><span class="sxs-lookup"><span data-stu-id="2debe-160">In the case of free trial ISV offers:</span></span>

- <span data-ttu-id="2debe-161">免费试用期涵盖在此期间 ISV 基于许可证的 SaaS 产品的成本。</span><span class="sxs-lookup"><span data-stu-id="2debe-161">The free trial period covers the cost of the ISV's license-based SaaS product during that time.</span></span> <span data-ttu-id="2debe-162">对于该 SaaS 产品的关联 Azure 基础结构使用，也不需要付费。</span><span class="sxs-lookup"><span data-stu-id="2debe-162">You will also not be charged for associated Azure infrastructure use of that SaaS product.</span></span>  <span data-ttu-id="2debe-163">但是，如果使用的是基于使用情况的 ISV 产品/服务，则免费试用版不包括基础 Azure 基础结构使用的成本。</span><span class="sxs-lookup"><span data-stu-id="2debe-163">If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage.</span></span> <span data-ttu-id="2debe-164">在这种情况下，Azure 基础结构使用费用将显示在单独的 Azure 对帐文件中。</span><span class="sxs-lookup"><span data-stu-id="2debe-164">In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.</span></span>

- <span data-ttu-id="2debe-165">为客户购买和部署符合 ISV 免费试用版资格的产品时，ISV 发布者会自动将客户注册到免费试用版中。</span><span class="sxs-lookup"><span data-stu-id="2debe-165">When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher.</span></span> <span data-ttu-id="2debe-166">免费试用期在 ISV 发布者定义的期限之后自动结束。</span><span class="sxs-lookup"><span data-stu-id="2debe-166">The free trial period ends automatically after the period defined by the ISV publisher.</span></span> <span data-ttu-id="2debe-167">在期限结束后，将收取客户费用。</span><span class="sxs-lookup"><span data-stu-id="2debe-167">After the period ends, the customer will be charged.</span></span> <span data-ttu-id="2debe-168">这意味着，对帐文件可能会显示符合试用条件的产品的两行：一行跟踪试用期，另一行跟踪付费产品/服务 (在试用期结束后显示费用为 0 美元) 。</span><span class="sxs-lookup"><span data-stu-id="2debe-168">This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends).</span></span> <span data-ttu-id="2debe-169">试用结束后，显示付费产品/服务行将开始显示费用。</span><span class="sxs-lookup"><span data-stu-id="2debe-169">Once the trial ends, the row showing the paid offer will start to show charges.</span></span> 

<span data-ttu-id="2debe-170">有关每个列代表的内容的详细信息，请参阅 [使用对帐文件](use-the-reconciliation-files.md)。</span><span class="sxs-lookup"><span data-stu-id="2debe-170">For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md).</span></span> <span data-ttu-id="2debe-171">另请参阅 [合作伙伴中心的计费类型](./billing-basics.md)</span><span class="sxs-lookup"><span data-stu-id="2debe-171">See also [Types of billing in Partner Center](./billing-basics.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="2debe-172">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2debe-172">Next steps</span></span>

- [<span data-ttu-id="2debe-173">为客户管理商业 marketplace 产品</span><span class="sxs-lookup"><span data-stu-id="2debe-173">Manage commercial marketplace products for customers</span></span>](csp-commercial-marketplace-manage.md)
- [<span data-ttu-id="2debe-174">了解对商业 marketplace 产品的支持</span><span class="sxs-lookup"><span data-stu-id="2debe-174">Learn about support for commercial marketplace products</span></span>](csp-commercial-marketplace-support.md)