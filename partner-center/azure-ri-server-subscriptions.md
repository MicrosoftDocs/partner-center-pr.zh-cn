---
title: Azure 预订 & 服务器订阅
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解云解决方案提供商的机会，以便为客户获取、预配和管理 Azure 预订和服务器订阅。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 408f0e59bb1d6da7caebdcf323ebcd242c49af97
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943944"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>获取、设置、& 管理客户的 Azure 保留 VM 实例（RI） + 服务器订阅

适用于：

- 合作伙伴中心

**相应的角色**

- 管理员代理
- 全局管理员
- 支持人员代理
- 销售代理
- “用户管理”管理员
 
## <a name="what-are-azure-reservations"></a>什么是 Azure 预留项？

Azure 预订可帮助节省一年或三年的虚拟机、SQL 数据库计算能力、Azure Cosmos DB 吞吐量或其他 Azure 资源，从而节省资金。 通过预付，能够以折扣价购买所用资源。 与即用即付价格相比，预订可显著减少虚拟机、SQL 数据库计算、Azure Cosmos DB 和其他资源成本，最高可达72%。 预订提供计费折扣，并且不会影响资源的运行时状态。 有关详细信息，请参阅[什么是 Azure 保留？](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>客户为何应购买预订？

如果客户有一段时间运行的虚拟机、Azure Cosmos DB 或 SQL 数据库，则购买保留将为他们提供最经济实惠的选项。 例如，如果客户连续运行四个服务实例而没有保留，则按现用现付费率对它们收费。 如果他们购买了这些资源的预留，它们会立即获得预订折扣。 这些资源不再按即用即付费率收费。

### <a name="compelling-new-azure-offer-in-csp"></a>云解决方案提供商计划中引人注目的新 Azure 产品/服务

通过将 Azure 保留和服务器订阅引入其 CSP 计划，Microsoft 可以更好地满足快速增长的客户需求，以支持高度可预测、持久的云工作负荷。 通过 CSP 计划，合作伙伴可以通过 Microsoft 合作伙伴中心和 Azure 门户代表商业客户获取、预配和管理 Azure 预订和服务器订阅。

我们甚至会在 CSP 计划中为合作伙伴提供有关如何购买 Azure 预订的选项。 CSP 合作伙伴可以[代表客户购买 Azure 保留](azure-reservations-buying.md)，也可以允许客户从合作伙伴为其购买的以前的 azure 订阅[购买自己的预订](give-customers-permission.md)。

Azure 预订为客户提供了一系列计算解决方案的灵活性，包括开发和测试、运行应用程序以及扩展数据中心。

例如，使用[Azure 保留 VM 实例](https://azure.microsoft.com/pricing/reserved-vm-instances/)，商业客户现在可以节省高达72% 与即用即付 Azure VM 定价，只需购买或 "预留"-虚拟机一年或三年即可实现。 与即付即用定价相比，具有 Azure 混合权益（软件保障所附带）的 Windows Server 客户最多可以节省 80% 的费用。

由于有说服力的定价和无与伦比的部署灵活性，客户在选择 Azure 预留时将看到最佳的总体价值：

#### <a name="azure-reservations"></a>Azure 预留项

- Azure 保留 VM 实例
- SQL DB 保留
- SQL 托管实例
- Azure Cosmos DB
- Azure SQL 数据仓库
- 应用服务
- Azure Databricks 单位预订
- 托管磁盘
- 块 blob
- MySQL
- Azure 数据资源管理器
- MariaDB
- PostgreSQL

#### <a name="server-subscriptions"></a>服务器订阅

- Windows Server
- 远程桌面服务（RDS） Cal
- SQL Server

#### <a name="linux-isv-annual-subscriptions"></a>Linux ISV 年度订阅

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

#### <a name="isv-annual-subscriptions"></a>ISV 年度订阅

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>入门

若要了解如何将 Azure 保留与客户定位，并尽快启动并运行操作性，我们建议采用以下方法查看准备情况资料：

1. 查看概述演示文稿和相关的网络研讨会，了解客户价值主张和定位
2. 查看并了解《现代商务操作指南》
3. 查看 Azure RI 和服务器订阅常见问题
4. 了解[合作伙伴中心 API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure 预订和服务器订阅更新

## <a name="resources"></a>资源

以下是一个全面的资源列表，用于帮助你快速上手以通过合作伙伴中心执行 Azure 预订事务：

### <a name="sales-readiness"></a>销售准备情况

- [Azure 预订和服务器订阅与 Azure 混合权益概述](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [销售工作表](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [Azure 预订的合作伙伴常见问题解答](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [Azure 预订和 SQL 数据库的合作伙伴常见问题解答](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [远程桌面服务（RDS）客户端访问许可证（CAL）（公告）](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [Azure 保留 VM 实例（Azure 门户）](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [服务器订阅](csp-software-subscriptions.md)
- [Azure 中的 SQL DB 概述](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [SQL DB 保留（Azure 门户）](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [Azure Cosmos DB （Azure 门户）](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [SQL 托管实例（Azure 门户）](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [SUSE 和 Red Hat Enterprise Linux （Azure 门户）](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [Azure 上的 Red Hat Linux](https://azure.com/redhat)
- [Azure 上的 SUSE Linux](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [Azure 上的 Linux](https://azure.microsoft.com/overview/linux-on-azure/)
- [Azure 定价概述](https://azure.microsoft.com/pricing/)
- [Azure 价格计算器](https://azure.microsoft.com/pricing/calculator)
- [Azure Databricks 单位预订](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- CSP 价目表： " **Microsoft Azure 预订实例**" 和 "**软件订阅**价格列表" 均位于 "合作伙伴中心[定价 & 产品/服务](https://partner.microsoft.com/pcv/sales)" 页上。

### <a name="training"></a>培训

注册以查看[商业许可准备情况网络研讨会](https://commercial-licensing.eventbuilder.com/FY2019_ALL)和点播事件。

许可准备情况事件包括以下主题：

- CSP 在线服务、CSP Azure 和常规许可更新，包括 Azure （2018年11月）
- SQL DB 保留容量 & 实例大小灵活性（2018年8月）
- CSP 中的服务器订阅（2018年7月）
- CSP 中的 Azure 预订概述（可能为2018）

其他有用的培训包括[合作伙伴大学上的 Azure 许可模块](https://aka.ms/azure_partner_licensing)。

### <a name="operations"></a>操作

- [新式商务操作指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)（已更新）：涵盖重要策略和操作方面的综合指南，其中包含协议、按合作伙伴中心、发票、价目表详细信息、奖励、协调文件、API/SDK、沙箱和 Azure 合作伙伴共享服务等。
- [现代产品/服务国家/地区可用性和客户货币矩阵](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [销售 Microsoft Azure 预留实例](https://go.microsoft.com/fwlink/?linkid=872806)
- [代表客户购买 Microsoft Azure 预订](https://go.microsoft.com/fwlink/?linkid=872807)
- [代表客户管理 Azure 预订](https://go.microsoft.com/fwlink/?linkid=872808)
- [Azure 预订计费](azure-plan-billing.md)
- [针对最大预订利用率确定虚拟机大小](https://go.microsoft.com/fwlink/?linkid=872810)
- [合作伙伴中心 API （API/SDK）](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [远程桌面服务](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a>Azure 混合权益

[Azure 混合权益](https://azure.microsoft.com/pricing/hybrid-benefit)可帮助你从 Windows Server 许可证中获取更多价值，最多可节省 47%* 的虚拟机费用。 可以通过软件保障所涵盖的 Windows Server Datacenter 和 Standard Edition 许可证来使用此权益。 根据版本，你可以转换或重复使用你的许可证以在 Azure 中运行 Windows Server 虚拟机，并按较低的基础计算费率（Linux 虚拟机速率）。

另请参阅 [Azure 混合权益常见问题解答](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* 实际节省的费用可能因区域、实例类型或使用情况而异。
