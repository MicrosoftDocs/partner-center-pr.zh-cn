---
title: Azure 计划计费 | 合作伙伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何访问和理解与 Azure 计划计费相关的发票和对帐文件结构。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: b52030f4956f8b3f86eec5aad72628dc64099729
ms.sourcegitcommit: f5dbf96c1dece9c766e9b4c1527e599872e2ab14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/26/2019
ms.locfileid: "74536452"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP 中的新商务体验 - Azure 计费 

**相应的角色：**

- 帐单管理员
- 管理员代理
- 全局管理员


Azure 计划中的计费是一个简化的计费体验，它使用一致的单一计费日期和基于日历月份的计费周期。 有关该计费平台的信息，请阅读[计费概述](billing-basics.md)。

## <a name="summary-of-billing-essentials"></a>计费概要

- **发票日期**：发票和对帐文件将在 8 号（UTC 午夜）在合作伙伴中心仪表板/API 中提供。

- **发票计费周期**：发票计费周期与日历月份相一致，例如 10/1 - 10/31、11/1 - 11/30。

- **费用服务周期**：费用与日历月份相一致。 例如，如果计费合作伙伴在 10/15 通过 Azure 计划添加了 Azure 服务，而客户在 10/15 开始使用 Azure 服务，则计费合作伙伴将在 11/8 收到客户在服务周期 10/15 - 10/31 的使用费发票/对帐文件。 在 12/8 生成的下个月发票包含服务周期 11/1 - 11/31 的所有费用。

- **发票付款期限**：净 60 天。

- **发票货币**：继续按客户所在国家/地区的指定货币对合作伙伴计费。 例如，如果计费合作伙伴位于爱尔兰，而客户位于英国、挪威和德国，则计费合作伙伴将收到英镑、挪威克朗和欧元货币的发票/对帐文件。

- **合作伙伴奖励**：从发票月份结束时间起的 45 天付费。

## <a name="access-your-invoices-and-reconciliation-files"></a>访问发票和对帐文件

当某份发票可供查看时，公司的全局管理员或计费管理员会收到电子邮件。 

**访问发票和对帐文件**

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/en-us/dashboard/)。

2. 在“合作伙伴中心”菜单中，选择“计费”。 

3. 选择“定期”和“一次性”选项卡，以及所需货币   。

![计费](images/azure/billing1.png)

4. 选择“发票”或“对帐文件”   。  

若要查看历史发票和对帐文件，请展开下面的“计费历史记录”行。


## <a name="understanding-usage-data"></a>了解使用情况数据 

1. Azure 计划是使用情况的根或顶级容器。 所有使用情况都要关联回单个 Azure 计划。 

2. 一个计划中将有一个或多个 Azure 订阅。 这些容器用于资源管理和部署。 

3. 在订阅中，资源组将添加到组资源。 每个资源都将部署到一个资源组。 

4. 示例资源包括虚拟机和存储帐户。 

5. 资源发出计量：计量是资源的消耗度量，一个资源可能会为多个计量发出使用情况。 计量由 ProductId、SKUId 和 AvailabilityId 标识。 

### <a name="heirarchy-of-subscription-resource-groups-and-metering"></a>订阅资源组和计量的层次结构

**Azure 帐户（租户）**

- 订阅 A
    - ResourceGroup 1
        - 虚拟机（资源）
            - 计算计量
        - 虚拟网络（资源）
            - 无计费计量

    - ResourceGroup 2
        - 虚拟机（资源）
            - 计算机计量
        - 高级 SSD 托管磁盘（资源）
            - 存储容量计量
            - 存储操作计量

- 订阅 B   -ResourceGroup 1       - Azure SQL（资源）           - DTU 计量       - VPN 网关（资源）           - VPN 网关计量

    - ResourceGroup 2
        - 虚拟网络接口（资源）
            - 无计费计量

## <a name="read-the-invoice"></a>阅读发票

1. 提供发票的日期不会晚于每个月的 8 号。

2. 合作伙伴可在 60 天内汇款。

3. 计费周期涵盖给定的日历月份，例如 10/1 - 10/31。

