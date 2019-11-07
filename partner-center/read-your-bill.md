---
title: 阅读帐单 | 合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 发票是当前月期间的所有费用（包括计划、产品和客户的费用）汇总。 合作伙伴中心提供此功能。
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: 订阅计费, 计费, 在合作伙伴中心计费, 合作伙伴中心计费, 阅读我的帐单, 发票, 合作伙伴中心发票, 云解决方案提供商发票, 我的帐单在哪里？
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652172"
---
# <a name="read-your-bill"></a>阅读帐单

**适用于**

-  合作伙伴中心
-  Microsoft Cloud for US Government 合作伙伴中心


对于帐单，请访问 "**合作伙伴中心**" 菜单，然后选择 "**计费**"，查看您的帐单历史记录和趋势，链接到您的发票和协调文件以及您最近的付款。

云解决方案提供商计划中选择按月计费的合作伙伴会为其客户的订阅（基于许可证和基于使用情况）向 Microsoft 支付为期 60 天的欠款。

> [!NOTE]  
> 您的发票会在计划、产品和客户之间的所有费用中汇总，并在当前计费周期内提供，在所选计费日期的两（2）天内可用（UTC 时间）。 例如，如果你有9月12日的计费日期，则在第13个，发票生成过程将在第13个，并在第14天的12： 00 (UTC 处开始 如果你在15日未看到你的发票11： 59PM UTC，则你的服务级别协议不会超出你的要求，因此应进行服务请求。 

你将收到基于许可证 (Office365) 和基于使用情况 (Azure) 的费用的一张发票，以及一次性（Azure 虚拟机预留实例）费用的单独发票。

有关费用的明细，请使用随附的对帐文件。 对帐文件包括用于创建客户发票的客户 ID 和订阅 ID。 有关详细信息，请参阅[如何使用对帐文件](use-the-reconciliation-files.md)。

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
<td>我们发送发票的地址。 若要更改公司名称或地址，请编辑合作伙伴中心帐单配置文件。 </td>
</tr>
<tr class="odd">
<td>基于许可证的费用</td>
<td>统一月度（或年度）支付已购买的基于使用情况的许可证费用，预先收取该服务的费用。 此数字是基于许可证的对帐文件（列 T）中“小计”列中所有费用的总和。</td>
</tr>
<tr class="even">
<td>基于使用情况的费用</td>
<td>Azure 使用情况，包括在帐单月份期间启用和使用的新服务或应用程序。 此数字是基于使用情况的对帐文件（列 Z）中“税前费用”列中所有费用的总和。</td>
</tr>
<tr class="odd">
<td>折扣</td>
<td>例如，客户从正常订阅价格收到的折扣。 此折扣显示为统一金额，而非根据单元或许可证制定的价格。</td>
</tr>
<tr class="odd">
<td>退款额</td>
<td>对订阅所做更改（示例：增加或减少席位）的退款或调整。</td>
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
<li>基于许可证的文件（列 U）的“税款”列。</li>
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
<td>按发票日期的月期间。 这是使用基于使用情况的服务和基于许可证的服务对许可证计数的任何信用调整或更改进行协调的时间段。</td>
</tr>
<tr class="even">
<td>发票日期</td>
<td>每月生成发票的帐单日期或周年周年日。</td>
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
<td>使用服务的地址。 （这是与公司审核相关的合法公司地址。）</td>
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
 



