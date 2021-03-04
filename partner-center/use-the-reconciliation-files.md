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
ms.openlocfilehash: d927b138c32b3e5f6f5d906db898e17f89a85aae
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755783"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="8aea2-103">了解如何读取伙伴中心对帐文件中的行项</span><span class="sxs-lookup"><span data-stu-id="8aea2-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="8aea2-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="8aea2-104">Applies to:</span></span>

- <span data-ttu-id="8aea2-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8aea2-105">Partner Center</span></span>
- <span data-ttu-id="8aea2-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8aea2-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8aea2-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="8aea2-107">**Appropriate roles**</span></span>

- <span data-ttu-id="8aea2-108">计费管理员</span><span class="sxs-lookup"><span data-stu-id="8aea2-108">Billing admin</span></span>
- <span data-ttu-id="8aea2-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8aea2-109">Global admin</span></span>

<span data-ttu-id="8aea2-110">你可以从合作伙伴中心下载你的对帐文件，以获取计费周期中每个费用的详细的行项目视图。</span><span class="sxs-lookup"><span data-stu-id="8aea2-110">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="8aea2-111">行项详细信息包括每个客户的订阅的费用，以及详细事件 (例如，将许可证添加到订阅) 。</span><span class="sxs-lookup"><span data-stu-id="8aea2-111">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="8aea2-112">有关如何读取 **发票** 的详细信息，请参阅 [阅读帐单](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="8aea2-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="8aea2-113">了解协调文件字段</span><span class="sxs-lookup"><span data-stu-id="8aea2-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="8aea2-114">基于许可证的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="8aea2-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="8aea2-115">基于用量的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="8aea2-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="8aea2-116">每日分级用量对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="8aea2-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="8aea2-117">一次性购买 CSP 对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="8aea2-117">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="8aea2-118">了解对帐文件中的费用类型</span><span class="sxs-lookup"><span data-stu-id="8aea2-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="8aea2-119">若要了解 **ChargeType** 列)  (对帐文件中的费用类型，请参阅 [对帐文件费用类型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="8aea2-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="8aea2-120">解决格式问题</span><span class="sxs-lookup"><span data-stu-id="8aea2-120">Fix formatting issues</span></span>

<span data-ttu-id="8aea2-121">有时，对帐文件可能包含格式设置问题。</span><span class="sxs-lookup"><span data-stu-id="8aea2-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="8aea2-122">例如，如果不使用 en-us 区域设置，则可能出现此问题。</span><span class="sxs-lookup"><span data-stu-id="8aea2-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="8aea2-123">请按照以下步骤修复对帐文件中的任何格式设置问题：</span><span class="sxs-lookup"><span data-stu-id="8aea2-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="8aea2-124">在 Microsoft Excel 中打开 (为 .csv 格式的协调文件) 。</span><span class="sxs-lookup"><span data-stu-id="8aea2-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="8aea2-125">选择该文件中的第一列。</span><span class="sxs-lookup"><span data-stu-id="8aea2-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="8aea2-126">打开 " **将文本转换为列" 向导**。</span><span class="sxs-lookup"><span data-stu-id="8aea2-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="8aea2-127">在功能区上，选择 " **数据**"，然后选择 " **文本到列**"。</span><span class="sxs-lookup"><span data-stu-id="8aea2-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="8aea2-128">在向导中，选择 " **带分隔符的文件类型**"。</span><span class="sxs-lookup"><span data-stu-id="8aea2-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="8aea2-129">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="8aea2-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="8aea2-130">在 " **分隔符** " 字段中，选择 " **逗号**"。</span><span class="sxs-lookup"><span data-stu-id="8aea2-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="8aea2-131"> (如果已选择 **选项卡** ，则可以选择此选项。 ) 然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="8aea2-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="8aea2-132">在 " **列数据格式** " 字段中，选择 **Date： MDY**。</span><span class="sxs-lookup"><span data-stu-id="8aea2-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="8aea2-133">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="8aea2-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="8aea2-134">在 " **列数据格式** " 字段中，选择 "所有金额列的 **文本** "。</span><span class="sxs-lookup"><span data-stu-id="8aea2-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="8aea2-135">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="8aea2-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="8aea2-136">以编程方式下载对帐文件</span><span class="sxs-lookup"><span data-stu-id="8aea2-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="8aea2-137">协调文件可能非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="8aea2-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="8aea2-138">若要以编程方式下载对帐文件，请参阅 [获取发票行项](/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="8aea2-138">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="8aea2-139">映射税金或 VAT</span><span class="sxs-lookup"><span data-stu-id="8aea2-139">Map taxes or VAT</span></span>

<span data-ttu-id="8aea2-140">若要将增值税或销售税 (增值税) 映射到发票：</span><span class="sxs-lookup"><span data-stu-id="8aea2-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="8aea2-141">对基于许可证的文件中的 **税务** 列求和。</span><span class="sxs-lookup"><span data-stu-id="8aea2-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="8aea2-142">在基于使用情况的文件中对 **TaxAmount** 列求和。</span><span class="sxs-lookup"><span data-stu-id="8aea2-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="8aea2-143">按合作伙伴列举帐文件</span><span class="sxs-lookup"><span data-stu-id="8aea2-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="8aea2-144">**间接模型** 中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些附加字段，按经销商对文件进行详细列举。</span><span class="sxs-lookup"><span data-stu-id="8aea2-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="8aea2-145">MPN ID</span><span class="sxs-lookup"><span data-stu-id="8aea2-145">MPN ID</span></span> | <span data-ttu-id="8aea2-146">说明</span><span class="sxs-lookup"><span data-stu-id="8aea2-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="8aea2-147">MPN ID</span><span class="sxs-lookup"><span data-stu-id="8aea2-147">MPN ID</span></span> | <span data-ttu-id="8aea2-148">Microsoft 合作伙伴网络 (MPN) 云解决方案提供程序的标识符 (CSP) 直接或间接 (。</span><span class="sxs-lookup"><span data-stu-id="8aea2-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="8aea2-149">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="8aea2-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="8aea2-150">[订阅的记录分销商的 MPN 标识符](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="8aea2-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="8aea2-151">此字段对应于 "合作伙伴中心" 中为特定订阅列出的分销商 ID。</span><span class="sxs-lookup"><span data-stu-id="8aea2-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="8aea2-152">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="8aea2-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="8aea2-153">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="8aea2-153">Reseller MPN ID</span></span>

<span data-ttu-id="8aea2-154">如果 CSP 合作伙伴将订阅直接销售给客户，则其 **MPN id** 将列出两次，同时作为 **MPN ID** 和 **经销商 MPN ID**。</span><span class="sxs-lookup"><span data-stu-id="8aea2-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="8aea2-155">如果 CSP 合作伙伴的分销商没有 **MPN id**，则此值将改为设置为合作伙伴的 **MPN id** 。</span><span class="sxs-lookup"><span data-stu-id="8aea2-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="8aea2-156">如果 CSP 合作伙伴删除了 **经销商 MPN ID**，此值将设置为 *-1*。</span><span class="sxs-lookup"><span data-stu-id="8aea2-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="8aea2-157">查看或更新 **经销商 MPN ID**：</span><span class="sxs-lookup"><span data-stu-id="8aea2-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="8aea2-158">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="8aea2-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="8aea2-159">在 "合作伙伴中心" 菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="8aea2-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="8aea2-160">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="8aea2-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="8aea2-161">在 customer 菜单中，选择 " **订阅**"。</span><span class="sxs-lookup"><span data-stu-id="8aea2-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="8aea2-162">从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="8aea2-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="8aea2-163">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="8aea2-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8aea2-164">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8aea2-164">Next steps</span></span>

- [<span data-ttu-id="8aea2-165">如何读取帐单 & 侦测文件</span><span class="sxs-lookup"><span data-stu-id="8aea2-165">How to read your bill & recon file</span></span>](read-your-bill.md) 