---
title: '& 产品/服务管理 marketplace 产品'
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作伙伴中心，了解云解决方案提供商可以如何管理从商业市场为客户购买的第三方 ISV 产品/服务。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147898"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>为客户管理商业 marketplace 产品和产品/服务


**适当的角色**：全局管理员 |管理代理

云解决方案提供商中的合作伙伴 (CSP) 计划可以使用合作伙伴中心门户为其客户从商用 marketplace 购买许多 ISV SaaS 产品/服务或订阅。 购买产品/服务后，你可以通过多种方式对其进行管理。

## <a name="view-or-edit-a-subscription"></a>查看或编辑订阅

从第三方 ISV 发布者购买订阅后，可以查看或编辑它，如下所示：

1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)，然后从左侧导航菜单中选择 " **客户** "。

2. 选择适当的客户，然后选择 " **订阅**"。 这会列出已为客户购买的任何基于许可证的订阅。

3. 在 " **订阅** " 列中，选择要查看或编辑的订阅。 这为你提供了有关设置或设置产品/服务的详细信息。  (如果此产品/服务需要更多操作，还可能会看到 "状态" 列中显示 "需要操作" 状态。 这还可能附带了 ISV 发布者站点的链接。 ) 

4. 选择要查看或编辑的订阅后，"订阅详细信息" 页允许您编辑订阅和执行以下操作：

    - 更改订阅昵称

    - 添加/减少订阅中的许可证数量

    - 取消订阅

    - “关闭自动续订”

    - 添加间接经销商 MPN ID （如果适用）

> [!NOTE]
> 你可能需要完成 ISV 发布者定义的某些步骤，然后才能对订阅执行某些更改，如取消订阅。

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>代表客户分配许可证并激活订阅

在商业市场中购买独立软件供应商 (ISV) 发布者提供的软件即服务 (SaaS) 产品/服务时，ISV 发布者可帮助管理代表客户分配许可证和激活订阅的过程。

发布者应提供个性化链接和用于标识特定购买的授权代码。

1. 可以通过多种方式从 ISV 发布者找到此个性化链接：

   - 可以从购买 ISV SaaS 产品/服务后出现的确认页中查看链接。 若要在页面上找到此链接，请查找并选择"**转到发布者的站点"。**

   - 可以从特定客户的"订阅"页查看链接。 此发布者链接显示在与客户购买的 ISV 产品/服务或订阅关联的行上。

   - 可以使用 [API 检索合作伙伴中心链接](/partner-center/develop/get-activation-link-by-order-line-item)。

   > [!NOTE]
   > 若要代表客户执行此操作，可能需要复制个性化链接，将其粘贴到专用浏览器，然后输入客户的凭据。

2. 进入 ISV 发布者的站点或系统后，发布者将告知你完成客户安装过程以及预配或分配许可证所需的任何其他步骤。

3. 作为代表客户工作的 CSP 计划的合作伙伴，你负责执行以下任务：

    - 将任何必需信息提交到发布者。

    - 将任何所需的 URL 直接发送到 (或直接将有关此订阅的详细信息传达给客户) 

4. 向发布者提供所需信息后，发布者将预配和分配相应的许可证。 只有在发生以下事件后，订阅计费才开始：

    - ISV 发布者已成功分配适当的许可证

    - ISV 发布者已通过单独的 SaaS 履单 API 确认了 Microsoft (，) 帐户设置已成功完成

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>从 ISV 发布者取消基于许可证的 SaaS 订阅

当你订阅由商业应用商店内的 ISV 发布者提供的基于许可证的 SaaS 产品时，你可以选择在其指定的取消期限内取消订阅。 此取消时间段根据你是具有每月订阅还是年度订阅而发生变化。 也可选择是否自动续订订阅。

有关适用的取消期间、如何取消或如何自动续订订阅的详细信息，请参阅：

- [取消订阅](create-a-new-subscription.md#cancel-a-subscription)

- [自动续订商业市场订阅](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>添加或删除 SaaS 订阅的许可证

对于 SaaS 商用 marketplace 产品/服务，可以添加或删除客户订阅的用户许可证。

1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)，然后从左侧导航菜单中选择 " **客户** "。

2. 选择适当的客户，然后选择 " **订阅**"。 这会列出已为客户购买的任何基于许可证的订阅。

3. 在 " **订阅** " 列中，选择要修改的订阅。

4. 在 "订阅详细信息" 页中，找到 " **数量** " 字段。 这是可以增加或减少许可证数量的位置。

5. 更改数量，然后选择 " **提交**"。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作伙伴中心 API 管理订阅

你还可以使用合作伙伴中心 Api 来执行生命周期管理并管理你的订阅的发票。 有关详细信息，请参阅 [为商用 marketplace 产品创建订阅](/partner-center/develop/create-subscription-azure-marketplace-products)。

## <a name="next-steps"></a>后续步骤

- [购买商业市场优惠](csp-commercial-marketplace-purchase.md)
- [了解商用 marketplace 中的计费](csp-commercial-marketplace-billing.md)