4. 费用是净调整额（金额是“合作伙伴赚取的托管服务返点”的净额）。

5. 查看发票对帐文件和每日分类的使用情况文件，以了解更多计费详细信息。

![发票](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a>阅读发票对帐文件

1. 在对帐文件中，每个 Azure 计划和计量组合最多可以有两个计费行。

2. 如果该计量项目符合任何类型的折扣或返点（例如，分级折扣，或合作伙伴赚取的托管服务返点）条件，则对帐文件只包含一个计费行。 PriceAdjusmentDescription 列将引用折扣或赚取的返点  。

3. 如果特定计量项目中的资源都不符合折扣或合作伙伴赚取的返点条件，则对帐文件只包含一个计费行，有效单价是零售价（即单价）。

4. 如果该计量项目或发出该计量项目的任何资源在当月的某些日期符合合作伙伴赚取的托管服务返点条件，则对帐文件将包含两个计费行  。 其中一行表示该计量项目符合条件的天数，另一行表示该计量项目不符合条件的天数。 

## <a name="read-the-daily-usage-file"></a>阅读每日使用情况文件

- Azure 计划中的订阅计量项目将会分类，并每日累积。 

- **合作伙伴赚取的托管服务返点**按日确定和应用。

- 对于月份中发生了消耗的每个日期，每个订阅计量项目都有对应的一行。

- 在以下示例中：

  - 计量项目在 7/1 - 7/3 符合**合作伙伴赚取的托管服务返点**条件（请注意，有效单价为零售价减去合作伙伴获取的返点）。

   - 计量项目在 7/4 - 7/7 不符合**合作伙伴赚取的托管服务返点**条件（请注意，有效单价为零售价）。

    - 计量项目在 7/8 - 7/31 符合**合作伙伴赚取的托管服务返点**条件（请注意，有效单价为零售价减去合作伙伴获取的返点）。

![对帐 2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a>采用客户货币的发票 

通过 Azure 计划销售的 Azure 服务按美元定价，并按客户所在国家/地区指定的货币计费。 如果计费货币不是美元，则发票的最后一页上会显示使用的外汇汇率 (FX)。 外汇汇率每月确定，并应用于随后的发票。 有关国家/地区货币的完整列表，请查看[新商务套餐在各个国家/地区的上市情况和客户货币矩阵](https://go.microsoft.com/fwlink/?linkid=2112354)。 

Microsoft 将使用 [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) 来确定外汇汇率，以此确定定价货币与计费货币之间的兑换率。 外汇汇率将在月份最后一日的前一天刷新，然后将会应用。

**示例**：服务周期 8 月 1 日 - 8 月 31 日的使用费将按 7 月 31 日发布的外汇汇率计费。 这些费用将显示在 9 月份的发票上，该发票的最后一页将注明外汇汇率。 

 
## <a name="azure-reservations"></a>Azure 预订 

如果通过 Azure 计划购买 [Azure 预留项](https://docs.microsoft.com/partner-center/azure-reservations)，最初只能在合作伙伴中心选择一次性计费。 Azure 门户提供每月计费。 将来，合作伙伴中心也会提供每月计费。 

## <a name="azure-spending"></a>Azure 支出 

现有 Azure 支出体验已更新，以支持合作伙伴中心中的新 Azure 计划计费。 这样合作伙伴可以实现以下操作：

- 查看、管理和接收在客户级设置的预算的警报 

- 查看 Azure 计划的总估算支出（按资源和计量级别细分）

由于通过 Azure 计划销售的 Azure 服务的计费模型是付后使用，因此，为了避免帐单超过预期，合作伙伴可以应用每月预算并跟踪用量百分比。 一次可对一个或多个客户应用预算。 

![Azure 支出](images/azure/azurespend.png)

**详细信息**

-  通过合作伙伴中心[面板](https://partner.microsoft.com/en-us/dashboard/)（需要登录）提供的价目表中提供了合作伙伴赚取的返点 (PEC) 的计算方式。 
   
-  [购买 Azure 计划](purchase-azure-plan.md)

-  [CSP 新商务体验的价目表](azure-plan-price-list.md)
