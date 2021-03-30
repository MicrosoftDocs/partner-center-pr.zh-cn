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
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730071"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>了解如何读取伙伴中心对帐文件中的行项

**相应的角色**

- 计费管理员
- 全局管理员

你可以从合作伙伴中心下载你的对帐文件，以获取计费周期中每个费用的详细的行项目视图。 行项详细信息包括每个客户的订阅的费用，以及详细事件 (例如，将许可证添加到订阅) 。

有关如何读取 **发票** 的详细信息，请参阅 [阅读帐单](read-your-bill.md)。

## <a name="understand-reconciliation-file-fields"></a>了解协调文件字段

- [基于许可证的对帐文件字段](license-based-recon-files.md)
- [基于用量的对帐文件字段](usage-based-recon-files.md)
- [每日分级用量对帐文件字段](daily-rated-usage-recon-files.md)
- [一次性购买 CSP 对帐文件字段](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>了解对帐文件中的费用类型

若要了解 **ChargeType** 列)  (对帐文件中的费用类型，请参阅 [对帐文件费用类型](recon-file-charge-types.md)。

## <a name="fix-formatting-issues"></a>解决格式问题

有时，对帐文件可能包含格式设置问题。 例如，如果不使用 en-us 区域设置，则可能出现此问题。

请按照以下步骤修复对帐文件中的任何格式设置问题：

1. 在 Microsoft Excel 中打开 (为 .csv 格式的协调文件) 。
2. 选择该文件中的第一列。
3. 打开 " **将文本转换为列" 向导**。 在功能区上，选择 " **数据**"，然后选择 " **文本到列**"。
4. 在向导中，选择 " **带分隔符的文件类型**"。 然后，选择“下一步”  。
5. 在 " **分隔符** " 字段中，选择 " **逗号**"。  (如果已选择 **选项卡** ，则可以选择此选项。 ) 然后选择 " **下一步**"。
6. 在 " **列数据格式** " 字段中，选择 **Date： MDY**。 然后，选择“下一步”  。
7. 在 " **列数据格式** " 字段中，选择 "所有金额列的 **文本** "。 然后选择“完成”。

## <a name="download-reconciliation-files-programmatically"></a>以编程方式下载对帐文件

协调文件可能非常大，有时很难下载。 若要以编程方式下载对帐文件，请参阅 [获取发票行项](/partner-center/develop/get-invoiceline-items)。

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>如果文件超出 Excel 中的行限制

如果能够下载并不在 Microsoft Excel 中打开对帐文件，这可能意味着该文件包含的行数超过了 Excel 所允许的数目。 如果发生这种情况，可以使用以下任一过程打开文件。

### <a name="open-a-recon-file-in-power-bi"></a>在 Power BI 中打开侦测文件

1. 按常规方式下载协调文件。
2. 下载、安装和打开 Power BI 的实例。
3. 在 Power BI **主页** "选项卡上，选择" **获取数据**"。
4. 在 **公共数据源** 列表中，选择 " **Text/CSV**"。
5. 出现提示时，打开侦测文件。

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>在 Excel 数据透视表中打开侦测文件

1. 按常规方式下载协调文件。
2. 在 Microsoft Excel 中打开新文件。
3. 在 " **数据** " 选项卡上，选择 " **获取数据**"，选择 " **从文件**"，然后选择 " **文本/CSV**"。
4. 出现提示时，打开侦测文件。 你的数据将会显示。
5. 在 " **加载** " 下拉菜单中，选择 " **加载到**"，然后选择 **"确定"**。
6. 在 " **导入数据** " 对话框中，选择 " **数据透视表** " 以打开文件。

## <a name="negative-amount-displayed"></a>显示负金额

你可能会在对帐文件中看到负值。 这可能是由以下原因之一导致的：

- 你最近取消或减少了许可证数量
- 你已收到 (SLA) 或 Azure 使用情况的服务许可协议信用额度

若要获取有关此事务的详细信息，请在对帐文件中查看其费用类型属性。

## <a name="map-taxes-or-vat"></a>映射税金或 VAT

若要将增值税或销售税 (增值税) 映射到发票：

- 对基于许可证的文件中的 **税务** 列求和。
- 在基于使用情况的文件中对 **TaxAmount** 列求和。

## <a name="itemize-reconciliation-files-by-partner"></a>按合作伙伴列举帐文件

**间接模型** 中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些附加字段，按经销商对文件进行详细列举。

| MPN ID | 说明 |
| ------ | ----------- |
| MPN ID | Microsoft 合作伙伴网络 (MPN) 云解决方案提供程序的标识符 (CSP) 直接或间接 (。 |
| [经销商 MPN ID](#reseller-mpn-id) | [订阅的记录分销商的 MPN 标识符](#reseller-mpn-id)。 此字段对应于 "合作伙伴中心" 中为特定订阅列出的分销商 ID。 仅显示在间接模型中合作伙伴的对帐文件上。 |

### <a name="reseller-mpn-id"></a>经销商 MPN ID

如果 CSP 合作伙伴将订阅直接销售给客户，则其 **MPN id** 将列出两次，同时作为 **MPN ID** 和 **经销商 MPN ID**。

如果 CSP 合作伙伴的分销商没有 **MPN id**，则此值将改为设置为合作伙伴的 **MPN id** 。

如果 CSP 合作伙伴删除了 **经销商 MPN ID**，此值将设置为 *-1*。

查看或更新 **经销商 MPN ID**：

1. 登录到合作伙伴中心。
2. 在 "合作伙伴中心" 菜单中，选择 " **客户**"。
3. 从列表中选择客户。
4. 在 customer 菜单中，选择 " **订阅**"。
5. 从列表中选择订阅。
6. 选择“更新”以更改“经销商 (MPN ID)”。

## <a name="next-steps"></a>后续步骤

- [如何读取帐单 & 侦测文件](read-your-bill.md) 