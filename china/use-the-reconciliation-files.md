---
title: "使用对帐文件（由世纪互联运营的合作伙伴中心）"
description: "有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。"
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: bcbfcb8db46b65e9c81d787038708fc3d0f8ec6a
ms.openlocfilehash: 85cfd718898e653f744d731d800979c15c665be2

---

# 使用对帐文件向客户开具帐单

**适用于**

-   由世纪互联运营的合作伙伴中心


有关计费周期中每项费用的明细项目详细视图，请从合作伙伴中心仪表板下载对帐文件。 详细信息包括每个客户的订阅费用和详细事件（例如中途向订阅添加席位）。


## 由合作伙伴列出明细

间接模型中的合作伙伴可以在基于许可证的对帐文件中使用这些额外字段，以便由经销商列出明细。

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
<td><p>云解决方案提供商合作伙伴（直接或间接）的 MPN ID。</p></td>
</tr>
<tr class="even">
<td>经销商 MPN ID</td>
<td><p>仅显示在间接模型中合作伙伴的对帐文件上。</p>
<p>订阅记录的经销商 MPN ID。 这对应于针对合作伙伴中心中的特定订阅所列的经销商 ID。</p>
<p>若要查看或更新经销商，请在“仪表板”菜单中，选择“客户”<strong></strong>，然后从列表中选择该客户。 在客户菜单中，选择“订阅”<strong></strong>，然后从列表中选择该订阅。 选择“更新”<strong></strong>以更改“经销商 (MPN ID)”<strong></strong>。</p>
<p>如果云解决方案提供商合作伙伴将订阅直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。</p>
<p>如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。</p>
<p>如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。</p></td>
</tr>
</tbody>
</table>

 

## 基于许可证的文件字段


若要针对你的客户订单进行费用对帐，请比较对帐文件中的 Syndication\_Partner\_Subscription\_Number 与合作伙伴中心中的订阅 ID。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>列</strong></td>
<td><strong>描述</strong></td>
<td><strong>示例值</strong></td>
</tr>
<tr class="even">
<td>OperatingUnit</td>
<td><p>特定计费单位的唯一标识符（采用 GUID 格式）。 对帐不需要，但可能是有用的信息。 在所有行中均相同。</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerNumber</td>
<td><p>客户的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别客户非常有用。</p></td>
<td>123456789</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>订单的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订单非常有用。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>订阅的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别订阅非常有用。</p>
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
<td><p>唯一的产品/服务 ID。 根据价目表的标准产品/服务 ID。</p></td>
<td>306855</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>唯一的持久型产品 ID，如价目表中所定义。</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>客户购买的服务产品的名称，如价目表中所定义。</p></td>
<td>Office 365</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>订阅开始日期，设置为提交订单后的第二天。 通过结合查看订阅开始日期和结束日期，你可以确定客户是仍在第一年的订阅期内，还是需要续订下一年的订阅。</p>
<p>时间始终是一天的开始，即 0:00。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>订阅结束日期：12 个月 + 开始日期之后的 x 天（以便与合作伙伴帐单日期一致）或从续订日期算起的 12 个月。</p>
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
<td><p>费用或调整的类型。</p>
<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>费用：</td>
<td><ul>
<li>PURCHASE_FEE：订阅的初始费用</li>
<li>CYCLE_FEE：订阅的定期费用</li>
</ul></td>
</tr>
<tr class="even">
<td>ConvertResources</td>
<td><ul>
<li>CANCEL_USAGEFEE：在当前计费周期期间，取消后未付款使用情况的访问使用情况费用</li>
<li>CYCLE_USAGEFEE：当前计费周期的访问使用情况费用</li>
</ul></td>
</tr>
<tr class="odd">
<td>按比例：</td>
<td><ul>
<li>PURCHASE_PRORATE：购买后按比例计算的费用</li>
<li>CANCEL_PRORATE：取消后服务的未使用部分按比例计算的退款</li>
<li>ACTIVATION_PRORATE：从激活到计费周期结束时间段内按比例计算的费用</li>
<li>RENEW_PRORATE：订阅续订后按比例计算的费用</li>
</ul></td>
</tr>
<tr class="even">
<td>InstanceProrates：</td>
<td><ul>
<li>CANCEL_INSTANCEPRORATE：相关席位发生变化时，退款给客户的按比例计算的费用</li>
<li>CYCLE_INSTANCEPRORATE：相关席位发生变化时，客户评估的按比例计算的费用</li>
</ul></td>
</tr>
<tr class="odd">
<td>积分：</td>
<td><ul>
<li>CREDIT：适用于付款方式的积分</li>
</ul></td>
</tr>
<tr class="even">
<td>抵消：</td>
<td><ul>
<li>OFFSET_LINEITEM：明细项目的部分或全部退款</li>
<li>ONE_TIME_REFUND：针对客户处理的一次性退款</li>
<li>TAX_REFUND：因验证免税证而产生的退款</li>
</ul></td>
</tr>
<tr class="odd">
<td>折扣：</td>
<td><ul>
<li>ACTIVATION_DISCOUNT：订阅激活时所应用的折扣</li>
<li>CYCLE_DISCOUNT：定期费用所应用的折扣</li>
<li>RENEW_DISCOUNT：订阅续订时所应用的折扣</li>
<li>CANCEL_DISCOUNT：折扣取消时所应用的费用</li>
</ul></td>
</tr>
</tbody>
</table>
<p> </p></td>
<td></td>
</tr>
<tr class="odd">
<td>单价</td>
<td><p>每一席位的价格。 确保这与在对帐期间你的计费系统中存储的信息相匹配。</p></td>
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
<td><p>适用于这些费用的折扣金额。 IUR 或有资格获得奖励的新订阅还将包含此列中的折扣金额。</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>小计</td>
<td><p>税前总额。 如果有折扣，请检查你的小计是否匹配你的预期总额。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>税务</td>
<td><p>税务金额费用，基于你的市场税务规则和特定情况。</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>税后总额。 检查你是否在发票中计入了税务。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>货币</td>
<td><p>货币类型。 每个计费单位仅使用一种货币。 检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>在合作伙伴中心中报告的客户的组织名称。 这在使用系统信息对发票进行对帐时非常有用。</p></td>
<td>测试客户 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>云解决方案提供商合作伙伴的 MPN ID。</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>订阅的记录经销商的 MPN ID。</p></td>
<td>4390934</td>
</tr>
</tbody>
</table>

 



<!--HONumber=Oct16_HO3-->


