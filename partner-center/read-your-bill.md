---
title: 阅读帐单 | 合作伙伴中心
description: 发票是当前月期间的所有费用（包括计划、产品和客户的费用）汇总。 发票将在合作伙伴中心仪表板上提供。
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
keywords: 订阅计费, 计费, 在合作伙伴中心计费, 合作伙伴中心计费, 阅读我的帐单, 发票, 合作伙伴中心发票, 云解决方案提供商发票, 我的帐单在哪里？
ms.localizationpriority: medium
ms.openlocfilehash: e43a3ea778c60f1009f5cd3489a24f4c9f0b1e4f
ms.sourcegitcommit: 5b720c2ad126ec52564ad5264596ca1cf6a12489
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2018
ms.locfileid: "4377539"
---
# <a name="read-your-bill"></a>阅读帐单

**适用于**

-  合作伙伴中心
-  美国政府 Microsoft 云合作伙伴中心
-  德国 Microsoft 云合作伙伴中心

若要查看帐单，请转到**仪表板**菜单，然后选择**计费**以查看你的计费历史记录和趋势、指向发票和对帐文件的链接，以及你的最新付款。

云解决方案提供商计划中选择按月计费的合作伙伴会为其客户的订阅（基于许可证和基于使用情况）向 Microsoft 支付为期 60 天的欠款。

> [!NOTE]  
> 发票是当前计费周期的所有费用（包括计划、产品和客户的费用）汇总，并且从选定计费日期起四 (4) 天内可提供发票。

你将收到一张基于许可证的 (Office365) 和基于使用情况 (Azure) 费用的发票和一次性 （Azure 虚拟机预留实例） 的单独发票费用。

有关费用的明细，使用随附的对帐文件。 对帐文件包括用于创建客户发票的客户 ID 和订阅 ID。 有关详细信息，请参阅[如何使用对帐文件](use-the-reconciliation-files.md)。

## <a name="invoice-file-definitions"></a>发票文件定义


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>字段</strong></td>
<td><strong>说明</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>联邦税收 ID 编号。</td>
</tr>
<tr class="odd">
<td>客户编号</td>
<td>你的客户编号。</td>
</tr>
<tr class="even">
<td>帐单邮寄地址</td>
<td>我们发送发票的地址。 若要更改此地址，请转到“帐户设置”>“合作伙伴计费配置文件”。 </td>
</tr>
<tr class="odd">
<td>基于许可证的费用</td>
<td>统一月度（或年度）支付已购买的基于使用情况的许可证费用，预先收取该服务的费用。 此数字是基于许可证的对帐文件（列 T）中“小计”列中所有费用的总和。</td>
</tr>
<tr class="even">
<td>基于使用情况费用</td>
<td>Azure 使用情况，包括在帐单月份期间启用和使用的新服务或应用程序。 此数字是基于使用情况的对帐文件（列 Z）中“税前费用”&quot;&quot;列中所有费用的总和。</td>
</tr>
<tr class="odd">
<td>折扣</td>
<td>例如，客户从正常订阅价格收到的折扣。 此折扣显示为统一金额，而非根据单元或许可证制定的价格。</td>
</tr>
<tr class="odd">
<td>退款额</td>
<td>对订阅所做更改的信用或调整（示例：增加或减少席位）。</td>
</tr>
<tr class="even">
<tr class="even">
<td>小计</td>
<td>税前的税款和税务独占费用和信用。</td>
</tr>
<td>税务</td>
<td>在发票第 2 页开始的详细信息部分中统计的当前费用的总税款。 此数字是以下列中所有费用的总和：
<ul>
<li>基于使用情况的对帐文件（列 AA）的“税额”&quot;&quot;列和</li>
<li>基于许可证的文件（列 U）的“税款”&quot;&quot;列。</li>
</ul></td>
</tr>
<tr class="odd">
<td>其他信用额度</td>
<td>税务独占的信用。</td>
</tr>
<tr class="even">
<td>当前总费用</td>
<td>计费周期内以计费货币为单位的到期金额，在付款到期日期时到期。</td>
</tr>
<tr class="odd">
<td>付款指示</td>
<td>介绍如何根据所在区域支付你的发票。 在付款时，始终包括你的发票编号。</td>
</tr>
<tr class="even">
<td>发票编号</td>
<td>发票的编号。</td>
</tr>
<tr class="odd">
<td>计费周期</td>
<td>云解决方案提供商合作伙伴按月或按年计费。</td>
</tr>
<tr class="even">
<td>发票日期</td>
<td>收到发票的日期。</td>
</tr>
<tr class="odd">
<td>付款期限</td>
<td>对于一次性购买，此期限将始终为 60 天。</td>
</tr>
<tr class="even">
<td>付款截止日期</td>
<td>必须在此日期前收到你的付款。</td>
</tr>
<tr class="odd">
<td>客户 PO</td>
<td>购买订单编号。</td>
</tr>
<tr class="even">
<td>客户服务</td>
<td>访问客户服务的网站地址。</td>
</tr>
<tr class="odd">
<td>服务接收方</td>
<td>使用服务的地址。 （这是与公司审查关联的法定公司地址，不可更改。）</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>一次性费用的明细列表

|**字段** |**定义**|
|:----------------|:-----------------------------|
|日期 |购买的日期。 |
|说明 |产品名称。 |
|数量 |所购买的产品（例如预订）的数量。 |
|单价 |每个产品（例如预订）的价格。 |
|折扣 |任何适用的折扣。 |
|税前金额 |税前购物小计。 |
|销售税 |税额。 |
|总计 |要付款的总额。 |
 



