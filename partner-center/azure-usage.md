---
title: Microsoft Azure VM 大小调整为最大的预订使用情况 |合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
Description: 代表客户购买 Microsoft Azure 预订时，你将需要选择一个大小能够满足客户计算需求的虚拟机 (VM)。
author: LauraBrenner
ms.author: v-petand
keywords: azure, 预订, 虚拟机, 管理, 利用率, 确定大小
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 9a398b73cf00bd71130d25f0ec94a33b457e216b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135499"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="07d5a-104">针对最大预定利用率确定 Microsoft Azure 虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="07d5a-104">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

<span data-ttu-id="07d5a-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="07d5a-105">**Applies to**</span></span>

-  <span data-ttu-id="07d5a-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="07d5a-106">Partner Center</span></span>
-  <span data-ttu-id="07d5a-107">Azure 门户</span><span class="sxs-lookup"><span data-stu-id="07d5a-107">Azure portal</span></span>
-  <span data-ttu-id="07d5a-108">云解决方案提供商计划中的合作伙伴</span><span class="sxs-lookup"><span data-stu-id="07d5a-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="07d5a-109">确定客户 Azure 预订的虚拟机大小</span><span class="sxs-lookup"><span data-stu-id="07d5a-109">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="07d5a-110">代表客户购买 Microsoft Azure 预订时，你将需要选择一个大小能够满足客户计算需求的虚拟机 (VM)。</span><span class="sxs-lookup"><span data-stu-id="07d5a-110">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="07d5a-111">你可以使用以下方法之一查找此信息：</span><span class="sxs-lookup"><span data-stu-id="07d5a-111">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="07d5a-112">Azure 使用率 API</span><span class="sxs-lookup"><span data-stu-id="07d5a-112">Azure utilization API</span></span>
-   <span data-ttu-id="07d5a-113">Azure 门户</span><span class="sxs-lookup"><span data-stu-id="07d5a-113">The Azure portal</span></span>
-   <span data-ttu-id="07d5a-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="07d5a-114">Azure PowerShell</span></span>
-   <span data-ttu-id="07d5a-115">Azure 资源管理器 (ARM) API</span><span class="sxs-lookup"><span data-stu-id="07d5a-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="07d5a-116">每种方法的使用说明如下。</span><span class="sxs-lookup"><span data-stu-id="07d5a-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="07d5a-117">购买预订后，预订折扣会自动应用于与预订的属性和数量相匹配的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="07d5a-118">你不需要将预订分配给虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-118">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="07d5a-119">预订折扣不适用于经典或促销的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-119">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="07d5a-120">若要正确识别要代表客户购买的虚拟机的类型和大小，你必须使用下述方法之一，因为合作伙伴中心对帐文件中未正确显示虚拟机系列类型。</span><span class="sxs-lookup"><span data-stu-id="07d5a-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


<span data-ttu-id="07d5a-121">**获取虚拟机的大小调整信息使用的 Azure 使用率 API**</span><span class="sxs-lookup"><span data-stu-id="07d5a-121">**Get VM sizing information using the Azure utilization API**</span></span>

1.  <span data-ttu-id="07d5a-122">使用 API 响应中 additionalInfo 的 ServiceType 属性值来标识要购买的虚拟机大小。</span><span class="sxs-lookup"><span data-stu-id="07d5a-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="07d5a-123">有关详细信息，请参阅[合作伙伴中心 API](https://docs.microsoft.com/partner-center/develop/) 中的[获取客户的 Azure 利用率记录](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。</span><span class="sxs-lookup"><span data-stu-id="07d5a-123">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

<span data-ttu-id="07d5a-124">**获取虚拟机的大小调整信息使用 Microsoft Azure 门户**</span><span class="sxs-lookup"><span data-stu-id="07d5a-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1.  <span data-ttu-id="07d5a-125">在合作伙伴中心，请转到您**客户**页。</span><span class="sxs-lookup"><span data-stu-id="07d5a-125">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="07d5a-126">查找想要购买 Azure 虚拟机预订的客户，然后选择向下箭头以展开客户的信息。</span><span class="sxs-lookup"><span data-stu-id="07d5a-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="07d5a-127">选择 **Microsoft Azure 管理门户**以在 Azure 门户中打开客户的记录。</span><span class="sxs-lookup"><span data-stu-id="07d5a-127">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="07d5a-128">从门户菜单中选择**虚拟机**，然后选择你想要为其购买预订的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="07d5a-129">在虚拟机的详细信息页面上，查找大小和区域信息，如下所示，并使用此信息在合作伙伴中心购买预订。</span><span class="sxs-lookup"><span data-stu-id="07d5a-129">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![在详细信息页上的大小和区域信息](images/usage1.png)

