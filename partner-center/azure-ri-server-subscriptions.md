---
title: Azure 预订 & 服务器订阅
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解云解决方案提供商的机会，以便为客户获取、预配和管理 Azure 预订和服务器订阅。
author: LauraBrenner
ms.author: labrenne
keywords: Azure，订阅，VM，预订，保留实例
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4e5e5d88b1f629b07932d37dedb70d0309a26dce
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198625"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="04e5e-104">获取、设置、& 管理客户的 Azure 保留 VM 实例（RI） + 服务器订阅</span><span class="sxs-lookup"><span data-stu-id="04e5e-104">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="04e5e-105">适用于：</span><span class="sxs-lookup"><span data-stu-id="04e5e-105">Applies to:</span></span>

- <span data-ttu-id="04e5e-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="04e5e-106">Partner Center</span></span>

<span data-ttu-id="04e5e-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="04e5e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="04e5e-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="04e5e-108">Admin agent</span></span>
- <span data-ttu-id="04e5e-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="04e5e-109">Global admin</span></span>
- <span data-ttu-id="04e5e-110">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="04e5e-110">Helpdesk agent</span></span>
- <span data-ttu-id="04e5e-111">销售代理</span><span class="sxs-lookup"><span data-stu-id="04e5e-111">Sales agent</span></span>
- <span data-ttu-id="04e5e-112">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="04e5e-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="04e5e-113">什么是 Azure 预留项？</span><span class="sxs-lookup"><span data-stu-id="04e5e-113">What are Azure Reservations?</span></span>

