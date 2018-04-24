---
title: 计费基础知识 | 合作伙伴中心
Description: Information on basic billing scenarios and the differences between license-based and usage-based billing
author: labrenne
keywords: 计费, 付款, 订单, 取消, 订单管理, 拒不付款, 欺诈, 滥用, 税款, 免税, 对帐文件
ms.openlocfilehash: f06e663e6e3d5dc32efb1423a17f02e19a2425f5
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2018
---
# <a name="billing-basics"></a>计费基础知识

**适用范围**

-  合作伙伴中心
-  美国政府 Microsoft 云合作伙伴中心
-  德国 Microsoft 云合作伙伴中心

## <a name="overview-of-billing"></a>计费概述
除了按月计费选项之外，现在可使用按年计费选项。 有关详细信息，请参阅[关于新计费功能的常见问题解答](faq-about-new-billing-features.md)。

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>日期</td>
<td><ul>
<li>每月计费日期是注册时选择的月份中的一天。 Microsoft 将发送一封包含计费日期的确认电子邮件。</li>
<li>可提前一 (1) 个月查找价目表，价目表每月更新一次。 订阅期限内可以保证基于许可证的价格，该期限通常是自购买日期起的 12 个月。 基于使用情况的价格可每月更改。 我们将通过发布合作伙伴价目表对任何价格更改公告 30 日。</li>
</ul></td>
</tr>
<tr class="even">
<td>付款期限</td>
<td><ul>
<li>付款期限 - 净 60 天。</li>
<li>必须在发票到期日（计费日期后 60 天）前进行支付，否则帐户将欠费。</li>
<li>欠费帐户将随时从云解决方案提供商计划中暂停和/或终止。 已暂停帐户无法创建新客户或订单、请求经销商关系、增加或减少订阅量、订购加载项订阅、转换或过渡订阅，并且仅限于管理现有客户、订阅和资源，直到帐户付清欠款为止。 合作伙伴支付其未付清的帐单后，可以重新获得其暂停帐户的完整功能。</li>
</ul></td>
</tr>
<tr class="odd">
<td>计费规则</td>
<td><ul>
<li>每月你将收到一张云解决方案提供商计划的发票。</li>
<li>基于许可证的订阅根据所购买的许可证（而非所使用的许可证）进行计费。</li>
<li>Azure（基于使用情况的订阅）基于消耗情况根据所计量的费率进行计费。</li>
<li>价格由订阅条款保证。 价格可能会在订阅续订时发生更改。</li>
</ul></td>
</tr>
<tr class="even">
<td>发票可用性</td>
<td><ul>
<li>可从合作伙伴仪表板的“计费”页面查看和下载发票和对帐文件。 请注意，从选定计费日期起四 (4) 天内可在合作伙伴仪表板获得每月发票。</li>
</ul></td>
</tr>
<tr class="odd">
<td>调整/信用/取消</td>
<td><ul>
<li>应用信用或调整后，可在下一张计费发票上看到调整和拖欠的信用。</li>
</ul></td>
</tr>
<tr class="even">
<td>税务</td>
<td><ul>
<li>将根据你的详细信息（而非客户的详细信息）对你收取税款 ，因为计费关系在你和 Microsoft 之间产生。</li>
<li>可在登记过程中或通过服务请求提交税收 ID。 你将看到在下一个计费周期上反映的更改。</li>
<li>对于<strong>扣缴税款和营业税免征</strong>，必须通过服务请求提交税收文档。 你将在下一个计费周期上看到更改和相应退款。</li>
<li>对于<strong>增值税 (VAT) 免征</strong>，必须通过服务请求提交 VAT ID（由 Microsoft 验证）。 你将在下一个计费周期上看到更改和相应退款。</li>
<li>从本地税务局或税务顾问查找进一步的税收详细信息。</li>
</ul></td>
</tr>
</tbody>
</table>

 

## <a name="license-based-billing"></a>基于许可证的计费



<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>计费规则</td>
<td><ul>
<li>订阅为一年期并且自动续订。</li>
<li>每个年度订阅的计费分 12 个月付款。</li>
<li>对于基于许可证的服务，将会提前向你收取下一个计费时段费用（取决于上一个计费时段结束时的许可证数）。</li>
<li>将针对许可证数目发生的任何更改对你计费/记入欠款（根据许可证天数按比例计算）。 按比例计算使用以下公式：[ROUND((ROUND(单价 * 数量 / 按比例计算的月份的天数, 2) * 按比例计算的天数) / 数量, 2) * 数量]</li>
<li>将针对所售席位（而非预配的席位）收取相关付款。</li>
</ul></td>
</tr>
<tr class="even">
<td>调整/信用/取消</td>
<td><ul>
<li>当前不对取消基于许可证的服务收取提前终止费用。</li>
<li>对于周期中取消，基于许可证的服务的取消信用针对未使用天数（以及按照上述公式的许可证减少）按比例计算。</li>
</ul></td>
</tr>
</tbody>
</table>

 

## <a name="usage-based-billing"></a>基于使用情况的计费


Azure 按“即付即用”模型运作，在此模型中仅针对已使用的 Azure 服务向你计费。

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>计费规则</td>
<td><ul>
<li>订阅按月划分，并且以新的按使用量计费的服务费率自动续订。 计费基于使用情况按月延后。</li>
<li>按使用量计费的服务费率可能在发票周期内更改。
<ul>
<li>提价：提前 30 天通知。</li>
<li>降价：在更改之日反映。</li>
<li>现有订阅使用在计费周期开始时生效的费率。</li>
<li>新订阅（在计费周期内创建）使用创建当日生效的费率。</li>
</ul></li>
</ul></td>
</tr>
<tr class="even">
<td>调整/信用/取消</td>
<td><ul>
<li>你将在下一个每月计费发票上看到经过调整的付款。</li>
<li>当前不对取消基于使用情况的服务收取早期终止费用。</li>
<li>你将在下一个每月计费发票上看到所有类型的信用，包括 SLA 信用。</li>
</ul></td>
</tr>
</tbody>
</table>

