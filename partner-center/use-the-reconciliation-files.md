---
title: 使用你的对帐文件
ms.topic: article
ms.date: 03/26/2021
description: 了解合作伙伴中心中的对帐文件以及如何解释给定计费周期的详细的行项视图。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633890"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="7aaf6-103">了解如何读取伙伴中心对帐文件中的行项</span><span class="sxs-lookup"><span data-stu-id="7aaf6-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="7aaf6-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="7aaf6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7aaf6-105">计费管理员</span><span class="sxs-lookup"><span data-stu-id="7aaf6-105">Billing admin</span></span>
- <span data-ttu-id="7aaf6-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7aaf6-106">Global admin</span></span>

<span data-ttu-id="7aaf6-107">你可以从合作伙伴中心下载你的对帐文件，以获取计费周期中每个费用的详细的行项目视图。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="7aaf6-108">行项详细信息包括每个客户的订阅的费用，以及详细事件 (例如，将许可证添加到订阅) 。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="7aaf6-109">有关如何读取 **发票** 的详细信息，请参阅 [阅读帐单](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="7aaf6-110">了解协调文件字段</span><span class="sxs-lookup"><span data-stu-id="7aaf6-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="7aaf6-111">基于许可证的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="7aaf6-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="7aaf6-112">基于用量的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="7aaf6-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="7aaf6-113">每日分级用量对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="7aaf6-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="7aaf6-114">一次性购买 CSP 对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="7aaf6-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="7aaf6-115">了解对帐文件中的费用类型</span><span class="sxs-lookup"><span data-stu-id="7aaf6-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="7aaf6-116">若要了解 **ChargeType** 列)  (对帐文件中的费用类型，请参阅 [对帐文件费用类型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="7aaf6-117">解决格式问题</span><span class="sxs-lookup"><span data-stu-id="7aaf6-117">Fix formatting issues</span></span>

<span data-ttu-id="7aaf6-118">有时，对帐文件可能包含格式设置问题。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="7aaf6-119">例如，如果不使用 en-us 区域设置，则可能出现此问题。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="7aaf6-120">请按照以下步骤修复对帐文件中的任何格式设置问题：</span><span class="sxs-lookup"><span data-stu-id="7aaf6-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="7aaf6-121">在 Microsoft Excel 中打开 (为 .csv 格式的协调文件) 。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="7aaf6-122">选择该文件中的第一列。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="7aaf6-123">打开 " **将文本转换为列" 向导**。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="7aaf6-124">在功能区上，选择 " **数据**"，然后选择 " **文本到列**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="7aaf6-125">在向导中，选择 " **带分隔符的文件类型**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="7aaf6-126">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="7aaf6-127">在 " **分隔符** " 字段中，选择 " **逗号**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="7aaf6-128"> (如果已选择 **选项卡** ，则可以选择此选项。 ) 然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="7aaf6-129">在 " **列数据格式** " 字段中，选择 **Date： MDY**。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="7aaf6-130">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="7aaf6-131">在 " **列数据格式** " 字段中，选择 "所有金额列的 **文本** "。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="7aaf6-132">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="7aaf6-133">以编程方式下载对帐文件</span><span class="sxs-lookup"><span data-stu-id="7aaf6-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="7aaf6-134">协调文件可能非常大，有时很难下载。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="7aaf6-135">若要以编程方式下载对帐文件，请参阅 [获取发票行项](/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="7aaf6-136">如果文件超出 Excel 中的行限制</span><span class="sxs-lookup"><span data-stu-id="7aaf6-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="7aaf6-137">如果能够下载并不在 Microsoft Excel 中打开对帐文件，这可能意味着该文件包含的行数超过了 Excel 所允许的数目。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="7aaf6-138">如果发生这种情况，可以使用以下任一过程打开文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="7aaf6-139">在 Power BI 中打开侦测文件</span><span class="sxs-lookup"><span data-stu-id="7aaf6-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="7aaf6-140">按常规方式下载协调文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="7aaf6-141">下载、安装和打开 Power BI 的实例。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="7aaf6-142">在 Power BI **主页** "选项卡上，选择" **获取数据**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="7aaf6-143">在 **公共数据源** 列表中，选择 " **Text/CSV**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="7aaf6-144">出现提示时，打开侦测文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="7aaf6-145">在 Excel 数据透视表中打开侦测文件</span><span class="sxs-lookup"><span data-stu-id="7aaf6-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="7aaf6-146">按常规方式下载协调文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="7aaf6-147">在 Microsoft Excel 中打开新文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="7aaf6-148">在 " **数据** " 选项卡上，选择 " **获取数据**"，选择 " **从文件**"，然后选择 " **文本/CSV**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="7aaf6-149">出现提示时，打开侦测文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-149">When prompted, open your recon file.</span></span> <span data-ttu-id="7aaf6-150">你的数据将会显示。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-150">Your data will appear.</span></span>
5. <span data-ttu-id="7aaf6-151">在 " **加载** " 下拉菜单中，选择 " **加载到**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="7aaf6-152">在 " **导入数据** " 对话框中，选择 " **数据透视表** " 以打开文件。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="7aaf6-153">映射税金或 VAT</span><span class="sxs-lookup"><span data-stu-id="7aaf6-153">Map taxes or VAT</span></span>

<span data-ttu-id="7aaf6-154">若要将增值税或销售税 (增值税) 映射到发票：</span><span class="sxs-lookup"><span data-stu-id="7aaf6-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="7aaf6-155">对基于许可证的文件中的 **税务** 列求和。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="7aaf6-156">在基于使用情况的文件中对 **TaxAmount** 列求和。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="7aaf6-157">按合作伙伴列举帐文件</span><span class="sxs-lookup"><span data-stu-id="7aaf6-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="7aaf6-158">**间接模型** 中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些附加字段，按经销商对文件进行详细列举。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="7aaf6-159">MPN ID</span><span class="sxs-lookup"><span data-stu-id="7aaf6-159">MPN ID</span></span> | <span data-ttu-id="7aaf6-160">说明</span><span class="sxs-lookup"><span data-stu-id="7aaf6-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="7aaf6-161">MPN ID</span><span class="sxs-lookup"><span data-stu-id="7aaf6-161">MPN ID</span></span> | <span data-ttu-id="7aaf6-162">Microsoft 合作伙伴网络 (MPN) 云解决方案提供程序的标识符 (CSP) 直接或间接 (。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="7aaf6-163">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="7aaf6-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="7aaf6-164">[订阅的记录分销商的 MPN 标识符](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="7aaf6-165">此字段对应于 "合作伙伴中心" 中为特定订阅列出的分销商 ID。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="7aaf6-166">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="7aaf6-167">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="7aaf6-167">Reseller MPN ID</span></span>

<span data-ttu-id="7aaf6-168">如果 CSP 合作伙伴将订阅直接销售给客户，则其 **MPN id** 将列出两次，同时作为 **MPN ID** 和 **经销商 MPN ID**。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="7aaf6-169">如果 CSP 合作伙伴的分销商没有 **MPN id**，则此值将改为设置为合作伙伴的 **MPN id** 。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="7aaf6-170">如果 CSP 合作伙伴删除了 **经销商 MPN ID**，此值将设置为 *-1*。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="7aaf6-171">查看或更新 **经销商 MPN ID**：</span><span class="sxs-lookup"><span data-stu-id="7aaf6-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="7aaf6-172">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="7aaf6-173">在 "合作伙伴中心" 菜单中，选择 " **客户**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="7aaf6-174">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="7aaf6-175">在 customer 菜单中，选择 " **订阅**"。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="7aaf6-176">从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="7aaf6-177">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="7aaf6-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7aaf6-178">后续步骤</span><span class="sxs-lookup"><span data-stu-id="7aaf6-178">Next steps</span></span>

- [<span data-ttu-id="7aaf6-179">如何读取帐单 & 侦测文件</span><span class="sxs-lookup"><span data-stu-id="7aaf6-179">How to read your bill & recon file</span></span>](read-your-bill.md) 