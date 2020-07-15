---
title: 为最大预留使用量调整 Azure VM 大小
ms.topic: article
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解在购买 Microsoft Azure 预订时，如何将虚拟机（VM）大小调整为客户的计算需求。
author: BillLinzbach
ms.author: BillLi
keywords: azure, 预订, 虚拟机, 管理, 利用率, 确定大小
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 00da6723fc8aa4a5b3f1e0f747cb63acc1a504a8
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377651"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>针对最大预定利用率确定 Microsoft Azure 虚拟机大小

**适用于**

- 合作伙伴中心
- Azure 门户
- 云解决方案提供商计划中的合作伙伴

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>确定客户的 Azure 预留的 VM 大小

代表你的客户购买 Microsoft Azure 预订时，你需要选择一个规模为满足客户计算需求的虚拟机（VM）。 你可以使用以下方法之一查找此信息：

- Azure 使用率 API
- Azure 门户
- Azure PowerShell
- Azure 资源管理器 (ARM) API

每种方法的使用说明如下。 购买预订后，预订折扣会自动应用于与预订的属性和数量相匹配的虚拟机。 不需要将保留分配给 VM。

>[!NOTE]
>预订折扣不适用于经典或促销 Vm。

>[!IMPORTANT]
>若要正确识别要代表客户购买的虚拟机的类型和大小，你必须使用下述方法之一，因为合作伙伴中心对帐文件中未正确显示虚拟机系列类型。

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>使用 Azure 利用率 API 获取虚拟机大小信息

1. 使用 API 响应中 additionalInfo 的 ServiceType 属性值来标识要购买的虚拟机大小。

2. 有关详细信息，请参阅在[合作伙伴中心 API](https://docs.microsoft.com/partner-center/develop/)中[获取客户的 Azure 利用率记录](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>使用 Microsoft Azure 门户获取虚拟机大小信息

1. 在合作伙伴中心，请参阅 "**客户**" 页。

2. 找到想要购买 Azure VM 预留的客户，然后选择向下箭头以展开客户的信息。 选择 " **Microsoft Azure 管理门户**" 以打开 Azure 门户中的客户记录。

3. 从门户菜单中选择**虚拟机**，然后选择你想要为其购买预订的虚拟机。

4. 在 VM 的详细信息页上，查找大小和区域信息（如下所示），并使用此信息在合作伙伴中心购买预订。  

   :::image type="content" source="images/usage1.png" alt-text="详细信息页上的大小和区域信息":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>使用 Microsoft Azure PowerShell 获取虚拟机大小信息

使用下图中的信息，以获取你想要为其购买预订的虚拟机的位置和大小。 

:::image type="content" source="images/usage2.png" alt-text="VM 位置和大小":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>使用 Azure 资源管理器 (ARM) API 获取虚拟机大小信息

1. 使用 ARMClient 或 ARM API，为你想要为其购买预订的虚拟机调用 ARM 客户端。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 此调用将返回 **vmSize** 和 **location** 的值，如下所示。

    :::image type="content" source="images/usage3.png" alt-text="vmSize 值":::
    :::image type="content" source="images/usage4.png" alt-text="位置值":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>验证 Azure 虚拟机使用情况和预订折扣

代表客户购买 Azure 保留 VM 实例后，预先为 VM 空间付费的折扣将自动应用于与客户预订的属性和数量匹配的虚拟机。

可以通过使用以下方法之一来验证客户的预订使用情况并查看预订折扣应用到的虚拟机：

- Azure 门户
- Azure 使用率 API

每种方法的使用说明如下。

>[!NOTE]
>只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>验证客户在 Microsoft Azure 门户

1. 在合作伙伴中心，请参阅 "**客户**" 页。

2. 查找其预订折扣和使用情况要验证的客户，然后选择向下箭头以展开客户的信息。 选择 " **Microsoft Azure 管理门户**" 以打开 Azure 门户中的客户记录。
3. 从门户菜单中选择**预订**，然后选择想要检查其使用情况的预订。
4. 在 "**概述**" 页上，检查预订的 "使用率" 图，其中显示了已将预订应用到虚拟机的数量。

    >[!NOTE]
    >利用率数据最多可能会延迟 8 小时。

    a. 如果预订的利用率为100%，则您的客户将获得预订购买所能提供的全部费用。
    b. 如果预订的使用量为0%，则不会将折扣应用到任何虚拟机。
    c. 如果预订的使用量介于1% 和99% 之间，则有未使用的权益。

5. 若要避免这种情况，请在进行购买之前确定正确的 VM 以支持客户的计算需求。

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>使用 Azure 使用情况 API 验证客户的预订使用情况

>[!NOTE]
>只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。  

你可以使用 Azure 利用率 API 获取预定利用率数据，以验证客户是否获得了预订折扣并查看折扣应用于的 VM（虚拟机）。 将示例 A 与示例 B 进行比较，以了解如何验证客户的预订使用情况。

:::image type="content" source="images/usage5.png" alt-text="预订使用示例":::

- reservationId 标识用于将折扣应用于虚拟机的 Azure 预定。
- consumptionMeter 是应用了预订折扣的虚拟机的 MeterId。
- 由于应用了预订折扣，ReservationMeter 会显示 0 美元的成本。

有关详细信息，请参阅在[合作伙伴中心 API](https://docs.microsoft.com/partner-center/develop/)中[获取客户的 Azure 利用率记录](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。

>[!IMPORTANT]
>软件（如 Microsoft Windows Server）成本目前未包含在虚拟机预定的价格中，并且在订单记录和发票上显示为单独的行项目。 但是，如果客户拥有 Azure 混合使用权益，则不会应用软件成本。 有关详细信息，请参阅[预留实例中不包含 Windows 软件成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。  

## <a name="azure-reservations-resources"></a>Azure 预订资源

|**有关以下方面的信息**   |**阅读此文**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [销售 Microsoft Azure 虚拟机预留实例](azure-reservations.md)
|在合作伙伴中心为客户购买 Azure 保留   | [购买 Azure 预订](azure-reservations-buying.md)
|管理合作伙伴中心的 Azure 保留 | [管理合作伙伴中心的 Azure 保留](azure-reservations-manage.md)
|在 Azure 门户中购买 Azure 预订 | Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 门户中管理 Azure 预订   | Azure 帮助中的[管理虚拟机预留实例](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)   |
|为客户提供从为他们购买的订阅购买自己的 Azure 预订的权限。 | [授予客户购买自己的 Azure 预订的权限](give-customers-permission.md)   |
