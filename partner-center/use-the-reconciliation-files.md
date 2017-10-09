---
title: Use the reconciliation files | Partner Center
description: For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 551afa2468e2bd79f1779a82e6ece3725b33237b
ms.sourcegitcommit: 4c29498e3d6d4038044b4cb2cb19a19e6a586823
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="ddefc-103">Use the reconciliation files</span><span class="sxs-lookup"><span data-stu-id="ddefc-103">Use the reconciliation files</span></span>

**<span data-ttu-id="ddefc-104">Applies to</span><span class="sxs-lookup"><span data-stu-id="ddefc-104">Applies to</span></span>**

-  <span data-ttu-id="ddefc-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="ddefc-105">Partner Center</span></span>
-  <span data-ttu-id="ddefc-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="ddefc-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="ddefc-107">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="ddefc-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="ddefc-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span><span class="sxs-lookup"><span data-stu-id="ddefc-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="ddefc-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span><span class="sxs-lookup"><span data-stu-id="ddefc-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <span data-ttu-id="ddefc-110"><a href="" id="itemizebypartner"></a>Itemize by partner</span><span class="sxs-lookup"><span data-stu-id="ddefc-110"><a href="" id="itemizebypartner"></a>Itemize by partner</span></span>


<span data-ttu-id="ddefc-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span><span class="sxs-lookup"><span data-stu-id="ddefc-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ddefc-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="ddefc-112">MPN ID</span></span></th>
<th><span data-ttu-id="ddefc-113">Description</span><span class="sxs-lookup"><span data-stu-id="ddefc-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ddefc-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="ddefc-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="ddefc-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span><span class="sxs-lookup"><span data-stu-id="ddefc-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-116">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="ddefc-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="ddefc-117">Only appears on reconciliation files for partners in the indirect model.</span><span class="sxs-lookup"><span data-stu-id="ddefc-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="ddefc-118">The MPN ID of the reseller of record for the subscription.</span><span class="sxs-lookup"><span data-stu-id="ddefc-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ddefc-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddefc-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="ddefc-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="ddefc-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="ddefc-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span><span class="sxs-lookup"><span data-stu-id="ddefc-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="ddefc-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span><span class="sxs-lookup"><span data-stu-id="ddefc-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="ddefc-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span><span class="sxs-lookup"><span data-stu-id="ddefc-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="ddefc-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span><span class="sxs-lookup"><span data-stu-id="ddefc-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <span data-ttu-id="ddefc-126"><a href="" id="licensebasedfiles"></a> License-based file fields</span><span class="sxs-lookup"><span data-stu-id="ddefc-126"><a href="" id="licensebasedfiles"></a> License-based file fields</span></span>


