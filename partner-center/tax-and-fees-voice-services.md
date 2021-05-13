---
title: 区域 PSTN 服务税款和费用
description: 作为处理语音产品Microsoft 365 Office 365 合作伙伴，你可能需要支付 PSTN 服务的区域税、费用或法规要求。
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854717"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>区域税、公共交换机电话网络 (PTSN) 法规

**适当的角色**：全局管理员|用户管理员|管理员代理

某些 (的公用电话 (PSTN) 服务可能需遵守可能影响合作伙伴订单和开票的特殊税务和法规要求。 在 美国（包括美国）中，PSTN 服务（包括音频会议、通话套餐和通信额度）需要遵守特殊的税务和法规要求。 在美国和波多黎各，Microsoft 将 PSTN 服务的价格作为含税价格。  唯一的 PSTN 税款和法规将影响交易语音产品Microsoft 365 Office 365 合作伙伴。  如果合作伙伴标记了 Microsoft PSTN 服务的价格，则可能有责任计算和汇寄 PSTN 税款和费用。

## <a name="partner-recommendations"></a>合作伙伴建议

与税务和税务部门联系，了解组织对 PSTN 服务的法规、税款和费用以及其他潜在责任的责任。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>发票显示和合作伙伴对帐文件

美国、墨西哥和加拿大的 CSP 发票和 CSP 对帐文件（包括 Skype for Business PSTN 和 Microsoft 365 Voice 服务）将为 PSTN 和非 PSTN 组件提供单独的行项。

此外，CSP 发票将显示以下脚注：

* 显示的价格是音频会议与通话套餐服务的费用。  除在交易范围内进行的销售外，任何适用的交易税都只收取美国。  在美国，显示的价格是含税的，因为它包括通话计划和音频会议服务的费用，以及我们收取的税款和费用。  音频会议服务和通话套餐服务由有权提供音频会议与通话套餐的 Microsoft 关联机构提供服务。  有关详细信息，请参阅 [Microsoft 批量授权](https://go.microsoft.com/fwlink/?LinkId=690247)。

## <a name="reconciliation-file-example"></a>对帐文件示例

Office 365 企业版 E5 在协调文件上显示两个具有相同名称和相同 Id 的行项，但每个行项都具有唯一的单位价格 (例如： $28.40 和 $2.00) 。 这可区分 Office 365 产品/服务的 Skype for Business PSTN 会议组件，以便正确征税。

**伙伴对帐示例 #1 (选择列) ：**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |周期费用   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |周期费用   |2.00   |

**合作伙伴对帐示例 #2**

加拿大提供的 Microsoft 365 商业版语音包含附加的 PSTN 应缴税组件，这些组件合并在 CSP 发票 (类似于 Office 365 E5，提供两个行项，一个用于 PSTN 组件，另一个用于非 PSTN 组件) 。  Microsoft 365 商业版语音的 CSP 协调程序文件将单独显示所有的 PSTN 应缴税组件 (单独的 PSTN 组件不会合并在其中。CSV 或 API 工具) 。  对帐文件中找到的客户的订单详细信息和计费金额之和将匹配 CSP 发票。

## <a name="additional-resources"></a>其他资源
有关详细信息，请访问合作伙伴Microsoft 365 [站点](https://www.microsoft.com/microsoft-365/partners/) 。

