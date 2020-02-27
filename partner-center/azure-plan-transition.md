---
title: 将客户过渡到 Azure 计划 | 合作伙伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将客户轻松迁移到 Azure 计划。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567233"
---
# <a name="transition-your-customers-to-azure-plan"></a>将客户过渡到 Azure 计划

**相应的角色**

- 管理员代理
- 计费管理员
- 全局管理员
- 支持人员代理
- 销售代理
- “用户管理”管理员

间接提供商和直接计费合作伙伴可以转换到 Azure 的 Microsoft 云服务提供商计划 (CSP) 中提供的新商务体验。 （间接经销商需通过其间接提供商才能实现此转换。）然后，客户可以通过简便的方式来购买云服务，无论是从合作伙伴、Microsoft 经销商还是直接在 Web 上购买。

转换功能仅适用于要转换到 Azure 新商务体验且已签署 Microsoft 客户协议的客户，而不适用于 CSP 中的其他套餐（例如 Office 365 或 Dynamics 365）。

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP 中提供的 Azure 服务

本部分介绍了 Azure 云解决方案提供商 (CSP) 计划中可用的和不可用的 Azure 服务。 另外还介绍了 [Microsoft Azure 德国](https://azure.microsoft.com/overview/clouds/germany/)和 [Microsoft Azure 政府](https://azure.microsoft.com/overview/clouds/government/)这两个国家/地区云中的服务可用性。

>[!Note]
>[Azure 中国]( https://www.azure.cn/)在 Azure CSP 计划中不可用。

### <a name="global-cloud"></a>全球云 

CSP 计划中提供了基于 Azure 资源管理器模型的所有服务。  非 Azure 资源管理器服务在 CSP 计划中不可用。  

### <a name="csp-specific-service-configurations"></a>特定于 CSP 的服务配置

以下服务需要 CSP 中的特殊配置：

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory 域服务](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure 时序见解](https://azure.microsoft.com/services/time-series-insights/) 仅客户租户中的用户可以访问其时序见解环境中的数据。 默认情况下，合作伙伴可以管理其客户的时序见解环境，但如果合作伙伴需要访问其中的数据，则必须将合作伙伴添加到客户租户中。 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

现在可以从 Visual Studio Marketplace 中购买下面列出的项目，但第三方扩展除外。

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Visual Studio 订阅](https://www.visualstudio.com/subscriptions/)

- [Xamarin University 培训](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

为帮助你入门，我们创建了关于在 CSP 中[如何设置、购买和管理 Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) 的视频和文档。

### <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP 中的 Azure 市场项

目前，并非所有 Azure 市场项在 Azure CSP 订阅中都可用。

- 基于 Microsoft 的 Azure 服务：这些服务可用。 请查看以前的表和注释。

- 自带许可 (BYOL) 项：这些项可用。 [Azure 市场 BYOL 页](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)上提供了支持 BYOL 的 Azure 市场项的完整列表。

- 即用即付第三方 Azure 市场项：如果提供程序已发布到 CSP 渠道，则可以使用这些项。 有关详细信息，请参阅[销售 Azure 市场产品的订阅](https://aka.ms/marketplaceincsp)。   

- Citrix XenApp Essentials：合作伙伴可以为 CSP 中的客户购买 XenApp Essentials。 有关详细信息，请参阅以下 Citrix 博客：[XenApp Essentials 发行版现可通过 Microsoft 云解决方案提供商渠道获取](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)。

### <a name="national-clouds"></a>国家/地区云 
下表显示了国家/地区云中适用于 CSP 的第一方 Azure 产品、服务和功能的定期更新列表。 

| Azure 产品、服务或功能 | 美国政府 | 德国 |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  虚拟机  |  X  |  X  |
|  云服务  |    |    |
|  虚拟机规模集  |  X  |  X  |
|  功能  |    |    |
|  Azure 容器服务  |    |    |
|  **网络**  |    |    |
|  Azure DNS  |    |    |
|  内容分发网络  |    |    |
|  流量管理器  |    |    |
|  ExpressRoute  |  X  |  X  |
|  虚拟网络  |  X  |  X  |
|  负载平衡器  |  X  |  X  |
|  VPN 网关  |  X  |  X  |
|  应用程序网关  |  X  |  X  |
|  网络观察程序  |  X  |  X  |
|  **存储**  |    |    |
|  存储  |  X  |  X  |
|  备份  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  托管磁盘  |  X  |  X  |
|  **Web + 移动**  |    |    |
|  应用服务  |  X  |  X  |
|  Linux 上的应用服务  |    |  X  |
|  API 管理  |  X  |    |
|  内容分发网络  |    |    |
|  媒体服务  |  X  |  X  |
|  通知中心  |  X  |  X  |
|  Azure 搜索  |    |    |
|  Azure 应用服务的逻辑应用功能  |    |    |
|  **容器**  |    |    |
|  应用服务  |  X  |  X  |
|  Linux 上的应用服务  |    |  X  |
|  Batch  |  X  |  X  |
|  容器注册表  |    |    |
|  容器实例  |    |    |
|  Service Fabric  |  X  |  X  |
|  容器服务  |    |    |
|  **数据库**  |    |    |
|  SQL 数据库  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL 数据仓库  |  X  |  X  |
|  Redis 缓存  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **数据 + 分析**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  流分析  |    |  X  |
|  数据工厂  |    |    |
|  Log Analytics  |  X  |    |
|  数据目录  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + 认知服务**  |    |    |
|  机器学习  |    |  X  |
|  Azure 机器人服务  |    |    |
|  认知服务  |    |    |
|  Azure Batch AI  |    |    |
|  **物联网**  |    |    |
|  IoT 中心  |  X  |  X  |
|  IoT Central  |    |    |
|  机器学习  |    |  X  |
|  流分析  |    |  X  |
|  事件中心  |  X  |  X  |
|  基于位置的服务  |    |    |
|  通知中心  |  X  |  X  |
|  时序见解  |    |    |
|  **Enterprise Integration**  |    |    |
|  StorSimple  |  X  |    |
|  API 管理  |    |    |
|  事件网格  |    |    |
|  数据工厂  |    |    |
|  Service Bus  |  X  |  X  |
|  数据目录  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Azure 应用服务的逻辑应用功能  |    |    |
|  **安全 + 标识**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  多重身份验证  |    |    |
|  Azure Active Directory 域服务  |    |    |
|  Key Vault  |  X  |  X  |
|  安全中心  |  X  |  X  |
|  **开发人员工具**  |    |    |
|  Visual Studio 团队服务  |    |    |
|  Application Insights  |    |    |
|  开发测试实验室  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **监视 + 管理**  |    |    |
|  Advisor  |    |    |
|  备份  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  计划程序  |  X  |  X  |
|  自动化  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure 托管应用程序  |    |    |
|  Azure Migrate  |    |    |
|  管理组  |    |  

### <a name="next-steps"></a>后续步骤

- [了解](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview)适用于合作伙伴中心的 Azure 的功能。

- 在 Azure CSP 中[创建](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer)第一个客户，并部署 Azure 服务。

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>将现有的 CSP 套餐过渡到 Azure 计划

可以在合作伙伴中心内部，将客户从其现有 CSP 套餐过渡到 CSP 计划中新商务体验的 Azure 计划下的 Azure 服务。 为此，合作伙伴和客户必须已通过合作伙伴中心建立了分销商关系，并且客户必须已签署 Microsoft 客户协议。

### <a name="select-transition-to-azure-plan"></a>选择过渡到 Azure 计划

1. 选择适用于客户的 Azure 计划。

2. 选择“将计费过渡到 Azure 计划”。 

![过渡](images/azure/transition1.png)

3. 选择“继续” 

![过渡](images/azure/transition2.png)

客户将过渡到 Azure 计划。

**过渡工作流会自动完成前提步骤**：

- 购买 Azure 计划
- Direct CSP 方案中每个客户有一个计划  
- 每个分销商有一个计划  

例如，某家合作伙伴购买了两个 Microsoft Azure 套餐，并在购买时包含了两个不同的 POR。 在这种情况下，过渡工作流将购买两个 Azure 计划（每个分销商有一个），并自动在 Azure 计划下映射相应的 Azure 订阅。  

**将 Azure 订阅映射到 Azure 计划**

购买 Azure 计划后，我们的系统会将现有的 Azure 订阅映射到 Azure 计划。 可以在 Azure 门户以及合作伙伴中心查看进度。 

4. 返回到客户的合作伙伴中心“订阅”页，使用其本地货币更新其预算限制。  

![过渡](images/azure/transition3.png)

>[!NOTE]
>在合作伙伴中心设置的预算不会传播到 Azure 门户。 还应在 Azure 门户中设置预算和警报。

过渡到 Azure 计划后，不再可为此客户购买 Azure 订阅。 在 Azure 门户的 Azure 计划下创建订阅。

>[!NOTE]
> 所有通过 RBAC 在 Azure 计划中购买的 Azure 订阅都将按当地货币定价和计费。 不会使用外汇汇率。

### <a name="track-your-transition-details"></a>跟踪过渡详细信息

可以在 Azure 门户以及合作伙伴中心跟踪过渡进度。

![显示详细信息](images/azure/details1.png)

**对合作伙伴计费的影响**

如果从现有的 CSP Azure 套餐过渡客户，将产生以下计费影响：

- 在退出原始 CSP Azure 订阅之前，将在现有 CSP 发票中计收所有使用费。

- 如果你对现有 CSP 订阅拥有管理员访问权限，则在迁移该订阅时继续拥有访问权限。

若要将直接企业协议过渡到 CSP，并将服务器和云注册过渡到 Azure 服务，请阅读[获取 Microsoft 合作伙伴协议的 Azure 订阅计费所有权](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

**审核日志**：

若要核对计费，请查看“订阅”页上的“Microsoft Azure”(0145P) 订阅历史记录。  

“Microsoft Azure”(0145P) 订阅由两个部分组成：
1. 商务订阅 
2. Azure 订阅（权利）

过渡完成后，Azure 订阅将移到新的 Azure 计划下，商务订阅将会暂停，以便不再报告其使用情况。  

>[注意]：在 CSP 中购买 Microsoft Azure (0145P) 订阅时，商务订阅和 Azure 订阅（权利）具有相同的值。 仅当计费所有权发生更改或转移时，值才会不同。 

**转换问题**

转换期间预计不会发生任何问题。 但如果失败，我们将在过渡工作流本身中提供最新信息。 Azure 的使用不会受到干扰。  

## <a name="next-steps"></a>后续步骤

- [管理 Azure 计划中的订阅和资源](azure-plan-manage.md)

- [合作伙伴赚取的返点 - 概述](partner-earned-credit.md)



