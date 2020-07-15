---
title: Microsoft Azure 预订销售客户
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 作为云解决方案提供商，你可以购买、销售或管理客户的 Azure 保留。 使用合作伙伴中心、Azure 门户或合作伙伴中心 API。
author: BillLinzbach
ms.author: BillLi
keywords: azure, 预订, 管理, 计费, 购买, Azure RI, Azure 预留实例
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 93c6353922197270245b4b21f3bc210f26c7ec8f
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377641"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="2afdb-105">使用合作伙伴中心、Azure 门户或 Api 向客户销售 Microsoft Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2afdb-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="2afdb-106">**适用于**</span><span class="sxs-lookup"><span data-stu-id="2afdb-106">**Applies to**</span></span>

- <span data-ttu-id="2afdb-107">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2afdb-107">Partner Center</span></span>
- <span data-ttu-id="2afdb-108">Microsoft Azure 门户</span><span class="sxs-lookup"><span data-stu-id="2afdb-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="2afdb-109">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="2afdb-109">Partners in CSP</span></span>

<span data-ttu-id="2afdb-110">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="2afdb-110">**Appropriate roles**</span></span>

- <span data-ttu-id="2afdb-111">管理员代理</span><span class="sxs-lookup"><span data-stu-id="2afdb-111">Admin agent</span></span>
- <span data-ttu-id="2afdb-112">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2afdb-112">Global admin</span></span>
- <span data-ttu-id="2afdb-113">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="2afdb-113">Helpdesk agent</span></span>
- <span data-ttu-id="2afdb-114">销售代理</span><span class="sxs-lookup"><span data-stu-id="2afdb-114">Sales agent</span></span>
- <span data-ttu-id="2afdb-115">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="2afdb-115">User management admin</span></span>

<span data-ttu-id="2afdb-116">云解决方案提供商计划（CSP）中的合作伙伴可为其客户提供 Microsoft Azure 预订。</span><span class="sxs-lookup"><span data-stu-id="2afdb-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="2afdb-117">如果客户预先预订空间，可以节省大量成本。</span><span class="sxs-lookup"><span data-stu-id="2afdb-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="2afdb-118">Azure 保留通过以下方式为客户提供简单和灵活性：</span><span class="sxs-lookup"><span data-stu-id="2afdb-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="2afdb-119">预订一年或三年</span><span class="sxs-lookup"><span data-stu-id="2afdb-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="2afdb-120">轻松入门；几秒内即可完成设置</span><span class="sxs-lookup"><span data-stu-id="2afdb-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="2afdb-121">随时取消或兑换预留实例以获取调整的退款</span><span class="sxs-lookup"><span data-stu-id="2afdb-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="2afdb-122">在组织或单个部门级别管理预留实例的使用</span><span class="sxs-lookup"><span data-stu-id="2afdb-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="2afdb-123">Azure 预订可通过以下方式吸引客户：</span><span class="sxs-lookup"><span data-stu-id="2afdb-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="2afdb-124">预订可以通过即用即付（PAYG）定价显著节省费用</span><span class="sxs-lookup"><span data-stu-id="2afdb-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="2afdb-125">通过一年或三年的预付款更好地进行预算和预测</span><span class="sxs-lookup"><span data-stu-id="2afdb-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="2afdb-126">最接近办公室的 Azure 区域中优先选择的计算能力</span><span class="sxs-lookup"><span data-stu-id="2afdb-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="2afdb-127">当与 Microsoft Windows Server 和 Azure SQL Database 等软件结合时，Azure 保留提供端到端基础结构解决方案的基础</span><span class="sxs-lookup"><span data-stu-id="2afdb-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="2afdb-128">你可以在合作伙伴中心和 Azure 门户中购买、销售和管理 Azure 预订，并使用合作伙伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="2afdb-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="2afdb-129">你还可以为客户提供从为他们购买的 Azure 订阅购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="2afdb-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="2afdb-130">单击下面的链接以了解如何操作。</span><span class="sxs-lookup"><span data-stu-id="2afdb-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="2afdb-131">Azure 预订资源</span><span class="sxs-lookup"><span data-stu-id="2afdb-131">Azure reservations resources</span></span>

|<span data-ttu-id="2afdb-132">**有关以下方面的信息**</span><span class="sxs-lookup"><span data-stu-id="2afdb-132">**For information about**</span></span>   |<span data-ttu-id="2afdb-133">**阅读此文**</span><span class="sxs-lookup"><span data-stu-id="2afdb-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="2afdb-134">适用于你的客户的 Azure 预订文档</span><span class="sxs-lookup"><span data-stu-id="2afdb-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="2afdb-135">什么是 Azure 预留？</span><span class="sxs-lookup"><span data-stu-id="2afdb-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="2afdb-136">在合作伙伴中心为客户购买 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="2afdb-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="2afdb-137">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2afdb-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="2afdb-138">管理合作伙伴中心的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="2afdb-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="2afdb-139">管理合作伙伴中心的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="2afdb-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="2afdb-140">确定正确的 VM 大小并验证客户 VM 使用情况</span><span class="sxs-lookup"><span data-stu-id="2afdb-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="2afdb-141">针对最大 Azure 预订利用率确定虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="2afdb-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="2afdb-142">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2afdb-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="2afdb-143">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="2afdb-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="2afdb-144">为客户提供从 CSP 订阅购买自己的 Azure 预订的权限。</span><span class="sxs-lookup"><span data-stu-id="2afdb-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="2afdb-145">授予客户购买自己的 Azure 预订的权限</span><span class="sxs-lookup"><span data-stu-id="2afdb-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