<span data-ttu-id="ddefc-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddefc-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="ddefc-128">Column</span><span class="sxs-lookup"><span data-stu-id="ddefc-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="ddefc-129">Description</span><span class="sxs-lookup"><span data-stu-id="ddefc-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="ddefc-130">Sample Value</span><span class="sxs-lookup"><span data-stu-id="ddefc-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ddefc-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="ddefc-132">Unique identifier for a specific billing entity, in GUID format.</span><span class="sxs-lookup"><span data-stu-id="ddefc-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ddefc-133">Not required for reconciliation, however may be useful information.</span><span class="sxs-lookup"><span data-stu-id="ddefc-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ddefc-134">Same in all rows.</span><span class="sxs-lookup"><span data-stu-id="ddefc-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="ddefc-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="ddefc-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ddefc-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="ddefc-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span><span class="sxs-lookup"><span data-stu-id="ddefc-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ddefc-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="ddefc-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="ddefc-139">OrderID</span></span></td>
<td><p><span data-ttu-id="ddefc-140">Unique identifier for an order in the Microsoft billing platform.</span><span class="sxs-lookup"><span data-stu-id="ddefc-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ddefc-141">May be useful to identify the order when contacting support but not for reconciliation.</span><span class="sxs-lookup"><span data-stu-id="ddefc-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ddefc-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ddefc-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ddefc-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ddefc-144">Unique identifier for a subscription in the Microsoft billing platform.</span><span class="sxs-lookup"><span data-stu-id="ddefc-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ddefc-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span><span class="sxs-lookup"><span data-stu-id="ddefc-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ddefc-146">This is not the same as the Subscription ID on the Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="ddefc-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="ddefc-147">Please see Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="ddefc-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="ddefc-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ddefc-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="ddefc-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="ddefc-150">Unique identifier for subscriptions.</span><span class="sxs-lookup"><span data-stu-id="ddefc-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="ddefc-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span><span class="sxs-lookup"><span data-stu-id="ddefc-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="ddefc-152">This field maps to the Subscription ID in the Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="ddefc-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ddefc-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="ddefc-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="ddefc-154">OfferID</span></span></td>
<td><p><span data-ttu-id="ddefc-155">Unique offer ID.</span><span class="sxs-lookup"><span data-stu-id="ddefc-155">Unique offer ID.</span></span> <span data-ttu-id="ddefc-156">Standard offer ID as per price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="ddefc-157"><b>Note</b>: This value does not match Offer ID from the price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="ddefc-158">See DurableOfferID below.</span><span class="sxs-lookup"><span data-stu-id="ddefc-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="ddefc-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="ddefc-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="ddefc-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="ddefc-161">Unique durable offer ID, as defined in the price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="ddefc-162"><b>Note</b>: This value matches the Offer ID from the price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="ddefc-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="ddefc-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="ddefc-164">OfferName</span></span></td>
<td><p><span data-ttu-id="ddefc-165">The name of the service offering purchased by the customer, as defined in the price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="ddefc-166">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="ddefc-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="ddefc-168">The subscription start date, set to the day after the order is submitted.</span><span class="sxs-lookup"><span data-stu-id="ddefc-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="ddefc-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span><span class="sxs-lookup"><span data-stu-id="ddefc-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="ddefc-170">The time is always the beginning of the day, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ddefc-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ddefc-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ddefc-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="ddefc-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span><span class="sxs-lookup"><span data-stu-id="ddefc-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="ddefc-174">At renewal, prices are updated to the current price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="ddefc-175">Customer communication may be required in advance of automated renewal.</span><span class="sxs-lookup"><span data-stu-id="ddefc-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="ddefc-176">The time is always the beginning of the day, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ddefc-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ddefc-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ddefc-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ddefc-179">Start day of the charges.</span><span class="sxs-lookup"><span data-stu-id="ddefc-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="ddefc-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span><span class="sxs-lookup"><span data-stu-id="ddefc-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ddefc-181">The time is always the beginning of the day, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ddefc-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ddefc-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ddefc-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ddefc-184">End day of the charges.</span><span class="sxs-lookup"><span data-stu-id="ddefc-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="ddefc-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span><span class="sxs-lookup"><span data-stu-id="ddefc-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ddefc-186">The time is always the end of the day, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ddefc-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ddefc-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="ddefc-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ddefc-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="ddefc-189">The type of charge or adjustment.</span><span class="sxs-lookup"><span data-stu-id="ddefc-189">The type of charge or adjustment.</span></span> <span data-ttu-id="ddefc-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span><span class="sxs-lookup"><span data-stu-id="ddefc-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ddefc-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span><span class="sxs-lookup"><span data-stu-id="ddefc-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ddefc-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="ddefc-193">Price per seat.</span><span class="sxs-lookup"><span data-stu-id="ddefc-193">Price per seat.</span></span> <span data-ttu-id="ddefc-194">Ensure this matches the information stored in your billing system during reconciliation.</span><span class="sxs-lookup"><span data-stu-id="ddefc-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ddefc-195">6.82</span><span class="sxs-lookup"><span data-stu-id="ddefc-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="ddefc-196">Quantity</span></span></td>
<td><p><span data-ttu-id="ddefc-197">Number of seats.</span><span class="sxs-lookup"><span data-stu-id="ddefc-197">Number of seats.</span></span> <span data-ttu-id="ddefc-198">Ensure this matches the information stored in your billing system during reconciliation.</span><span class="sxs-lookup"><span data-stu-id="ddefc-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ddefc-199">2</span><span class="sxs-lookup"><span data-stu-id="ddefc-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-200">Amount</span><span class="sxs-lookup"><span data-stu-id="ddefc-200">Amount</span></span></td>
<td><p><span data-ttu-id="ddefc-201">Total of price for quantity.</span><span class="sxs-lookup"><span data-stu-id="ddefc-201">Total of price for quantity.</span></span> <span data-ttu-id="ddefc-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span><span class="sxs-lookup"><span data-stu-id="ddefc-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="ddefc-203">13.32</span><span class="sxs-lookup"><span data-stu-id="ddefc-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="ddefc-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="ddefc-205">Amount of discount applied to these charges.</span><span class="sxs-lookup"><span data-stu-id="ddefc-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="ddefc-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span><span class="sxs-lookup"><span data-stu-id="ddefc-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="ddefc-207">2.32</span><span class="sxs-lookup"><span data-stu-id="ddefc-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="ddefc-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="ddefc-209">Total before tax.</span><span class="sxs-lookup"><span data-stu-id="ddefc-209">Total before tax.</span></span> <span data-ttu-id="ddefc-210">Checks that your subtotal matches your expected total, in case of a discount.</span><span class="sxs-lookup"><span data-stu-id="ddefc-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="ddefc-211">11</span><span class="sxs-lookup"><span data-stu-id="ddefc-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-212">Tax</span><span class="sxs-lookup"><span data-stu-id="ddefc-212">Tax</span></span></td>
<td><p><span data-ttu-id="ddefc-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span><span class="sxs-lookup"><span data-stu-id="ddefc-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ddefc-214">0</span><span class="sxs-lookup"><span data-stu-id="ddefc-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="ddefc-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="ddefc-216">Total after tax.</span><span class="sxs-lookup"><span data-stu-id="ddefc-216">Total after tax.</span></span> <span data-ttu-id="ddefc-217">Checks if you are charged tax in the invoice.</span><span class="sxs-lookup"><span data-stu-id="ddefc-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="ddefc-218">11</span><span class="sxs-lookup"><span data-stu-id="ddefc-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-219">Currency</span><span class="sxs-lookup"><span data-stu-id="ddefc-219">Currency</span></span></td>
<td><p><span data-ttu-id="ddefc-220">Currency type.</span><span class="sxs-lookup"><span data-stu-id="ddefc-220">Currency type.</span></span> <span data-ttu-id="ddefc-221">Each billing entity has only one currency.</span><span class="sxs-lookup"><span data-stu-id="ddefc-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="ddefc-222">Check that it matches your first invoice and then after any major billing platform update.</span><span class="sxs-lookup"><span data-stu-id="ddefc-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ddefc-223">EUR</span><span class="sxs-lookup"><span data-stu-id="ddefc-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ddefc-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="ddefc-225">Customer's organization name as reported in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddefc-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ddefc-226">This is very important for reconciling the invoice with your system information.</span><span class="sxs-lookup"><span data-stu-id="ddefc-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ddefc-227">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="ddefc-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="ddefc-228">MPNID</span></span></td>
<td><p><span data-ttu-id="ddefc-229">MPN ID of the CSP partner</span><span class="sxs-lookup"><span data-stu-id="ddefc-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="ddefc-230">4390934</span><span class="sxs-lookup"><span data-stu-id="ddefc-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ddefc-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ddefc-232">MPN ID of the reseller of record for the subscription.</span><span class="sxs-lookup"><span data-stu-id="ddefc-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ddefc-233">See [Itemize by partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="ddefc-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="ddefc-234">4390934</span><span class="sxs-lookup"><span data-stu-id="ddefc-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="ddefc-235">DomainName</span></span></td>
<td><p><span data-ttu-id="ddefc-236">Customer's domain name, used to help identify the customer.</span><span class="sxs-lookup"><span data-stu-id="ddefc-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="ddefc-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ddefc-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ddefc-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ddefc-239">Subscription nickname.</span><span class="sxs-lookup"><span data-stu-id="ddefc-239">Subscription nickname.</span></span> <span data-ttu-id="ddefc-240">If no nickname is specified, Partner Center uses the OfferName.</span><span class="sxs-lookup"><span data-stu-id="ddefc-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="ddefc-241">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="ddefc-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ddefc-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ddefc-243">The name of the service offering purchased by the customer, as defined in the price list.</span><span class="sxs-lookup"><span data-stu-id="ddefc-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ddefc-244">(This is an identical field to Offer name).</span><span class="sxs-lookup"><span data-stu-id="ddefc-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="ddefc-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="ddefc-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <span data-ttu-id="ddefc-246"><a href="" id="usagebasedfiles"></a>Usage-based file fields</span><span class="sxs-lookup"><span data-stu-id="ddefc-246"><a href="" id="usagebasedfiles"></a>Usage-based file fields</span></span>


