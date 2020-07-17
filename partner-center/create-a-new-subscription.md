---
title: 在合作伙伴中心创建客户订阅
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何向 Microsoft 发布的产品以及第三方 Isv 发布的 SaaS 产品销售客户订阅。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 47291be42523cbcc3aafbb76a6fd9512191ca806
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435246"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="0ecff-103">创建、暂停或取消客户订阅</span><span class="sxs-lookup"><span data-stu-id="0ecff-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="0ecff-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="0ecff-104">**Applies to**</span></span>

- <span data-ttu-id="0ecff-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="0ecff-105">Partner Center</span></span>
- <span data-ttu-id="0ecff-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="0ecff-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="0ecff-107">云解决方案提供商合作伙伴</span><span class="sxs-lookup"><span data-stu-id="0ecff-107">CSP partners</span></span>

<span data-ttu-id="0ecff-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="0ecff-108">**Appropriate roles**</span></span>

- <span data-ttu-id="0ecff-109">管理员代理</span><span class="sxs-lookup"><span data-stu-id="0ecff-109">Admin agent</span></span>
- <span data-ttu-id="0ecff-110">计费管理员</span><span class="sxs-lookup"><span data-stu-id="0ecff-110">Billing admin</span></span>
- <span data-ttu-id="0ecff-111">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0ecff-111">Global admin</span></span>
- <span data-ttu-id="0ecff-112">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="0ecff-112">Helpdesk agent</span></span>
- <span data-ttu-id="0ecff-113">销售代理</span><span class="sxs-lookup"><span data-stu-id="0ecff-113">Sales agent</span></span>

