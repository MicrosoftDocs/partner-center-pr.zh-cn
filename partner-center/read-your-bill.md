---
title: 阅读帐单 | 合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
description: 发票是当前月期间的所有费用（包括计划、产品和客户的费用）汇总。 该命令适用于合作伙伴中心。
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: 订阅计费, 计费, 在合作伙伴中心计费, 合作伙伴中心计费, 阅读我的帐单, 发票, 合作伙伴中心发票, 云解决方案提供商发票, 我的帐单在哪里？
ms.localizationpriority: medium
ms.openlocfilehash: aec344eb7e4ed6e0a4d5e7e506c9bcf195654293
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584540"
---
# <a name="read-your-bill"></a>阅读帐单

**适用于**

-  合作伙伴中心
-  Microsoft Cloud for US Government 合作伙伴中心


对于你的帐单，请转到**合作伙伴中心**菜单，然后选择**计费**若要查看你的帐单历史记录和趋势，链接到你的发票和对帐文件，以及最近付款。

云解决方案提供商计划中选择按月计费的合作伙伴会为其客户的订阅（基于许可证和基于使用情况）向 Microsoft 支付为期 60 天的欠款。

> [!NOTE]  
> 发票的所有费用摘要-程序、 产品和客户-当前计费周期以及间在 UTC 时间中你所选计费日期的两 （2） 天内可用。 例如，如果有 12 年 9 月计费日期，发票生成过程将开始在 13 上的 UTC 时间上午 12:00，并完成 14 在 UTC 时间上午 12:00。 如果你没有在 15 日看到由 11:59 PM UTC 发票，您不够用你的服务级别协议，并应提交服务请求。 

你将收到基于许可证 (Office365) 和基于使用情况 (Azure) 的费用的一张发票，以及一次性（Azure 虚拟机预留实例）费用的单独发票。

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
<td><strong>描述</strong></td>
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
<td>我们发送发票的地址。 若要更改公司名称或地址，请编辑你的合作伙伴中心计费配置文件。 </td>
</tr>
<tr class="odd">
<td>基于许可证的费用</td>
<td>统一月度（或年度）支付已购买的基于使用情况的许可证费用，预先收取该服务的费用。 此数字是基于许可证的对帐文件（列 T）中“小计”列中所有费用的总和。</td>
</tr>
<tr class="even">
<td>基于使用情况的费用</td>
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
<td>税前总额以及不含税的费用和退款。</td>
</tr>
<td>税</td>
<td>在发票第 2 页开始的详细信息部分中统计的当前费用的总税款。 此数字是以下列中所有费用的总和：
<ul>
<li>基于使用情况的对帐文件（列 AA）的“税额”&quot;&quot;列和</li>
<li>基于许可证的文件（列 U）的“税款”&quot;&quot;列。</li>
</ul></td>
</tr>
<tr class="odd">
<td>其他退款</td>
<td>不含税的退款。</td>
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
<td>指向在发票日期的月。 这是在此期间使用基于使用情况的服务和基于许可证的服务已得到协调任何信用额度调整或许可证计数中的更改的段。</td>
</tr>
<tr class="even">
<td>发票日期</td>
<td>您的计费日期或发票在其生成每个月的周年日。</td>
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
<td>使用服务的地址。 （这是与审核公司关联的法律公司地址）。</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>一次性费用的明细列表

|**字段** |**定义**|
|:----------------|:-----------------------------|
|日期 |购买的日期。 |
|描述 |产品名称。 |
|数量 |所购买的产品（例如预订）的数量。 |
|单价 |每个产品（例如预订）的价格。 |
|折扣 |任何适用的折扣。 |
|税前金额 |税前购物小计。 |
|销售税 |税额。 |
|总计 |要付款的总额。 |
 



