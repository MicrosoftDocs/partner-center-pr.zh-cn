---
title: 如何读取帐单 & 侦测文件
ms.topic: article
ms.date: 06/05/2020
description: 了解发票 & 协调文件。 你的帐单会在计划、产品和客户的每月期限内显示合作伙伴中心费用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215809"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>了解帐单和对帐文件-了解如何在合作伙伴中心查找这些文件


**相应的角色**

- 全局管理员
- 计费管理员
- 管理员代理


你的 **发票****汇总了你的所有合作伙伴中心费用** (整个计划、所有产品和所有客户) 。 

## <a name="invoice-types"></a>发票类型

Microsoft 将为任何基于许可证的 (收费（例如 Office 365) 和基于使用情况的收费 (，例如 azure) ）和一个单独的发票（如 Azure RI、Marketplace 或 Azure 计划 (）发布一张发票。

例如，应用于对象的  

**方案 1 [单一货币]**：合作伙伴购买了145P 产品/服务和 O365 许可证，  

- 合作伙伴将获得一个发票 PDF 和2个协调文件，涵盖 O365 和 Azure (145p) 的费用。  

**方案 2 [单一货币]**：合作伙伴已购买 azure RI、Marketplace 和/或 azure 计划以及145p 购买。

- 合作伙伴将获得一个发票 PDF 和一个对帐文件，涵盖 Azure (145p) 的费用。 

- 合作伙伴将收到另一个发票 PDF 和对帐文件，其中包括对 Azure RI、Marketplace、Azure 计划收费。 

**方案 3 [多币种]**：合作伙伴在克朗和 azure 计划中购买了 azure RI，还提供了 eur 的145p 购买。

- 合作伙伴将收到一个发票 PDF 和一个对帐文件，其中包含克朗的 Azure RI 费用。 

- 合作伙伴将收到一个发票 PDF 和一个对帐文件，涵盖了 EUR 的 Azure 计划收费。 

- 合作伙伴将收到另一个发票 PDF 和一个对帐文件，其中包含145p 产品在 EUR (或合作伙伴计费货币) 的收费。 

## <a name="find-your-bill"></a>查找帐单 

你可以在合作伙伴中心的仪表板的 "帐单" 页上找到你的发票。 您还可以在此页上找到您的帐单历史记录、支出趋势和协调文件。 

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/home)。 

2. 在左侧菜单中，选择 " **计费**"。 

3. 在 "帐单" 页上，选择要下载的发票。 

您可以在页面顶部的 "帐户余额" 下，找到指向最新发票的链接。 

您可以在 "帐单历史记录" 部分中找到以前的发票。 选择相应的年份，然后选择适当的计费周期旁的下拉箭头。 选择 "发票 (" 旁边的链接) 下载该时间段的发票。 

## <a name="understanding-invoice-pdf"></a>了解发票 PDF 

**使用情况和基于许可证的费用发票**： Office 365 和 Azure 等服务的费用发票将在所选计费日期 [UTC] 的两 (2) 天内可用。  

**一次性和定期计费发票**： azure RI、azure 计划、Marketplace 等服务的费用发票将于每个月不到8日后可用。  

下面是发票 PDF 文档中的一些关键字段–

**发票编号**：为各自计费期间生成的发票文档的唯一标识符。 

**计费周期**：这是你拥有使用情况和基于许可证的服务的时间段。 

**发票日期**：每月生成发票的帐单日期或周年周年日。 

**付款截止日期**：必须接收付款的日期。 

**费用**：按计费币种计算各自计费期间的到期金额。 

**信用额度**：信用 (如 SLA) 或对订阅所做更改的调整 (例如，许可证增加或减少) 。 

**付款说明**：描述如何根据你所在的区域为发票付费。 付款时，请始终确保包含发票号。 

有关发票文件中所有字段的详细说明 (包括) 一次费用的字段，请参阅 [发票文件字段](invoice-file.md)。 

## <a name="understand-reconciliation-files"></a>了解协调文件

 对帐文件提供了向下钻取/详细说明收费的详细信息，可与发票 PDF 一起下载。 对帐文件包括可用于创建客户发票的客户标识符和订阅标识符。 有关侦测文件的更多详细信息，请参阅  [如何使用对帐文件](use-the-reconciliation-files.md) 。 

## <a name="next-steps"></a>后续步骤

- [如何使用对帐文件](use-the-reconciliation-files.md)