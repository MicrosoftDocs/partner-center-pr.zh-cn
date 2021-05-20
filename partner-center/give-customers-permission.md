---
title: 让客户在 CSP 中购买自己的服务
description: 了解 CSP 计划合作伙伴如何让客户购买自己的服务（例如 Azure 预留）来购买在 合作伙伴中心。
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150754"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>授予客户合作伙伴中心购买自己的产品或服务的权限

**适当的角色**：管理员代理|销售代理

本文介绍云解决方案提供商云解决方案提供商 (合作伙伴) 如何授予客户购买自己的一些服务或资源的权限。

CSP 计划的合作伙伴通常使用 合作伙伴中心及其商业市场为客户购买解决方案和服务。 然后，合作伙伴允许某些客户直接从客户Azure 门户。

下面是一个示例。 假设你为 合作伙伴中心 中的客户购买 Azure 计划合作伙伴中心。 然后，你决定代表客户将其他资源或服务添加到该订阅。 在这种情况下，可以将 Azure 预留添加到客户的订阅 (例如，将虚拟机预留实例添加到) 。 然后，可以允许客户在门户中进一步预配 Azure 预留Azure 门户。

现在，使用 **"客户权限** "功能，可以为客户提供更多 Azure 资源的自助服务选项。 通过为客户启用权限，可以让客户购买自己的资源，例如 (购买自己的 Azure 预留) 。  

## <a name="overview-of-customer-permissions-in-partner-center"></a>客户权限概述合作伙伴中心

使用" **客户帐户** "页可以启用 (或关闭) 权限。 目前，此功能支持：

- **Azure 预留：** 启用此权限后，客户可以购买自己为特定 Azure 订阅购买的 Azure 预留。

在启用客户权限之前，请注意以下要点：

- 默认情况下，客户权限在 (中) 自动合作伙伴中心。

- 你必须在合作伙伴中心为你分配 "管理员代理" 角色，然后才能打开 (或关闭客户的) 权限。

  分配有 "销售代理" 或 "技术支持" 代理角色的合作伙伴具有只读访问权限，并且不能打开或关闭客户权限。

- 您可以打开 (为您选择的任何客户启用) 权限。

- 你可以使用合作伙伴中心仪表板或 [合作伙伴中心 api](/partner-center/develop/manage-customers)打开 (或关闭) 客户权限。

- 开启 (为特定客户启用) 权限后，你将负责为该客户所进行的任何后续购买付费。 如果客户想要交换、取消或续订已 (的购买，或者他们想要更改预订) 的初始范围，他们将不能这样做。 他们需要询问你，作为合作伙伴，帮助他们交换、取消和续订购买，或在以后对预订范围做出更改。  

- 为特定客户启用权限后，你将 **不** 会收到客户对你的任何以后购买的通知。

- 以后购买的客户将显示在合作伙伴中心，以及你所做的任何购买。 您可以在客户的 **订单历史记录** 页、其 **预订** 页或 [**活动日志**](activity-logs.md)中找到这些购买内容。

