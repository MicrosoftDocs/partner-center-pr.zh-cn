---
title: 区域性 PSTN 服务税款和费用
description: 作为 Microsoft 365 语音产品开展的 Office 365 合作伙伴，你可能会受到 PSTN 服务的区域性、费用或法规要求。
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "90594453"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>区域税收，公共交换电话网络的法规 (PTSN) 服务

**适用于**

- 合作伙伴中心
- Office 365 合作伙伴约束力 Microsoft 365 语音产品

**相应的角色**
-    全局管理员
-    用户管理员
-    管理员代理

某些司法辖区中 (PSTN) 服务的公共交换电话网络可能会受到特殊的税务和法规要求，这些要求可能会影响合作伙伴订单和发票。 在美国中，包括波多黎各、包含音频会议、呼叫计划和通信信用额度的 PSTN 服务，受特殊的税务和法规要求。 在美国和波多黎各中，Microsoft 价格的 PSTN 服务以税收包含。  唯一的 PSTN 税和法规将影响 Office 365 合作伙伴约束力 Microsoft 365 语音产品。  如果合作伙伴标记了 Microsoft PSTN 服务的价格，则可能有责任计算和汇寄 PSTN 税款和费用。

## <a name="partner-recommendations"></a>合作伙伴建议

联系你的税务和法律顾问，了解你的组织对 PSTN 服务法规、税费和费用以及其他潜在责任的责任。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>发票演示和合作伙伴对帐文件

美国、波多黎各和加拿大的 CSP 发票和 CSP 协调文件（包括 Skype for Business PSTN 和 Microsoft 365 语音服务）将为 PSTN 和非 PSTN 组件提供单独的行项。

此外，CSP 发票还会显示以下脚注：

* 显示的价格是音频会议和电话计划服务的收费。  任何适用的事务税款仅根据显示的金额（美国中的销售额除外）进行收费。  在美国，显示的价格是含税的，因为它包括呼叫计划和音频会议服务的费用，以及收取的税费和费用费用。  音频会议和调用计划服务由有权提供它们的 Microsoft 关联服务提供服务。  有关详细信息，请参阅 [Microsoft 批量授权](https://go.microsoft.com/fwlink/?LinkId=690247)。

## <a name="reconciliation-file-example"></a>协调文件示例

Office 365 企业版 E5 在协调文件上显示两个具有相同名称和相同 Id 的行项，但每个行项都具有唯一的单位价格 (例如： $28.40 和 $2.00) 。 这可区分 Office 365 产品/服务的 Skype for Business PSTN 会议组件，以便正确征税。

**伙伴对帐示例 #1 (选择列) ：**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |周期费用   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |周期费用   |2.00   |

**合作伙伴对帐示例 #2**

加拿大提供的 Microsoft 365 商业版语音包含附加的 PSTN 应缴税组件，这些组件合并在 CSP 发票 (类似于 Office 365 E5，提供两个行项，一个用于 PSTN 组件，另一个用于非 PSTN 组件) 。  Microsoft 365 商业版语音的 CSP 协调程序文件将单独显示所有的 PSTN 应缴税组件 (单独的 PSTN 组件不会合并在其中。CSV 或 API 工具) 。  在对帐文件中找到的客户的订单详细信息和计费金额的合计将与 CSP 发票匹配。

## <a name="additional-resources"></a>其他资源
有关更多详细信息，请访问合作伙伴网站的 [Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) 。

