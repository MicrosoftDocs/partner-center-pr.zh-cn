---
title: Insights 数据定义
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 该文档提供了各个报表的列表和每个报表的数据定义，这些报表可以从 "Insights 下载报表" 页下载。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501743"
---
# <a name="export--data-definitions"></a>导出–数据定义 

 **相应的角色** 

- 报表查看器 
- 主管人员报表查看器 

## <a name="introduction"></a>简介 

利用 Insights 仪表板中的 "下载报表" 中心，你可以导出原始数据集。  

可以与数据定义一起下载的各种报表如下所示： 

**合作伙伴配置文件**：配置文件报表的各个字段的数据定义如下： 


| **列名称** | **数据说明** |
|---------|:---------|
|MPNId|Microsoft 合作伙伴网络 ID|
|PartnerName|合作伙伴的名称 |
|PGA_MPNId|合作伙伴全局帐户 MPN ID|
|PGA_PartnerName|合作伙伴全局帐户名称|
|城市|合作伙伴的城市位置 |
|国家/地区|合作伙伴的国家/地区位置 |
|HierarchyLevel|指示它是全局 MPN ID 还是位置 MPN ID|

**客户详细信息**：客户详细信息报表的各个字段的数据定义包括：

| **列名称** | **数据说明** |
|---------|:---------|
|CustomerName|客户的名称 |
|CustomerTenantId|客户租户 ID |
|CustomerTpid|客户的上层父标识符 |
|CustomerSegment|Customer 段 |
|CustomerMarket|客户的地理市场  |
|CustomerStatus|客户状态 (Active/Inactive)  |
|产品|MPN 销售给客户的产品。 此项将是 O365、D365、企业移动性 Power BI Microsoft Azure 中的一个。|
|SKU|   产品 SKU|
|月份| 报告使用情况和收入的月份|
|MPNId| Microsoft 合作伙伴网络 ID|
|PartnerName|   合作伙伴的名称|
|PartnerLocation|   合作伙伴的地理位置|
|PartnerAttributionType|    伙伴的特性类型|
|SalesChannel|  销售渠道|
|AvailableSeats|    可用座位| 
|RevenueUSD|    以美元为单位的收入|

**经销商绩效**：《分销商性能报告的各个字段的数据定义：

> [!Note]
> 收入和 ACR 数据仅适用于作为 Executive 报表查看者的用户。

