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
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551191"
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

**方案 1 [单一货币]**：合作伙伴已购买 145P 产品/服务许可证和 Office 365 许可证，  

- 合作伙伴将获取一份发票 PDF 和两份对帐文件，涵盖 Office 365 和 Azure (145p) 。  

**方案 2 [单一货币]**：合作伙伴购买 Azure RI、市场和/或 Azure 计划以及 145p 购买。

- 合作伙伴将获取一份发票 PDF 和一份对帐文件，其中涵盖 Azure (145p) 。 

- 合作伙伴将收到另一份发票 PDF 和一份对帐文件，其中涵盖了 AZURE 预留实例的费用 (RI) 、市场、Azure 计划。 

**方案 3 [多货币]**：合作伙伴购买 Azure RI（采用 D按 D且以 EUR 计）和 Azure 计划（以 EUR 计）以及 145p 购买（以 EUR 计）。

- 合作伙伴将收到一份发票 PDF 和一份对帐文件，其中涵盖了 D按 D用于 AZURE RI 的费用。 

- 合作伙伴将收到一份发票 PDF 和一份对帐文件，其中涵盖 Azure 计划的费用（以 EUR 计）。 

- 合作伙伴将收到另一份发票 PDF 和一份对帐文件，其中涵盖 145p 产品/服务的费用（以 EUR (或合作伙伴计费货币) 。 


## <a name="understanding-invoice-pdf"></a>了解发票 PDF 

**使用情况和** 基于许可证的费用的发票：Office 365 和 Azure 等服务的费用发票将在所选计费日期 [UTC] 的 () 天内提供。  

**一次性和** 定期费用的发票：Azure RI、Azure 计划、市场等服务的费用发票不晚于每月 8 号。  

下面是发票 PDF 文档中的一些关键字段 -

**发票号**：为相应计费周期生成的发票文档的唯一标识符。 

**计费** 周期：这是使用和基于许可证的服务的时间段。 

**发票日期**：每月生成发票的计费日期或周年日期。 

**付款截止日期**：必须收到付款的日期。 

**费用**：相应计费周期的计费货币到期金额。 

额度 **：信用** 额度 (例如服务级别协议 (SLA) ) 或对订阅所做的更改的调整 (例如，许可证增加或) 。 

**付款** 说明：说明如何根据区域支付发票。 付款时，请务必包含发票号。 

有关发票文件中所有字段的详细说明 (包括一次费用字段) ，请参阅 [发票文件字段](invoice-file.md)。 

## <a name="understand-reconciliation-files"></a>了解对帐文件

 提供费用明细/明细详细信息的对帐文件可以连同发票 PDF 一起下载。 对帐文件包括客户标识符和订阅标识符，可用于创建客户发票。 有关对帐文件的信息，请参阅 [如何使用对帐文件](use-the-reconciliation-files.md)。 

## <a name="next-steps"></a>后续步骤

- [如何使用对帐文件](use-the-reconciliation-files.md)