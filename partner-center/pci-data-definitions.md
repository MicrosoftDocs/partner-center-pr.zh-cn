---
title: 见解数据定义
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 该文档列出了各种报表及其数据定义，您可以从 "Insights 下载报表" 页下载这些报表和数据定义。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 721caed2d8b0e24940e7adedeb90cc689a82d2e7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152828"
---
# <a name="export--data-definitions"></a>导出–数据定义 

**适当的角色**：报表查看器 |Executive 报表查看器

## <a name="introduction"></a>简介 

通过使用 Insights 仪表板上的 "下载报表" 中心，你可以导出原始数据集。 

下表列出了可与数据定义一起下载的各种报表： 

### <a name="partner-profile-report"></a>**合作伙伴配置文件报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| MPNId | Microsoft 合作伙伴网络的标识符 (MPN)  | 
| PartnerName | 合作伙伴的名称 | 
| PGA_MPNId | 合作伙伴全局帐户 MPN 的标识符 | 
| PGA_PartnerName | 合作伙伴全局帐户名称 | 
| 城市 | 合作伙伴的城市位置 | 
| 国家/地区 | 合作伙伴的国家/地区位置 | 
| HierarchyLevel | 指示是全局 MPN ID 还是位置 MPN ID | 

### <a name="customer-details-report"></a>**客户详细信息报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerTenantId | 客户租户的标识符 | 
| CustomerTpid | 客户最顶层父级的标识符 | 
| CustomerSegment | 客户细分 | 
| CustomerMarket | 客户的地理市场 | 
| CustomerStatus | 客户状态 (活动或非活动)  | 
| 产品 | MPN 销售给客户的产品：O365、DYNAMICS 365、企业移动性 + 安全性、Power BI 或 Microsoft Azure | 
| SKU | 产品 SKU | 
| 月份 | 报告使用情况和收入月份 | 
| MPNId | 标识符Microsoft 合作伙伴网络 | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理位置 | 
| PartnerAttributionType | 合作伙伴的归属类型 | 
| SalesChannel | 销售渠道 | 
| AvailableSeats | 可用席位 | 
| RevenueUSD | 美元收入 | 

### <a name="reseller-performance-report"></a>**分销商性能报告**

> [!Note]
> 收入和 ACR 数据仅适用于作为 Executive 报表查看者的用户。

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| ResellerMPNid | 经销商 Microsoft 合作伙伴网络标识符 | 
| ResellerName | 经销商名称 | 
| ResellerMarket | 市场分销商国家/地区 | 
| IndirectProviderMPNId | 间接提供程序的标识符 Microsoft 合作伙伴网络 | 
| IndirectProviderName | 间接提供程序名称 | 
| 月份 | 报告使用情况和收入的月份 | 
| 产品 | 产品名称 | 
| 订阅 ID | 订阅的标识符 | 
| AvailableSeats | 可用座位数 | 
| AssignedSeats | 已分配的座位数 | 
| BilledRevenueUSD | 美元计费收入 | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerTPid | 客户最顶层父级的标识符 | 
| CustomerSegment | 客户细分 | 
| CustomerMarket | 客户的地理市场 | 
| ResellerStatus | 经销商状态 | 

### <a name="subscription-details-report"></a>**订阅详细信息报表**

>[!Note]
>只有作为主管报表查看者的用户才能使用收入数据和 ACR 数据。

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| SubscriptionId | 订阅的 GUID | 
| SubscriptionStartDate | 订阅的开始日期 | 
| SubscriptionEndDate | 订阅的结束日期 | 
| SubscriptionState | 活动或流失 (订阅的状态)  | 
| 月份 | 报告使用情况和收入月份 | 
| IsAutoRenew | 指示订阅是自动续订 (是还是否)  | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerTenantId | 客户的 GUID | 
| CustomerTpid | 客户最顶层的父标识符 | 
| CustomerSegment | 客户市场领域 | 
| CustomerMarket | 客户的地理市场 | 
| 产品 | 合作伙伴向客户销售的产品 | 
| SKU | 产品 SKU | 
| MPNId | 合作伙伴 Microsoft 合作伙伴网络 ID | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理位置 | 
| PartnerAttributionType | 订阅的特性类型 | 
| SalesChannel | 销售直接、CSP (云解决方案提供商) 等的渠道 | 
| AvailableSeats | 当前可用座位 | 
| RevenueUSD | 美元收入 | 
| 注册 ID | 订阅的注册 ID | 

### <a name="azure-usage-report"></a>**Azure 使用情况报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| SubscriptionId | 订阅的 GUID | 
| SubscriptionStartDate | 订阅开始日期 | 
| SubscriptionEndDate | 订阅结束日期 | 
| SubscriptionState | 订阅的当前状态 (打开、关闭、活动或宽限期)  | 
| 月份 | 按月聚合的日期 | 
| ServiceName | Azure 服务的名称 | 
| MeterCategory | 计量类别的名称 | 
| UsageUnits | 计费周期中使用的单位数 | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerTenantId | 客户的租户 ID | 
| CustomerTpid | 客户排名前父级 ID | 
| CustomerSegment | 客户细分 | 
| CustomerMarket | 客户的地理市场 | 
| MPNId | Microsoft 合作伙伴网络 ID | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理国家/地区位置 | 
| PartnerAttributionType | 合作伙伴的特性类型 | 
| SalesChannel | 销售渠道 (直接/CSP、间接/CSP、直接等)  | 
| ACR_USD | Azure 使用了年收入 (ACR) 美元 | 
| 注册 ID | Azure 订阅的注册 ID | 

