---
title: 使用你的对帐文件
ms.topic: article
ms.date: 03/10/2021
description: 了解合作伙伴中心中的对帐文件以及如何解释给定计费周期的详细的行项视图。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022768"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="09016-103">了解如何读取伙伴中心对帐文件中的行项</span><span class="sxs-lookup"><span data-stu-id="09016-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="09016-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="09016-104">**Appropriate roles**</span></span>

- <span data-ttu-id="09016-105">计费管理员</span><span class="sxs-lookup"><span data-stu-id="09016-105">Billing admin</span></span>
- <span data-ttu-id="09016-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="09016-106">Global admin</span></span>

<span data-ttu-id="09016-107">你可以从合作伙伴中心下载你的对帐文件，以获取计费周期中每个费用的详细的行项目视图。</span><span class="sxs-lookup"><span data-stu-id="09016-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="09016-108">行项详细信息包括每个客户的订阅的费用，以及详细事件 (例如，将许可证添加到订阅) 。</span><span class="sxs-lookup"><span data-stu-id="09016-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="09016-109">有关如何读取 **发票** 的详细信息，请参阅 [阅读帐单](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="09016-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="09016-110">了解协调文件字段</span><span class="sxs-lookup"><span data-stu-id="09016-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="09016-111">基于许可证的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="09016-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="09016-112">基于用量的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="09016-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="09016-113">每日分级用量对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="09016-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="09016-114">一次性购买 CSP 对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="09016-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="09016-115">了解对帐文件中的费用类型</span><span class="sxs-lookup"><span data-stu-id="09016-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="09016-116">若要了解 **ChargeType** 列)  (对帐文件中的费用类型，请参阅 [对帐文件费用类型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="09016-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="09016-117">解决格式问题</span><span class="sxs-lookup"><span data-stu-id="09016-117">Fix formatting issues</span></span>

<span data-ttu-id="09016-118">有时，对帐文件可能包含格式设置问题。</span><span class="sxs-lookup"><span data-stu-id="09016-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="09016-119">例如，如果不使用 en-us 区域设置，则可能出现此问题。</span><span class="sxs-lookup"><span data-stu-id="09016-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="09016-120">请按照以下步骤修复对帐文件中的任何格式设置问题：</span><span class="sxs-lookup"><span data-stu-id="09016-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="09016-121">在 Microsoft Excel 中打开 (为 .csv 格式的协调文件) 。</span><span class="sxs-lookup"><span data-stu-id="09016-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="09016-122">选择该文件中的第一列。</span><span class="sxs-lookup"><span data-stu-id="09016-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="09016-123">打开 " **将文本转换为列" 向导**。</span><span class="sxs-lookup"><span data-stu-id="09016-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="09016-124">在功能区上，选择 " **数据**"，然后选择 " **文本到列**"。</span><span class="sxs-lookup"><span data-stu-id="09016-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="09016-125">在向导中，选择 " **带分隔符的文件类型**"。</span><span class="sxs-lookup"><span data-stu-id="09016-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="09016-126">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="09016-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="09016-127">在 " **分隔符** " 字段中，选择 " **逗号**"。</span><span class="sxs-lookup"><span data-stu-id="09016-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="09016-128"> (如果已选择 **选项卡** ，则可以选择此选项。 ) 然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="09016-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="09016-129">在 " **列数据格式** " 字段中，选择 **Date： MDY**。</span><span class="sxs-lookup"><span data-stu-id="09016-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="09016-130">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="09016-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="09016-131">在 " **列数据格式** " 字段中，选择 "所有金额列的 **文本** "。</span><span class="sxs-lookup"><span data-stu-id="09016-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="09016-132">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="09016-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="09016-133">以编程方式下载对帐文件</span><span class="sxs-lookup"><span data-stu-id="09016-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="09016-134">协调文件可能非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="09016-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="09016-135">若要以编程方式下载对帐文件，请参阅 [获取发票行项](/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="09016-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="09016-136">映射税金或 VAT</span><span class="sxs-lookup"><span data-stu-id="09016-136">Map taxes or VAT</span></span>

<span data-ttu-id="09016-137">若要将增值税或销售税 (增值税) 映射到发票：</span><span class="sxs-lookup"><span data-stu-id="09016-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="09016-138">对基于许可证的文件中的 **税务** 列求和。</span><span class="sxs-lookup"><span data-stu-id="09016-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="09016-139">在基于使用情况的文件中对 **TaxAmount** 列求和。</span><span class="sxs-lookup"><span data-stu-id="09016-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="09016-140">按合作伙伴列举帐文件</span><span class="sxs-lookup"><span data-stu-id="09016-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="09016-141">**间接模型** 中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些附加字段，按经销商对文件进行详细列举。</span><span class="sxs-lookup"><span data-stu-id="09016-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="09016-142">MPN ID</span><span class="sxs-lookup"><span data-stu-id="09016-142">MPN ID</span></span> | <span data-ttu-id="09016-143">描述</span><span class="sxs-lookup"><span data-stu-id="09016-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="09016-144">MPN ID</span><span class="sxs-lookup"><span data-stu-id="09016-144">MPN ID</span></span> | <span data-ttu-id="09016-145">Microsoft 合作伙伴网络 (MPN) 云解决方案提供程序的标识符 (CSP) 直接或间接 (。</span><span class="sxs-lookup"><span data-stu-id="09016-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="09016-146">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="09016-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="09016-147">[订阅的记录分销商的 MPN 标识符](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="09016-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="09016-148">此字段对应于 "合作伙伴中心" 中为特定订阅列出的分销商 ID。</span><span class="sxs-lookup"><span data-stu-id="09016-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="09016-149">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="09016-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="09016-150">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="09016-150">Reseller MPN ID</span></span>

<span data-ttu-id="09016-151">如果 CSP 合作伙伴将订阅直接销售给客户，则其 **MPN id** 将列出两次，同时作为 **MPN ID** 和 **经销商 MPN ID**。</span><span class="sxs-lookup"><span data-stu-id="09016-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="09016-152">如果 CSP 合作伙伴的分销商没有 **MPN id**，则此值将改为设置为合作伙伴的 **MPN id** 。</span><span class="sxs-lookup"><span data-stu-id="09016-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="09016-153">如果 CSP 合作伙伴删除了 **经销商 MPN ID**，此值将设置为 *-1*。</span><span class="sxs-lookup"><span data-stu-id="09016-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="09016-154">查看或更新 **经销商 MPN ID**：</span><span class="sxs-lookup"><span data-stu-id="09016-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="09016-155">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="09016-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="09016-156">在 "合作伙伴中心" 菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="09016-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="09016-157">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="09016-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="09016-158">在 customer 菜单中，选择 " **订阅**"。</span><span class="sxs-lookup"><span data-stu-id="09016-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="09016-159">从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="09016-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="09016-160">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="09016-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="09016-161">后续步骤</span><span class="sxs-lookup"><span data-stu-id="09016-161">Next steps</span></span>

- [<span data-ttu-id="09016-162">如何读取帐单 & 侦测文件</span><span class="sxs-lookup"><span data-stu-id="09016-162">How to read your bill & recon file</span></span>](read-your-bill.md) 