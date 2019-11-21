---
title: Microsoft Azure VM sizing for maximum reservation usage  | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.
author: LauraBrenner
ms.author: labrenne
keywords: azure, 预订, 虚拟机, 管理, 利用率, 确定大小
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2b8148d66be8a439056efa41eccb60cbc3e4274b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253249"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>针对最大预定利用率确定 Microsoft Azure 虚拟机大小

**适用于**

- 合作伙伴中心
- Azure 门户
- 云解决方案提供商计划中的合作伙伴

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determine the VM size for a customer's Azure reservation 

When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs. 你可以使用以下方法之一查找此信息：

- Azure 使用率 API
- Azure 门户
- Azure PowerShell
- Azure 资源管理器 (ARM) API

每种方法的使用说明如下。 购买预订后，预订折扣会自动应用于与预订的属性和数量相匹配的虚拟机。 You don't need to assign the reservation to a VM.

>[!NOTE]
>Reservation discounts don't apply to classic or promotional VMs.

>[!IMPORTANT]
>若要正确识别要代表客户购买的虚拟机的类型和大小，你必须使用下述方法之一，因为合作伙伴中心对帐文件中未正确显示虚拟机系列类型。

**Get VM sizing information using the Azure utilization API**

1. 使用 API 响应中 additionalInfo 的 ServiceType 属性值来标识要购买的虚拟机大小。
2. For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

**Get VM sizing information using the Microsoft Azure portal**

1. In Partner Center, go to your **Customers** page.
2. Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. 从门户菜单中选择**虚拟机**，然后选择你想要为其购买预订的虚拟机。
4. On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.  

    ![Size and region information on detail page](images/usage1.png)

**Get VM sizing information using Microsoft Azure PowerShell**

使用下图中的信息，以获取你想要为其购买预订的虚拟机的位置和大小。 

![VM location and size](images/usage2.png)

**Get VM sizing information using the Azure Resource Manager (ARM) API**

1. 使用 ARMClient 或 ARM API，为你想要为其购买预订的虚拟机调用 ARM 客户端。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 此调用将返回 **vmSize** 和 **location** 的值，如下所示。

    ![vmSize value](images/usage3.png) ![location value](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>验证 Azure 虚拟机使用情况和预订折扣

After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.

You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:

- Azure 门户
- Azure 使用率 API

每种方法的使用说明如下。

>[!NOTE]
>只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verify the customer's reservation usage in the Microsoft Azure portal

1. In Partner Center, go to your **Customers** page.

2. Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. 从门户菜单中选择**预订**，然后选择想要检查其使用情况的预订。
4. On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.

    >[!NOTE]
    >利用率数据最多可能会延迟 8 小时。

    a. If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.
    b. If the reservation's usage is 0%, the discount is not being applied to any virtual machine.
    c. If the reservation's usage is between 1% and 99%, there are unused benefits.

5. To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verify the customer's reservation usage with the Azure utilization API

>[!NOTE]
>只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。  

你可以使用 Azure 利用率 API 获取预定利用率数据，以验证客户是否获得了预订折扣并查看折扣应用于的 VM（虚拟机）。 Compare Example A to Example B to see how to verify a customer's reservation usage.

![Reservation usage examples](images/usage5.png)

- reservationId 标识用于将折扣应用于虚拟机的 Azure 预定。
- consumptionMeter 是应用了预订折扣的虚拟机的 MeterId。
- 由于应用了预订折扣，ReservationMeter 会显示 0 美元的成本。

For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>软件（如 Microsoft Windows Server）成本目前未包含在虚拟机预定的价格中，并且在订单记录和发票上显示为单独的行项目。 但是，如果客户拥有 Azure 混合使用权益，则不会应用软件成本。 有关详细信息，请参阅[预留实例中不包含 Windows 软件成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。  

## <a name="azure-reservations-resources"></a>Azure 预订资源

|**For information about**   |**阅读此文**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [Sell Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Purchasing Azure reservations for your customers in Partner Center   |[Buy Azure reservations](azure-reservations-buying.md)
|Managing Azure reservations in Partner Center | [Managing Azure reservations in Partner Center](azure-reservations-manage.md)
|在 Azure 门户中购买 Azure 预订 | Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 门户中管理 Azure 预订   |Azure 帮助中的[管理虚拟机预留实例](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)
