---
title: 针对最大预留项使用率调整 Azure VM 的大小
description: 了解如何在为客户购买 (预留时) VM 大小，Microsoft Azure计算需求。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 2d8bc76e0da51abf433e49028445b398c6a1db31
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276988"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="2d213-103">针对最大预定利用率确定 Microsoft Azure 虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="2d213-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="2d213-104">**适当的角色**：管理员代理|销售代理</span><span class="sxs-lookup"><span data-stu-id="2d213-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="2d213-105">本文介绍如何在为客户购买 (预留时) VM 大小，Microsoft Azure计算需求。</span><span class="sxs-lookup"><span data-stu-id="2d213-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="2d213-106">本文仅适用于云解决方案提供商计划云解决方案提供商 () 合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="2d213-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="2d213-107">使用其他类型的订阅（例如 (即用即付、个人、Microsoft 客户协议 或 企业协议 订阅) 应改为阅读 [此 Azure](/azure/cost-management-billing/reservations)预留文档。</span><span class="sxs-lookup"><span data-stu-id="2d213-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="2d213-108">确定客户的 Azure 预留的 VM 大小</span><span class="sxs-lookup"><span data-stu-id="2d213-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="2d213-109">代表Microsoft Azure购买预留时，需要选择虚拟机 (VM) 以满足客户的计算需求。</span><span class="sxs-lookup"><span data-stu-id="2d213-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="2d213-110">你可以使用以下方法之一查找此信息：</span><span class="sxs-lookup"><span data-stu-id="2d213-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="2d213-111">Azure 使用率 API</span><span class="sxs-lookup"><span data-stu-id="2d213-111">Azure utilization API</span></span>
- <span data-ttu-id="2d213-112">Azure 门户</span><span class="sxs-lookup"><span data-stu-id="2d213-112">The Azure portal</span></span>
- <span data-ttu-id="2d213-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2d213-113">Azure PowerShell</span></span>
- <span data-ttu-id="2d213-114">Azure 资源管理器 (ARM) API</span><span class="sxs-lookup"><span data-stu-id="2d213-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="2d213-115">每种方法的使用说明如下。</span><span class="sxs-lookup"><span data-stu-id="2d213-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="2d213-116">购买预订后，预订折扣会自动应用于与预订的属性和数量相匹配的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="2d213-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="2d213-117">无需将预留分配给 VM。</span><span class="sxs-lookup"><span data-stu-id="2d213-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="2d213-118">预留折扣不适用于经典或促销 VM。</span><span class="sxs-lookup"><span data-stu-id="2d213-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="2d213-119">若要正确识别要代表客户购买的虚拟机的类型和大小，你必须使用下述方法之一，因为合作伙伴中心对帐文件中未正确显示虚拟机系列类型。</span><span class="sxs-lookup"><span data-stu-id="2d213-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="2d213-120">使用 Azure 利用率 API 获取虚拟机大小信息</span><span class="sxs-lookup"><span data-stu-id="2d213-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="2d213-121">使用 API 响应中 additionalInfo 的 ServiceType 属性值来标识要购买的虚拟机大小。</span><span class="sxs-lookup"><span data-stu-id="2d213-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="2d213-122">有关详细信息，请参阅在 Azure API 中获取 [客户的 Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [合作伙伴中心记录](/partner-center/develop/)。</span><span class="sxs-lookup"><span data-stu-id="2d213-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="2d213-123">使用 Microsoft Azure 门户获取虚拟机大小信息</span><span class="sxs-lookup"><span data-stu-id="2d213-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="2d213-124">在合作伙伴中心中，转到"客户 **"** 页。</span><span class="sxs-lookup"><span data-stu-id="2d213-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="2d213-125">找到想要购买 Azure VM 预留的客户，然后选择向下箭头以展开客户的信息。</span><span class="sxs-lookup"><span data-stu-id="2d213-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="2d213-126">选择 **Microsoft Azure 管理门户"，** 打开客户在 Azure 门户 中的记录。</span><span class="sxs-lookup"><span data-stu-id="2d213-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="2d213-127">从门户菜单中选择 **虚拟机**，然后选择你想要为其购买预订的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="2d213-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="2d213-128">在 VM 的详细信息页上，找到大小和区域信息（如下所示）并使用此信息在虚拟机中合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="2d213-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="详细信息页上的大小和区域信息。":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="2d213-130">使用 Microsoft Azure PowerShell 获取虚拟机大小信息</span><span class="sxs-lookup"><span data-stu-id="2d213-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="2d213-131">使用下图中的信息，以获取你想要为其购买预订的虚拟机的位置和大小。</span><span class="sxs-lookup"><span data-stu-id="2d213-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM 位置和大小。":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="2d213-133">使用 Azure 资源管理器 (ARM) API 获取虚拟机大小信息</span><span class="sxs-lookup"><span data-stu-id="2d213-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="2d213-134">使用 ARMClient 或 ARM API，为你想要为其购买预订的虚拟机调用 ARM 客户端。</span><span class="sxs-lookup"><span data-stu-id="2d213-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="2d213-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="2d213-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="2d213-136">此调用将返回 **vmSize** 和 **location** 的值，如下所示。</span><span class="sxs-lookup"><span data-stu-id="2d213-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 值。":::
    :::image type="content" source="images/usage4.png" alt-text="location 值。":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="2d213-139">验证 Azure 虚拟机使用情况和预订折扣</span><span class="sxs-lookup"><span data-stu-id="2d213-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="2d213-140">代表客户购买 Azure 虚拟机预留实例后，提前支付 VM 空间的折扣将自动应用于与客户预留的属性和数量匹配的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="2d213-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="2d213-141">可以使用以下方法之一验证客户的预留使用情况，并查看预留折扣应用到的虚拟机：</span><span class="sxs-lookup"><span data-stu-id="2d213-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="2d213-142">Azure 门户</span><span class="sxs-lookup"><span data-stu-id="2d213-142">The Azure portal</span></span>
- <span data-ttu-id="2d213-143">Azure 使用率 API</span><span class="sxs-lookup"><span data-stu-id="2d213-143">Azure utilization API</span></span>

<span data-ttu-id="2d213-144">每种方法的使用说明如下。</span><span class="sxs-lookup"><span data-stu-id="2d213-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="2d213-145">只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="2d213-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="2d213-146">验证客户的预留使用情况Microsoft Azure 门户</span><span class="sxs-lookup"><span data-stu-id="2d213-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="2d213-147">在合作伙伴中心中，转到"客户 **"** 页。</span><span class="sxs-lookup"><span data-stu-id="2d213-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="2d213-148">找到要验证其预留折扣和使用情况的客户，然后选择向下箭头以展开客户的信息。</span><span class="sxs-lookup"><span data-stu-id="2d213-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="2d213-149">选择 **Microsoft Azure 管理门户"，** 打开客户在 Azure 门户 中的记录。</span><span class="sxs-lookup"><span data-stu-id="2d213-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="2d213-150">从门户菜单中选择 **预订**，然后选择想要检查其使用情况的预订。</span><span class="sxs-lookup"><span data-stu-id="2d213-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="2d213-151">在 **"概述** "页上，检查预留的利用率图，其中显示了已应用到虚拟机的预留数。</span><span class="sxs-lookup"><span data-stu-id="2d213-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2d213-152">利用率数据最多可能会延迟 8 小时。</span><span class="sxs-lookup"><span data-stu-id="2d213-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="2d213-153">a.</span><span class="sxs-lookup"><span data-stu-id="2d213-153">a.</span></span> <span data-ttu-id="2d213-154">如果预留的利用率为 100%，则客户将获得预留购买可以提供的所有可能节省。</span><span class="sxs-lookup"><span data-stu-id="2d213-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="2d213-155">b.</span><span class="sxs-lookup"><span data-stu-id="2d213-155">b.</span></span> <span data-ttu-id="2d213-156">如果预留使用量为 0%，则折扣不会应用于任何虚拟机。</span><span class="sxs-lookup"><span data-stu-id="2d213-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="2d213-157">c.</span><span class="sxs-lookup"><span data-stu-id="2d213-157">c.</span></span> <span data-ttu-id="2d213-158">如果预留使用量在 1% 到 99% 之间，则有未使用的权益。</span><span class="sxs-lookup"><span data-stu-id="2d213-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="2d213-159">若要避免这种情况，在购买之前，请确定支持客户计算需求的正确 VM 大小。</span><span class="sxs-lookup"><span data-stu-id="2d213-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="2d213-160">使用 Azure 利用率 API 验证客户的预留使用情况</span><span class="sxs-lookup"><span data-stu-id="2d213-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="2d213-161">只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="2d213-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="2d213-162">你可以使用 Azure 利用率 API 获取预定利用率数据，以验证客户是否获得了预订折扣并查看折扣应用于的 VM（虚拟机）。</span><span class="sxs-lookup"><span data-stu-id="2d213-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="2d213-163">将示例 A 与示例 B 进行比较，了解如何验证客户的预留使用情况。</span><span class="sxs-lookup"><span data-stu-id="2d213-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="预留使用情况示例。":::

- <span data-ttu-id="2d213-165">reservationId 标识用于将折扣应用于虚拟机的 Azure 预定。</span><span class="sxs-lookup"><span data-stu-id="2d213-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="2d213-166">consumptionMeter 是应用了预订折扣的虚拟机的 MeterId。</span><span class="sxs-lookup"><span data-stu-id="2d213-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="2d213-167">由于应用了预订折扣，ReservationMeter 会显示 0 美元的成本。</span><span class="sxs-lookup"><span data-stu-id="2d213-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="2d213-168">有关详细信息，请参阅在 Azure API 中获取 [客户的 Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [合作伙伴中心记录](/partner-center/develop/)。</span><span class="sxs-lookup"><span data-stu-id="2d213-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="2d213-169">软件（如 Microsoft Windows Server）成本目前未包含在虚拟机预定的价格中，并且在订单记录和发票上显示为单独的行项目。</span><span class="sxs-lookup"><span data-stu-id="2d213-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="2d213-170">但是，如果客户拥有 Azure 混合使用权益，则不会应用软件成本。</span><span class="sxs-lookup"><span data-stu-id="2d213-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="2d213-171">有关详细信息，请参阅[预留实例中不包含 Windows 软件成本](/azure/billing/billing-reserved-instance-windows-software-costs)。</span><span class="sxs-lookup"><span data-stu-id="2d213-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="2d213-172">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2d213-172">Next steps</span></span>

|<span data-ttu-id="2d213-173">**有关以下方面的信息**</span><span class="sxs-lookup"><span data-stu-id="2d213-173">**For information about**</span></span>   |<span data-ttu-id="2d213-174">**阅读此文**</span><span class="sxs-lookup"><span data-stu-id="2d213-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="2d213-175">云解决方案提供商计划中的 Azure 预订概述</span><span class="sxs-lookup"><span data-stu-id="2d213-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="2d213-176">销售 Microsoft Azure 虚拟机预留实例</span><span class="sxs-lookup"><span data-stu-id="2d213-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="2d213-177">在 Azure 门户中为客户购买 Azure 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2d213-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="2d213-178">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2d213-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="2d213-179">在门户中管理 Azure 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2d213-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="2d213-180">在门户中管理 Azure 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="2d213-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="2d213-181">在 Azure 门户中购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2d213-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="2d213-182">Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="2d213-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="2d213-183">在 Azure 门户中管理 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2d213-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="2d213-184">Azure 帮助中的[管理虚拟机预留实例](/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="2d213-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="2d213-185">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="2d213-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="2d213-186">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="2d213-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="2d213-187">为客户提供从你为订阅购买自己的 Azure 预留的权限。</span><span class="sxs-lookup"><span data-stu-id="2d213-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="2d213-188">为客户提供购买自己的 Azure 预留的权限</span><span class="sxs-lookup"><span data-stu-id="2d213-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |