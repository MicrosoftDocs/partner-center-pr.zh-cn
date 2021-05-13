---
title: 如何读取帐单&对帐文件
ms.topic: article
ms.date: 06/05/2020
description: 了解发票&对帐文件。 帐单显示合作伙伴中心、产品和客户的每月费用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f16b619aba838da1d1da0c5eb13648ebb107c802
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855907"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>了解帐单和对帐文件 - 了解如何在合作伙伴中心


**适当的角色**：全局管理员|计费管理员|管理员代理


发票 **是****计划、** 所有产品合作伙伴中心客户 (费用的) 。 

## <a name="find-your-bill-and-reconciliation-file"></a>查找帐单和对帐文件 

可以在仪表板的"计费"页上找到发票合作伙伴中心。 还可以在此页上找到计费历史记录、支出趋势和对帐文件。 

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard/home)。 

2. 在左侧菜单中，选择"计费 **"。** 

3. 在“计费状态”页面上，选择某一发票或对帐文件以查看更多详细信息。 

可以在页面顶部的"帐户余额截至上次发票日期为止"下找到最新发票的链接。 

可以在"计费历史记录"部分找到以前的发票。 选择适当的年份，然后选择相应计费周期旁边的下拉箭头。 选择"发票" (.pdf) 旁边的链接，下载该周期的发票。 

## <a name="invoice-types"></a>发票类型

Microsoft 将针对任何基于许可证的费用 (例如 Office 365) 和基于使用情况的费用 (（例如 Azure) ）发出一份发票，并单独开具一次费用的发票 (例如 Azure RI、市场或 Azure 计划) 。

例如，  

**方案 1 [单一货币]**：合作伙伴已购买 145P 产品/服务许可证和 O365 许可证，  

- 合作伙伴将获取一份发票 PDF 和 2 份对帐文件，涵盖 O365 和 Azure (145p) 。  

**方案 2 [单一货币]**：合作伙伴购买 Azure RI、市场和/或 Azure 计划以及 145p 购买。

- 合作伙伴将获取一份发票 PDF 和一份对帐文件，其中涵盖 Azure (145p) 。 

- 合作伙伴将收到另一个发票 PDF 和对帐文件，其中包括对 Azure RI、Marketplace、Azure 计划收费。 

**方案 3 [多币种]**：合作伙伴在克朗和 azure 计划中购买了 azure RI，还提供了 eur 的145p 购买。

- 合作伙伴将收到一个发票 PDF 和一个对帐文件，其中包含克朗的 Azure RI 费用。 

- 合作伙伴将收到一个发票 PDF 和一个对帐文件，涵盖了 EUR 的 Azure 计划收费。 

- 合作伙伴将收到另一个发票 PDF 和一个对帐文件，其中包含145p 产品在 EUR (或合作伙伴计费货币) 的收费。 


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

有关发票文件中所有字段的详细说明 (包括一次费用字段) ，请参阅 [发票文件字段](invoice-file.md)。 

## <a name="understand-reconciliation-files"></a>了解对帐文件

 对帐文件提供费用的向下钻取/明细详细信息，可以连同发票 PDF 一起下载。 对帐文件包括客户标识符和订阅标识符，可用于创建客户发票。 请参阅  [如何使用对帐文件](use-the-reconciliation-files.md) 获取有关对帐文件的更多详细信息。 

## <a name="next-steps"></a>后续步骤

- [如何使用对帐文件](use-the-reconciliation-files.md)