>[!NOTE]
> 有关客户将支付的价格以及如何帮助客户管理其购买的信息，请参阅 [帮助客户管理他们购买的预订](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>授予客户购买自己的 Azure 预订的权限

Azure 预订是以折扣价购买 Azure 服务的一种绝佳方式。 若要详细了解 Azure 保留项的优点，请参阅 [什么是 Azure 保留？](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

现在，你可以选择代表你的客户购买 Azure 预订，因为你可能已经做了。 或者，你可以授予客户购买自己的 Azure 预订的权限。

>[!NOTE]
> 向客户授予购买自己的 Azure 预订的权限后，可帮助他们管理他们购买的任何预订。 有关详细信息，请参阅帮助 [客户管理他们购买的预留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>使客户能够购买自己的 Azure 预留

1. 验证客户是否拥有你代表他们购买的现有 Azure 计划或 Azure 全局订阅。

2. 验证是否为客户分配了 **此订阅的** "所有者"角色。

3. 启用客户权限 (开启此功能 **)** 购买自己的 Azure 预留。

每个步骤如下所示。

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>验证客户是否具有现有的 Azure 订阅

在授予客户购买自己的 Azure 预留项的权限之前，必须验证客户是否具有现有的 Azure 计划或 Azure 全球订阅。 如果客户在订阅中未显示当前 Azure 合作伙伴中心，则必须在启用其客户权限之前为这些用户购买订阅。

- 若要了解客户是否已有 Azure 订阅，请登录到 合作伙伴中心 仪表板，然后选择 **"CSP"，** 然后选择"**客户"。** 从列表中选择特定客户。 然后选择 **"订阅** "，然后查找 Azure 计划或 Azure Global 的任何基于使用情况的订阅。

- 如果客户没有现有的 Azure 订阅，可以购买其订阅。 请参阅 [购买 Azure 计划](purchase-azure-plan.md)。

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>验证客户在 Azure 中是否分配了正确的角色

验证客户是否具有现有的 Azure 订阅后，还需要验证是否为与客户关联的密钥用户分配了该 Azure 订阅的正确所有者角色。  这是基于角色的访问 (RBAC) 客户需要为购买的 Azure 订阅购买 Azure 预留。

某些合作伙伴可能已经将"所有者"角色分配给想要主动管理和预配自己的 Azure 资源的客户。 如果已 **为客户分配"** 所有者"状态来管理之前为其购买的订阅，可以跳过此步骤。  

> [!IMPORTANT]
> 如果尚未为某个客户分配 " **所有者** " 角色，则他们将收到一个错误，Azure 门户阻止他们购买 Azure 预订。

若要验证是否已为客户分配 Azure 订阅的 **所有者** 角色，请执行以下操作：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 依次选择 " **CSP**"、" **客户** " 和 "特定客户"。

3. 选择该客户的 **订阅** ，并找到特定的 Azure 订阅。

4. 选择该客户的订阅旁边的 " **管理** " 按钮。 这样做会打开 [Azure 门户](https://portal.azure.com/)。

5. 若要将 **所有者** 角色分配给特定用户，请按照以下步骤将 [用户分配为管理员](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>启用或禁用客户权限以购买自己的 Azure 保留

验证客户是否有现有的 Azure 订阅，并为用户分配了该订阅的 **所有者** 角色后，便可以打开 (启用) 客户权限。 你还可以使用这些步骤关闭 (禁用) 客户权限。 你可以使用合作伙伴中心仪表板或 [合作伙伴中心 api](/partner-center/develop/manage-customers)启用或禁用客户权限。

若要打开 (或关闭合作伙伴中心) 客户权限：

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 从左侧导航菜单中，依次选择 " **CSP**"、" **客户**"。 此时将显示客户列表。

3. 选择特定的客户名称。

4. 从 "客户" 菜单中选择 " **帐户** "。 此时会显示 "客户 **帐户** " 页。

5. 查找页面底部的 " **客户权限** " 区域。

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="客户权限帐户页。" border="true":::

6. 在 " **Azure 保留**" 下，找到 " **允许客户购买** " 选项。

7. 若要启用客户权限，请将此选项旁的开关移到 " **开** " 位置。 若要关闭客户权限，请将开关移到 " **关闭** " 位置。

>[!NOTE]
> 若要了解当你打开客户的权限来购买自己的 Azure 预订时，还会发生什么情况，请参阅 [合作伙伴中心的客户权限概述](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。
>
>打开 (或关闭) 客户权限时，活动日志会记录每个操作。 从 "合作伙伴中心" 仪表板) 顶部选择齿轮图标时， (可以访问此日志。 当你打开或关闭客户权限时，该操作将在活动日志中显示为 " **创建客户购买权限** " 或 " **删除客户购买权限** "。

## <a name="help-customers-manage-reservations-they-purchase"></a>帮助客户管理他们购买的预订

一旦你向客户提供购买其自己的 Azure 预订的权限，你就可以帮助他们更好地管理他们购买的任何资源。 客户可以直接从 [Azure 门户](https://portal.azure.com/)管理 Azure 预订的许多方面。 他们将需要你的帮助来管理他们在 CSP 订阅中购买的 Azure 保留部分的其他方面。  

帮助客户更详细地了解如何管理 Azure 预订的这些方面：

- 价格客户将支付 Azure 预订费用
- 客户如何优化 Azure 预订的使用
- 当客户购买具有共享作用域的预留时，会发生什么情况？
- 如果客户想要更改、取消和续订预订，或更改其作用域，会发生什么情况？

**价格客户将为其预留付费。** 你的客户将根据你先前为 CSP 合作伙伴计费帐户购买的订阅购买 Azure 预订。 客户根据此订阅购买的任何 Azure 预订的价格也由您设置。 此价格可能与客户在 Azure 门户中看到的 Web 直接价格不同。

**客户如何优化预订的使用。** 一些客户可能会从详细了解如何优化预留的使用或在购买期间分配预留的初始范围中获益。 有关详细信息，请让客户阅读 [管理 Azure 资源的预留](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。

**客户购买具有共享范围的预留时会发生什么情况？** 当客户基于以前的 CSP 订阅购买预留并将共享范围分配给该预留时，CSP 提供的任何折扣将应用于 CSP 合作伙伴为客户购买的所有订阅的匹配使用情况。

**如果客户想要交换、取消或续订已购买的购买，或更改预留的初始范围，应该怎么办？** 客户需要请求其合作伙伴帮助他们更改预留的初始范围。 他们还需要合作伙伴的帮助来交换、取消或续订预留。 他们无法根据 CSP 合作伙伴为它们购买的订阅，使用预留自行执行这些任务。

## <a name="next-steps"></a>后续步骤

- [代表客户购买 Azure 预留](azure-reservations-buying.md)

- [合作伙伴中心 - 销售 Microsoft 预留](azure-reservations.md)

- [代表客户管理 Azure 预订](azure-reservations-manage.md)