---
title: 使用对帐文件 | 合作伙伴中心
ms.topic: article
ms.date: 07/08/2019
description: 若要详细了解计费周期中的每个费用, 请从合作伙伴中心下载协调文件。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8fae84790aa84b3c5a006d65a632668a33ac24a7
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820564"
---
# <a name="use-the-reconciliation-files"></a>使用对帐文件

**适用于**

-  合作伙伴中心
-  Microsoft Cloud for US Government 合作伙伴中心


若要详细了解计费周期中的每个费用, 请从合作伙伴中心下载协调文件。 详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。

## <a name="formatting-issues"></a>格式化问题

有时, 侦测文件可能会出现格式问题。 (例如, 如果不使用 EN-US 区域设置, 则可能会发生这种情况。)请按照以下步骤来解决这些问题。 

<ol>
<li>在 Excel 中打开 .csv 文件, 然后选择第一列。 在功能区上, 选择 "<strong>数据</strong>", 然后选择 "<strong>文本到列</strong>"。</li>

<li>在 "将文本转换为列" 向导中, 选择 "<strong>分隔文件类型</strong>", 然后选择 "<strong>下一步</strong>"。</li> 

<li>在分隔符字段中, 选择 "<strong>逗号</strong>"。 如果已选择<strong>"选项卡</strong>", 则可以保留它。 选择“<strong>下一步</strong>”。</li>

<li>在 "列数据格式" 字段中<strong>, 选择 Date:MDY</strong>, 然后选择 "<strong>下一步</strong>"。</li> 

<li>在 "列数据格式" 字段中, 为 "所有数量" 列选择 "<strong>文本</strong>", 然后选择 "<strong>完成</strong>"。</li>
</ol>

## <a name="downloading-a-large-recon-file"></a>下载大型侦测文件