<span data-ttu-id="0ecff-114">在合作伙伴中心中创建客户的记录后，你可以向他们销售目录中产品的订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="0ecff-115">这包括 Microsoft 发布的产品以及由第三方独立软件供应商（Isv）发布的软件即服务（SaaS）产品到[商业市场](https://azuremarketplace.microsoft.com/marketplace)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="0ecff-116">某些产品/服务仅限每个客户一个订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="0ecff-117">若要查看受限制的套餐列表，请访问合作伙伴中心定价和套餐页面。</span><span class="sxs-lookup"><span data-stu-id="0ecff-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0ecff-118">作为 CSP 计划中的合作伙伴，只能从合作伙伴中心内的 ISV 发布者购买**基于许可证的**SaaS 订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="0ecff-119">这意味着你可以购买 ISV 发布者提供的任何**基于许可证**的 SaaS 产品/服务，包括你有权访问的[独家产品/服务](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="0ecff-120">若要购买或管理其他商业市场，请参阅 Isv 提供的产品/服务（例如**基于使用情况**、按流量计费或基于消耗的产品/服务，包括 azure 应用程序、容器或 vm），你必须使用[azure 管理门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="0ecff-121">有关详细信息，请参阅[购买商业 marketplace 产品](csp-commercial-marketplace-purchase.md)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="0ecff-122">创建新订阅</span><span class="sxs-lookup"><span data-stu-id="0ecff-122">Create a new subscription</span></span>

1. <span data-ttu-id="0ecff-123">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="0ecff-124">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="0ecff-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="0ecff-125">选择“添加订阅”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="0ecff-125">Select **Add subscription**.</span></span> <span data-ttu-id="0ecff-126">"**联机服务**" 选项卡将显示所有可用的 Marketplace SaaS 产品/服务。</span><span class="sxs-lookup"><span data-stu-id="0ecff-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="0ecff-127">若只要查看特定类型的订阅，请在可用筛选器中进行选择：</span><span class="sxs-lookup"><span data-stu-id="0ecff-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="0ecff-128">**发布者**：选择**microsoft**仅查看来自 microsoft 或**合作伙伴**的产品/服务，以查看由 isv 发布的商业 marketplace 产品。</span><span class="sxs-lookup"><span data-stu-id="0ecff-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="0ecff-129">**计费类型**：选择要使用的订阅计费类型： "**许可证**" 或 "**使用情况**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="0ecff-130">请参阅[关于新计费功能的常见问题解答](faq-about-new-billing-features.md)，了解如何决定是采用按月计费还是按年计费频率。</span><span class="sxs-lookup"><span data-stu-id="0ecff-130">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="0ecff-131">**类别**：选择 "**企业**"、"**小企业**" 或 "**试用**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="0ecff-132">若要了解试用版订阅，请参阅[为客户提供 Microsoft 产品试用版](offer-your-customers-trials-of-microsoft-products.md)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="0ecff-133">选择要为客户购买的产品订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="0ecff-134">所看到的产品取决于客户段的类型（教育、政府等）和应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="0ecff-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="0ecff-135">Marketplace 上显示的某些产品/服务可能并不总是用于特定客户或特定的 CSP 合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="0ecff-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="0ecff-136">这可能是因为：</span><span class="sxs-lookup"><span data-stu-id="0ecff-136">This can be because:</span></span>

   - <span data-ttu-id="0ecff-137">该客户已订阅该产品，只允许使用一个</span><span class="sxs-lookup"><span data-stu-id="0ecff-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="0ecff-138">客户的订阅可能已挂起（在这种情况下，您可以重新激活订阅，而不是购买新订阅。）</span><span class="sxs-lookup"><span data-stu-id="0ecff-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="0ecff-139">对于 ISV SaaS 产品/服务，可能有几个原因无法购买产品/服务： ISV 可能不支持客户的计费国家或地区;ISV 可能已选择不通过 CSP 计划提供产品/服务;或者，ISV 可能已[仅向特定的 CSP](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)合作伙伴提供产品/服务。</span><span class="sxs-lookup"><span data-stu-id="0ecff-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="0ecff-140">ISV 产品/服务可能也不会通过合作伙伴中心事务（例如，容器或某些基于使用情况的产品/服务）。</span><span class="sxs-lookup"><span data-stu-id="0ecff-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="0ecff-141">对于要添加的每个订阅，输入许可证数量（如果需要），并选择 "**添加到购物车**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="0ecff-142">添加完订阅后，请选择 "**查看**并查看你的订单"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="0ecff-143">查看订单并准备好购买这些订阅后，选择 "**购买**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="0ecff-144">为客户购买订阅后，将发生以下情况：</span><span class="sxs-lookup"><span data-stu-id="0ecff-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="0ecff-145">您可以通过从该客户的 "**订阅**" 页中选择订阅名称来查看或编辑该订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="0ecff-146">在这里，可以选择附加许可证（如果有）、更改许可证数量，或者暂停订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="0ecff-147">**对于 ISV SaaS （基于许可证）订阅：**</span><span class="sxs-lookup"><span data-stu-id="0ecff-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="0ecff-148">你将收到 ISV 发布者网站的链接。</span><span class="sxs-lookup"><span data-stu-id="0ecff-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="0ecff-149">此链接应有助于你完成客户订阅的部署或帐户设置。</span><span class="sxs-lookup"><span data-stu-id="0ecff-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="0ecff-150">你和你的客户都不会收到一封电子邮件，其中包含为此类型的 ISV 订阅设置/预配的说明。）</span><span class="sxs-lookup"><span data-stu-id="0ecff-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="0ecff-151">如果订阅附带30天的免费试用版，则将自动应用免费试用期。</span><span class="sxs-lookup"><span data-stu-id="0ecff-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="0ecff-152">作为 CSP 计划中的合作伙伴，你不能停征你为客户购买的产品/服务的免费试用期。</span><span class="sxs-lookup"><span data-stu-id="0ecff-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="0ecff-153">在免费试用期结束后，订阅期限将开始，订阅将转换为付费状态。</span><span class="sxs-lookup"><span data-stu-id="0ecff-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="0ecff-154">然后，将根据相同的计划 autorenew 订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-154">The subscription will then autorenew according to the same schedule.</span></span>

## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="0ecff-155">暂停或取消订阅</span><span class="sxs-lookup"><span data-stu-id="0ecff-155">Suspend or cancel a subscription</span></span>

<span data-ttu-id="0ecff-156">在客户提出申请，或者在未付款或欺诈的情况下，合作伙伴可以暂停或取消订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-156">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="0ecff-157">暂停订阅</span><span class="sxs-lookup"><span data-stu-id="0ecff-157">Suspend a subscription</span></span>

<span data-ttu-id="0ecff-158">当你将订阅状态更改为“已暂停”\*\*\*\* 时，用户将无法登录或访问服务。</span><span class="sxs-lookup"><span data-stu-id="0ecff-158">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="0ecff-159">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-159">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="0ecff-160">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="0ecff-160">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="0ecff-161">选择要管理的订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-161">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="0ecff-162">在“状态”部分，选择“已暂停”   。</span><span class="sxs-lookup"><span data-stu-id="0ecff-162">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="0ecff-163">然后“提交”更改  。</span><span class="sxs-lookup"><span data-stu-id="0ecff-163">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="0ecff-164">除非在 90 天内或在 90 天加上帐户开具时间与第一个计费周期之间的天数内（最长 120 天）重新激活订阅，否则所有数据将被删除。</span><span class="sxs-lookup"><span data-stu-id="0ecff-164">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="0ecff-165">暂停订阅后，你在“暂停”\*\*\*\* 按钮下看到的日期即是在不重新激活订阅的情况下，该订阅的自动过期日期。</span><span class="sxs-lookup"><span data-stu-id="0ecff-165">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> <span data-ttu-id="0ecff-166">有关详细信息，请参阅[有关新的计费功能的常见问题](faq-about-new-billing-features.md)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-166">For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="0ecff-167">取消订阅</span><span class="sxs-lookup"><span data-stu-id="0ecff-167">Cancel a subscription</span></span>

<span data-ttu-id="0ecff-168">你可以选择从合作伙伴中心[商业市场](csp-commercial-marketplace-overview.md)中的第三方 ISV 发布者处取消基于许可证的 SaaS 订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-168">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="0ecff-169">只要你在取消期限内取消，你就会获得全额退款。</span><span class="sxs-lookup"><span data-stu-id="0ecff-169">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="0ecff-170">对于按月计费的 ISV 产品/服务：</span><span class="sxs-lookup"><span data-stu-id="0ecff-170">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="0ecff-171">如果您在下一次订单后取消了24小时，则您将在下一张发票上收到完全信用额度。</span><span class="sxs-lookup"><span data-stu-id="0ecff-171">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="0ecff-172">如果您在下一次订单后的24小时内取消，则会计划在续订时进行取消。</span><span class="sxs-lookup"><span data-stu-id="0ecff-172">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="0ecff-173">每年按优惠收费：</span><span class="sxs-lookup"><span data-stu-id="0ecff-173">For offers billed annually:</span></span>

- <span data-ttu-id="0ecff-174">如果您在订购订单后取消14天，则您将在下一张发票上收到完全信用额度。</span><span class="sxs-lookup"><span data-stu-id="0ecff-174">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="0ecff-175">如果您在下一次订单后取消了14天，则会计划在续订时进行取消。</span><span class="sxs-lookup"><span data-stu-id="0ecff-175">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="0ecff-176">在这些时间段结束后，你将无法再看到取消订阅的选项。</span><span class="sxs-lookup"><span data-stu-id="0ecff-176">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="0ecff-177">使用基于使用情况和计量的第三方 ISV 服务（例如，使用虚拟机或容器的服务）不适合返回。</span><span class="sxs-lookup"><span data-stu-id="0ecff-177">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="0ecff-178">基于使用情况的服务可以取消预配为取消方法。</span><span class="sxs-lookup"><span data-stu-id="0ecff-178">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="0ecff-179">由于在使用后费用会计费，因此这些服务没有资格获得退款。</span><span class="sxs-lookup"><span data-stu-id="0ecff-179">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="0ecff-180">若要从 ISV 发行商取消基于许可证的 SaaS 订阅，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0ecff-180">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="0ecff-181">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-181">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="0ecff-182">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="0ecff-182">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="0ecff-183">找到要取消的订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-183">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="0ecff-184">在 "**状态**" 列中，选择 "**取消**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-184">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="0ecff-185">然后“提交”更改  。</span><span class="sxs-lookup"><span data-stu-id="0ecff-185">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="0ecff-186">如果出现一个对话框，请填写所有相关的详细信息，然后选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-186">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="0ecff-187">若要确认取消，请选择 **"是，取消**"。</span><span class="sxs-lookup"><span data-stu-id="0ecff-187">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="0ecff-188">还可以选择使用 Api 取消 Azure Marketplace 订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-188">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="0ecff-189">为此，请参阅[取消 Azure Marketplace 订阅](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-189">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="0ecff-190">选择是否自动续订商业市场订阅</span><span class="sxs-lookup"><span data-stu-id="0ecff-190">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="0ecff-191">默认情况下，活动订阅设置为订阅期限过期时自动续订。</span><span class="sxs-lookup"><span data-stu-id="0ecff-191">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="0ecff-192">对于[商业 marketplace 产品订阅](csp-commercial-marketplace-overview.md)，你可以选择不自动续订订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-192">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="0ecff-193">若要阻止有效的商业市场订阅自动续订：</span><span class="sxs-lookup"><span data-stu-id="0ecff-193">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="0ecff-194">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="0ecff-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="0ecff-195">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="0ecff-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="0ecff-196">选择“订阅”。</span><span class="sxs-lookup"><span data-stu-id="0ecff-196">Select **Subscriptions**.</span></span> <span data-ttu-id="0ecff-197">这会列出已为客户购买的任何基于许可证的订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-197">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="0ecff-198">在 "**订阅**" 列中，选择要修改的订阅。</span><span class="sxs-lookup"><span data-stu-id="0ecff-198">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="0ecff-199">在 "订阅详细信息" 页中，找到 "**状态**" 部分并取消选中 "**自动续订**" 框。</span><span class="sxs-lookup"><span data-stu-id="0ecff-199">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="0ecff-200">选择“提交”。</span><span class="sxs-lookup"><span data-stu-id="0ecff-200">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0ecff-201">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0ecff-201">Next steps</span></span>

- [<span data-ttu-id="0ecff-202">为客户购买商业市场产品</span><span class="sxs-lookup"><span data-stu-id="0ecff-202">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="0ecff-203">为客户管理商业 marketplace 产品</span><span class="sxs-lookup"><span data-stu-id="0ecff-203">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="0ecff-204">商业市场概述</span><span class="sxs-lookup"><span data-stu-id="0ecff-204">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