<span data-ttu-id="ddefc-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddefc-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="ddefc-248">The following fields explain which services were used and the rate.</span><span class="sxs-lookup"><span data-stu-id="ddefc-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="ddefc-249">Column</span><span class="sxs-lookup"><span data-stu-id="ddefc-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="ddefc-250">Description</span><span class="sxs-lookup"><span data-stu-id="ddefc-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="ddefc-251">Sample value</span><span class="sxs-lookup"><span data-stu-id="ddefc-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="ddefc-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="ddefc-253">Partner ID, in GUID format.</span><span class="sxs-lookup"><span data-stu-id="ddefc-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="ddefc-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ddefc-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ddefc-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="ddefc-256">Partner Name.</span><span class="sxs-lookup"><span data-stu-id="ddefc-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="ddefc-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="ddefc-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="ddefc-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="ddefc-259">Partner Account ID.</span><span class="sxs-lookup"><span data-stu-id="ddefc-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="ddefc-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="ddefc-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ddefc-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="ddefc-262">Customer's organization name as reported in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddefc-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ddefc-263">This is very important for reconciling the invoice with your system information.</span><span class="sxs-lookup"><span data-stu-id="ddefc-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ddefc-264">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="ddefc-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="ddefc-265">MPNID</span></span></td>
<td><p><span data-ttu-id="ddefc-266">MPN ID of the CSP partner.</span><span class="sxs-lookup"><span data-stu-id="ddefc-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="ddefc-267">4390934</span><span class="sxs-lookup"><span data-stu-id="ddefc-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ddefc-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ddefc-269">MPN ID of the reseller of record for the subscription.</span><span class="sxs-lookup"><span data-stu-id="ddefc-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ddefc-270">See [Itemize by partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="ddefc-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="ddefc-271">4390934</span><span class="sxs-lookup"><span data-stu-id="ddefc-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ddefc-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ddefc-273">Invoice number where the specified transaction appears.</span><span class="sxs-lookup"><span data-stu-id="ddefc-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="ddefc-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="ddefc-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ddefc-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span><span class="sxs-lookup"><span data-stu-id="ddefc-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ddefc-277">The time is always the beginning of the day, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ddefc-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ddefc-278">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ddefc-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ddefc-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span><span class="sxs-lookup"><span data-stu-id="ddefc-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ddefc-281">The time is always the end of the day, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ddefc-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ddefc-282">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="ddefc-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ddefc-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ddefc-284">Unique identifier for a subscription in the Microsoft billing platform.</span><span class="sxs-lookup"><span data-stu-id="ddefc-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ddefc-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span><span class="sxs-lookup"><span data-stu-id="ddefc-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ddefc-286">This is not the same as the Subscription ID on the Partner Admin Console.</span><span class="sxs-lookup"><span data-stu-id="ddefc-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ddefc-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ddefc-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ddefc-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ddefc-289">Nickname of the service offering.</span><span class="sxs-lookup"><span data-stu-id="ddefc-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="ddefc-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ddefc-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ddefc-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ddefc-292">Line of business of the service offering</span><span class="sxs-lookup"><span data-stu-id="ddefc-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="ddefc-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ddefc-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="ddefc-294">OrderID</span></span></td>
<td><p><span data-ttu-id="ddefc-295">Unique identifier for an order in the Microsoft billing platform.</span><span class="sxs-lookup"><span data-stu-id="ddefc-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ddefc-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span><span class="sxs-lookup"><span data-stu-id="ddefc-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ddefc-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ddefc-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="ddefc-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="ddefc-299">The name of the Azure service in question.</span><span class="sxs-lookup"><span data-stu-id="ddefc-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="ddefc-300">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="ddefc-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="ddefc-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="ddefc-302">The specific type of Windows Azure service.</span><span class="sxs-lookup"><span data-stu-id="ddefc-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ddefc-303">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="ddefc-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="ddefc-304">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="ddefc-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="ddefc-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="ddefc-306">Specific unique identifier for all the service data and pricing structure.</span><span class="sxs-lookup"><span data-stu-id="ddefc-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="ddefc-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ddefc-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-308">Resource Name</span><span class="sxs-lookup"><span data-stu-id="ddefc-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="ddefc-309">The name of the Azure resource.</span><span class="sxs-lookup"><span data-stu-id="ddefc-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ddefc-310">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="ddefc-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="ddefc-311">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="ddefc-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-312">Region</span><span class="sxs-lookup"><span data-stu-id="ddefc-312">Region</span></span></td>
<td><p><span data-ttu-id="ddefc-313">The region the usage applies to.</span><span class="sxs-lookup"><span data-stu-id="ddefc-313">The region the usage applies to.</span></span> <span data-ttu-id="ddefc-314">Primarily used to assign rates to data transfers, as rates vary by region.</span><span class="sxs-lookup"><span data-stu-id="ddefc-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="ddefc-315">Asia Pacific, Europe, Latin America, North America</span><span class="sxs-lookup"><span data-stu-id="ddefc-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-316">SKU</span><span class="sxs-lookup"><span data-stu-id="ddefc-316">SKU</span></span></td>
<td><p><span data-ttu-id="ddefc-317">MSFT unique identifier for offer</span><span class="sxs-lookup"><span data-stu-id="ddefc-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="ddefc-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="ddefc-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="ddefc-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="ddefc-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="ddefc-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span><span class="sxs-lookup"><span data-stu-id="ddefc-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="ddefc-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span><span class="sxs-lookup"><span data-stu-id="ddefc-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="ddefc-322">1</span><span class="sxs-lookup"><span data-stu-id="ddefc-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="ddefc-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="ddefc-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span><span class="sxs-lookup"><span data-stu-id="ddefc-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="ddefc-325">Also includes any unbilled usage from previous reporting periods.</span><span class="sxs-lookup"><span data-stu-id="ddefc-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="ddefc-326">11</span><span class="sxs-lookup"><span data-stu-id="ddefc-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="ddefc-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="ddefc-328">Units included as part of the offer.</span><span class="sxs-lookup"><span data-stu-id="ddefc-328">Units included as part of the offer.</span></span> <span data-ttu-id="ddefc-329">Not typically present in CSP.</span><span class="sxs-lookup"><span data-stu-id="ddefc-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="ddefc-330">0</span><span class="sxs-lookup"><span data-stu-id="ddefc-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="ddefc-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="ddefc-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="ddefc-332">Units not included as part of the offer, that must be paid for by the partner.</span><span class="sxs-lookup"><span data-stu-id="ddefc-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="ddefc-333">Equal to the ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="ddefc-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="ddefc-334">11</span><span class="sxs-lookup"><span data-stu-id="ddefc-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="ddefc-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="ddefc-336">Offer price in effect at subscription start date.</span><span class="sxs-lookup"><span data-stu-id="ddefc-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="ddefc-337">$0.0808</span><span class="sxs-lookup"><span data-stu-id="ddefc-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="ddefc-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="ddefc-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="ddefc-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ddefc-340">$0.085</span><span class="sxs-lookup"><span data-stu-id="ddefc-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="ddefc-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="ddefc-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span><span class="sxs-lookup"><span data-stu-id="ddefc-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ddefc-343">$0.08</span><span class="sxs-lookup"><span data-stu-id="ddefc-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="ddefc-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="ddefc-345">Total after tax, when tax is applicable.</span><span class="sxs-lookup"><span data-stu-id="ddefc-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="ddefc-346">$0.93</span><span class="sxs-lookup"><span data-stu-id="ddefc-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-347">Currency</span><span class="sxs-lookup"><span data-stu-id="ddefc-347">Currency</span></span></td>
<td><p><span data-ttu-id="ddefc-348">Currency type.</span><span class="sxs-lookup"><span data-stu-id="ddefc-348">Currency type.</span></span> <span data-ttu-id="ddefc-349">Each billing entity has only one currency.</span><span class="sxs-lookup"><span data-stu-id="ddefc-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="ddefc-350">Check that it matches your first invoice and then after any major billing platform update.</span><span class="sxs-lookup"><span data-stu-id="ddefc-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ddefc-351">EUR</span><span class="sxs-lookup"><span data-stu-id="ddefc-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ddefc-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ddefc-353">Pretax price per unit.</span><span class="sxs-lookup"><span data-stu-id="ddefc-353">Pretax price per unit.</span></span> <span data-ttu-id="ddefc-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="ddefc-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ddefc-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="ddefc-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ddefc-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ddefc-357">Post tax price per unit.</span><span class="sxs-lookup"><span data-stu-id="ddefc-357">Post tax price per unit.</span></span> <span data-ttu-id="ddefc-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="ddefc-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ddefc-359">$0.08</span><span class="sxs-lookup"><span data-stu-id="ddefc-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ddefc-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="ddefc-361">The type of charge or adjustment.</span><span class="sxs-lookup"><span data-stu-id="ddefc-361">The type of charge or adjustment.</span></span> <span data-ttu-id="ddefc-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span><span class="sxs-lookup"><span data-stu-id="ddefc-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ddefc-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span><span class="sxs-lookup"><span data-stu-id="ddefc-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="ddefc-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="ddefc-365">Unique account ID in the MSFT billing platform.</span><span class="sxs-lookup"><span data-stu-id="ddefc-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="ddefc-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="ddefc-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="ddefc-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="ddefc-368">Date of service deployment.</span><span class="sxs-lookup"><span data-stu-id="ddefc-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="ddefc-369">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ddefc-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="ddefc-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="ddefc-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span><span class="sxs-lookup"><span data-stu-id="ddefc-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="ddefc-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="ddefc-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="ddefc-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="ddefc-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span><span class="sxs-lookup"><span data-stu-id="ddefc-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="ddefc-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span><span class="sxs-lookup"><span data-stu-id="ddefc-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="ddefc-376">This MeteredService column will indicate to which specific service the usage pertains.</span><span class="sxs-lookup"><span data-stu-id="ddefc-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="ddefc-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="ddefc-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="ddefc-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="ddefc-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span><span class="sxs-lookup"><span data-stu-id="ddefc-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="ddefc-380">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="ddefc-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-381">Project</span><span class="sxs-lookup"><span data-stu-id="ddefc-381">Project</span></span></td>
<td><p><span data-ttu-id="ddefc-382">Customer-defined name for their service instance</span><span class="sxs-lookup"><span data-stu-id="ddefc-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="ddefc-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ddefc-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="ddefc-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="ddefc-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span><span class="sxs-lookup"><span data-stu-id="ddefc-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="ddefc-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span><span class="sxs-lookup"><span data-stu-id="ddefc-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="ddefc-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="ddefc-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ddefc-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="ddefc-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span><span class="sxs-lookup"><span data-stu-id="ddefc-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ddefc-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ddefc-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ddefc-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="ddefc-391">DomainName</span></span></td>
<td><p><span data-ttu-id="ddefc-392">Customer's domain name, used to help identify the customer.</span><span class="sxs-lookup"><span data-stu-id="ddefc-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="ddefc-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ddefc-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="ddefc-394">单位</span><span class="sxs-lookup"><span data-stu-id="ddefc-394">Unit</span></span></td>
<td><p><span data-ttu-id="ddefc-395">资源名称的单位</span><span class="sxs-lookup"><span data-stu-id="ddefc-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="ddefc-396">GB 或小时</span><span class="sxs-lookup"><span data-stu-id="ddefc-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <span data-ttu-id="ddefc-397"><a href="" id="charge_types"></a>映射发票与对帐文件之间的费用</span><span class="sxs-lookup"><span data-stu-id="ddefc-397"><a href="" id="charge_types"></a>Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="ddefc-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="ddefc-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="ddefc-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="ddefc-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="ddefc-400">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span><span class="sxs-lookup"><span data-stu-id="ddefc-400">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="ddefc-401">Invoice charge description</span><span class="sxs-lookup"><span data-stu-id="ddefc-401">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="ddefc-402">Reconciliation file charge description (ChargeType column)</span><span class="sxs-lookup"><span data-stu-id="ddefc-402">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="ddefc-403">What is this charge?</span><span class="sxs-lookup"><span data-stu-id="ddefc-403">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="ddefc-404">How do I map these ChargeTypes to the invoice?</span><span class="sxs-lookup"><span data-stu-id="ddefc-404">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="ddefc-405">Recurring Charges</span><span class="sxs-lookup"><span data-stu-id="ddefc-405">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ddefc-406">Cancel instance prorate</span><span class="sxs-lookup"><span data-stu-id="ddefc-406">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-407">Prorated charges refunded to the customer when associated seats are changed</span><span class="sxs-lookup"><span data-stu-id="ddefc-407">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="ddefc-408">From license-based file, sum the <strong>Amount</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-408">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-409">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="ddefc-409">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-410">Periodic charges for a subscription</span><span class="sxs-lookup"><span data-stu-id="ddefc-410">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-411">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="ddefc-411">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-412">Prorated charges assessed from the customer when associated seats are changed</span><span class="sxs-lookup"><span data-stu-id="ddefc-412">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-413">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="ddefc-413">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-414">Prorated refund for unused portion of service upon cancellation</span><span class="sxs-lookup"><span data-stu-id="ddefc-414">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-415">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="ddefc-415">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-416">Prorated fees upon purchase</span><span class="sxs-lookup"><span data-stu-id="ddefc-416">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-417">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="ddefc-417">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-418">Initial charge for a subscription</span><span class="sxs-lookup"><span data-stu-id="ddefc-418">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-419">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="ddefc-419">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-420">Prorated fees upon subscription renewal</span><span class="sxs-lookup"><span data-stu-id="ddefc-420">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-421">Renew fee</span><span class="sxs-lookup"><span data-stu-id="ddefc-421">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-422">Charge for renewing a subscription</span><span class="sxs-lookup"><span data-stu-id="ddefc-422">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="ddefc-423">Other Products and Services</span><span class="sxs-lookup"><span data-stu-id="ddefc-423">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ddefc-424">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="ddefc-424">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-425">Prorated fees from activation until end of billing period</span><span class="sxs-lookup"><span data-stu-id="ddefc-425">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-426">From license-based file, sum the <strong>Amount</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-426">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="ddefc-427">Usage Charges</span><span class="sxs-lookup"><span data-stu-id="ddefc-427">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ddefc-428">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="ddefc-428">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-429">Access usage fee upon cancellation for unpaid usage during the current billing period</span><span class="sxs-lookup"><span data-stu-id="ddefc-429">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="ddefc-430">From usage-based file, sum the <strong>PretaxCharges</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-430">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-431">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="ddefc-431">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-432">Access usage fee for the current billing period</span><span class="sxs-lookup"><span data-stu-id="ddefc-432">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="ddefc-433">Credits &amp; Adjustments</span><span class="sxs-lookup"><span data-stu-id="ddefc-433">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ddefc-434">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="ddefc-434">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-435">Partial or whole refund to a line item, including taxes</span><span class="sxs-lookup"><span data-stu-id="ddefc-435">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-436">From license-based file, sum the <strong>TotalForCustomer</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-436">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="ddefc-437">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-437">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="ddefc-438">Other Discounts</span><span class="sxs-lookup"><span data-stu-id="ddefc-438">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="ddefc-439">(usage-based)</span><span class="sxs-lookup"><span data-stu-id="ddefc-439">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="ddefc-440">Activation discount</span><span class="sxs-lookup"><span data-stu-id="ddefc-440">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-441">Discount applied when subscription activated</span><span class="sxs-lookup"><span data-stu-id="ddefc-441">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="ddefc-442">From usage-based file, sum the <strong>PretaxCharges</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-442">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-443">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="ddefc-443">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-444">Discount applied on periodic charges</span><span class="sxs-lookup"><span data-stu-id="ddefc-444">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="ddefc-445">Renew discount</span><span class="sxs-lookup"><span data-stu-id="ddefc-445">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-446">Discount applied when subscription renewed</span><span class="sxs-lookup"><span data-stu-id="ddefc-446">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="ddefc-447">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="ddefc-447">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-448">Charges applied when discounts cancelled</span><span class="sxs-lookup"><span data-stu-id="ddefc-448">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="ddefc-449">Other Discounts</span><span class="sxs-lookup"><span data-stu-id="ddefc-449">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="ddefc-450">(license-based)</span><span class="sxs-lookup"><span data-stu-id="ddefc-450">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="ddefc-451">May be applied to multiple charge types</span><span class="sxs-lookup"><span data-stu-id="ddefc-451">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="ddefc-452">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-452">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ddefc-453"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="ddefc-453"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="ddefc-454">May be applied to multiple charge types</span><span class="sxs-lookup"><span data-stu-id="ddefc-454">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="ddefc-455">Exception: "Offset a line item" already includes taxes.</span><span class="sxs-lookup"><span data-stu-id="ddefc-455">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="ddefc-456">See Credits &amp; Adjustments, above.</span><span class="sxs-lookup"><span data-stu-id="ddefc-456">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="ddefc-457">Taxes or value-added taxes (VAT)</span><span class="sxs-lookup"><span data-stu-id="ddefc-457">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="ddefc-458">From license-based file, sum the <strong>Tax</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-458">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="ddefc-459">From usage-based file, sum the <strong>TaxAmount</strong> column</span><span class="sxs-lookup"><span data-stu-id="ddefc-459">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