### <a name="office-365-license-usage-report"></a>**Office 365 许可证使用情况报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客户的租户 ID | 
| CustomerTpid | 客户的上层父 ID | 
| WorkloadName | Skype for Business、团队、Exchange Online | 
| 月份 | 报告使用情况的月份 | 
| PaidAvailableUnits | 付费可用单位数 | 
| MonthlyActiveUsers | 每月活动用户数 | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerMarket | 客户市场的国家/地区位置 | 
| CustomerSegment | 客户细分 | 
| MPNId | 标识符Microsoft 合作伙伴网络 | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理位置 | 
| PartnerAttributionType | 合作伙伴的归属类型 | 

### <a name="enterprise-mobility-license-usage-report"></a>**企业移动性许可证使用情况报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客户的租户 ID | 
| CustomerTpid | 客户排名前父级 ID | 
| WorkloadName | EMS 企业移动性 + 安全性 (工作负荷) 的名称 | 
| 月份 | 报告使用情况的月份 | 
| PaidAvailableUnits | 付费可用单位数 | 
| MonthlyActiveUsers | 每月活动用户数 | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerMarket | 客户市场的地理国家/地区位置 | 
| CustomerSegment | Customer 段 | 
| MPNId | Microsoft 合作伙伴网络的标识符 | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理位置 | 
| PartnerAttributionType | 合作伙伴的特性类型 | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 许可证使用情况报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| SubscriptionId | 订阅的 GUID | 
| SubscriptionStartDate | 订阅的开始日期 | 
| SubscriptionEndDate | 订阅的结束日期 | 
| SubscriptionStatus | 订阅状态 | 
| 月份 | 报告使用情况的月份 | 
| RevSumDivisionName | Rev sum 相除的名称 | 
| RevSumCategoryName | 修订总和类别的名称 | 
| SKU | 产品的 SKU | 
| SKUId | 产品的 SKU ID | 
| FreeVsPaidSKU | 指示它是免费 SKU 还是付费 SKU | 
| SalesModel | 用于销售订阅的销售渠道 | 
| DetailedSalesModel | 订阅的详细销售模型 | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerTenantId | 客户租户的 GUID | 
| CustomerTpid | 客户最顶层的父标识符 | 
| CustomerSegment | 客户的细分市场 | 
| CustomerMarket | 客户的地理市场 | 
| MPNId | 标识符Microsoft 合作伙伴网络 | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理国家/地区位置 | 
| PartnerAttachType | 订阅的特性类型 | 
| AvailableSeats | 当前可用座位 | 
| AssignedSeats | 当前分配的座位 | 
| ActiveSeats | 当前活动座位数 | 
| DeploymentOpportunity | 当前部署机会 | 
| ActiveUsagePercent | 当前活动使用百分比 | 

### <a name="power-bi-license-usage-report"></a>**Power BI 许可证使用情况报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| SubscriptionId | 订阅的 GUID | 
| SubscriptionStartDate | 订阅的开始日期 | 
| SubscriptionEndDate | 订阅的结束日期 | 
| SubscriptionStatus | 订阅状态 ("活动"、"非活动" 或 "宽限期")  | 
| 月份 | 按月聚合的日期 | 
| SKU | 产品的 SKU | 
| SKUId | 产品的 SKU ID | 
| FreeVsPaidSKU | 免费或付费 SKU 差异 | 
| SalesModel | 用于销售订阅的销售模型 | 
| DetailedSalesModel | 订阅的详细销售模型 | 
| CustomerName | 购买订阅的客户的名称 | 
| CustomerTenantId | 客户租户的 GUID | 
| CustomerTpid | 客户最顶层父级的标识符 | 
| CustomerSegment | 客户的细分市场 | 
| CustomerMarket | 客户的地理市场 | 
| MPNId | 标识符Microsoft 合作伙伴网络 | 
| PartnerName | 合作伙伴的名称 | 
| PartnerLocation | 合作伙伴的地理国家/地区位置 | 
| PartnerAttachType | 订阅的特性类型 | 
| AvailableSeats | 当前可用座位 | 
| AssignedSeats | 当前分配的座位 | 
| ActiveSeats | 当前活动座位数 | 
| DeploymentOpportunity | 当前部署机会 | 
| ActiveUsagePercent | 当前活动使用百分比 | 

### <a name="teams-meetings-and-calls-report"></a>**团队会议和呼叫报告**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客户的租户 ID | 
| CustomerTpid | 客户的顶级父级的标识符 | 
| 月份 | 报告使用情况的月份 | 
| Subworkload | 在会议、电话或电话系统 (报告使用情况的子)  | 
| 会议计数 | 会议次数 | 
| 会议持续时间 | 总会议持续时间（以小时表示） | 