<span data-ttu-id="04e5e-114">Azure 预订可帮助节省一年或三年的虚拟机、SQL 数据库计算能力、Azure Cosmos DB 吞吐量或其他 Azure 资源，从而节省资金。</span><span class="sxs-lookup"><span data-stu-id="04e5e-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="04e5e-115">通过预付，能够以折扣价购买所用资源。</span><span class="sxs-lookup"><span data-stu-id="04e5e-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="04e5e-116">与即用即付价格相比，预订可显著减少虚拟机、SQL 数据库计算、Azure Cosmos DB 和其他资源成本，最高可达72%。</span><span class="sxs-lookup"><span data-stu-id="04e5e-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="04e5e-117">预订提供计费折扣，并且不会影响资源的运行时状态。</span><span class="sxs-lookup"><span data-stu-id="04e5e-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="04e5e-118">有关详细信息，请参阅[什么是 Azure 保留？](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="04e5e-118">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="04e5e-119">客户为何应购买预订？</span><span class="sxs-lookup"><span data-stu-id="04e5e-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="04e5e-120">如果客户有一段时间运行的虚拟机、Azure Cosmos DB 或 SQL 数据库，则购买保留将为他们提供最经济实惠的选项。</span><span class="sxs-lookup"><span data-stu-id="04e5e-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="04e5e-121">例如，如果客户连续运行四个服务实例而没有保留，则按现用现付费率对它们收费。</span><span class="sxs-lookup"><span data-stu-id="04e5e-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="04e5e-122">如果他们购买了这些资源的预留，它们会立即获得预订折扣。</span><span class="sxs-lookup"><span data-stu-id="04e5e-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="04e5e-123">这些资源不再按即用即付费率收费。</span><span class="sxs-lookup"><span data-stu-id="04e5e-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="04e5e-124">云解决方案提供商计划中引人注目的新 Azure 产品/服务</span><span class="sxs-lookup"><span data-stu-id="04e5e-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="04e5e-125">通过将 Azure 保留和服务器订阅引入其 CSP 计划，Microsoft 可以更好地满足快速增长的客户需求，以支持高度可预测、持久的云工作负荷。</span><span class="sxs-lookup"><span data-stu-id="04e5e-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="04e5e-126">通过 CSP 计划，合作伙伴可以通过 Microsoft 合作伙伴中心和 Azure 门户代表商业客户获取、预配和管理 Azure 预订和服务器订阅。</span><span class="sxs-lookup"><span data-stu-id="04e5e-126">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="04e5e-127">我们甚至会在 CSP 计划中为合作伙伴提供有关如何购买 Azure 预订的选项。</span><span class="sxs-lookup"><span data-stu-id="04e5e-127">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="04e5e-128">CSP 合作伙伴可以[代表客户购买 Azure 保留](azure-reservations-buying.md)，也可以允许客户从合作伙伴为其购买的以前的 azure 订阅[购买自己的预订](give-customers-permission.md)。</span><span class="sxs-lookup"><span data-stu-id="04e5e-128">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="04e5e-129">Azure 预订为客户提供了一系列计算解决方案的灵活性，包括开发和测试、运行应用程序以及扩展数据中心。</span><span class="sxs-lookup"><span data-stu-id="04e5e-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="04e5e-130">例如，使用[Azure 保留 VM 实例](https://azure.microsoft.com/pricing/reserved-vm-instances/)，商业客户现在可以节省高达72% 与即用即付 Azure VM 定价，只需购买或 "预留"-虚拟机一年或三年即可实现。</span><span class="sxs-lookup"><span data-stu-id="04e5e-130">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="04e5e-131">与即付即用定价相比，具有 Azure 混合权益（软件保障所附带）的 Windows Server 客户最多可以节省 80% 的费用。</span><span class="sxs-lookup"><span data-stu-id="04e5e-131">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="04e5e-132">由于有说服力的定价和无与伦比的部署灵活性，客户在选择 Azure 预留时将看到最佳的总体价值：</span><span class="sxs-lookup"><span data-stu-id="04e5e-132">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="04e5e-133">Azure 预订</span><span class="sxs-lookup"><span data-stu-id="04e5e-133">Azure reservations</span></span>

- <span data-ttu-id="04e5e-134">Azure 保留 VM 实例</span><span class="sxs-lookup"><span data-stu-id="04e5e-134">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="04e5e-135">SQL DB 保留</span><span class="sxs-lookup"><span data-stu-id="04e5e-135">SQL DB Reservations</span></span>
- <span data-ttu-id="04e5e-136">SQL 托管实例</span><span class="sxs-lookup"><span data-stu-id="04e5e-136">SQL Managed Instance</span></span>
- <span data-ttu-id="04e5e-137">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="04e5e-137">Azure Cosmos DB</span></span>
- <span data-ttu-id="04e5e-138">Azure SQL 数据仓库</span><span class="sxs-lookup"><span data-stu-id="04e5e-138">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="04e5e-139">应用服务</span><span class="sxs-lookup"><span data-stu-id="04e5e-139">App Services</span></span>
- <span data-ttu-id="04e5e-140">Azure Databricks 单位预订</span><span class="sxs-lookup"><span data-stu-id="04e5e-140">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="04e5e-141">托管磁盘</span><span class="sxs-lookup"><span data-stu-id="04e5e-141">Managed Disk</span></span>
- <span data-ttu-id="04e5e-142">块 blob</span><span class="sxs-lookup"><span data-stu-id="04e5e-142">Block blob</span></span>
- <span data-ttu-id="04e5e-143">MySQL</span><span class="sxs-lookup"><span data-stu-id="04e5e-143">MySQL</span></span>
- <span data-ttu-id="04e5e-144">Azure 数据资源管理器</span><span class="sxs-lookup"><span data-stu-id="04e5e-144">Azure Data explorer</span></span>
- <span data-ttu-id="04e5e-145">MariaDB</span><span class="sxs-lookup"><span data-stu-id="04e5e-145">MariaDB</span></span>
- <span data-ttu-id="04e5e-146">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="04e5e-146">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="04e5e-147">服务器订阅</span><span class="sxs-lookup"><span data-stu-id="04e5e-147">Server subscriptions</span></span>

- <span data-ttu-id="04e5e-148">Windows Server</span><span class="sxs-lookup"><span data-stu-id="04e5e-148">Windows Server</span></span>
- <span data-ttu-id="04e5e-149">远程桌面服务（RDS） Cal</span><span class="sxs-lookup"><span data-stu-id="04e5e-149">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="04e5e-150">SQL Server</span><span class="sxs-lookup"><span data-stu-id="04e5e-150">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="04e5e-151">Linux ISV 年度订阅</span><span class="sxs-lookup"><span data-stu-id="04e5e-151">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="04e5e-152">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="04e5e-152">SUSE Linux</span></span>
- <span data-ttu-id="04e5e-153">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="04e5e-153">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="04e5e-154">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="04e5e-154">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="04e5e-155">ISV 年度订阅</span><span class="sxs-lookup"><span data-stu-id="04e5e-155">ISV annual subscriptions</span></span>

- <span data-ttu-id="04e5e-156">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="04e5e-156">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="04e5e-157">入门</span><span class="sxs-lookup"><span data-stu-id="04e5e-157">Getting started</span></span>

<span data-ttu-id="04e5e-158">若要了解如何将 Azure 保留与客户定位，并尽快启动并运行操作性，我们建议采用以下方法查看准备情况资料：</span><span class="sxs-lookup"><span data-stu-id="04e5e-158">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="04e5e-159">查看概述演示文稿和相关的网络研讨会，了解客户价值主张和定位</span><span class="sxs-lookup"><span data-stu-id="04e5e-159">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="04e5e-160">查看并了解《现代商务操作指南》</span><span class="sxs-lookup"><span data-stu-id="04e5e-160">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="04e5e-161">查看 Azure RI 和服务器订阅常见问题</span><span class="sxs-lookup"><span data-stu-id="04e5e-161">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="04e5e-162">了解[合作伙伴中心 API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure 预订和服务器订阅更新</span><span class="sxs-lookup"><span data-stu-id="04e5e-162">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="04e5e-163">资源</span><span class="sxs-lookup"><span data-stu-id="04e5e-163">Resources</span></span>

<span data-ttu-id="04e5e-164">以下是一个全面的资源列表，用于帮助你快速上手以通过合作伙伴中心执行 Azure 预订事务：</span><span class="sxs-lookup"><span data-stu-id="04e5e-164">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="04e5e-165">销售准备情况</span><span class="sxs-lookup"><span data-stu-id="04e5e-165">Sales readiness</span></span>

- [<span data-ttu-id="04e5e-166">Azure 预订和服务器订阅与 Azure 混合权益概述</span><span class="sxs-lookup"><span data-stu-id="04e5e-166">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="04e5e-167">销售工作表</span><span class="sxs-lookup"><span data-stu-id="04e5e-167">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="04e5e-168">Azure 预订的合作伙伴常见问题解答</span><span class="sxs-lookup"><span data-stu-id="04e5e-168">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="04e5e-169">Azure 预订和 SQL 数据库的合作伙伴常见问题解答</span><span class="sxs-lookup"><span data-stu-id="04e5e-169">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="04e5e-170">远程桌面服务（RDS）客户端访问许可证（CAL）（公告）</span><span class="sxs-lookup"><span data-stu-id="04e5e-170">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="04e5e-171">Azure 保留 VM 实例（Azure 门户）</span><span class="sxs-lookup"><span data-stu-id="04e5e-171">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="04e5e-172">服务器订阅</span><span class="sxs-lookup"><span data-stu-id="04e5e-172">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="04e5e-173">Azure 中的 SQL DB 概述</span><span class="sxs-lookup"><span data-stu-id="04e5e-173">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="04e5e-174">SQL DB 保留（Azure 门户）</span><span class="sxs-lookup"><span data-stu-id="04e5e-174">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="04e5e-175">Azure Cosmos DB （Azure 门户）</span><span class="sxs-lookup"><span data-stu-id="04e5e-175">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="04e5e-176">SQL 托管实例（Azure 门户）</span><span class="sxs-lookup"><span data-stu-id="04e5e-176">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="04e5e-177">SUSE 和 Red Hat Enterprise Linux （Azure 门户）</span><span class="sxs-lookup"><span data-stu-id="04e5e-177">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="04e5e-178">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="04e5e-178">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="04e5e-179">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="04e5e-179">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="04e5e-180">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="04e5e-180">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="04e5e-181">Azure 定价概述</span><span class="sxs-lookup"><span data-stu-id="04e5e-181">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="04e5e-182">Azure 价格计算器</span><span class="sxs-lookup"><span data-stu-id="04e5e-182">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="04e5e-183">Azure Databricks 单位预订</span><span class="sxs-lookup"><span data-stu-id="04e5e-183">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="04e5e-184">CSP 价目表： " **Microsoft Azure 预订实例**" 和 "**软件订阅**价格列表" 均位于 "合作伙伴中心[定价 & 产品/服务](https://partner.microsoft.com/pcv/sales)" 页上。</span><span class="sxs-lookup"><span data-stu-id="04e5e-184">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="04e5e-185">培训</span><span class="sxs-lookup"><span data-stu-id="04e5e-185">Training</span></span>

<span data-ttu-id="04e5e-186">注册以查看[商业许可准备情况网络研讨会](https://commercial-licensing.eventbuilder.com/FY2019_ALL)和点播事件。</span><span class="sxs-lookup"><span data-stu-id="04e5e-186">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="04e5e-187">许可准备情况事件包括以下主题：</span><span class="sxs-lookup"><span data-stu-id="04e5e-187">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="04e5e-188">CSP 在线服务、CSP Azure 和常规许可更新，包括 Azure （2018年11月）</span><span class="sxs-lookup"><span data-stu-id="04e5e-188">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="04e5e-189">SQL DB 保留容量 & 实例大小灵活性（2018年8月）</span><span class="sxs-lookup"><span data-stu-id="04e5e-189">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="04e5e-190">CSP 中的服务器订阅（2018年7月）</span><span class="sxs-lookup"><span data-stu-id="04e5e-190">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="04e5e-191">CSP 中的 Azure 预订概述（可能为2018）</span><span class="sxs-lookup"><span data-stu-id="04e5e-191">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="04e5e-192">其他有用的培训包括[合作伙伴大学上的 Azure 许可模块](https://aka.ms/azure_partner_licensing)。</span><span class="sxs-lookup"><span data-stu-id="04e5e-192">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="04e5e-193">Operations</span><span class="sxs-lookup"><span data-stu-id="04e5e-193">Operations</span></span>

- <span data-ttu-id="04e5e-194">[新式商务操作指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)（已更新）：涵盖重要策略和操作方面的综合指南，其中包含协议、按合作伙伴中心、发票、价目表详细信息、奖励、协调文件、API/SDK、沙箱和 Azure 合作伙伴共享服务等。</span><span class="sxs-lookup"><span data-stu-id="04e5e-194">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="04e5e-195">现代产品/服务国家/地区可用性和客户货币矩阵</span><span class="sxs-lookup"><span data-stu-id="04e5e-195">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="04e5e-196">销售 Microsoft Azure 预留实例</span><span class="sxs-lookup"><span data-stu-id="04e5e-196">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="04e5e-197">代表客户购买 Microsoft Azure 预订</span><span class="sxs-lookup"><span data-stu-id="04e5e-197">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="04e5e-198">代表客户管理 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="04e5e-198">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="04e5e-199">Azure 预订计费</span><span class="sxs-lookup"><span data-stu-id="04e5e-199">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="04e5e-200">针对最大预订利用率确定虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="04e5e-200">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="04e5e-201">合作伙伴中心 API （API/SDK）</span><span class="sxs-lookup"><span data-stu-id="04e5e-201">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="04e5e-202">远程桌面服务</span><span class="sxs-lookup"><span data-stu-id="04e5e-202">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="04e5e-203">Azure 混合权益</span><span class="sxs-lookup"><span data-stu-id="04e5e-203">Azure Hybrid Benefit</span></span>

<span data-ttu-id="04e5e-204">[Azure 混合权益](https://azure.microsoft.com/pricing/hybrid-benefit)可帮助你从 Windows Server 许可证中获取更多价值，最多可节省 47%\* 的虚拟机费用。</span><span class="sxs-lookup"><span data-stu-id="04e5e-204">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="04e5e-205">可以通过软件保障所涵盖的 Windows Server Datacenter 和 Standard Edition 许可证来使用此权益。</span><span class="sxs-lookup"><span data-stu-id="04e5e-205">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="04e5e-206">根据版本，你可以转换或重复使用你的许可证以在 Azure 中运行 Windows Server 虚拟机，并按较低的基础计算费率（Linux 虚拟机速率）。</span><span class="sxs-lookup"><span data-stu-id="04e5e-206">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="04e5e-207">另请参阅 [Azure 混合权益常见问题解答](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="04e5e-207">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="04e5e-208">\* 实际节省的费用可能因区域、实例类型或使用情况而异。</span><span class="sxs-lookup"><span data-stu-id="04e5e-208">\*Actual savings may vary based on region, instance type, or usage.</span></span>
