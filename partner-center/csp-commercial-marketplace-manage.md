---
title: 为客户管理商业 marketplace 产品或产品/服务 |合作伙伴中心
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作伙伴中心，了解云解决方案提供商如何管理从商业市场为客户购买的不同的第三方 ISV 产品。
author: MicheleHope
ms.author: v-mihope
keywords: 订阅，Marketplace，第三方，ISV，SaaS 服务，云解决方案提供商计划，管理产品/服务，管理订阅，许可证，取消订阅，座位，关闭自动续订，间接经销商 MPN ID
ms.localizationpriority: medium
ms.openlocfilehash: 7dbcc978340240175d2c03a5ba1e9312b48d7bdc
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253805"
---
# <a name="manage-commercial-marketplace-products-for-your-customers"></a>为客户管理商业 marketplace 产品

**适用于**

- 合作伙伴中心
- 云解决方案提供商计划中的合作伙伴

**适当的角色**

- 全局管理员
- 管理员代理

云解决方案提供商（CSP）计划中的合作伙伴可以使用合作伙伴中心门户为其客户从商用 marketplace 购买许多 ISV SaaS 产品/服务或订阅。 购买产品/服务后，你可以通过多种方式对其进行管理。

## <a name="view-or-edit-a-subscription"></a>查看或编辑订阅

从第三方 ISV 发布者购买订阅后，可以查看或编辑它，如下所示：

1. 登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard)，然后从左侧导航菜单中选择 "**客户**"。

2. 选择适当的客户，然后选择 "**订阅**"。 这会列出已为客户购买的任何基于许可证的订阅。

3. 在 "**订阅**" 列中，选择要查看或编辑的订阅。 这为你提供了有关设置或设置产品/服务的详细信息。 （如果此产品/服务需要更多操作，你可能还会在 "状态" 列中看到 "需要操作" 状态。 这也可能伴随有 ISV 发布者站点的链接。）

4. 选择要查看或编辑的订阅后，"订阅详细信息" 页允许您编辑订阅和执行以下操作：

    - 更改订阅昵称

    - 在订阅中添加/减少座位数（许可证）

    - 取消订阅

    - “关闭自动续订”

    - 添加间接经销商 MPN ID （如果适用）

> [!NOTE]
> 你可能需要完成 ISV 发布者定义的某些步骤，然后才能对订阅执行某些更改，如取消订阅。

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>分配许可证并代表客户激活订阅

当你购买由商业应用商店中的独立软件供应商（ISV）出版商提供的软件即服务（SaaS）产品/服务（SaaS）产品/服务（SaaS）产品/服务面向.

发布者应为你提供一个个性化链接和一个用于标识特定购买的授权代码。

1. 可以通过以下几种方式在 ISV 发布者那里找到此个性化链接：

    - 你可以看到在购买 ISV SaaS 产品/服务后显示的 "确认" 页的链接。

    - 可以从特定客户的订阅页查看链接。 此发布服务器链接显示在与为客户购买的 ISV 产品或订阅关联的行上。

    - 可以[使用合作伙伴中心 api 检索链接](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)。

2. 一旦你进入 ISV 发布者的站点或系统后，发布者将向你提供完成客户设置过程和预配或分配许可证所需执行的任何其他步骤。

3. 作为代表你的客户的 CSP 程序中的合作伙伴，你需要执行以下任务：

    - 将所有必需的信息提交到发布服务器。

    - 将任何所需 URL 直接发送给你的客户（或以其他方式直接向客户传达有关此订阅的详细信息）

4. 向发布者提供所需的信息后，发布者将设置并分配适当的许可证。 仅在发生以下事件之后，才会开始订阅计费：

    - ISV 发布者已成功分配适当的许可证

    - ISV 发布者已通过单独的 SaaS 履单 API 向 Microsoft 确认了帐户设置已成功完成

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>从 ISV 发布者取消基于许可证的 SaaS 订阅

当你订阅由商业应用商店内的 ISV 发布者提供的基于许可证的 SaaS 产品时，你可以选择在其指定的取消期限内取消订阅。 此取消时间段根据你是具有每月订阅还是年度订阅而发生变化。 你还可以选择是否自动续订订阅。

有关适用的取消期间、如何取消或如何自动续订订阅的详细信息，请参阅：

- [取消订阅](create-a-new-subscription.md#cancel-a-subscription)

- [自动续订商业市场订阅](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>添加或删除 SaaS 订阅的许可证

对于 SaaS 商用 marketplace 产品/服务，可以添加或删除客户订阅的用户许可证。

1. 登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard)，然后从左侧导航菜单中选择 "**客户**"。

2. 选择适当的客户，然后选择 "**订阅**"。 这会列出已为客户购买的任何基于许可证的订阅。

3. 在 "**订阅**" 列中，选择要修改的订阅。

4. 在 "订阅详细信息" 页中，找到 "**数量**" 字段。 这是可以增加或减少许可证数量的位置。

5. 更改数量，然后选择 "**提交**"。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作伙伴中心 API 管理订阅

你还可以使用合作伙伴中心 Api 来执行生命周期管理并管理你的订阅的发票。 有关详细信息，请参阅[为商用 marketplace 产品创建订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。

## <a name="next-steps"></a>后续步骤

- [购买商业市场优惠](csp-commercial-marketplace-purchase.md)
- [了解商用 marketplace 中的计费](csp-commercial-marketplace-billing.md)