### <a name="teams-monthly-usage-report"></a>**Teams 每月使用情况报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客户的租户 ID | 
| CustomerTpid | 客户最顶层父级的标识符 | 
| 月份 | 报告使用情况的月份 | 
| 子工作加载 | 在会议、电话或电话系统 (报告使用情况的子)  | 
| 桌面用户 | 在桌面上使用 Teams 的用户数 | 
| 移动用户 | 在移动设备上使用 Teams 的用户数 | 
| Web 用户 | 在 Web 上使用 Teams 的用户数 | 
| AllUpParticipants | 当月 Teams 的唯一用户数 | 

### <a name="teams-usage-3p-apps-report"></a>**Teams 使用情况 3P 应用报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客户的租户 ID | 
| CustomerTpid | 客户的上层父 ID | 
| 月份 | 报告使用情况的月份 | 
| w 应用名称 | 团队应用的名称 | 
| 用户计数 | 应用的用户数 | 


### <a name="training-details-report"></a>**训练详细信息报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| TrainingActivityId | 定型标识符 | 
| TrainingTitle | 培训的标题 | 
| TrainingType |  (认证或考试) 的定型类型 | 
| IndividualFirstName | 客户的名字 | 
| IndividualLastName | 客户的姓氏 | 
| 电子邮件 | 客户的个人电子邮件 ID | 
| CorpEmail | 客户的 Office 电子邮件 ID | 
| TrainingCompletionDate | 训练的完成日期 | 
| 月份 | 报告数据的月份 | 
| IcMCP | 指示用户是否是 Microsoft 认证专家 (MCP)  | 
| MCPID | 用户的 MCP ID | 
| MPNId | 标识符Microsoft 合作伙伴网络 | 
| PartnerName | 合作伙伴的名称 | 
| PartnerCityLocation | 合作伙伴的地理位置 | 
| PartnerCountryLocation | 合作伙伴的地理位置 | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| UserName | 用户的名称 | 
| UserId | 用户的 GUID | 
| TrainingName | 训练的名称 | 
| TrainingType | 定型类型 (模块或学习路径)  | 
| 产品 | 学习模块适用的产品 | 
| 角色 | 适用于定型的角色 | 
| CompletionDate | 完成培训的日期 | 
| MPNId | Microsoft 合作伙伴网络的标识符 | 
| PartnerName | 合作伙伴的名称 | 
| 国家/地区 | 合作伙伴的地理国家/地区位置 | 

### <a name="competency-summary-and-history-report"></a>**资格汇总和历史记录报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CompetencyName | 能力的名称 | 
| CompetencyLevel | 资格级别 (金牌或银)  | 
| CompetencyStatus | 工作能力的当前状态 (活动、非活动或处于宽限期)  | 
| CompetencyStartDate | 胜任度的开始日期 | 
| CompetencyEndDate | 资格结束日期 | 

