---
title: 客户计费和Azure 市场开票
description: 本文介绍有关客户计费和开票的Azure 市场问题。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 05/04/2021
ms.openlocfilehash: 6fdbbf9ad2b31e2b61eec20193717f60dd8e199a
ms.sourcegitcommit: b6959846c30d062d05028c9b4ba14c07e903e61a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112970185"
---
# <a name="azure-marketplace-billing-and-invoicing"></a>Azure 市场计费和开票

本文介绍客户计费和开票Azure 市场信息。

## <a name="microsoft-supports-multiple-currencies"></a>Microsoft 支持多种货币

Azure 市场产品/服务按以下 17 种货币定价和计费：

- 澳大利亚元 (AUD) 
- 巴西 real (BRL) 
- 英国磅 (GBP) 
- 加拿大元 (CAD) 
- 中国 (元) 
- 丹麦 krone (DKR) 
- 欧洲 (EUR) 
- 印度 (INR) 
- 日语 (JPY) 
- 朝鲜语 (KRW) 
- 新西兰元 (NZD) 
- 挪威 krone (NOK) 
- 俄语 (或) 
- 瑞典语 (SEK) 
- 中国 (CHF) 
- 台元 (TWD) 
- 美元 (美元) 

## <a name="billing"></a>计费

在购买定期购买期间，将按定期购买计费。 这些费用将显示在相应日历月发票上。 在原始购买日期的同一天，他们将继续在下一个时段自动进行自动启动。

[![如何按月和按年定期购买计费的示例时间线。](media/billing/billing-charges-recurring.png)](media/billing/billing-charges-recurring.png#lightbox)

>[!NOTE]
> 服务期是使用该服务付费的时间段。 除非事先取消，否则它将在服务时段的 和 自动续订。

> [!NOTE]
> 如果续订月份日期不能 (月份日期，我们会调整计费期限) 或计费月的最后一天。 这意味着，如果订阅日期为 1/31，则计费结束日期将调整为 2/27，续订日期分别为 2/28 (2/28 和 2/29（如果从闰年) 开始）。

## <a name="invoices"></a>发票

当发票在日历月开始时，你将收到一封电子邮件Azure 门户。 发票将显示在日历月购买和/或消耗的所有免费和付费产品/服务。 如果只有免费产品/服务，则只会看到 $0 行项目，无需执行任何付款操作。 **企业协议客户** 将收到一份合并发票，其中显示 Azure 和 Azure 市场 费用 (澳大利亚、日本和新加坡客户除外) 。 **直接从客户购买Azure 市场** 客户将收到仅针对Azure 市场的帐单。 有关详细信息，请参阅 [MOSP 帐户的发票](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)。

收到发票时，会有所不同：

- 如果付款方式是信用卡，则购买预留后立即开具发票。 此发票将独立于每月发票。
- 如果付款方式是支票/电汇，则此购买将包含在每月市场发票中。

系统会为 Microsoft 在线服务计划 (MOSP)、Microsoft 客户协议 (MCA) 和 Microsoft 合作伙伴协议 (MPA) 计费帐户创建发票。 发票根据计费帐户类型生成。 Azure 市场在计费周期结束后的几天内计费。 客户、Azure 市场和即用 VM 的发票是在当月的第 [9 天左右生成的](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)。 它显示上个月各自的费用。 例如，如果用户在 3 月 1 日购买了预留，在 3 月 30 日购买了另一个预留，则 4 月的单个发票将包含这两个预留。

有关发票详细信息，请参阅 [了解 Azure 外部服务费用](/azure/cost-management-billing/understand/understand-azure-marketplace-charges)。

## <a name="next-steps"></a>后续步骤

- [什么是 Azure 市场？](azure-marketplace-overview.md)
- [Azure 市场购买](azure-purchasing-invoicing.md)