| **列名称** | **数据说明** |
|---------|:---------|
|ResellerMpnid|经销商 Microsoft 合作伙伴网络标识符| 
|经销商名称|经销商名称|
|ResellerMarket|市场分销商国家/地区| 
|IndirectProviderMPNId|间接提供程序 Microsoft 合作伙伴网络标识符|
|IndirectProviderName|间接提供程序名称|
|月份|报告使用情况和收入的月份|
|产品|产品名称|
|订阅 ID|订阅标识符|
|AvailableSeats|可用座位数|
|AssignedSeats|已分配的座位数|
|BilledRevenueUSD|$) 中的计费收入 (|
|CustomerName|客户的名称| 
|CustomerTPid|客户的上层父标识符| 
|CustomerSegment|Customer 段 |
|CustomerMarket|客户的地理市场 |
|ResellerStatus|经销商状态| 

**订阅详细信息**： "订阅详细信息" 报表的各个字段的数据定义包括：

>[!Note]
>收入和 ACR 数据仅适用于作为 Executive 报表查看者的用户

| **列名称** | **数据说明** |
|---------|:---------|
|SubscriptionId|    订阅的 GUID|
|SubscriptionStartDate| 订阅的开始日期|
|SubscriptionEndDate|   订阅的结束日期|
|SubscriptionState| 订阅 (Active 或改动) 的状态|
|月份| 报告使用情况和收入的月份|
|IsAutoRenew|   指示订阅是否自动续订或不 (的 Y/N) |
|CustomerName|  客户名称| 
|CustomerTenantId|  客户 GUID|
|CustomerTpid|  客户的上层父标识符| 
|CustomerSegment|   客户市场领域| 
|CustomerMarket|    客户的地理市场|
|产品|   合作伙伴向客户销售的产品| 
|SKU|   产品 Sku |
|MPNId| 合作伙伴 Microsoft 合作伙伴网络 ID |
|PartnerName|   合作伙伴的名称 |
|PartnerLocation|   合作伙伴的地理位置 |
|PartnerAttributionType|    订阅的特性类型|
|SalesChannel|  销售 (直接/CSP 等销售渠道 )  |
|AvailableSeats|    当前可用座位|
|RevenueUSD|    以美元为单位的收入|
|注册 ID| 订阅的注册 ID|

**Azure 使用情况**： Azure 使用情况报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|SubscriptionId|    订阅的 GUID|
|SubscriptionStartDate| 订阅的开始日期。|
|SubscriptionEndDate|   订阅结束的日期。|
|SubscriptionState| 订阅的当前状态 (打开/关闭/活动/InGrace 周期) |
|月份| 按月聚合的日期 |
|ServiceName|   Azure 服务的名称|
|MeterCategory| 计量类别的名称|
|UsageUnits|    计费周期期间使用的单位数 |
|CustomerName|  客户的名称 |
|CustomerTenantId|  客户的租户 ID |
|CustomerTpid|  客户的上层父 ID |
|CustomerSegment|   客户的细分 |
|CustomerMarket|    客户的地理市场 |
|MPNId  |客户 Microsoft 合作伙伴网络 ID |
|PartnerName|   合作伙伴的名称 |
|PartnerLocation    |合作伙伴的地理国家/地区位置 |
|PartnerAttributionType |伙伴的特性类型|
|SalesChannel|  销售渠道 (直接/CSP 间接/CSP 直接等 )  |
|ACR_USD|   采用 USD 的 Azure 消耗收入|
|注册 ID| Azure 订阅的注册 ID|

**Office 365-许可证使用**： office 365-许可证使用情况报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|CustomerTenantId|  客户的租户 ID| 
|CustomerTpid|  客户的上层父 ID |
|WorkloadName|  Sfb、团队、EXO 除外 |
|月份| 报告使用情况的月份|
|PaidAvailableUnits|    付费可用单位数|
|MonthlyActiveUsers|    每月活动用户数|
|CustomerName|  客户的名称|
|CustomerMarket|    客户市场的地理国家/地区位置 |
|CustomerSegment|   Customer 段 |
|MPNId| Microsoft 合作伙伴网络 ID|
|PartnerName|   合作伙伴的名称|
|PartnerLocation|   合作伙伴的地理位置|
|PartnerAttributionType|    伙伴的特性类型|

**企业移动性–许可证使用**： EMS –许可证使用情况报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|CustomerTenantId|  客户的租户 ID| 
|CustomerTpid|  客户的上层父 ID |
|WorkloadName|  EMS 工作负荷的名称 |
|月份| 报告使用情况的月份|
|PaidAvailableUnits|    付费可用单位数|
|MonthlyActiveUsers|    每月活动用户数|
|CustomerName|  客户的名称|
|CustomerMarket|客户市场的地理国家/地区位置 |
|CustomerSegment|   Customer 段 |
|MPNId| Microsoft 合作伙伴网络 ID|
|PartnerName|   合作伙伴的名称|
|PartnerLocation|   合作伙伴的地理位置|
|PartnerAttributionType|    伙伴的特性类型|

**Dynamics 365 –许可证使用**： Dynamics 365 –许可证使用情况报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|SubscriptionId|订阅的 GUID|
|SubscriptionStartDate| 订阅的开始日期|
|SubscriptionEndDate|   订阅的结束日期|
|SubscriptionStatus|    订阅状态 |
|月份| 报告使用情况的月份|
|RevSumDivisionName|    Rev sum 相除的名称|
|RevSumCategoryName|    Rev sum 类别的名称|
|SKU|   产品 Sku |
|SKUId| 产品的 Sku ID |
|FreeVsPaidSKU| 指示它是免费或付费 SKU |
|SalesModel|    用于销售订阅的销售渠道|
|DetailedSalesModel|    订阅的详细销售模型|
|CustomerName|  客户名称 |
|CustomerTenantId|  客户租户 GUID |
|CustomerTpid|  客户的上层父标识符 |
|CustomerSegment|   客户市场领域 |
|CustomerMarket|    客户的地理市场 |
|MPNId| Microsoft 合作伙伴网络 ID |
|PartnerName|   合作伙伴的名称 |
|PartnerLocation|   合作伙伴的地理国家/地区位置 |
|PartnerAttachType| 订阅的特性类型|
|AvailableSeats|    当前可用座位|
|AssignedSeats| 当前分配的座位 |
|ActiveSeats|   当前活动座位数 |
|DeploymentOpportunity| 当前部署机会|
|ActiveUsagePercent|    当前活动用量百分比|
 
**Power BI 许可证用法**： Power BI –许可证使用情况报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|SubscriptionId|    订阅的 GUID|
|SubscriptionStartDate| 订阅的开始日期|
|SubscriptionEndDate|   订阅的结束日期|
|SubscriptionStatus|    订阅状态 (活动或 In-Active 或宽限期) |
|月份| 按月聚合的日期 |
|SKU|   产品 Sku |
|SKUId| 产品的 Sku ID |
|FreeVsPaidSKU| 免费或付费 Sku 的优势 |
|SalesModel|    用于销售订阅的销售模型|
|DetailedSalesModel|    订阅的详细销售模型|
|CustomerName|  客户名称 |
|CustomerTenantId|  客户租户 GUID |
|CustomerTpid|  客户的上层父标识符| 
|CustomerSegment|   客户市场领域 |
|CustomerMarket|    客户的地理市场 |
|MPNId| Microsoft 合作伙伴网络 ID |
|PartnerName|   合作伙伴的名称 |
|PartnerLocation|   合作伙伴的地理国家/地区位置 |
|PartnerAttachType| 订阅的特性类型|
|AvailableSeats|    当前可用座位|
|AssignedSeats| 当前分配的座位|
|ActiveSeats|   当前活动座位数|
|DeploymentOpportunity| 当前部署机会|
|ActiveUsagePercent|    当前活动用量百分比|

**团队使用情况–会议和呼叫**：各个字段的数据定义如下：

| **列名称** | **数据说明** |
|---------|:---------|
|CustomerTenantId|  客户的租户 ID |
|CustomerTpid|  客户的上层父 ID |
|月份| 报告使用情况的月份|
|Subworkload|    (会议、呼叫、电话系统报告其使用情况的子工作负荷) |
|会议计数| 会议数量|
|会议持续时间|  总会议持续时间（小时）|

**团队-每月使用情况详细信息**：各种字段的数据定义如下：

| **列名称** | **数据说明** |
|---------|:---------|
|CustomerTenantId|  客户的租户 ID |
|CustomerTpid|  客户的上层父 ID |
|月份| 报告使用情况的月份|
|Subworkload|    (会议、呼叫、电话系统报告其使用情况的子工作负荷) |
|桌面用户| 使用桌面上的团队的用户数|
|移动用户|  在移动设备上使用团队的用户数|
|Web 用户| 在 Web 上使用团队的用户数|
|AllUpParticipants| 每月的团队不同用户数|

**团队使用– w apps**：各个字段的数据定义如下：

| **列名称** | **数据说明** |
|---------|:---------|
|CustomerTenantId|  客户的租户 ID| 
|CustomerTpid|  客户的上层父 ID |
|月份| 报告使用情况的月份|
|w 应用名称|   团队应用的名称|
|用户计数|    应用的用户数|


**训练详细信息**： "培训详细信息" 报表的各个字段的数据定义如下：

| **列名称** | **数据说明** |
|---------|:---------|
|TrainingActivityId|    定型标识符 |
|TrainingTitle| 培训的标题 |
|TrainingType|   (认证/考试) 的定型类型|
|IndividualFirstName|   客户的名字| 
|IndividualLastName|    客户的姓氏| 
|电子邮件| 客户的个人电子邮件 ID|
|CorpEmail| 客户的 Office 电子邮件 ID|
|TrainingCompletionDate|    训练的完成日期 |
|月份| 报告数据的月份|
|IcMCP| 指示用户是否为 Microsoft 认证专业人员|
|MCPID| 用户的 MCP ID|
|MPNId| Microsoft 合作伙伴网络 ID |
|PartnerName|   合作伙伴的名称 |
|PartnerCityLocation|   合作伙伴的地理城市位置 |
|PartnerCountryLocation|    合作伙伴的地理国家/地区位置 |

**Microsoft Learn**： Microsoft Learn 报表的各个字段的数据定义为：

| **列名称** | **数据说明** |
|---------|:---------|
|用户名|用户的名称| 
|UserId|用户 GUID |
|TrainingName|定型名称 |
|TrainingType|定型类型 (模块/Learning 路径) |
|产品|学习模块适用的产品|
|角色|适用于定型的角色 |
|CompletionDate|完成培训的日期 |
|MPNId|Microsoft 合作伙伴网络 ID |
|PartnerName|合作伙伴的名称 |
|国家/地区|合作伙伴的地理国家/地区位置 |

**资格汇总和历史记录**： "能力摘要" 和 "历史记录" 报表的各个字段的数据定义如下：

| **列名称** | **数据说明** |
|---------|:---------|
|CompetencyName|能力的名称 |
|CompetencyLevel|资格级别 (金牌/Silver) |
|CompetencyStatus|当前职称状态 (活动/非活动/宽限期) |
|CompetencyStartDate|给定资格的开始日期| 
|CompetencyEndDate|给定职称的结束日期 |

**胜任度性能**：绩效绩效报表各字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|CompetencyName|    能力的名称 |
|CompetencyAttainmentOptionName|    胜任度选项的名称|
|月份| 报告度量值的月份|
|MetricName|    与资格相关的度量值的名称|
|MetricMonthlyContribution| 指标的每月贡献|
|TTMAggregate|  尾随12个月的聚合指标|
|AnniversaryYearAggregate|  当前周年年份的聚合指标|
|GoldThreshold| 满足黄金能力的性能要求|
|SilverThreshold|   满足银色能力的性能要求|

**云上升-M365 电网**：云上升-M365 电网报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|MPN ID|    Microsoft 合作伙伴网络 ID|
|合作伙伴名称|  合作伙伴的名称|
|客户 ID|   客户标识符编号 |
|DUNS 号|   Dun & 为电网评分的客户的 Bradstreet 号码|
|帐户名|  帐户的名称 |
|域|    帐户的域|
|组织规模|  组织大小|
|行业|  行业  |
|垂直|  客户对电网的纵向评分，由 Microsoft 和其他行业标准 (D&B 提供) |
|区域|  位置的地理区域|
|附属公司|    正在为电网评分的客户的子公司|
|销售区域|   正在为电网评分的客户的销售区域|
|城市|  地理城市位置 |
|州省/自治区/直辖市| 地理位置状态|
|邮政编码|   邮政编码|
|国家/地区|   地理国家/地区 |
|段|   市场段 |
|子段|   市场子段 |
|SMC 类型摘要|  SMC 类型 |
|顶级非托管计算基础|  排名靠前的非托管客户-计算|
|顶级非托管用户基| 排名靠前的非托管客户-用户|
|IsNonProfit|   是不是利润还是利润 (是/否) |
|启用远程工作目标 Exchange Online|   具有活动的 exchange online 订阅、追加到 M365 的客户|
|启用远程本地获取 (当前版本) 与 CLAS 电网-+ 10 许可证|具有当前本地 Office 或 Win 客户端 (的客户（即，在 EOS 产品) 之后的版本）。 客户有10个或更多许可证。 具有电网分数的客户。 合作伙伴应定位到 M365。|
|启用远程本地采集 (当前版本) 与 CLAS 电网-<10 许可证|具有当前本地 Office 或 Win 客户端 (的客户（即，在 EOS 产品) 之后的版本）。 客户的许可证少于10个。 具有电网分数的客户。 合作伙伴应定位到 M365。|
|启用远程本地获取 (当前版本) ，不使用 CLAS 电网-+ 10 个许可证| 具有当前本地 Office 或 Win 客户端 (的客户（即，在 EOS 产品) 之后的版本）。 客户有10个或更多许可证。 客户没有电网分数。 合作伙伴应定位到 M365。|
|启用远程本地采集 (当前版本) ，不使用 CLAS 电网-<10 个许可证| 具有当前本地 Office 或 Win 客户端 (的客户（即，在 EOS 产品) 之后的版本）。 客户的许可证少于10个。 客户没有电网分数。 合作伙伴应定位到 M365。|
|使用 CLAS 电网-+ 10 许可证启用远程本地采集 (EOS) |如果客户的本地办公室或 Win 客户端 (就是，并在该客户之前包含了 EOS 产品。 客户有10个或更多许可证。 客户具有电网分数。 合作伙伴应定位到 M365。|
|启用使用 CLAS 电网的远程本地采集 (EOS) -<10 个许可证|如果客户的本地办公室或 Win 客户端 (就是，并在该客户之前包含了 EOS 产品。 客户的许可证少于10个。 客户具有电网分数。 合作伙伴应定位到 M365。|
|启用远程本地采集 (EOS) ，无需 CLAS 电网-+ 10 个许可证| 具有当前本地 Office 或 Win 客户端 (的客户（即，在和包含 EOS 产品) 之前的版本）。 客户有10个或更多许可证。 客户没有电网分数。 合作伙伴应定位到 M365。|
|启用远程本地采集 (EOS) ，而无需 CLAS 电网-<10 个许可证| 具有当前本地 Office 或 Win 客户端 (的客户（即，在和包含 EOS 产品) 之前的版本）。 客户的许可证少于10个。 客户没有电网分数。 合作伙伴应定位到 M365。|
|启用远程工作-高电网客户端 M365 (立即操作/评估) | M365 的电网的客户。|
|启用远程工作-与 M365 的 (缩放) 的竞争| 具有缩放和 M365 的客户、用于转换到团队的目标|
|启用远程工作- (缩放) 无需 M365|  具有缩放的客户、用于转换到团队的目标|
|降低 M365 E3 目标为 M365 E5 的成本和管理| 具有 M365 E3 的现有客户，M365 E5 目标|
|降低成本，并管理针对 M365 BP 的 M365 BB 和 BS.1770 客户|    现有的 M365 BB 和 BS.1770 客户，以这些客户为目标 M365 的最佳实践|
|转换组织工作效率-Surface 电网|    Customer 正在显示电网的图面。|
|M365Cluster|标识客户要购买 M365 的电网。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|M365Fit|   定义 firmographics 的内部和外部数据点。 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。 按季度更新适合评分。|
|M365Intent|    与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。|
|SurfaceCluster|    这可通过将 "拟合" 和 "意向" 建议合并到群集来识别客户的电网购买面。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|SurfaceFit|    定义 firmographics 的内部和外部数据点。 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。 按季度更新适合评分。|
|SurfaceIntent| 与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。|
|O365Cluster|   这会标识客户电网购买 O365。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|O365Fit|   定义 firmographics 的内部和外部数据点。 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。 按季度更新适合评分。|
|O365Intent|    与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。|
|M365UpsellCustomer|    这会确定客户是否显示 M365 的追加销售电网|
|具有 Google|    此标志确定客户是否显示了所属 Google 产品的竞争信号|
|具有 AWS|   此标志确定客户是否正在显示适用于所属 AWS 产品的竞争信号|
|具有 EA|    这会标识续订是 (EA) 或 EA 订阅的企业协议|
|已打开|  这会标识续订是开放还是开盘值协议|

**云上升-D365 电网**：云上升-D365 电网报表的各个字段的数据定义：

| **列名称** | **数据说明** |
|---------|:---------|
|MPN ID|    Microsoft 合作伙伴网络 ID|
|合作伙伴名称|  合作伙伴的名称|
|客户 ID|   客户标识符编号 |
|DUNS 号|   Dun & 为电网评分的客户的 Bradstreet 号码|
|帐户名|  帐户的名称 |
|域|    帐户的域|
|组织规模|  组织大小|
|行业|  行业  |
|垂直|  客户对电网的纵向评分，由 Microsoft 和其他行业标准 (D&B 提供) 
|区域|  位置的地理区域|
|附属公司|    正在为电网评分的客户的子公司|
|销售区域|   销售区域|
|城市|  地理城市位置 |
|州省/自治区/直辖市| 地理位置状态|
|邮政编码|   邮政编码|
|国家/地区|   地理国家/地区 |
|段|   市场段 |
|子段|   市场子段 |
|SMC 类型摘要|  客户的分类：排名靠前的非托管用户群的客户是具有300多位员工的客户，顶级非托管计算基础是在 Azure 3 年中具有 $ 10k 的客户，中型企业是拥有25名员工或更高版本的客户|
|顶级非托管计算基础   |排名靠前的非托管客户-计算|
|顶级非托管用户基| 排名靠前的非托管客户-用户|
|IsNonProfit|   是不是利润还是利润 (是/否) |
|激活 M365-座位大小 >= 25 座位 (SalesPro 电网型号) |   无 D365 的客户。 座位大小： 25 +。 合作伙伴应瞄准 D365 Salespro 的交叉销售|
|激活数字销售-D365 SalesPro 电网 (立即操作/评估)  |高电网客户，无需 D365。  合作伙伴应面向 D365 SalesPro。|
|& 欺诈 Navision (BC 电网模型管理金融风险) |具有 OnPrem Navision 的现有客户。  合作伙伴应面向 D365 BC|
|& 欺诈 (F&O 电网模型，管理金融风险)     |具有 OnPrem AX 的现有客户。  伙伴应面向 D365 F&O|
|& 欺诈 Plains (BC 电网模型来管理金融风险) |  具有 OnPrem 优秀 Plains 的现有客户。  合作伙伴应面向 D365 BC|
|& 欺诈 (BC 电网模型，从而管理金融风险) |具有 OnPrem 所罗门群岛的现有客户。  合作伙伴应面向 D365 BC|
|管理财务风险 & 欺诈本地安装基础-其他 (BC 电网型号)  |具有上面未列出的其他 OnPrem 解决方案的现有客户。  合作伙伴应面向 D365 BC|
|构建 Agile Business 流程-Dynamics 本地 Install D365 电网 Model/NAV/其他 (Model) |   构建 Agile Business 流程-Dynamics 本地 Install D365 电网 Model/NAV/其他 (Model) |
|构建 Agile 业务流程-动态竞争 Mendix/Outsystems/Salesforce (D365 电网模型) | 构建 Agile 业务流程-动态竞争 Mendix/Outsystems/Salesforce (D365 电网模型) |
|构建 Agile 业务流程-D365 F&O 安装基础 |现有的 D365 F&O 个客户。  面向电源应用的合作伙伴。|
|构建 Agile 业务流程-D365 BC 安装基础| 现有的 D365 BC 客户。 面向电源应用的合作伙伴。|
|构建 Agile 业务流程-D365 CE 安装基础| 现有的 D365 CE 客户。 面向电源应用的合作伙伴。|
|构建复原供应链-Win，并将第一个 D365 工作负荷作为与非 Oracle/SAP ERP 客户的 D365 供应链一起激活|  面向 D365 供应链的客户。|
|构建复原供应链-跨向现有 D365 CE 客户销售 D365 供应链和/或零售/商务 |面向交叉销售 D365 供应链的现有 D365 CE 客户|
|构建复原供应链-交叉销售 D365 Sup。 将零售/商业链接到 D365 CE 并 (Oracle 或 SAP) | 具有 Oracle 或 SAP 的现有 D365 CE 客户面向 D365 供应链的目标|
|D365BCCluster| 这会标识客户电网购买 D365 Business Central。  显示电网的客户将处于中等和小类别。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|D365BCFit| 定义 firmographics 的内部和外部数据点。 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。 按季度更新适合评分。|
|D365BCIntent|  与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。|
|D365FOCluster| 这会标识客户电网购买 D365 财务和运营。  显示电网 for F&O 的客户将位于顶层非托管类别中。 群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|D365FOFit| 定义 firmographics 的内部和外部数据点。 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。 按季度更新适合评分。|
|D365FOIntent|  与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。|
|D365CECluster| 这会标识客户电网购买 D365 Customer Engagement。  显示电网 for CE 的客户将采用 "中" 和 "小" 类别。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|D365CEFit| 适用于 D365 CE|
|D365CEIntent|  D365 CE 的意向|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  这会确定客户是否有本地 AX 或 CRM 的开放式续订。|
|M365UpsellCustomer|    这会确定客户是否显示 M365 的追加销售电网|
|具有 Google|    此标志确定客户是否显示了所属 Google 产品的竞争信号|
|具有 AWS|   此标志确定客户是否正在显示适用于所属 AWS 产品的竞争信号|
|具有 EA |这会标识续订是 (EA) 或 EA 订阅的企业协议|
|已打开|  这会标识续订是开放还是开盘值协议|

**Cloud Ascent-Azure 电网**： Cloud Ascent-Azure 电网报表的各个字段的数据定义：

|**列名称** |**数据说明** |
|---------|:---------|
|MPN ID|    Microsoft 合作伙伴网络 ID|
|合作伙伴名称|  合作伙伴的名称|
|客户 ID|   客户标识符编号 |
|DUNS 号|   Dun & 为电网评分的客户的 Bradstreet 号码|
|帐户名|  帐户的名称 |
|域|    帐户的域|
|组织规模|  组织大小|
|行业|  行业  |
|垂直|  客户对电网的纵向评分，由 Microsoft 和其他行业标准 (D&B 提供) |
|区域|  位置的地理区域|
|附属公司|    正在为电网评分的客户的子公司|
|销售区域|   销售区域|
|城市|  地理城市位置 |
|州省/自治区/直辖市| 地理位置状态|
|邮政编码|   邮政编码|
|国家/地区|   地理国家/地区 |
|段|   市场段 |
|子段|   市场子段 |
|SMC 类型摘要|  SMC 类型 |
|顶级非托管计算基础|  排名靠前的非托管客户-计算|
|顶级非托管用户基| 排名靠前的非托管客户-用户|
|IsNonProfit|   是不是利润还是利润 (是/否) |
|通过 CLAS 电网-5 + 许可证，迁移-EOS Win Server-EOS Windows Server IB|   具有本地 Win 服务器 (的客户（即早于和包含 EOS 产品) 的版本）。 客户有5个或更多许可证。 具有电网分数的客户。  合作伙伴应以这些客户为目标迁移到 Azure。|
|通过 CLAS 电网-<5 许可证迁移-EOS Win Server-EOS Windows Server IB|   ) 本地 Win 服务器的 Win Server ( (端的客户，该服务是之前的版本，并包含 EOS 产品) 。 客户的许可证数少于5。 具有电网分数的客户。  合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-EOS Win Server-不带 CLAS 电网-5 + 许可证的 EOS Windows Server IB |具有本地 Win 服务器 (的客户（即早于和包含 EOS 产品) 的版本）。 客户拥有超过5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-EOS Win Server-未 CLAS 电网 Windows Server IB-<5 许可证|    具有本地 Win 服务器 (的客户（即早于和包含 EOS 产品) 的版本）。 具有少于5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|通过 CLAS 电网-5 + 许可证迁移-EOS SQL-EOS SQL Server IB|  具有本地的 (SQL Server 的客户（即，在和包含 EOS 产品) 之前的版本）。 客户有5个许可证。 客户具有电网分数。  合作伙伴应以这些客户为目标迁移到 Azure。|
|通过 CLAS <电网在5许可证的情况上迁移-EOS SQL-EOS SQL Server IB|  具有本地的 (SQL Server 的客户（即，在和包含 EOS 产品) 之前的版本）。 具有少于5个许可证。 具有电网分数的客户。 合作伙伴应以这些客户为目标迁移到 Azure。|
|在未 CLAS 电网 + 许可证的情况下，迁移-EOS SQL-EOS SQL Server IB|   具有本地的 (SQL Server 的客户（即，在和包含 EOS 产品) 之前的版本）。 客户有5个或更多许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|在没有 CLAS 电网 <的情况下，将 SQL-EOS SQL Server IB 迁移到5许可证|   具有本地的 (SQL Server 的客户（即，在和包含 EOS 产品) 之前的版本）。 客户拥有少于5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移本地 Win 服务器-当前 Windows Server IB 与 CLAS 电网 + 许可证|   具有当前本地 Win 服务器 (的客户（即，在 EOS 产品) 之后的版本。 客户有5个许可证。 客户具有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移本地 Win 服务器-当前 Windows Server IB 与 CLAS 电网-<5 许可证|   具有当前本地 Win 服务器 (的客户（即，在 EOS 产品) 之后的版本。 客户拥有少于5个许可证。 客户具有适用于 Azure 的电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移本地 Win 服务器-当前 Windows Server IB，无需 CLAS 电网 + 许可证|    具有当前本地 Win 服务器 (的客户（即，在 EOS 产品) 之后的版本。 客户有5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移本地 Win Server-当前 Windows Server IB，无需 CLAS 电网-<5 许可证 |具有当前本地 Win 服务器 (的客户（即，在 EOS 产品) 之后的版本。 客户拥有少于5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移到 Azure SQL 或 SQL Vm-当前 SQL Server IB 与 CLAS 电网 + 许可证|  具有当前本地 SQL Server 的客户 (即，) 的 EOS 产品后的版本。 客户有5个许可证。 客户具有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移到 Azure SQL 或 SQL Vm-当前 SQL Server IB 与 CLAS 电网-<5 许可证|  具有当前本地 SQL Server 的客户 (即，) 的 EOS 产品后的版本。 客户拥有少于5个许可证。 客户具有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移到 Azure SQL 或 SQL Vm-当前 SQL Server IB，无需 CLAS 电网 + 许可证|   具有当前本地 SQL Server 的客户 (即，) 的 EOS 产品后的版本。 客户有5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-迁移到 Azure SQL 或 SQL Vm-当前 SQL Server IB，无需 CLAS 电网-<5 许可证|   具有当前本地 SQL Server 的客户 (即，) 的 EOS 产品后的版本。 客户拥有少于5个许可证。 客户没有电网分数。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-OSS-迁移到 OSS DB| 具有以下任何竞争产品的现有客户： PostgreSQL、MySQL、MariaDB。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-OSS-Azure 上的 Linux |产品： Linux 的现有客户。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-SAP-Azure 上的 SAP|  产品： SAP 的现有客户。 合作伙伴应以这些客户为目标迁移到 Azure。|
|WVD-RDS IB |标识具有活动 Windows 远程桌面服务的客户。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-WVD-将新式工作交叉销售到 Azure/WVD|   标识具有 M365 的客户，但没有 Azure。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-VMware IB|   产品： VMware 的现有客户。 合作伙伴应以这些客户为目标迁移到 Azure。|
|迁移-Citrix IB|   产品： Citrix 系统的现有客户。 合作伙伴应以这些客户为目标迁移到 Azure。|
|创新-分析-Power BI IB （高 Azure 电网）|   具有和 Active Power BI 订阅的客户，包括： Power BI 独立 Pro、Power BI Azure 套件、Power BI-Office 套件、Power BI 套件-M365|
|使用 GitHub-VisualStudio/MSDN IB 启用-DevOps|    已识别具有活动 visual studio 的客户|
|Win Server Standard 版本|   这会显示客户的 Windows Server Standard 购买版本|
|Win Server Standard 许可证|   这会显示客户的 Windows Server 标准购买许可证类型|
|Win Server Data Center 版本|    这会显示客户的 Windows 数据中心购买版本|
|Win Server 数据中心许可证| 这会显示客户的 Windows 数据中心购买许可证类型|
|AzureFit|  定义 firmographics 的内部和外部数据点。 适应评分使用类似的模型来比较客户，并查看其是否适合 Microsoft 云产品。 按季度更新适合评分。|
|AzureIntent|   与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。|
|AzureCluster|  这可通过将 "调整和意向" 建议合并到群集来确定客户电网购买 Azure。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|WindowsServerDataCenter_HasOpenRenewal|    这会确定客户是否已打开 windows server 数据中心的续订|
|WindowsServerStandard_HasOpenRenewal|  这会确定客户是否有适用于 windows server standard 的开放式续订|
|AzureUpsellCustomer|   这会确定客户是否显示 Azure 的追加销售电网|
|具有 Google|    此标志确定客户是否显示了所属 Google 产品的竞争信号|
|具有 AWS|   此标志确定客户是否正在显示适用于所属 AWS 产品的竞争信号|
|具有 EA |这会标识续订是 (EA) 或 EA 订阅的企业协议|
|已打开|  这会标识续订是开放还是开盘值协议|

**Cloud Ascent-Agreement 续订电网**： Cloud 升高协议续订电网报告的各个字段的数据定义：

|**列名称** |**数据说明** |
|---------|:---------|
|MPN ID|    Microsoft 合作伙伴网络 ID|
|合作伙伴名称|  合作伙伴的名称|
|客户 ID|   客户标识符编号 |
|DUNS 号|   Dun & 为电网评分的客户的 Bradstreet 号码|
|帐户名|  帐户的名称 |
|域|    帐户的域|
|组织规模|  组织大小|
|行业|  行业  |
|垂直|  客户对电网的纵向评分，由 Microsoft 和其他行业标准 (D&B 提供) |
|区域|  位置的地理区域|
|附属公司|    正在为电网评分的客户的子公司|
|销售区域|   销售区域|
|城市|  地理城市位置 |
|州省/自治区/直辖市| 地理位置状态|
|邮政编码|   邮政编码|
|国家/地区|   地理国家/地区 |
|段|   市场段 |
|子段|   市场子段 |
|SMC 类型摘要|  SMC 类型 |
|顶级非托管计算基础|  排名靠前的非托管客户-计算|
|顶级非托管用户基| 排名靠前的非托管客户-用户|
|IsNonProfit|是不是利润还是利润 (是/否) |
|具有 Google|此标志确定客户是否正在显示适用于所属 AWS 产品的竞争信号|
|具有 AWS|此标志确定客户是否正在显示适用于所属 AWS 产品的竞争信号|
|Azure 群集|这会标识客户电网购买 Azure。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|D365 F&O 群集|  这会标识客户电网购买 D365 财务和运营。  显示电网 for F&O 的客户将位于顶层非托管类别中。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|D365 CE 群集|   这会标识客户电网购买 D365 Customer Engagement。  显示电网 for CE 的客户将采用 "中" 和 "小" 类别。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|D365 BC 群集|   这会标识客户电网购买 D365 Business Central。  显示电网的客户将处于中等和小类别。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|M365 群集|  这会标识客户电网购买 M365。  群集立即行动和评估应面向，因为它们将产生更高的收益。  仅当目标为 "立即操作" 并评估客户后，才应将维护和培训客户设定为目标。|
|许可计划|   这会标识续订的许可证计划类型|
|协议 ID|  协议标识符|
|协议结束日期|    协议结束日期 |
|有效期限类型|   过期类型|
|过期收入|  与过期订阅关联的收入|
|具有 EA|    这会标识续订是 (EA) 或 EA 订阅的企业协议|
|已打开|  这会标识续订是开放还是开盘值协议|
|Azure 追加客户| 这会确定客户是否显示 Azure 的追加销售电网|
|M365 追加销售客户|  这会确定客户是否显示 M365 的追加销售电网|
|RevSumDivisionName|    这会标识用于续订的产品|

## <a name="next-steps"></a>后续步骤

对于报表，请参阅 [下载报表](pci-download-reports.md)。
