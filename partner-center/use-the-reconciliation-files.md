---
title: 使用你的对帐文件
ms.topic: article
ms.date: 06/08/2020
description: 了解合作伙伴中心中的对帐文件以及如何解释给定计费周期的详细的行项视图。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05939dc5edaddeb2f74b3b75017e2062dff25e31
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468328"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="6d9fa-103">了解如何读取伙伴中心对帐文件中的行项</span><span class="sxs-lookup"><span data-stu-id="6d9fa-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="6d9fa-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="6d9fa-104">Applies to:</span></span>

- <span data-ttu-id="6d9fa-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6d9fa-105">Partner Center</span></span>
- <span data-ttu-id="6d9fa-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="6d9fa-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6d9fa-107">你可以从合作伙伴中心下载你的对帐文件，以获取计费周期中每个费用的详细的行项目视图。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="6d9fa-108">行项详细信息包括每个客户的订阅的费用，以及详细事件（例如，将许可证添加到订阅中）。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="6d9fa-109">适当的角色：</span><span class="sxs-lookup"><span data-stu-id="6d9fa-109">Appropriate roles:</span></span>

- <span data-ttu-id="6d9fa-110">计费管理员</span><span class="sxs-lookup"><span data-stu-id="6d9fa-110">Billing admin</span></span>
- <span data-ttu-id="6d9fa-111">全局管理员</span><span class="sxs-lookup"><span data-stu-id="6d9fa-111">Global admin</span></span>

<span data-ttu-id="6d9fa-112">有关如何读取**发票**的详细信息，请参阅[阅读帐单](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="6d9fa-113">了解协调文件字段</span><span class="sxs-lookup"><span data-stu-id="6d9fa-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="6d9fa-114">基于许可证的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="6d9fa-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="6d9fa-115">基于使用情况的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="6d9fa-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="6d9fa-116">每日分级使用情况协调文件字段</span><span class="sxs-lookup"><span data-stu-id="6d9fa-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="6d9fa-117">了解对帐文件中的费用类型</span><span class="sxs-lookup"><span data-stu-id="6d9fa-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="6d9fa-118">若要了解对帐文件（ **ChargeType**列）中的费用类型，请参阅[对帐文件费用类型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="6d9fa-119">解决格式问题</span><span class="sxs-lookup"><span data-stu-id="6d9fa-119">Fix formatting issues</span></span>

<span data-ttu-id="6d9fa-120">有时，对帐文件可能包含格式设置问题。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="6d9fa-121">例如，如果不使用 en-us 区域设置，则可能出现此问题。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="6d9fa-122">请按照以下步骤修复对帐文件中的任何格式设置问题：</span><span class="sxs-lookup"><span data-stu-id="6d9fa-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="6d9fa-123">在 Microsoft Excel 中打开对帐文件（采用 .csv 格式）。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="6d9fa-124">选择该文件中的第一列。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="6d9fa-125">打开 "**将文本转换为列" 向导**。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="6d9fa-126">在功能区上，选择 "**数据**"，然后选择 "**文本到列**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="6d9fa-127">在向导中，选择 "**带分隔符的文件类型**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="6d9fa-128">然后，选择“下一步”。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="6d9fa-129">在 "**分隔符**" 字段中，选择 "**逗号**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="6d9fa-130">（如果已选择**选项卡**，则可以选择此选项。）然后选择 "**下一步**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="6d9fa-131">在 "**列数据格式**" 字段中，选择**Date： MDY**。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="6d9fa-132">然后，选择“下一步”。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="6d9fa-133">在 "**列数据格式**" 字段中，选择 "所有金额列的**文本**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="6d9fa-134">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="6d9fa-135">以编程方式下载对帐文件</span><span class="sxs-lookup"><span data-stu-id="6d9fa-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="6d9fa-136">协调文件可能非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="6d9fa-137">若要以编程方式下载对帐文件，请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-137">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="6d9fa-138">映射税金或 VAT</span><span class="sxs-lookup"><span data-stu-id="6d9fa-138">Map taxes or VAT</span></span>

<span data-ttu-id="6d9fa-139">若要为发票映射税金或增值税（VAT）：</span><span class="sxs-lookup"><span data-stu-id="6d9fa-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="6d9fa-140">对基于许可证的文件中的**税务**列求和。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="6d9fa-141">在基于使用情况的文件中对**TaxAmount**列求和。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="6d9fa-142">按合作伙伴列举帐文件</span><span class="sxs-lookup"><span data-stu-id="6d9fa-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="6d9fa-143">**间接模型**中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些附加字段，按经销商对文件进行详细列举。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="6d9fa-144">MPN ID</span><span class="sxs-lookup"><span data-stu-id="6d9fa-144">MPN ID</span></span> | <span data-ttu-id="6d9fa-145">描述</span><span class="sxs-lookup"><span data-stu-id="6d9fa-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6d9fa-146">MPN ID</span><span class="sxs-lookup"><span data-stu-id="6d9fa-146">MPN ID</span></span> | <span data-ttu-id="6d9fa-147">云解决方案提供商（CSP）合作伙伴的 Microsoft 合作伙伴网络（MPN）标识符（直接或间接）。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="6d9fa-148">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="6d9fa-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="6d9fa-149">[订阅的记录分销商的 MPN 标识符](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="6d9fa-150">此字段对应于 "合作伙伴中心" 中为特定订阅列出的分销商 ID。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="6d9fa-151">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="6d9fa-152">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="6d9fa-152">Reseller MPN ID</span></span>

<span data-ttu-id="6d9fa-153">如果 CSP 合作伙伴将订阅直接销售给客户，则其**MPN id**将列出两次，同时作为**MPN ID**和**经销商 MPN ID**。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="6d9fa-154">如果 CSP 合作伙伴的分销商没有**MPN id**，则此值将改为设置为合作伙伴的**MPN id** 。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="6d9fa-155">如果 CSP 合作伙伴删除了**经销商 MPN ID**，此值将设置为 *-1*。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="6d9fa-156">查看或更新**经销商 MPN ID**：</span><span class="sxs-lookup"><span data-stu-id="6d9fa-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="6d9fa-157">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6d9fa-158">在 "合作伙伴中心" 菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="6d9fa-159">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="6d9fa-160">在 customer 菜单中，选择 "**订阅**"。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="6d9fa-161">从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="6d9fa-162">选择“更新”\*\*\*\* 以更改“经销商 (MPN ID)”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="6d9fa-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>
