---
title: 使用对帐文件
ms.topic: article
ms.date: 03/26/2021
description: 了解计费周期中的对帐合作伙伴中心以及如何解释给定计费周期的费用的详细行项视图。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431568"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="493f5-103">了解如何读取对帐文件中合作伙伴中心项</span><span class="sxs-lookup"><span data-stu-id="493f5-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="493f5-104">**适当的角色**：计费管理员|全局管理员</span><span class="sxs-lookup"><span data-stu-id="493f5-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="493f5-105">可以从计费周期合作伙伴中心下载对帐文件，获取计费周期中每个费用的详细行项视图。</span><span class="sxs-lookup"><span data-stu-id="493f5-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="493f5-106">行项详细信息包括每个客户订阅的费用，以及详细的事件 (例如，将许可证短期添加到订阅) 。</span><span class="sxs-lookup"><span data-stu-id="493f5-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="493f5-107">若要了解如何读取发票 **，请参阅**[阅读帐单](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="493f5-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="493f5-108">了解对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="493f5-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="493f5-109">基于许可证的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="493f5-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="493f5-110">基于用量的对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="493f5-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="493f5-111">每日分级用量对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="493f5-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="493f5-112">一次购买 CSP 对帐文件字段</span><span class="sxs-lookup"><span data-stu-id="493f5-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="493f5-113">了解对帐文件中的费用类型</span><span class="sxs-lookup"><span data-stu-id="493f5-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="493f5-114">若要了解 **"ChargeType"** 列 (中的费用) ，请参阅 [对帐文件费用类型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="493f5-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="493f5-115">修复格式设置问题</span><span class="sxs-lookup"><span data-stu-id="493f5-115">Fix formatting issues</span></span>

<span data-ttu-id="493f5-116">有时，对帐文件可能包含格式设置问题。</span><span class="sxs-lookup"><span data-stu-id="493f5-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="493f5-117">例如，如果未使用 en-US 区域设置，则可能会出现此问题。</span><span class="sxs-lookup"><span data-stu-id="493f5-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="493f5-118">请按照以下步骤修复对帐文件的任何格式设置问题：</span><span class="sxs-lookup"><span data-stu-id="493f5-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="493f5-119">在 Microsoft Excel (以.csv格式) 对帐文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="493f5-120">选择文件的第一列。</span><span class="sxs-lookup"><span data-stu-id="493f5-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="493f5-121">打开"**将文本转换为列向导"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="493f5-122">在功能区上，选择 **"数据"，** 然后选择"**文本到列"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="493f5-123">在向导中，选择 **"分隔的文件类型"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="493f5-124">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="493f5-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="493f5-125">在"**分隔符"字段中**，选择"**逗号"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="493f5-126"> (**选项卡** 已选中，可以将此选项保留为选中状态。) ，然后选择"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="493f5-127">在"**列数据格式"字段中**，选择 **"日期：MDY"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="493f5-128">然后，选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="493f5-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="493f5-129">在" **列数据格式"字段中** ， **选择"所有金额** 列的文本"。</span><span class="sxs-lookup"><span data-stu-id="493f5-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="493f5-130">然后选择“完成”。</span><span class="sxs-lookup"><span data-stu-id="493f5-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="493f5-131">以编程方式下载对帐文件</span><span class="sxs-lookup"><span data-stu-id="493f5-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="493f5-132">对帐文件可能非常大，有时难以下载。</span><span class="sxs-lookup"><span data-stu-id="493f5-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="493f5-133">若要以编程方式下载对帐文件，请参阅 [获取发票行项](/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="493f5-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="493f5-134">如果文件超出 Excel 中的行限制</span><span class="sxs-lookup"><span data-stu-id="493f5-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="493f5-135">如果能够下载对帐文件，但没有在 Microsoft Excel 中打开它，这可能意味着该文件包含的行数超过了 Excel 允许的行数。</span><span class="sxs-lookup"><span data-stu-id="493f5-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="493f5-136">如果发生这种情况，可以使用以下任一过程打开文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="493f5-137">在 Power BI</span><span class="sxs-lookup"><span data-stu-id="493f5-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="493f5-138">像平时一样下载对帐文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="493f5-139">下载、安装并打开 Microsoft Power BI。</span><span class="sxs-lookup"><span data-stu-id="493f5-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="493f5-140">在 **"Power BI"选项卡上**，选择"**获取数据"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="493f5-141">在"常见 **数据源"列表中，选择**"**文本/CSV"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="493f5-142">系统提示时，打开 recon 文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="493f5-143">在 Excel 透视表中打开 recon 文件</span><span class="sxs-lookup"><span data-stu-id="493f5-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="493f5-144">像平时一样下载对帐文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="493f5-145">在 Microsoft Excel 中打开新文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="493f5-146">在"**数据"** 选项卡上，**选择"获取数据**"，选择"**从文件"，** 然后选择"**文本/CSV"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="493f5-147">系统提示时，打开 recon 文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-147">When prompted, open your recon file.</span></span> <span data-ttu-id="493f5-148">将显示数据。</span><span class="sxs-lookup"><span data-stu-id="493f5-148">Your data will appear.</span></span>
5. <span data-ttu-id="493f5-149">在"**加载"** 下拉菜单中，选择"**加载到**"，然后选择"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="493f5-150">在" **导入数据"** 对话框中，选择 **"数据透视表报表** "以打开文件。</span><span class="sxs-lookup"><span data-stu-id="493f5-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="493f5-151">显示的负数</span><span class="sxs-lookup"><span data-stu-id="493f5-151">Negative amount displayed</span></span>

<span data-ttu-id="493f5-152">对帐文件中可能会看到负数。</span><span class="sxs-lookup"><span data-stu-id="493f5-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="493f5-153">此问题的原因如下：</span><span class="sxs-lookup"><span data-stu-id="493f5-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="493f5-154">你最近取消了或减少了许可证数</span><span class="sxs-lookup"><span data-stu-id="493f5-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="493f5-155">你收到了服务许可协议和 SLA (或) Azure 消耗的额度</span><span class="sxs-lookup"><span data-stu-id="493f5-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="493f5-156">若要获取有关此事务的详细信息，请在对帐文件中查看其费用类型属性。</span><span class="sxs-lookup"><span data-stu-id="493f5-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="493f5-157">地图税或增值税</span><span class="sxs-lookup"><span data-stu-id="493f5-157">Map taxes or VAT</span></span>

<span data-ttu-id="493f5-158">若要将增值税或增值税 (增值税) 映射到发票：</span><span class="sxs-lookup"><span data-stu-id="493f5-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="493f5-159">基于许可证的文件中" **税务** "列的总和。</span><span class="sxs-lookup"><span data-stu-id="493f5-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="493f5-160">基于 **使用情况的文件的 TaxAmount** 列的总和。</span><span class="sxs-lookup"><span data-stu-id="493f5-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="493f5-161">按合作伙伴对帐文件进行项化</span><span class="sxs-lookup"><span data-stu-id="493f5-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="493f5-162">间接模型中 **的合作伙伴可以在** 基于许可证和基于使用情况的对帐文件中使用这些附加字段按经销商对文件进行项化。</span><span class="sxs-lookup"><span data-stu-id="493f5-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="493f5-163">MPN ID</span><span class="sxs-lookup"><span data-stu-id="493f5-163">MPN ID</span></span> | <span data-ttu-id="493f5-164">说明</span><span class="sxs-lookup"><span data-stu-id="493f5-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="493f5-165">MPN ID</span><span class="sxs-lookup"><span data-stu-id="493f5-165">MPN ID</span></span> | <span data-ttu-id="493f5-166">MICROSOFT 合作伙伴网络 (CSP) 合作伙伴云解决方案提供商 (的) MPN (标识符) 。</span><span class="sxs-lookup"><span data-stu-id="493f5-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="493f5-167">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="493f5-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="493f5-168">订阅 [的记录经销商的 MPN 标识符](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="493f5-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="493f5-169">此字段对应于为订阅中列出的特定订阅的经销商 ID 合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="493f5-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="493f5-170">仅显示在间接模型中合作伙伴的对帐文件上。</span><span class="sxs-lookup"><span data-stu-id="493f5-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="493f5-171">经销商 MPN ID</span><span class="sxs-lookup"><span data-stu-id="493f5-171">Reseller MPN ID</span></span>

<span data-ttu-id="493f5-172">如果 CSP 合作伙伴直接向客户销售订阅，则其 **MPN ID** 将列出两次，即 **MPN ID** 和经销商 **MPN ID**。</span><span class="sxs-lookup"><span data-stu-id="493f5-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="493f5-173">如果 CSP 合作伙伴的经销商没有 **MPN ID，** 则此值改为设置为合作伙伴的 **MPN ID。**</span><span class="sxs-lookup"><span data-stu-id="493f5-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="493f5-174">如果 CSP 合作伙伴删除了经销商 **MPN ID，** 则此值将设置为 *-1。*</span><span class="sxs-lookup"><span data-stu-id="493f5-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="493f5-175">查看或更新经销商 **MPN ID：**</span><span class="sxs-lookup"><span data-stu-id="493f5-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="493f5-176">登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="493f5-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="493f5-177">在"合作伙伴中心菜单中，选择"客户 **"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="493f5-178">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="493f5-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="493f5-179">在客户菜单中，选择"**订阅"。**</span><span class="sxs-lookup"><span data-stu-id="493f5-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="493f5-180">从列表中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="493f5-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="493f5-181">选择“更新”以更改“经销商 (MPN ID)”。</span><span class="sxs-lookup"><span data-stu-id="493f5-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="493f5-182">后续步骤</span><span class="sxs-lookup"><span data-stu-id="493f5-182">Next steps</span></span>

- [<span data-ttu-id="493f5-183">如何读取帐单&对帐文件</span><span class="sxs-lookup"><span data-stu-id="493f5-183">How to read your bill & recon file</span></span>](read-your-bill.md) 