侦测文件可能会变得非常大, 有时很难下载。 有关用于帮助下载大型侦测文件的 PowerShell 脚本, 请参阅[获取发票行项](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。

## <a href="" id="itemizebypartner"></a>按合作伙伴列举


间接模型中的合作伙伴可以在基于许可证和基于使用情况的对帐文件中使用这些额外字段，以便由经销商列出明细。

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>MPN ID</th>
<th>描述</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>MPN ID</td>
<td><p>CSP 合作伙伴（直接或间接）的 Microsoft 合作伙伴网络 (MPN) ID。</p></td>
</tr>
<tr class="even">
<td>经销商 MPN ID</td>
<td><p>仅显示在间接模型中合作伙伴的对帐文件上。</p>
<p>订阅记录的经销商 MPN ID。 这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</p>
<p>eTo 查看或更新经销商, 从合作伙伴中心菜单中选择 "<strong>客户</strong>", 然后从列表中选择客户。 在客户菜单中，选择“订阅”，然后从列表中选择订阅。 选择“更新”以更改“经销商 (MPN ID)”。</p>
<p>如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</p>
<p>如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</p>
<p>如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a>基于许可证的文件字段


若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>该列</strong></td>
<td><strong>说明</strong></td>
<td><strong>示例值</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>特定计费单位的唯一标识符（采用 GUID 格式）。 对帐不需要，但可能是有用的信息。 在所有行中均相同。</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 帐单平台中订单的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订单非常有用。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 帐单平台中订阅的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</p>
<p>这与合作伙伴管理员控制台中的订阅 ID 不相同。 请参阅 Syndication_Partner_Subscription_Number。</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>订阅的唯一标识符。 客户的同一个计划可能有多个订阅，因此这对于对帐文件分析非常重要。</p>
<p>此字段将映射到合作伙伴管理员控制台中的订阅 ID。</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>唯一的产品/服务 ID。 根据价目表的标准产品/服务 ID。</p>
<p><b>注意</b>：此值与价目表中的产品 ID 不匹配。 请参阅下方的 DurableOfferID。</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>唯一的持久型产品 ID，如价目表中所定义。</p>
<p><b>注意</b>：此值与价目表中的产品 ID 匹配。</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>客户购买的服务产品的名称，如价目表中所定义。</p></td>
<td>Microsoft Office 365（计划 E3）</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>订阅开始日期，设置为提交订单后的第二天。 通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</p>
<p>时间始终是一天的开始，即 0:00。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>订阅结束日期:12个月 + 开始日期之后的 x 天 (与合作伙伴计费日期相同) 或从续订日期起的12个月。</p>
<p>续订时，价格将更新为当前价目表。 自动续订之前可能需要与客户进行通信。</p>
<p>时间始终是一天的开始，即 0:00。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>费用的开始日。</p>
<p>当客户更改座位数量时，此数字用于计算每日（按比例）费用。</p>
<p>时间始终是一天的开始，即 0:00。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>费用的结束日。</p>
<p>当客户更改座位数量时，此数字用于计算每日（按比例）费用。</p>
<p>时间始终是一天的结束，即 23:59。</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>费用或调整的类型。 请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</p></td>
<td><p>请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>购买时公布在价目表中的每一席位的价格。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>数量</td>
<td><p>席位的数量。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>金额</td>
<td><p>数量的总价。 在检查金额计算是否匹配你为客户计算此项的方式时非常有用。</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>适用于这些费用的折扣金额。 资格或地图随附的产品许可证或适用于激励的新订阅还将在此列中包含折扣金额。</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>小计</td>
<td><p>税前总额。 如果有折扣，请检查你的小计是否匹配你的预期总额。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>税</td>
<td><p>根据你的市场&#39;税率规则和特定情况收费。</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>税后总额。 检查你是否在发票中计入了税务。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>货币类型。 每个计费单位仅使用一种货币。 检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>合作伙伴&#39;中心报告的客户组织名称。 这在使用系统信息对发票进行对帐时非常有用。</p></td>
<td>测试客户 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>云解决方案提供商合作伙伴的 MPN ID</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>订阅的记录经销商的 MPN ID。 请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>客户&#39;的域名, 用于帮助确定客户身份。 这不应用于唯一地标识客户, 因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。 该字段在第二个计费周期之前可能会显示为空白。</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>订阅昵称。 如果未指定昵称，合作伙伴中心将使用 OfferName。</p></td>
<td>联机项目</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>客户购买的服务产品的名称，如价目表中所定义。 （与产品/服务名称字段相同）。</p></td>
<td>不带项目客户端的高级联机项目</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>基于使用情况的文件字段


若要针对你的客户的使用情况进行费用对帐，请比较对帐文件中的 ResellerID/ResellerName/ResellerBillableAccount、客户名称与合作伙伴中心中的订阅 ID。

以下字段说明已使用的服务和费率。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>该列</strong></td>
<td><strong>说明</strong></td>
<td><strong>示例值</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>合作伙伴 ID（采用 GUID 格式）。</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>合作伙伴名称。</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>合作伙伴帐户 ID。</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>合作伙伴&#39;中心报告的客户组织名称。 这在使用系统信息对发票进行对帐时非常有用。</p></td>
<td>测试客户 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>云解决方案提供商合作伙伴的 MPN ID。</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>订阅的记录经销商的 MPN ID。 请参阅<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">由合作伙伴列出明细</a>。</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>显示执行交易所在的发票号码。</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</p>
<p>时间始终是一天的开始，即 0:00。</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。</p>
<p>时间始终是一天的结束，即 23:59。</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 帐单平台中订阅的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</p>
<p>这与合作伙伴管理员控制台中的订阅 ID 不相同。</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>服务产品的昵称。</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>服务产品的业务线</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 帐单平台中订单的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>存在问题的 Azure 服务的名称。</p></td>
<td>虚拟机</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Windows Azure 服务的特定类型。</p></td>
<td><ul>
<li>服务总线 – 个人或包</li>
<li>SQL Azure 数据库 – 商用版或 Web 版</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>所有服务数据和定价结构的特定唯一标识符。</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>资源名称</td>
<td><p>Azure 资源的名称。</p></td>
<td><ul>
<li>数据传输入 (GB)</li>
<li>数据传输出 (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>使用情况适用的区域。 主要用于分配数据传输的速率，速率因地区而异。</p></td>
<td>亚太、欧洲、拉丁美洲、北美</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>产品/服务的 MSFT 唯一标识符</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>用于针对给定计费周期中的服务或资源细分不同费率的 ID 和数量。 对于 Azure 分层分级，某个特定数量的计费单位最多只有一个费率，之后就是不同的费率。</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>报告期间的服务消耗量（小时，GB 等）。</p>
<p>此外还包括来自以前报告期间任何未开票的使用量。</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>作为产品/服务的一部分包含在内的单位。 通常不显示在云解决方案提供商中。</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>不作为产品/服务的一部分包含在内的单位，但必须由合作伙伴支付费用。</p>
<p>等于 ConsumedQuantity - IncludedQuantity。</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>订阅开始日期的有效产品/服务价格。</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrice 乘以 OverageQuantity，四舍五入到最接近的分。</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>根据你的市场&#39;税率规则和特定情况收费。</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>税后总额（如果税务适用）。</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>货币类型。 每个计费单位仅使用一种货币。 检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>每一单位的税前价格。 等于 PretaxCharges / OverageQuantity，四舍五入到最接近的分。</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>每一单位的税后价格。 等于 PostTaxTotal / OverageQuantity，或者 PretaxEffectiveRate + 每一单位量税率，四舍五入到最接近的分。</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>费用或调整的类型。 请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</p></td>
<td><p>请参阅“<a href="#charge_types">映射发票与对帐文件之间的费用</a>”</p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>MSFT 帐单平台中的唯一帐户 ID。</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>服务部署日期。</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</p></td>
<td>东亚、东南亚、北欧、西欧、美国中北部、美国中南部</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>此列专用于跟踪无法在“服务名称”列中特别标识的个别 Microsoft Azure 服务。 例如，数据传输在“服务名称”列中报告为 &quot;Microsoft Azure - 所有服务&quot;。 此 MeteredService 列将指示使用情况适用的特定服务。</p></td>
<td>访问控制、CDN、计算、数据库、服务总线、存储</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>进一步阐明超过 MeteredService 字段所提供级别的个别 Microsoft Azure 服务的副标题。</p></td>
<td>外部</td>
</tr>
<tr class="even">
<td>项目</td>
<td><p>客户定义的用于其服务实例的名称</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>已预配并且已在指定日利用的服务总线连接数。</p></td>
<td>例如：如果你在一个月 30 天内有单独的已预配连接，则服务信息 1 将读取“1.000000 连接/ 30 天”。 如果你预配了25个 2: 1/2 pack 连接, 并且在该天内使用了 1, 则该天的每日使用声明将显示 "25 个连接/30 天-使用:1.000000 "。</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>客户&#39;的域名, 用于帮助确定客户身份。 该字段在第二个计费周期之前可能会显示为空白。</p></td>
<td>example.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>单位</td>
<td><p>资源名称的单位</p></td>
<td>GB 或小时</td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a>一次性和定期文件字段

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>列</th>
<th>描述</th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td>PartnerId</td>
<td><p>特定计费实体的唯一 Microsoft Azure Active Directory 租户标识符, 采用 GUID 格式。 对帐不需要，但可能是有用的信息。 在所有行中均相同。</p></td>
</tr>

<tr class="even">
<td>客户 Id</td>
<td><p>用于标识客户的唯一 Microsoft Azure Active Directory 租户 ID, 采用 GUID 格式。</p></td>
</tr>

<tr class="odd">
<td>客户名称</td>
<td><p>在合作伙伴中心中报告的客户的组织名称。</p></td>
</tr>

<tr class="even">
<td>CustomerDomainName</td>
<td><p>客户的域名，用于帮助识别客户。 这不应用于唯一地标识客户, 因为客户/合作伙伴可以通过 O365 门户更新虚/默认域。 该字段在第二个计费周期之前可能会显示为空白。</p></td>
</tr>

<tr class="odd">
<td>客户所在国家/地区</td>
<td><p>客户所在的国家/地区。</p></td>
</tr>

<tr class="even">
<td>发票编号</td>
<td><p>显示执行交易所在的发票号码。</p></td>
</tr>

<tr class="odd">
<td>MpnId</td>
<td><p>云解决方案提供商合作伙伴的 MPN ID。</p></td>
</tr>

<tr class="even">
<td>经销商 MpnId</td>
<td><p>订阅的记录经销商的 MPN ID。</p></td>
</tr>

<tr class="odd">
<td>订单编码</td>
<td><p>Microsoft commerce 平台中订单的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订单非常有用。</p></td>
</tr>

<tr class="even">
<td>订单日期</td>
<td><p>下达订单的日期。</p></td>
</tr>

<tr class="odd">
<td>ProductId</td>
<td><p>产品的 ID。</p></td>
</tr>

<tr class="even">
<td>SkuId</td>
<td><p>特定 SKU 的 ID。</p></td>
</tr>

<tr class="odd">
<td>AvailabilityId</td>
<td><p>特定可用性的 ID。 “可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</p></td>
</tr>

<tr class="even">
<td>SKU 名称</td>
<td><p>特定 SKU 的名称。</p></td>
</tr>

<tr class="odd">
<td>产品名称</td>
<td><p>产品的名称。</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>产品发布者的名称。</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>此发布服务器的唯一 ID。</p></td>
</tr>

<tr class="even">
<td>订阅说明</td>
<td><p>订阅的友好名称。</p></td>
</tr>

<tr class="odd">
<td>订阅 ID</td>
<td><p>Microsoft commerce 平台中订阅的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订阅非常有用。 这与合作伙伴管理员控制台中的订阅 ID 不相同。</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>费用的开始日。 时间始终是一天的开始，即 0:00。</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>费用的结束日。 时间始终是一天的结束，即 23:59。</p></td>
</tr>

<tr class="even">
<td>术语和 Billingcycle</td>
<td><p>采购的术语长度和计费周期。 例如, "1 年, 每月"。</p></td>
</tr>

<tr class="odd">
<td>费用类型</td>
<td><p>费用或调整的类型。</p></td>
</tr>

<tr class="even">
<td>单价</td>
<td><p>购买时在 pricelist 中发布的价格。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
</tr>

<tr class="odd">
<td>有效单价</td>
<td><p>进行调整后的单位价格。</p></td>
</tr>

<tr class="even">
<td>数量</td>
<td><p>单位数。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
</tr>

<tr class="odd">
<td>单位类型</td>
<td><p>要购买的单位类型。</p></td>
</tr>

<tr class="even">
<td>DiscountDetails</td>
<td><p>适用于任何适用折扣的说明。</p></td>
</tr>

<tr class="odd">
<td>Sub Total</td>
<td><p>税前总额。 如果有折扣，请检查你的小计是否匹配你的预期总额。</p></td>
</tr>

<tr class="even">
<td>税金总计</td>
<td><p>税务金额费用，基于你的市场税务规则和特定情况。</p></td>
</tr>

<tr class="odd">
<td>总计</td>
<td><p>税后总额。 检查你是否在发票中计入了税务。</p></td>
</tr>

<tr class="even">
<td>Currency</td>
<td><p>货币类型。 每个计费单位仅使用一种货币。 检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</p></td>
</tr>

<tr class="odd">
<td>AlternateID</td>
<td><p>订单 ID 的备用标识符。</p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a>每日分级使用文件字段


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>列</th>
<th>描述</th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td>PartnerId</td>
<td><p>合作伙伴 ID（采用 GUID 格式）。</p></td>
</tr>

<tr class="even">
<td>PartnerName</td>
<td><p>合作伙伴名称。</p></td>
</tr>

<tr class="odd">
<td>CustomerId</td>
<td><p>唯一 Microsoft ID（采用 GUID 格式），用于识别客户。</p></td>
</tr>

<tr class="even">
<td>CustomerCompanyName</td>
<td><p>在合作伙伴中心中报告的客户的组织名称。 这在使用系统信息对发票进行对帐时非常有用。</p></td>
</tr>

<tr class="odd">
<td>CustomerDomainName</td>
<td><p>客户的域名。 对当前活动不可用。</p></td>
</tr>

<tr class="even">
<td>客户所在国家/地区</td>
<td><p>客户所在的国家/地区。</p></td>
</tr>

<tr class="odd">
<td>MPNID</td>
<td><p>云解决方案提供商合作伙伴的 MPN ID。</p></td>
</tr>

<tr class="even">
<td>经销商 MPNID</td>
<td><p>订阅的记录经销商的 MPN ID。 对当前活动不可用。</p></td>
</tr>

<tr class="odd">
<td>InvoiceNumber</td>
<td><p>显示执行交易所在的发票号码。 对当前活动不可用。</p></td>
</tr>

<tr class="even">
<td>ProductId</td>
<td><p>产品的 ID。</p></td>
</tr>

<tr class="odd">
<td>SkuId</td>
<td><p>特定 SKU 的 ID。</p></td>
</tr>

<tr class="even">
<td>AvailabilityId</td>
<td><p>特定可用性的 ID。 “可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。</p></td>
</tr>

<tr class="odd">
<td>SKU 名称</td>
<td><p>特定 SKU 的名称。</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>发布服务器的名称。</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>GUID 格式的发布服务器的 ID。 对当前活动不可用。</p></td>
</tr>

<tr class=”even">
<td>订阅说明</td>
<td><p>客户购买的服务产品的名称，如价目表中所定义。 （与产品/服务名称字段相同）。</p></td>
</tr>

<tr class="odd">
<td>订阅 ID</td>
<td><p>Microsoft 帐单平台中订阅的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订阅非常有用。 这与合作伙伴管理员控制台中的订阅 ID 不相同。</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>计费周期的开始日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。 时间始终是一天的开始，即 0:00。</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>计费周期的结束日期，之前未付款的潜在使用情况数据（来自上一个计费周期）的显示日期除外。 时间始终是一天的结束，即 23:59。</p></td>
</tr>

<tr class="even">
<td>使用日期</td>
<td><p>服务使用日期。</p></td>
</tr>

<tr class="odd">
<td>计量类型</td>
<td><p>计量器的类型。</p></td>
</tr>

<tr class="even">
<td>计量类别</td>
<td><p>使用的顶级服务。</p></td>
</tr>

<tr class="odd">
<td>计量 Id</td>
<td><p>正在使用的计量的 ID。</p></td>
</tr>

<tr class="even">
<td>计量子类别</td>
<td><p>可能影响速度的 Azure 服务类型。</p></td>
</tr>

<tr class="odd">
<td>计量名称</td>
<td><p>所使用的计量的度量单位。</p></td>
</tr>

<tr class="even">
<td>计量区域</td>
<td><p>此列标识服务的区域内的数据中心的位置（该位置适用且人口密集）。</p></td>
</tr>

<tr class="odd">
<td>单位</td>
<td><p>资源名称的单位。</p></td>
</tr>

<tr class="even">
<td>已消耗数量</td>
<td><p>报告期间的服务消耗量（小时，GB 等）。 此外还包括来自以前报告期间任何未开票的使用量。</p></td>
</tr>

<tr class="odd">
<td>资源位置</td>
<td><p>计量器正在其中运行的数据中心。</p></td>
</tr>

<tr class="even">
<td>已使用服务</td>
<td><p>你使用的 Azure 平台服务。</p></td>
</tr>


<tr class="even">
<td>资源 URI</td>
<td><p>所使用资源的 URI。</p></td>
</tr>

<tr class="odd">
<td>费用类型</td>
<td><p>费用或调整的类型。 对当前活动不可用。</p></td>
</tr>

<tr class="even">
<td>单价</td>
<td><p>购买时在 pricelist 中发布的每个许可证的价格。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
</tr>

<tr class="odd">
<td>数量</td>
<td><p>许可证数量。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
</tr>

<tr class="even">
<td>单位类型</td>
<td><p>计量计量器的单位类型。 对当前活动不可用。</p></td>
</tr>

<tr class="odd">
<td>帐单税前税</td>
<td><p>税前的总金额。</p></td>
</tr>

<tr class="even">
<td>计费货币</td>
<td><p>客户的地理区域中的货币</p></td>
</tr>

<tr class="odd">
<td>定价 pretax 总计</td>
<td><p>添加税款之前的定价。</p></td>
</tr>

<tr class="even">
<td>定价货币</td>
<td><p>Pricelist 中的货币。</p></td>
</tr>

<tr class="odd">
<td>服务信息1</td>
<td><p>已预配并且已在指定日利用的服务总线连接数。</p></td>
</tr>

<tr class="even">
<td>服务信息2</td>
<td><p>捕获可选的服务特定元数据的旧字段。</p></td>
</tr>

<tr class="even">
<td>附加信息</td>
<td><p>其他列中未涵盖的任何其他信息。</p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a>发票与对帐文件之间的映射费用

发票是费用的汇总，而对帐文件提供行项交易的明细，包括费用类型。

若要交叉引用发票与对帐文件之间的费用金额，可以使用 Microsoft Excel 的筛选器选项在对帐文件上按照费用类型进行筛选，以将发票金额映射到对帐文件的一系列费用明细上。

基于使用情况和基于许可证的对帐文件仅显示与使用量相关的交易和费用（所用数量以及相关费用）。 对帐文件中不显示发票上显示为“调整”的一次性积分、折扣或退款。

下表显示了发票部分与可能在对帐文件上显示的相关费用类型之间的映射。 

<table>
<tbody>
<tr>
<td>
<p><strong>发票费用说明</strong></p>
</td>
<td>
<p><strong>对帐文件费用说明 (ChargeType 列)</strong></p>
</td>
<td>
<p><strong>此费用是什么？</strong></p>
</td>
<td>
<p><strong>如何实现将这些 ChargeTypes 映射到发票？</strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong>基于许可证的费用</strong></p>
</td>
<td>
<p>激活费用</p>
</td>
<td>
<p>客户购买后使用订阅时向其收取的金额</p>
</td>
<td rowspan="10">
<p>从基于许可证的文件，对 <strong>Amount</strong> 列求和</p>
</td>
</tr>
<tr>
<td>
<p>取消费用</p>
</td>
<td>
<p>相关席位发生变化时，退款给客户的按比例计算的费用</p>
</td>
</tr>
<tr>
<td>
<p>周期费用</p>
</td>
<td>
<p>订阅的定期费用</p>
</td>
</tr>
<tr>
<td>
<p>周期实例按比例计算</p>
</td>
<td>
<p>相关席位发生变化时，客户评估的按比例计算的费用</p>
</td>
</tr>
<tr>
<td>
<p>按比例计算取消时的费用</p>
</td>
<td>
<p>取消后服务的未使用部分按比例计算的退款</p>
</td>
</tr>
<tr>
<td>
<p>按比例计算购买时的费用</p>
</td>
<td>
<p>使用年度计费时的订阅费用类型</p>
</td>
</tr>
<tr>
<td>
<p>购买费用</p>
</td>
<td>
<p>使用月度帐单时的订阅费用类型</p>
</td>
</tr>
<tr>
<td>
<p>按比例计算续订时的费用</p>
</td>
<td>
<p>订阅续订后按比例计算的费用</p>
</td>
</tr>
<tr>

<td>
<p>续订费用</p>
</td>
<td>
<p>续订订阅费用</p>
</td>
</tr>
<tr>
<td>
<p>按比例计算激活时的费用</p>
</td>
<td>
<p>从激活到计费周期结束时间段内按比例计算的费用</p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><strong>一次性费用</strong></p>

</td>
<td>
<p>新增</p>
</td>
<td>
<p>创建新购买时使用</p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p>addQuantity</p>
</td>
<td>
<p>用于原始购买的退款和增加后的新数量</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>removeQuantity</p>
</td>
<td>
<p>用于原始购买的退款和减少后的新数量</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Cancel</p>
</td>
<td>
<p>取消订阅时使用</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>转换</p>
</td>
<td>
<p>升级许可证时使用, 但座位数保持不变</p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><strong>使用费用</strong></p>
</td>
<td>
<p>评估取消时的使用费用</p>
</td>
<td>
<p>评估当前计费周期内取消未付款使用量的使用费用</p>
</td>
<td rowspan="2">
<p>从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</p>
</td>
</tr>
<tr>
<td>
<p>评估当前周期的使用费用</p>
</td>
<td>
<p>访问当前计费周期的使用费用</p>
</td>
</tr>

<tr>
<td>
<p><strong>制作</strong></p>
</td>
<td>
<p>偏移行项</p>
</td>
<td>
<p>部分或全部退款到行项，包括税款</p>
</td>
<td>
<p>从基于许可证的文件，对 <strong>TotalForCustomer</strong> 列求和</p>
<p>从基于使用情况的文件，对 <strong>PostTaxTotal</strong> 列求和</p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong>基于使用情况的折扣</strong></p>
</td>
<td>
<p>激活折扣</p>
</td>
<td>
<p>激活订阅时应用的折扣</p>
</td>

<td rowspan="4">
<p>从基于使用情况的文件，对 <strong>PretaxCharges</strong> 列求和</p>
</td>
</tr>
<tr>
<td>
<p>周期折扣</p>
</td>
<td>
<p>对定期费用应用的折扣</p>
</td>
</tr>
<tr>
<td>
<p>续订折扣</p>
</td>
<td>
<p>续订订阅时应用的折扣</p>
</td>
</tr>
<tr>
<td>
<p>取消折扣</p>
</td>
<td>
<p>取消折扣时应用的费用</p>
</td>
</tr>


<tr>
<td>
<p><strong>基于许可证的折扣</strong></p>
</td>
<td>
<p><em>可应用于多种费用类型</em></p>
</td>
<td>
<p></p>
</td>
<td>
<p>从基于许可证的文件，对 <strong>TotalOtherDiscount</strong> 列求和</p>
</td>
</tr>
<tr>
<td>
<p><strong>税款</strong>&nbsp;或&nbsp; <strong>VAT</strong></p>
</td>
<td>
<p><em>可应用于多种费用类型</em></p>
<p><em>异常：&quot;偏移行项&quot;已包含税金。请参阅上面的信用额度。</em></p>
</td>
<td>
<p>税款或增值税 (VAT)</p>
</td>
<td>
<p>从基于许可证的文件，对 <strong>Tax</strong> 列求和</p>
<p>从基于使用情况的文件，对 <strong>TaxAmount</strong> 列求和</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