### <a name="competency-performance-report"></a>**能力绩效报告**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| CompetencyName | 能力的名称 | 
| CompetencyAttainmentOptionName | 资格认证选项的名称 | 
| 月份 | 报告指标的月份 | 
| MetricName | 与资格相关的指标的名称 | 
| MetricMonthlyContribution | 指标的每月贡献 | 
| TTMAggregate | 尾随 12 个月的聚合指标 | 
| AnniversaryYearAggregate | 当前周年年份的聚合指标 | 
| GoldThreshold | 满足黄金资格的性能要求 | 
| SilverThreshold | 满足银牌资格的性能要求 | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**云提升 - Microsoft 365性报告**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 合作伙伴网络 ID | 
| 合作伙伴名称 | 合作伙伴的名称 | 
| 客户 ID | 客户的标识符编号 | 
| DUNS 号 | Dun & Bradstreet (D&B) 为电网评分的客户的编号 | 
| 帐户名 | 帐户的名称 | 
| Domain | 帐户的域 | 
| 组织规模 | 组织规模 | 
| 行业 | 组织所属的行业 | 
| 垂直 | 按 Microsoft、D&B 和其他行业标准确定的电网评分的客户 | 
| 区域 | 位置的地理区域 | 
| 附属公司 | 正在为电网评分的客户的子公司 | 
| 销售区域 | 正在为电网评分的客户的销售区域 | 
| 城市 | 组织的地理城市位置 | 
| 状态 | 组织的地理位置状态 | 
| 邮政编码 | 组织的邮政编码 | 
| 国家/地区 | 组织的地理国家/地区位置 | 
| Segment | 市场段 | 
| 子段 | 市场子细分市场 | 
| SMC 类型摘要 | SMC 类型 | 
| 顶级非托管 - 计算基础 | 排名前非托管客户 - 计算 | 
| 排名前非托管 - 用户群 | 排名前非托管客户 - 用户 | 
| IsNonProfit | 指示组织是非利润组织 (是还是否)  | 
| 启用远程工作 - 目标 Exchange Online | 具有有效的 Exchange Online 订阅的客户，可向上Microsoft 365 | 
| 启用远程工作 - 使用云 (10 个许可证) 当前版本的本地获取 | 具有当前本地 Office 或 Windows 客户端的客户。 也就是说，客户端版本比 EOL (生命周期) 结束。 客户有 10 个或多个许可证。 具有属性分数的客户。 合作伙伴应目标为转换为Microsoft 365。 | 
| 使用 Cloud Ascent (启用远程工作 - (当前) 版本 - <10 个许可证 | 具有当前本地 Office 或 Windows 客户端 (，即版本高于 EOL) 。 客户许可证少于 10 个。 具有属性分数的客户。 合作伙伴应目标为转换为Microsoft 365。 | 
| 启用 (当前版本) 的远程工作本地获取，不使用云上升电网-+ 10 许可证 | 如果客户使用的是当前的本地 Office 或 Windows 客户端 (即，晚于 EOL) 的版本。 客户有10个或更多许可证。 客户没有电网分数。 合作伙伴应定位到 Microsoft 365。 | 
| 启用 (当前版本) 的远程工作本地获取，不使用云上升电网-<10 个许可证 | 如果客户使用的是当前的本地 Office 或 Windows 客户端 (即，晚于 EOL) 的版本。 客户的许可证少于10个。 客户没有电网分数。 合作伙伴应定位到 Microsoft 365。 | 
| 启用 (EOL 版本) 的远程工作本地获取与云提升电网-+ 10 许可证 | 拥有 EOL 本地办公室或 Windows 客户端 (的客户，即 EOL 版本或早期) 。 客户有10个或更多许可证。 客户具有电网分数。 合作伙伴应定位到 Microsoft 365。 | 
| 启用 (EOL 版本) 的远程工作本地购置，并使用云上升电网-<10 个许可证 | 拥有 EOL 本地办公室或 Windows 客户端 (的客户，即 EOL 版本或早期) 。 客户的许可证少于10个。 客户具有电网分数。 合作伙伴应定位到 Microsoft 365。 | 
| 启用远程工作 - 无需 Cloud Ascent (EOL) 本地获取 - +10 个许可证 | 具有当前本地 Office 或 Windows 客户端 (EOL 版本或更早版本) 。 客户有 10 个或多个许可证。 客户没有属性分数。 合作伙伴应目标为转换为Microsoft 365。 | 
| 启用远程工作 - 无需 Cloud Ascent (EOL) 本地获取 - <10 个许可证 | 具有当前本地 Office 或 Windows 客户端 (EOL 版本或更早版本) 。 客户许可证少于 10 个。 客户没有属性分数。 合作伙伴应目标为转换为Microsoft 365。 | 
| 启用远程工作 - 针对 Microsoft 365 (Act NowithEvaluate)  | 目标客户具有较高的目标Microsoft 365 | 
| 启用远程工作 - (Zoom) Microsoft 365 | 具有 Zoom 和 Microsoft 365 的客户，用于转换为 Teams 的目标 | 
| 启用远程工作 - 在不 (的情况下) Zoom Microsoft 365 | 具有 Zoom 的客户，用于转换为 Teams 的目标 | 
| 降低成本和管理 - Microsoft 365 E3 面向 Microsoft 365 E5 | 使用 E3 Microsoft 365客户，目标为 Microsoft 365 E5 | 
| 降低成本和管理 - Microsoft 365业务高级版的目标业务Microsoft 365业务标准版客户 | 现有 Microsoft 365 Business Basic 和业务标准版客户，面向 Microsoft 365 Business Premium | 
| 转换组织工作效率-Surface 电网 | Customer 显示电网 | 
| M365Cluster | 标识客户电网购买 Microsoft 365。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当 "立即行动" 和 "评估客户" 为目标时仍有容量时，才面向维护并为客户提供培训。 | 
| M365Fit | 定义 firmographics 的内部和外部数据点。 适应评分使用 lookalike 的模型， () 中小型企业中小型企业来比较客户，并查看其是否适用于 Microsoft 云产品。 按季度更新适合评分。 | 
| M365Intent | 与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。 | 
| SurfaceCluster | 通过将 "拟合" 和 "意向" 建议合并到群集中，确定客户的电网购买面。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当 "立即行动" 和 "评估客户" 为目标时仍有容量时，才面向维护并为客户提供培训。 | 
| SurfaceFit | 定义 firmographics 的内部和外部数据点。 拟合评分使用我们最佳 SMB 的类似模型来比较客户，并查看它们是否适合 Microsoft 云产品。 拟合评分每季度更新一次。 | 
| SurfaceIntent | 与社交媒体和客户在线行为相关的信号定义了意向。 意向评分叠加在"拟合"上以定义群集。 意向评分每月更新一次。 | 
| O365Cluster | 标识客户购买 Office 365 的念性。 目标"立即行动"和"评估群集"，因为它们将产生更高的收益。 只有在"立即行动"和"评估客户"之后仍有容量时，才面向目标"教育"和"培训客户"。 | 
| O365Fit | 用于定义公司图的内部和外部数据点。 拟合评分使用我们最佳 SMB 的类似模型来比较客户，并查看它们是否适合 Microsoft 云产品。 拟合评分每季度更新一次。 | 
| O365Intent | 与社交媒体和客户在线行为相关的信号定义了意向。 意向评分叠加在"拟合"上以定义群集。 意向评分每月更新一次。 | 
| M365UpsellCustomer | 标识客户是否显示客户对Microsoft 365 | 
| 具有 Google | 确定客户是否显示拥有的 Google 产品的竞争信号 | 
| 具有 AWS | 确定客户是否显示适用于拥有 Amazon Web Services (AWS) 产品的竞争信号 | 
| 具有 EA | 标识续订是 (EA) 还是 EA 订阅的企业协议 | 
| 已打开 | 标识续订是开放还是开盘值协议 | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**云上升-Dynamics 365 电网报告**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 合作伙伴网络 ID | 
| 合作伙伴名称 | 合作伙伴的名称 | 
| 客户 ID | 客户标识符编号 | 
| DUNS 号 | Dun & 为电网评分的客户的 Bradstreet 号码 | 
| 帐户名 | 帐户的名称 | 
| Domain | 帐户的域 | 
| 组织规模 | 组织规模 | 
| 行业 | 组织所属的行业 | 
| 垂直 | 按 Microsoft、D&B 和其他行业标准确定的电网评分的客户
| 区域 | 位置的地理区域 | 
| 附属公司 | 因属性而评分的客户子公司 | 
| 销售区域 | 因属性而评分的客户的销售区域 | 
| 城市 | 地理位置 | 
| 状态 | 地理位置 | 
| 邮政编码 | 组织的邮政编码 | 
| 国家/地区 | 地理位置 | 
| Segment | 市场细分 | 
| 子段 | 市场子类别 | 
| SMC 类型摘要 | 客户的分类：排名前非托管的用户库是拥有 300 多名员工的客户，排名前非托管的计算库是 Azure 三年可能拥有 10，000 美元的客户，中型企业是员工数超过 25 的客户，小型企业是员工少于 25 人的客户。 | 
| 顶级非托管 - 计算基础 | 排名前非托管客户 - 计算 | 
| 排名前非托管 - 用户群 | 排名前非托管客户 - 用户 | 
| IsNonProfit | 指示组织是非利润组织 (是还是否)  | 
| 激活数字销售 - Microsoft 365 - 席位大小 >= 25 (SalesProensity 模型)  | 没有 Dynamics 365 的客户。 席位大小：25+。 合作伙伴应瞄准 Dynamics 365 SalesPro 的交叉销售目标。 | 
| 激活数字销售-Dynamics 365 SalesPro 电网 (立即操作或评估)  | 无 Dynamics 365 的电网客户。 合作伙伴应以 Dynamics 365 SalesPro 为目标。 | 
| 管理财务风险 & 欺诈-Dynamics 本地安装 Navision (Business Central 电网模型)  | 具有本地 Navision 的现有客户。 合作伙伴应面向 Dynamics 365 Business Central。 | 
| 管理财务风险 & 欺诈-Dynamics 本地安装基本-Dynamics AX (Dynamics 365 财务 + Operations 电网模型)  | 具有本地 AX 的现有客户。 合作伙伴应面向 Dynamics 365 财务 + 运营。 | 
| 管理财务风险 & 欺诈-Dynamics 本地安装基本-优秀 Plains (Business Central 电网模型)  | 具有本地强大 Plains 的现有客户。 合作伙伴应面向 Dynamics 365 Business Central。 | 
| 管理财务风险 & 欺诈-Dynamics 本地安装基本-所罗门群岛 (Business Central 电网型号)  | 具有本地所罗门群岛的现有客户。 合作伙伴应面向 Dynamics 365 Business Central。 | 
| 管理金融风险 & 欺诈-Dynamics 本地安装基础-其他 (Business Central 电网模型)  | 具有以前未列出的其他本地解决方案的现有客户。 合作伙伴应面向 Dynamics 365 Business Central。 | 
| 构建 Agile 业务流程-动态本地安装基础-AX/GP/SL/NAV/其他 (Dynamics 365 电网模型)  | 生成敏捷业务流程 - Dynamics 本地安装基础 - AX/GP/SL/NAV/其他 (Dynamics 365 属性模型)  | 
| 构建敏捷业务流程 - Dynamics 竞争基础 - Mendix/OutSystems/Salesforce (Dynamics 365 属性模型)  | 构建敏捷业务流程 - Dynamics 竞争基础 - Mendix/OutSystems/Salesforce (Dynamics 365 属性模型)  | 
| 生成敏捷业务流程 - Dynamics 365 Finance + Operations 安装基础 | 现有 Dynamics 365 Finance + Operations 客户。 合作伙伴以Power Apps。 | 
| 生成敏捷业务流程 - Dynamics 365 Business Central 安装基础 | 现有 Dynamics 365 Business Central 客户。 合作伙伴以Power Apps。 | 
| 生成敏捷业务流程 - Dynamics 365 Customer Engagement 安装基础 | 现有 Dynamics 365 Customer Engagement 客户。 合作伙伴以Power Apps。 | 
| 构建可复原供应链 - Windows，并激活第一个 Dynamics 365 工作负荷，作为 Dynamics 365 Supply Chain Management（使用非 Oracle 或 SAP ERP (）) 客户 | Dynamics 365 Supply Chain Management 的目标客户 | 
| 构建可复原供应链 - 将 Dynamics 365 Supply Chain Management 和/或零售或商务产品交叉销售给现有 Dynamics 365 Customer Engagement 客户 | 现有 Dynamics 365 Customer Engagement 客户面向交叉销售 Dynamics 365 Supply Chain Management。 | 
| 构建弹性供应链 - 将 Dynamics 365 Supply Chain Management 和/或零售或商务产品交叉销售到 Dynamics 365 Customer Engagement 和 Oracle 或 SAP | 使用 Oracle 或 SAP 的现有 Dynamics 365 客户参与客户，以面向 Dynamics 365 Supply Chain Management | 
| D365BCCluster | 标识客户购买 Dynamics 365 Business Central 的倾向。 显示电网 for Business Central 的客户将处于中等和小类别。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当目标为 "立即操作" 并评估客户后，才将维护并向客户提供培训。 | 
| D365BCFit | 定义 firmographics 的内部和外部数据点。 适应评分使用 lookalike 模型来比较客户，并查看其是否适用于 Microsoft 云产品。 按季度更新适合评分。 | 
| D365BCIntent | 与社交媒体和客户的联机行为相关的信号定义意向。 意向计分重叠在一起以定义分类。 意向评分每月更新一次。 | 
| D365FOCluster | 确定客户电网购买 Dynamics 365 财务和运营。 显示电网 for 金融 + 操作的客户将位于前几个非托管类别。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当目标为 "立即操作" 并评估客户后，才将维护并向客户提供培训。 | 
| D365FOFit | 定义 firmographics 的内部和外部数据点。 适应评分使用 lookalike 模型来比较客户，并查看其是否适用于 Microsoft 云产品。 按季度更新适合评分。 | 
| D365FOIntent | 与社交媒体和客户在线行为相关的信号定义了意向。 意向评分叠加在"拟合"上以定义群集。 意向评分每月更新一次。 | 
| D365CECluster | 标识客户购买 Dynamics 365 Customer Engagement 的倾向。 显示客户参与倾向的客户将分为"中型"和"小"类别。 目标"立即行动"和"评估群集"，因为它们将产生更高的收益。 只有在面向"立即行动"和"评估客户"后仍有容量时，才面向"目标员工"和"培训客户"。 | 
| D365CEFit | 指示适合 Dynamics 365 客户参与 | 
| D365CEIntent | 指示 Dynamics 365 Customer Engagement 的意向 | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | 标识客户是否对 Dynamics 本地 AX 或 CRM 开放续订 | 
| M365UpsellCustomer | 标识客户是否显示客户对Microsoft 365 | 
| 具有 Google | 确定客户是否显示拥有 Google 产品的竞争信号 | 
| 具有 AWS | 确定客户是否显示适用于拥有 AWS 产品的竞争信号 | 
| 具有 EA | 标识续订是 EA 订阅还是 EA 订阅 | 
| 已打开 | 标识续订是开放还是开盘值协议 | 

### <a name="cloud-ascent---azure-propensity-report"></a>**云上升-Azure 电网报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 合作伙伴网络 ID | 
| 合作伙伴名称 | 合作伙伴的名称 | 
| 客户 ID | 客户标识符编号 | 
| DUNS 号 | Dun & 为电网评分的客户的 Bradstreet 号码 | 
| 帐户名 | 帐户的名称 | 
| Domain | 帐户的域 | 
| 组织规模 | 组织规模 | 
| 行业 | 行业 | 
| 垂直 | 按 Microsoft、D&B 和其他行业标准确定的电网评分的客户 | 
| 区域 | 位置的地理区域 | 
| 附属公司 | 正在为电网评分的客户的子公司 | 
| 销售区域 | 正在为电网评分的客户的销售区域 | 
| 城市 | 地理城市位置 | 
| 状态 | 地理位置状态 | 
| 邮政编码 | 组织的邮政编码 | 
| 国家/地区 | 地理位置 | 
| Segment | 市场细分 | 
| 子段 | 市场子类别 | 
| SMC 类型摘要 | SMC 类型 | 
| 顶级非托管 - 计算基础 | 排名前非托管客户 - 计算 | 
| 排名前非托管 - 用户群 | 排名前非托管客户 - 用户 | 
| IsNonProfit | 指示组织是非利润组织 (是还是否)  | 
| 迁移 - EOL Windows Server - 具有云提升属性的 EOL Windows Server IB - 5+ 许可证 | 具有 EOL 本地 Windows Server (（即 EOL 版本或更早版本）的客户) 。 客户有 5 个或多个许可证。 具有属性分数的客户。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - EOL Windows Server - EOL Windows Server IB 和 Cloud Ascent 属性 - <5 个许可证 | 具有 EOL 本地 Windows Server (（即 EOL 版本或更早版本）的客户) 。 客户的许可证数少于5。 具有电网分数的客户。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-EOL Windows Server-EOL Windows Server IB，无云上升电网-5 + 许可证 | 拥有 EOL 本地 Windows Server (的客户，即 EOL 版本或早期) 。 客户拥有超过5个许可证。 客户没有电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-EOL Windows Server-EOL Windows Server IB，无云上升电网-<5 许可证 | 拥有 EOL 本地 Windows Server (的客户，即 EOL 版本或早期) 。 具有少于5个许可证。 客户没有电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-EOL SQL-EOL SQL Server IB，其中包含 Cloud 升高电网 + 许可证 | 具有 EOL 本地 SQL Server 的客户 (即 EOL 版本或更早的) 。 客户有5个许可证。 客户具有电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-EOL SQL-EOL SQL Server IB 与云上升电网-<5 许可证 | 具有 EOL 本地 SQL Server 的客户 (即 EOL 版本或更早的) 。 许可证少于 5 个。 具有属性分数的客户。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - EOL SQL - EOL SQL Server IB，不含 Cloud Ascent 属性 - 5+ 许可证 | 具有 EOL 本地版本的客户SQL Server (EOL 版本或更早版本) 。 客户有 5 个或多个许可证。 客户没有属性分数。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - EOL SQL - EOL SQL Server IB（不含 Cloud Ascent 属性）- <5 个许可证 | 具有 EOL 本地版本的客户SQL Server (EOL 版本或更早版本) 。 客户许可证少于 5 个。 客户没有属性分数。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - 迁移本地 Windows Server - 具有云提升属性的当前 Windows Server IB - 5+ 许可证 | 具有当前本地 Windows Server (，即版本高于 EOL) 。 客户拥有 5+ 个许可证。 客户有一个属性分数。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - 迁移本地 Windows Server - 具有云提升属性的当前 Windows Server IB - <5 个许可证 | 具有当前本地 Windows Server (，即版本高于 EOL) 。 客户拥有少于5个许可证。 客户具有适用于 Azure 的电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-迁移本地 Windows Server-不带云升高的当前 Windows Server IB 电网 + 许可证 | 具有当前本地 Windows Server (的客户（即，晚于 EOL) 的版本）。 客户有5个许可证。 客户没有电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-迁移本地 Windows Server-不带云升高的当前 Windows Server IB 电网-<5 许可证 | 具有当前本地 Windows Server (的客户（即，晚于 EOL) 的版本）。 客户拥有少于5个许可证。 客户没有电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-迁移到 Azure SQL 或 SQL 虚拟机 (Vm) -当前 SQL Server IB 与云提升电网 + 许可证 | 当前本地 SQL Server 的客户 (即) 晚于 EOL 的版本。 客户有5个许可证。 客户具有电网分数。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-迁移到 Azure SQL 或 SQL Vm-当前 SQL Server IB 与云上升电网-<5 许可证 | 当前本地 SQL Server 的客户 (即) 晚于 EOL 的版本。 客户许可证少于 5 个。 客户有一个属性分数。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - 迁移到 Azure SQL 或 SQL VM - 当前 SQL SERVER IB（不含 Cloud Ascent 属性） - 5+ 个许可证 | 具有当前本地服务（即SQL Server (EOL 版本）的客户) 。 客户拥有 5+ 个许可证。 客户没有属性分数。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - 迁移到 Azure SQL 或 SQL VM - 当前为 IB SQL Server且没有 Cloud Ascent 属性 - <5 个许可证 | 具有当前本地服务（即SQL Server (EOL 版本）的客户) 。 客户许可证少于 5 个。 客户没有属性分数。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - OSS - 迁移到 OSS (DB) 开源 | 具有以下任一竞争产品的现有客户：PostgreSQL、MySQL、MariaDB。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - OSS - Azure 上的 Linux | Linux 的现有客户。 合作伙伴应面向此客户，以迁移到 Azure。 | 
| 迁移 - SAP - Azure 上的 SAP | 具有 SAP 的现有客户。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-Windows 虚拟桌面-远程桌面服务 IB | 标识具有活动 Windows 远程桌面服务的客户。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-Windows 虚拟桌面-交叉销售现代工作到 Azure/WVD | 标识具有 Microsoft 365 且没有 Azure 的客户。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-VMware IB | 产品： VMware 的现有客户。 合作伙伴应面向此客户迁移到 Azure。 | 
| 迁移-Citrix IB | 产品： Citrix 系统的现有客户。 合作伙伴应面向此客户迁移到 Azure。 | 
| 创新-通过高 Azure 电网进行分析-Power BI IB | 具有和 Active Power BI 订阅的客户，包括： Power BI 独立 Pro、Power BI Azure 套件、Power BI-Office 套件、Power BI 套件-Microsoft 365 | 
| 使用 GitHub 实现-DevOps-Visual Studio/MSDN IB | 标识具有活动的 Visual Studio 版本的客户 | 
| Windows Server Standard 版本 | 显示客户的 Windows Server Standard 购买版本 | 
| Windows Server Standard 许可证 | 显示客户购买 Windows Server Standard 的许可证类型 | 
| Windows Server 数据中心版本 | 显示客户购买 Windows 数据中心的版本 | 
| Windows Server 数据中心许可证 | 显示客户购买的 Windows 数据中心的许可证类型 | 
| AzureFit | 用于定义公司图的内部和外部数据点。 拟合评分使用我们最佳 SMB 的类似模型来比较客户，并查看它们是否适合 Microsoft 云产品。 拟合评分每季度更新一次。 | 
| AzureIntent | 与社交媒体和客户在线行为相关的信号定义了意向。 意向评分叠加在"拟合"上以定义群集。 意向评分每月更新一次。 | 
| AzureCluster | 通过将拟合和意向建议合并到群集中，确定客户购买 Azure 的意图。 目标"立即行动"和"评估群集"，因为它们将产生更高的收益。 只有在面向"立即行动"和"评估客户"后仍有容量时，才面向"目标员工"和"培训客户"。 | 
| WindowsServerDataCenter_HasOpenRenewal | 标识客户是否具有 Windows Server Datacenter 的开放续订 | 
| WindowsServerStandard_HasOpenRenewal | 确定客户是否有适用于 Windows Server Standard 的开放式续订 | 
| AzureUpsellCustomer | 确定客户是否显示 Azure 的追加销售电网 | 
| 具有 Google | 确定客户是否显示拥有的 Google 产品的竞争信号 | 
| 具有 AWS | 确定客户是否显示适用于拥有 AWS 产品的竞争信号 | 
| 具有 EA | 标识续订是 EA 订阅还是 EA 订阅 | 
| 已打开 | 标识续订是开放还是开盘值协议 | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**云上升-协议续订电网报表**

| 列名称 | 数据说明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 合作伙伴网络 ID | 
| 合作伙伴名称 | 合作伙伴的名称 | 
| 客户 ID | 客户标识符编号 | 
| DUNS 号 | Dun & 为电网评分的客户的 Bradstreet 号码 | 
| 帐户名 | 帐户的名称 | 
| Domain | 帐户的域 | 
| 组织规模 | 组织规模 | 
| 行业 | 行业 | 
| 垂直 | 按 Microsoft、D&B 和其他行业标准标识的被评分的客户的垂直方向 | 
| 区域 | 位置的地理区域 | 
| 附属公司 | 因属性而评分的客户子公司 | 
| 销售区域 | 因属性而评分的客户的销售区域 | 
| 城市 | 地理位置 | 
| 状态 | 地理位置 | 
| 邮政编码 | 组织的邮政编码 | 
| 国家/地区 | 地理位置 | 
| Segment | 市场细分 | 
| 子段 | 市场子类别 | 
| SMC 类型摘要 | SMC 类型 | 
| 顶级非托管 - 计算基础 | 排名前非托管客户 - 计算 | 
| 排名前非托管 - 用户群 | 排名前非托管客户 - 用户 | 
| IsNonProfit | 指示组织是非利润组织 (是还是否)  | 
| 具有 Google | 确定客户是否显示适用于拥有 AWS 产品的竞争信号 | 
| 具有 AWS | 确定客户是否显示适用于拥有 AWS 产品的竞争信号 | 
| Azure 群集 | 标识客户电网购买 Azure。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当目标为 "立即操作" 并评估客户后，才将维护并向客户提供培训。 | 
| D365 财经 + 运营群集 | 确定客户电网购买 Dynamics 365 财务和运营。 显示电网 for 金融 + 操作的客户将位于前几个非托管类别。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当目标为 "立即操作" 并评估客户后，才将维护并向客户提供培训。 | 
| D365 CE 群集 | 标识客户的电网，以购买 Dynamics 365 客户参与。 显示电网以供客户参与的客户将处于中等和小类别。 目标立即操作并评估群集，因为它们会产生更高的收益。 仅当目标为 "立即操作" 并评估客户后，才将维护并向客户提供培训。 | 
| D365 BC 群集 | 确定客户电网购买 Dynamics 365 Business Central。 显示 Business Central 倾向的客户将位于"中型"和"小型"类别中。 目标"立即行动"和"评估群集"，因为它们将产生更高的收益。 只有在面向"立即行动"和"评估客户"后仍有容量时，才面向"目标员工"和"培训客户"。 | 
| Microsoft 365群集 | 标识客户购买产品Microsoft 365。 目标"立即行动"和"评估群集"，因为它们将产生更高的收益。 只有在面向"立即行动"和"评估客户"后仍有容量时，才面向"目标员工"和"培训客户"。 | 
| 许可证计划 | 标识续订的许可证计划类型 | 
| 协议 ID | 协议的标识符 | 
| 协议结束日期 | 协议的结束日期 | 
| 有效期限类型 | 过期类型 | 
| 即将到期的收入 | 与即将过期的订阅关联的收入 | 
| 具有 EA | 标识续订是 EA 订阅还是 EA 订阅 | 
| 已打开 | 标识续订是开放式还是开放式价值协议 | 
| Azure Upsell 客户 | 标识客户是否显示 Azure 的向上销售属性 | 
| Microsoft 365 追加销售客户 | 标识客户是否显示 Microsoft 365 的追加销售电网 | 
| RevSumDivisionName | 标识用于续订的产品 | 

## <a name="next-steps"></a>后续步骤

有关详细信息，请参阅 [下载报表](pci-download-reports.md)。
