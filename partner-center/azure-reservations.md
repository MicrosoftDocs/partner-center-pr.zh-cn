---
title: 销售客户Microsoft Azure预留
description: 作为云解决方案提供商，你可以为客户购买、销售或管理 Azure 预留。 使用 合作伙伴中心、Azure 门户 或 合作伙伴中心 API。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: b97cafea9ad2f36718418c7c7cfca5f91ee8849c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149462"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="90ddf-104">使用 Microsoft Azure、Azure 门户 或 API 合作伙伴中心客户销售预留</span><span class="sxs-lookup"><span data-stu-id="90ddf-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="90ddf-105">**适当的角色**：管理员代理|全局管理员|支持人员代理|销售代理|用户管理管理员</span><span class="sxs-lookup"><span data-stu-id="90ddf-105">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

<span data-ttu-id="90ddf-106">作为云解决方案提供商云解决方案提供商计划 (合作伙伴) ，你可以为客户购买、销售或管理 Azure 预留。</span><span class="sxs-lookup"><span data-stu-id="90ddf-106">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="90ddf-107">使用 合作伙伴中心、Azure 门户 或 合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="90ddf-107">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="90ddf-108">本文仅适用于 CSP 中的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="90ddf-108">This article applies only to partners in CSP.</span></span> <span data-ttu-id="90ddf-109">使用其他类型的订阅（例如 (即用即付、个人、Microsoft 客户协议 或 企业协议 订阅) 应改为阅读 [此 Azure](/azure/cost-management-billing/reservations)预留文档。</span><span class="sxs-lookup"><span data-stu-id="90ddf-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="90ddf-110">CSP 计划中的合作伙伴可以为客户提供Microsoft Azure预留。</span><span class="sxs-lookup"><span data-stu-id="90ddf-110">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="90ddf-111">如果客户预先预订空间，可以节省大量成本。</span><span class="sxs-lookup"><span data-stu-id="90ddf-111">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="90ddf-112">Azure 预留通过以下方式为客户提供简单性和灵活性：</span><span class="sxs-lookup"><span data-stu-id="90ddf-112">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="90ddf-113">预订一年或三年</span><span class="sxs-lookup"><span data-stu-id="90ddf-113">One or three-year reservation terms</span></span>
- <span data-ttu-id="90ddf-114">轻松入门；几秒内即可完成设置</span><span class="sxs-lookup"><span data-stu-id="90ddf-114">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="90ddf-115">随时取消或兑换预留实例以获取调整的退款</span><span class="sxs-lookup"><span data-stu-id="90ddf-115">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="90ddf-116">在组织或单个部门级别管理预留实例的使用</span><span class="sxs-lookup"><span data-stu-id="90ddf-116">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="90ddf-117">Azure 预留可以通过以下方式吸引客户：</span><span class="sxs-lookup"><span data-stu-id="90ddf-117">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="90ddf-118">与使用 PAYG 或 PAYG 的"立即付款"定价 (节省) 成本</span><span class="sxs-lookup"><span data-stu-id="90ddf-118">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="90ddf-119">通过一年或三年的预付款更好地进行预算和预测</span><span class="sxs-lookup"><span data-stu-id="90ddf-119">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="90ddf-120">最接近办公室的 Azure 区域中优先选择的计算能力</span><span class="sxs-lookup"><span data-stu-id="90ddf-120">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="90ddf-121">与 Microsoft Windows Server 和 Azure SQL 数据库 等软件结合使用时，Azure 预留为端到端基础结构解决方案Azure SQL 数据库</span><span class="sxs-lookup"><span data-stu-id="90ddf-121">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="90ddf-122">可以在门户和门户中购买、销售和管理 Azure 合作伙伴中心Azure 门户，以及使用 合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="90ddf-122">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="90ddf-123">还可以授予客户从为客户购买的 Azure 订阅购买自己的 Azure 预留的权限。</span><span class="sxs-lookup"><span data-stu-id="90ddf-123">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="90ddf-124">单击下面的链接以了解如何操作。</span><span class="sxs-lookup"><span data-stu-id="90ddf-124">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="90ddf-125">Azure 预订资源</span><span class="sxs-lookup"><span data-stu-id="90ddf-125">Azure reservations resources</span></span>

|<span data-ttu-id="90ddf-126">**有关以下方面的信息**</span><span class="sxs-lookup"><span data-stu-id="90ddf-126">**For information about**</span></span>   |<span data-ttu-id="90ddf-127">**阅读此文**</span><span class="sxs-lookup"><span data-stu-id="90ddf-127">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="90ddf-128">适用于客户的 Azure 预留文档</span><span class="sxs-lookup"><span data-stu-id="90ddf-128">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="90ddf-129">什么是 Azure 预留？</span><span class="sxs-lookup"><span data-stu-id="90ddf-129">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="90ddf-130">在 Azure 门户中为客户购买 Azure 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="90ddf-130">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="90ddf-131">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="90ddf-131">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="90ddf-132">在门户中管理 Azure 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="90ddf-132">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="90ddf-133">在门户中管理 Azure 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="90ddf-133">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="90ddf-134">确定正确的 VM 大小并验证客户 VM 使用情况</span><span class="sxs-lookup"><span data-stu-id="90ddf-134">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="90ddf-135">针对最大 Azure 预订利用率确定虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="90ddf-135">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="90ddf-136">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="90ddf-136">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="90ddf-137">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="90ddf-137">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="90ddf-138">为客户提供从 CSP 订阅购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="90ddf-138">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="90ddf-139">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="90ddf-139">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |