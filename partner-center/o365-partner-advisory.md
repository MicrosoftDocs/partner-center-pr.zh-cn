---
title: CSP 合作伙伴咨询-Microsoft 365 语音
description: 了解某些国家/地区的 PSTN 服务以及可能应用和影响合作伙伴订单和开票的特殊税或法规要求。
ms.topic: article
ms.date: 05/05/2020
author: BillLinzbach
ms.author: BillLi
keywords: Office，O365，PSTN 服务，税款，要求，发票，开票
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96271a574ad84d28651e263c34a8238093e0d026
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377791"
---
# <a name="office-365-partner-advisory-microsoft-365-business-voice-in-the-csp-program"></a>Office 365 合作伙伴咨询：云解决方案提供商计划中的 Microsoft 365 商务语音

**适用于**

- 合作伙伴中心  

**相应的角色**
-    全局管理员
-    用户管理员
-    管理员代理

某些地区的公共交换电话网络（PSTN）服务可能会受到特殊的税务和法规要求，可能会影响合作伙伴的订单和发票。 在美国中，包括波多黎各、包含音频会议、呼叫计划和通信信用额度的 PSTN 服务，受特殊的税务和法规要求。 在美国和波多黎各中，Microsoft 价格的 PSTN 服务以税收包含。  唯一的 PSTN 税和法规将影响 Office 365 合作伙伴约束力 Microsoft 365 语音产品。  如果合作伙伴标记了 Microsoft PSTN 服务的价格，则可能有责任计算和汇寄 PSTN 税款和费用。

## <a name="partner-recommendations"></a>合作伙伴建议

联系你的税务和法律顾问，了解你的组织对 PSTN 服务法规、税费和费用以及其他潜在责任的责任。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>发票演示和合作伙伴对帐文件

美国、波多黎各和加拿大的 CSP 发票和 CSP 协调文件（包括 Skype for Business PSTN 和 Microsoft 365 语音服务）将为 PSTN 和非 PSTN 组件提供单独的行项。

此外，CSP 发票还会显示以下脚注：

* 显示的价格是音频会议和电话计划服务的收费。  任何适用的事务税款仅根据显示的金额（美国中的销售额除外）进行收费。  在美国，显示的价格是含税的，因为它包括呼叫计划和音频会议服务的费用，以及收取的税费和费用费用。  音频会议和调用计划服务由有权提供它们的 Microsoft 关联服务提供服务。  有关详细信息，请参阅 [Microsoft 批量授权](https://go.microsoft.com/fwlink/?LinkId=690247)。

## <a name="reconciliation-file-example"></a>协调文件示例

Office 365 企业版 E5 在协调文件上显示两个具有相同名称和相同 Id 的行项，但每个行项都具有唯一的单位价格（例如： $28.40 和 $2.00）。 这可区分 Office 365 产品/服务的 Skype for Business PSTN 会议组件，以便正确征税。

**伙伴对帐示例 #1 （选择列）：**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |周期费用   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |周期费用   |2.00   |

**合作伙伴对帐示例 #2**

加拿大提供的 Microsoft 365 商业版语音包含附加的 PSTN 应缴税组件，这些组件合并在 CSP 发票上（类似于 Office 365 E5，提供两个行项，一个用于 PSTN 组件，另一个用于非 PSTN 组件）。  Microsoft 365 商业版语音的 CSP 协调程序文件将单独显示所有的 PSTN 应缴税组件（不会合并单个 PSTN 组件。CSV 或 API 工具）。  在对帐文件中找到的客户的订单详细信息和计费金额的合计将与 CSP 发票匹配。

## <a name="additional-resources"></a>其他资源
有关更多详细信息，请访问合作伙伴网站的[Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) 。

