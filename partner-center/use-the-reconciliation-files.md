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
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>了解如何读取对帐文件中合作伙伴中心项

**适当的角色**：计费管理员|全局管理员

可以从计费周期合作伙伴中心下载对帐文件，获取计费周期中每个费用的详细行项视图。 行项详细信息包括每个客户订阅的费用，以及详细的事件 (例如，将许可证短期添加到订阅) 。

若要了解如何读取发票 **，请参阅**[阅读帐单](read-your-bill.md)。

## <a name="understand-reconciliation-file-fields"></a>了解对帐文件字段

- [基于许可证的对帐文件字段](license-based-recon-files.md)
- [基于用量的对帐文件字段](usage-based-recon-files.md)
- [每日分级用量对帐文件字段](daily-rated-usage-recon-files.md)
- [一次购买 CSP 对帐文件字段](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>了解对帐文件中的费用类型

若要了解 **"ChargeType"** 列 (中的费用) ，请参阅 [对帐文件费用类型](recon-file-charge-types.md)。

## <a name="fix-formatting-issues"></a>修复格式设置问题

有时，对帐文件可能包含格式设置问题。 例如，如果未使用 en-US 区域设置，则可能会出现此问题。

请按照以下步骤修复对帐文件的任何格式设置问题：

1. 在 Microsoft Excel (以.csv格式) 对帐文件。
2. 选择文件的第一列。
3. 打开"**将文本转换为列向导"。** 在功能区上，选择 **"数据"，** 然后选择"**文本到列"。**
4. 在向导中，选择 **"分隔的文件类型"。** 然后，选择“下一步”  。
5. 在"**分隔符"字段中**，选择"**逗号"。**  (**选项卡** 已选中，可以将此选项保留为选中状态。) ，然后选择"下一 **步"。**
6. 在"**列数据格式"字段中**，选择 **"日期：MDY"。** 然后，选择“下一步”  。
7. 在" **列数据格式"字段中** ， **选择"所有金额** 列的文本"。 然后选择“完成”。

## <a name="download-reconciliation-files-programmatically"></a>以编程方式下载对帐文件

对帐文件可能非常大，有时难以下载。 若要以编程方式下载对帐文件，请参阅 [获取发票行项](/partner-center/develop/get-invoiceline-items)。

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>如果文件超出 Excel 中的行限制

如果能够下载对帐文件，但没有在 Microsoft Excel 中打开它，这可能意味着该文件包含的行数超过了 Excel 允许的行数。 如果发生这种情况，可以使用以下任一过程打开文件。

### <a name="open-a-recon-file-in-power-bi"></a>在 Power BI

1. 像平时一样下载对帐文件。
2. 下载、安装并打开 Microsoft Power BI。
3. 在 **"Power BI"选项卡上**，选择"**获取数据"。**
4. 在"常见 **数据源"列表中，选择**"**文本/CSV"。**
5. 系统提示时，打开 recon 文件。

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>在 Excel 透视表中打开 recon 文件

1. 像平时一样下载对帐文件。
2. 在 Microsoft Excel 中打开新文件。
3. 在"**数据"** 选项卡上，**选择"获取数据**"，选择"**从文件"，** 然后选择"**文本/CSV"。**
4. 系统提示时，打开 recon 文件。 将显示数据。
5. 在"**加载"** 下拉菜单中，选择"**加载到**"，然后选择"确定 **"。**
6. 在" **导入数据"** 对话框中，选择 **"数据透视表报表** "以打开文件。

## <a name="negative-amount-displayed"></a>显示的负数

对帐文件中可能会看到负数。 此问题的原因如下：

- 你最近取消了或减少了许可证数
- 你收到了服务许可协议和 SLA (或) Azure 消耗的额度

若要获取有关此事务的详细信息，请在对帐文件中查看其费用类型属性。

## <a name="map-taxes-or-vat"></a>地图税或增值税

若要将增值税或增值税 (增值税) 映射到发票：

- 基于许可证的文件中" **税务** "列的总和。
- 基于 **使用情况的文件的 TaxAmount** 列的总和。

## <a name="itemize-reconciliation-files-by-partner"></a>按合作伙伴对帐文件进行项化

间接模型中 **的合作伙伴可以在** 基于许可证和基于使用情况的对帐文件中使用这些附加字段按经销商对文件进行项化。

| MPN ID | 说明 |
| ------ | ----------- |
| MPN ID | MICROSOFT 合作伙伴网络 (CSP) 合作伙伴云解决方案提供商 (的) MPN (标识符) 。 |
| [经销商 MPN ID](#reseller-mpn-id) | 订阅 [的记录经销商的 MPN 标识符](#reseller-mpn-id)。 此字段对应于为订阅中列出的特定订阅的经销商 ID 合作伙伴中心。 仅显示在间接模型中合作伙伴的对帐文件上。 |

### <a name="reseller-mpn-id"></a>经销商 MPN ID

如果 CSP 合作伙伴直接向客户销售订阅，则其 **MPN ID** 将列出两次，即 **MPN ID** 和经销商 **MPN ID**。

如果 CSP 合作伙伴的经销商没有 **MPN ID，** 则此值改为设置为合作伙伴的 **MPN ID。**

如果 CSP 合作伙伴删除了经销商 **MPN ID，** 则此值将设置为 *-1。*

查看或更新经销商 **MPN ID：**

1. 登录到合作伙伴中心。
2. 在"合作伙伴中心菜单中，选择"客户 **"。**
3. 从列表中选择客户。
4. 在客户菜单中，选择"**订阅"。**
5. 从列表中选择订阅。
6. 选择“更新”以更改“经销商 (MPN ID)”。

## <a name="next-steps"></a>后续步骤

- [如何读取帐单&对帐文件](read-your-bill.md) 