---
title: Azure 预订计费 | 合作伙伴中心
Description: Information about billing for Azure reservations.
author: v-petand
keywords: Azure RI, azure 预留实例, 预订, 虚拟机, 管理, 计费, 购买
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: 846f2863e9c4dc9967b8c337bcab40f153b99eb6
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489433"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Microsoft Azure 虚拟机预留实例计费

**适用范围**

-  合作伙伴中心
-  Microsoft Azure 门户
-  云解决方案提供商计划中的合作伙伴

云解决方案提供商计划 (CSP) 中的合作伙伴可以在 Microsoft Azure 虚拟机上为其客户提供预留实例。 客户可以提前预订一年或三年虚拟机 - 从而节省大量的 Azure 使用成本。   

客户可以提前为 Azure 虚拟机预留实例付款。 当你代表客户购买 Azure 虚拟机预留实例时，你将收到这些一次性费用的发票和对帐文件。 

>[!IMPORTANT]
>如果你在货币不同于你的货币的市场中为客户购买 Azure 虚拟机预留实例，则默认计费货币基于客户的市场，而不是你的位置。 如果你的客户遍布多个市场，那么你将收到对客户计费需要采用的每种货币的单独发票和对帐文件，并且能够使用相应的货币为客户开具发票。 

若要访问一次性费用发票和对帐文件，从合作伙伴中心中选择**计费**，然后选择**一次**。 

有关云解决方案提供商计划中的计费的更多一般信息，请参阅[计费基础知识](billing-basics.md)。

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Azure 虚拟机预留实例发票文件定义

**一般计费信息**

|**字段** |**定义**|
|:----------------|:-----------------------------|
|US FEIN |联邦税收 ID 编号。 |
|帐单邮寄地址 |用于税务用途的合法商业地址。 若要更改此地址，请转到“帐户设置”>“合作伙伴计费配置文件”。 |
|费用 |所有当前费用。 |
|退款额 |自首次购买以来退款活动的退款额。 |
|折扣 |可能适用于 Azure 预订或客户订单中的其他项目的折扣。 |
|税款 |在发票第 2 页开始的详细信息部分中统计的当前费用的总税款。 |
|当前总费用 |计费周期内以计费货币为单位的到期金额，在付款到期日期时到期。 |
|付款指示 |介绍何时以及如何根据所在区域支付你的发票。 在付款时，始终包括你的发票编号。 |
|发票编号 |发票的编号。 |
|发票日期 |生成发票的日期。 |
|付款期限 |对于一次性购买，此期限将始终为 60 天。 |
|付款截止日期 |必须在此日期前收到你的付款。 |


**一次性费用的明细列表**

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


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Azure 虚拟机预留实例对帐文件说明

|**字段** |**定义**|
|:----------------|:-----------------------------|
|PartnerId |合作伙伴 ID（采用 GUID 格式）。 |
|CustomerId |唯一 Microsoft ID（采用 GUID 格式），用于识别客户。 |
|CustomerName |在合作伙伴中心中报告的客户的组织名称。 这在使用系统信息对发票进行对帐时非常有用。 |
|CustomerDomainName |客户的域名。 |
|CustomerCountry |客户所在的国家/地区。 |
|InvoiceNumber |显示指定交易所在的发票号码。 |
|MpnId |云解决方案提供商合作伙伴（直接或间接）的 MPN ID。 |
|经销商 MPN ID |仅显示在间接模型中合作伙伴的对帐文件上。 预订记录的经销商 MPN ID。 这对应于针对合作伙伴中心中的特定预订所列的经销商 ID。 如果云解决方案提供商合作伙伴将预订直接销售给客户，他们的 MPN ID 会列出两次，即 MPN ID 和经销商 MPN ID。 如果云解决方案提供商合作伙伴的经销商没有 MPN ID，此值将设置为合作伙伴的 MPN ID。 如果云解决方案提供商合作伙伴删除经销商 ID，此值将设置为 -1。 |
|OrderId |Microsoft 帐单平台中订单的唯一标识符。 当联系支持人员而不用于对帐时，可能对识别 Azure 预订非常有用。 |
|OrderDate |下达订单的日期。 |
|ProductId |产品的 ID。 |
|SkuId  |特定 SKU 的 ID。 |
|AvailabilityId |特定可用性的 ID。 “可用性”是指针对给定的国家/地区、货币、行业细分市场等，是否可以购买特定 SKU。 |
|SkuName  |特定 SKU 的名称。 |
|ProductName |产品的名称。 |
|ChargeType |费用或调整的类型。 |
|UnitPrice |所订购的每个产品的价格。 |
|数量 |所订购产品的数量。 |
|小计 |税前总额。 如果有折扣，请检查你的小计是否匹配你的预期总额。 |
|TaxTotal |所有适用税款的总额。 |
|总计 |此订单的总额。 |
|货币 |货币类型。 每个计费单位仅使用一种货币。 检查它是否匹配你的第一张发票，然后检查在任何主要的帐单平台更新后是否匹配。 |
|DiscountDetails |任何相关折扣的详细列表。 |


## <a name="manage-your-billing"></a>管理你的计费

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>查看你的当前计费状态、发票和对帐文件

1.  在合作伙伴中心中，选择**计费**，然后**一次**以查看计费状态。 
2.  选择发票或对帐文件以查看更多详细信息。 

### <a name="view-a-customers-order-history"></a>查看客户的订单历史记录

1.  从合作伙伴中心菜单中选择**客户**。
2.  在你的**客户**页上，查找你想要查看其订单历史记录的客户，然后选择向下箭头以展开客户的记录。 
3.  选择**查看订单**以显示订单历史记录。

### <a name="create-a-credit-or-void-note"></a>创建退款或取消票据

在某些时候，你可能需要取消发票，然后开具一份新发票。 例如，客户可能会更改其公司的名称，然后收到具有旧名称的发票。 

若要取消发票并开具新发票，请在计费页面的调整下面下载表单。

## <a name="azure-reservations-resources"></a>Azure 预订资源
|**若要获取相关信息**   |**请阅读以下内容**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [销售 Microsoft Azure 虚拟机预留实例](azure-reservations.md)
|为你在合作伙伴中心中的客户购买 Azure 预订   |[购买 Azure 预订](azure-reservations-buying.md)
| 合作伙伴中心中管理 Azure 预订 | [合作伙伴中心中管理 Azure 预订](azure-reservations-manage.md)
|在 Azure 门户中购买 Azure 预订 | Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 门户中管理 Azure 预订   |Azure 帮助中的[管理虚拟机预留实例](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)

 