<span data-ttu-id="07d5a-131">**获取虚拟机的大小调整信息使用 Microsoft Azure PowerShell**</span><span class="sxs-lookup"><span data-stu-id="07d5a-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="07d5a-132">使用下图中的信息，以获取你想要为其购买预订的虚拟机的位置和大小。</span><span class="sxs-lookup"><span data-stu-id="07d5a-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![VM 位置和大小](images/usage2.png)

<span data-ttu-id="07d5a-134">**获取虚拟机的大小调整信息使用 Azure 资源管理器 (ARM) API**</span><span class="sxs-lookup"><span data-stu-id="07d5a-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1.  <span data-ttu-id="07d5a-135">使用 ARMClient 或 ARM API，为你想要为其购买预订的虚拟机调用 ARM 客户端。</span><span class="sxs-lookup"><span data-stu-id="07d5a-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="07d5a-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="07d5a-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="07d5a-137">此调用将返回 **vmSize** 和 **location** 的值，如下所示。</span><span class="sxs-lookup"><span data-stu-id="07d5a-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="07d5a-138">![vmSize 值](images/usage3.png)
    ![位置值](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="07d5a-138">![vmSize value](images/usage3.png)
![location value](images/usage4.png)</span></span>
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="07d5a-139">验证 Azure 虚拟机使用情况和预订折扣</span><span class="sxs-lookup"><span data-stu-id="07d5a-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="07d5a-140">代表客户购买 Azure 虚拟机预留实例后，预先为虚拟机空间付款的折扣会自动应用于与客户预订的属性和数量相匹配的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="07d5a-141">你可以使用以下方法之一来验证客户的预订利用率，并查看应用了预订折扣的虚拟机：</span><span class="sxs-lookup"><span data-stu-id="07d5a-141">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="07d5a-142">Azure 门户</span><span class="sxs-lookup"><span data-stu-id="07d5a-142">The Azure portal</span></span>
-   <span data-ttu-id="07d5a-143">Azure 使用率 API</span><span class="sxs-lookup"><span data-stu-id="07d5a-143">Azure utilization API</span></span>

<span data-ttu-id="07d5a-144">每种方法的使用说明如下。</span><span class="sxs-lookup"><span data-stu-id="07d5a-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="07d5a-145">只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="07d5a-146">在 Microsoft Azure 门户中验证客户的预订利用率</span><span class="sxs-lookup"><span data-stu-id="07d5a-146">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="07d5a-147">在合作伙伴中心，请转到您**客户**页。</span><span class="sxs-lookup"><span data-stu-id="07d5a-147">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="07d5a-148">查找想要验证其预订折扣和使用情况的客户，然后选择向下箭头以展开客户的信息。</span><span class="sxs-lookup"><span data-stu-id="07d5a-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="07d5a-149">选择 **Microsoft Azure 管理门户**以在 Azure 门户中打开客户的记录。</span><span class="sxs-lookup"><span data-stu-id="07d5a-149">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="07d5a-150">从门户菜单中选择**预订**，然后选择想要检查其使用情况的预订。</span><span class="sxs-lookup"><span data-stu-id="07d5a-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="07d5a-151">在**概述**页面上，查看预订的利用率图表，其中显示了应用于虚拟机的预订量。</span><span class="sxs-lookup"><span data-stu-id="07d5a-151">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="07d5a-152">利用率数据最多可能会延迟 8 小时。</span><span class="sxs-lookup"><span data-stu-id="07d5a-152">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="07d5a-153">a.</span><span class="sxs-lookup"><span data-stu-id="07d5a-153">a.</span></span>  <span data-ttu-id="07d5a-154">如果预订的利用率为 100%，则客户将实现预订购买可达到的所有可能的节省额。</span><span class="sxs-lookup"><span data-stu-id="07d5a-154">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="07d5a-155">b.</span><span class="sxs-lookup"><span data-stu-id="07d5a-155">b.</span></span>  <span data-ttu-id="07d5a-156">如果预订的利用率为 0%，那么折扣未应用于任何虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-156">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="07d5a-157">c.</span><span class="sxs-lookup"><span data-stu-id="07d5a-157">c.</span></span>  <span data-ttu-id="07d5a-158">如果预订的利用率介于 1% 和 99% 之间，则有未使用的权益。</span><span class="sxs-lookup"><span data-stu-id="07d5a-158">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="07d5a-159">为了避免这种情况，请在购买之前确定正确的虚拟机大小以满足客户的计算需求。</span><span class="sxs-lookup"><span data-stu-id="07d5a-159">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="07d5a-160">利用 Azure 利用率 API 验证客户的预订利用率</span><span class="sxs-lookup"><span data-stu-id="07d5a-160">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="07d5a-161">只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。</span><span class="sxs-lookup"><span data-stu-id="07d5a-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="07d5a-162">你可以使用 Azure 利用率 API 获取预定利用率数据，以验证客户是否获得了预订折扣并查看折扣应用于的 VM（虚拟机）。</span><span class="sxs-lookup"><span data-stu-id="07d5a-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="07d5a-163">比较示例 A 与示例 B，了解如何验证客户的预定利用率。</span><span class="sxs-lookup"><span data-stu-id="07d5a-163">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![保留用法示例](images/usage5.png)

-   <span data-ttu-id="07d5a-165">reservationId 标识用于将折扣应用于虚拟机的 Azure 预定。</span><span class="sxs-lookup"><span data-stu-id="07d5a-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="07d5a-166">consumptionMeter 是应用了预订折扣的虚拟机的 MeterId。</span><span class="sxs-lookup"><span data-stu-id="07d5a-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="07d5a-167">由于应用了预订折扣，ReservationMeter 会显示 0 美元的成本。</span><span class="sxs-lookup"><span data-stu-id="07d5a-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="07d5a-168">有关详细信息，请参阅[合作伙伴中心 API](https://docs.microsoft.com/partner-center/develop/) 中的[获取客户的 Azure 利用率记录](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。</span><span class="sxs-lookup"><span data-stu-id="07d5a-168">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="07d5a-169">软件（如 Microsoft Windows Server）成本目前未包含在虚拟机预定的价格中，并且在订单记录和发票上显示为单独的行项目。</span><span class="sxs-lookup"><span data-stu-id="07d5a-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="07d5a-170">但是，如果客户拥有 Azure 混合使用权益，则不会应用软件成本。</span><span class="sxs-lookup"><span data-stu-id="07d5a-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="07d5a-171">有关详细信息，请参阅[预留实例中不包含 Windows 软件成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。</span><span class="sxs-lookup"><span data-stu-id="07d5a-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="07d5a-172">Azure 预订资源</span><span class="sxs-lookup"><span data-stu-id="07d5a-172">Azure reservations resources</span></span>
|<span data-ttu-id="07d5a-173">**有关信息**</span><span class="sxs-lookup"><span data-stu-id="07d5a-173">**For information about**</span></span>   |<span data-ttu-id="07d5a-174">**阅读此内容**</span><span class="sxs-lookup"><span data-stu-id="07d5a-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="07d5a-175">云解决方案提供商计划中的 Azure 预订概述</span><span class="sxs-lookup"><span data-stu-id="07d5a-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="07d5a-176">销售 Microsoft Azure 保留的 VM 实例</span><span class="sxs-lookup"><span data-stu-id="07d5a-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="07d5a-177">在合作伙伴中心客户购买 Azure 保留项</span><span class="sxs-lookup"><span data-stu-id="07d5a-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="07d5a-178">购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="07d5a-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="07d5a-179">管理 Azure 保留在合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="07d5a-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="07d5a-180">管理 Azure 保留在合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="07d5a-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="07d5a-181">在 Azure 门户中购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="07d5a-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="07d5a-182">Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="07d5a-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="07d5a-183">在 Azure 门户中管理 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="07d5a-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="07d5a-184">Azure 帮助中的[管理虚拟机预留实例](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="07d5a-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="07d5a-185">使用合作伙伴中心 API 购买 Azure 预订</span><span class="sxs-lookup"><span data-stu-id="07d5a-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="07d5a-186">合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="07d5a-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



