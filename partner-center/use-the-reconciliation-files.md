---
title: 使用你的对帐文件
ms.topic: article
ms.date: 06/08/2020
description: 了解合作伙伴中心中的对帐文件以及如何解释给定计费周期的详细的行项视图。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f52c0b3d53fde6d5b5f68c54f8967e26a33b8c76
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991769"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>了解如何读取伙伴中心对帐文件中的行项

适用于：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

你可以从合作伙伴中心下载你的对帐文件，以获取计费周期中每个费用的详细的行项目视图。 行项详细信息包括每个客户的订阅的费用，以及详细事件（例如，将座位添加到订阅）。

适当的角色：

- 计费管理员
- 全局管理员

有关如何读取**发票**的详细信息，请参阅[阅读帐单](read-your-bill.md)。

## <a name="understand-reconciliation-file-fields"></a>了解协调文件字段

- [基于许可证的对帐文件字段](license-based-recon-files.md)
- [基于使用情况的对帐文件字段](usage-based-recon-files.md)
- [一次性和重复的对帐文件字段](one-time-recurring-recon-files.md)
- [每日分级使用情况协调文件字段](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>了解对帐文件中的费用类型

若要了解对帐文件（ **ChargeType**列）中的费用类型，请参阅[对帐文件费用类型](recon-file-charge-types.md)。

## <a name="fix-formatting-issues"></a>解决格式问题

有时，对帐文件可能包含格式设置问题。 例如，如果不使用 en-us 区域设置，则可能出现此问题。

请按照以下步骤修复对帐文件中的任何格式设置问题：

1. 在 Microsoft Excel 中打开对帐文件（采用 .csv 格式）。
2. 选择该文件中的第一列。
3. 打开 "**将文本转换为列" 向导**。 在功能区上，选择 "**数据**"，然后选择 "**文本到列**"。
4. 在向导中，选择 "**带分隔符的文件类型**"。 然后，选择“下一步”。
5. 在 "**分隔符**" 字段中，选择 "**逗号**"。 （如果已选择**选项卡**，则可以选择此选项。）然后选择 "**下一步**"。
6. 在 "**列数据格式**" 字段中，选择**Date： MDY**。 然后，选择“下一步”。
7. 在 "**列数据格式**" 字段中，选择 "所有金额列的**文本**"。 然后选择“完成”。

## <a name="download-reconciliation-files-programmatically"></a>以编程方式下载对帐文件

协调文件可能非常大，有时很难下载。 若要以编程方式下载对帐文件，请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。

## <a name="map-taxes-or-vat"></a>映射税金或 VAT

若要为发票映射税金或增值税（VAT）：

- 对基于许可证的文件中的**税务**列求和。
- 在基于使用情况的文件中对**TaxAmount**列求和。

## <a name="itemize-reconciliation-files-by-partner"></a>按合作伙伴列举帐文件

**间接模型**中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些附加字段，按经销商对文件进行详细列举。

| MPN ID | 说明 |
| ------ | ----------- |
| MPN ID | 云解决方案提供商（CSP）合作伙伴的 Microsoft 合作伙伴网络（MPN）标识符（直接或间接）。 |
| [经销商 MPN ID](#reseller-mpn-id) | [订阅的记录分销商的 MPN 标识符](#reseller-mpn-id)。 此字段对应于 "合作伙伴中心" 中为特定订阅列出的分销商 ID。 仅显示在间接模型中合作伙伴的对帐文件上。 |

### <a name="reseller-mpn-id"></a>经销商 MPN ID

如果 CSP 合作伙伴将订阅直接销售给客户，则其**MPN id**将列出两次，同时作为**MPN ID**和**经销商 MPN ID**。

如果 CSP 合作伙伴的分销商没有**MPN id**，则此值将改为设置为合作伙伴的**MPN id** 。

如果 CSP 合作伙伴删除了**经销商 MPN ID**，此值将设置为 *-1*。

查看或更新**经销商 MPN ID**：

1. 登录到合作伙伴中心。
2. 在 "合作伙伴中心" 菜单中，选择 "**客户**"。
3. 从列表中选择客户。
4. 在 customer 菜单中，选择 "**订阅**"。
5. 从列表中选择订阅。
6. 选择“更新”**** 以更改“经销商 (MPN ID)”****。
