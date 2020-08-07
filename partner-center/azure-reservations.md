---
title: Microsoft Azure 预订销售客户
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 作为云解决方案提供商，你可以购买、销售或管理客户的 Azure 保留。 使用合作伙伴中心、Azure 门户或合作伙伴中心 API。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3efe8ae6a955dee5cfe01d0571cd107f8ee50f5c
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900078"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="8f04e-104">使用合作伙伴中心、Azure 门户或 Api 向客户销售 Microsoft Azure 预订</span><span class="sxs-lookup"><span data-stu-id="8f04e-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="8f04e-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="8f04e-105">**Applies to**</span></span>

- <span data-ttu-id="8f04e-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8f04e-106">Partner Center</span></span>
- <span data-ttu-id="8f04e-107">Microsoft Azure 门户</span><span class="sxs-lookup"><span data-stu-id="8f04e-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="8f04e-108">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="8f04e-108">Partners in the CSP program</span></span>

<span data-ttu-id="8f04e-109">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="8f04e-109">**Appropriate roles**</span></span>

- <span data-ttu-id="8f04e-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="8f04e-110">Admin agent</span></span>
- <span data-ttu-id="8f04e-111">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8f04e-111">Global admin</span></span>
- <span data-ttu-id="8f04e-112">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="8f04e-112">Helpdesk agent</span></span>
- <span data-ttu-id="8f04e-113">销售代理</span><span class="sxs-lookup"><span data-stu-id="8f04e-113">Sales agent</span></span>
- <span data-ttu-id="8f04e-114">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="8f04e-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="8f04e-115">本文仅适用于云解决方案提供商 (CSP) 计划中的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="8f04e-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="8f04e-116">使用其他订阅类型的客户 (例如，即用即付、个人、Microsoft 客户协议或企业协议订阅) 应改为阅读[此 Azure 保留文档](https://docs.microsoft.com/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="8f04e-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="8f04e-117">CSP 计划中的合作伙伴可以为其客户提供 Microsoft Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="8f04e-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="8f04e-118">如果客户预先预订空间，可以节省大量成本。</span><span class="sxs-lookup"><span data-stu-id="8f04e-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="8f04e-119">Azure 保留通过以下方式为客户提供简单和灵活性：</span><span class="sxs-lookup"><span data-stu-id="8f04e-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="8f04e-120">预订一年或三年</span><span class="sxs-lookup"><span data-stu-id="8f04e-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="8f04e-121">轻松入门；几秒内即可完成设置</span><span class="sxs-lookup"><span data-stu-id="8f04e-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="8f04e-122">随时取消或兑换预留实例以获取调整的退款</span><span class="sxs-lookup"><span data-stu-id="8f04e-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="8f04e-123">在组织或单个部门级别管理预留实例的使用</span><span class="sxs-lookup"><span data-stu-id="8f04e-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="8f04e-124">Azure 预订可通过以下方式吸引客户：</span><span class="sxs-lookup"><span data-stu-id="8f04e-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="8f04e-125">预订可通过即用即付 (PAYG) 定价提供显著节省</span><span class="sxs-lookup"><span data-stu-id="8f04e-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="8f04e-126">通过一年或三年的预付款更好地进行预算和预测</span><span class="sxs-lookup"><span data-stu-id="8f04e-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="8f04e-127">最接近办公室的 Azure 区域中优先选择的计算能力</span><span class="sxs-lookup"><span data-stu-id="8f04e-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="8f04e-128">当与 Microsoft Windows Server 和 Azure SQL Database 等软件结合时，Azure 保留提供端到端基础结构解决方案的基础</span><span class="sxs-lookup"><span data-stu-id="8f04e-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="8f04e-129">你可以在合作伙伴中心和 Azure 门户中购买、销售和管理 Azure 预订，并使用合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="8f04e-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="8f04e-130">你还可以为客户提供从为他们购买的 Azure 订阅购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="8f04e-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="8f04e-131">单击下面的链接以了解如何操作。</span><span class="sxs-lookup"><span data-stu-id="8f04e-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="8f04e-132">Azure 预订资源</span><span class="sxs-lookup"><span data-stu-id="8f04e-132">Azure reservations resources</span></span>

|<span data-ttu-id="8f04e-133">**有关以下方面的信息**</span><span class="sxs-lookup"><span data-stu-id="8f04e-133">**For information about**</span></span>   |<span data-ttu-id="8f04e-134">**阅读此文**</span><span class="sxs-lookup"><span data-stu-id="8f04e-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="8f04e-135">适用于你的客户的 Azure 预订文档</span><span class="sxs-lookup"><span data-stu-id="8f04e-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="8f04e-136">什么是 Azure 预留？</span><span class="sxs-lookup"><span data-stu-id="8f04e-136">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="8f04e-137">在合作伙伴中心为客户购买 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="8f04e-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="8f04e-138">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="8f04e-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="8f04e-139">管理合作伙伴中心的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="8f04e-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="8f04e-140">管理合作伙伴中心的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="8f04e-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="8f04e-141">确定正确的 VM 大小并验证客户 VM 使用情况</span><span class="sxs-lookup"><span data-stu-id="8f04e-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="8f04e-142">针对最大 Azure 预订利用率确定虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="8f04e-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="8f04e-143">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="8f04e-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="8f04e-144">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="8f04e-144">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="8f04e-145">为客户提供从 CSP 订阅购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="8f04e-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="8f04e-146">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="8f04e-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
