---
title: 管理市场产品/服务中的许可
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何设置和管理 ISV 商用 marketplace 产品/服务的许可。
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147949"
---
# <a name="manage-licensing-in-marketplace-offers"></a>管理市场产品/服务中的许可

**适当的角色**：全局管理员 |帐户管理员

本文将指导你完成在合作伙伴中心设置产品/服务的过程，使其可用于 Microsoft AppSource，然后管理该产品的许可证。  

>[!IMPORTANT]
>本文中的功能目前为公共预览版。

## <a name="before-you-begin"></a>准备阶段

### <a name="commercial-marketplace-basics"></a>商业市场基础知识

在开始此过程之前，您应熟悉商业应用商店的基本知识。 下表中的文章将帮助你入门。 

| 主题  | 项目  |
|-------|--------|
|商业市场计划 | [商业市场产品/服务计划和定价](/azure/marketplace/plans-pricing)    |
|商业市场优惠  | [列表类型](/azure/marketplace/determine-your-listing-type)    |
|商业应用商店帐户 |  [在合作伙伴中心创建商业市场帐户](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>确定产品/服务 ID

在下面的过程中，系统将提示你输入产品/服务 ID。 现在请花一些时间来提供合适的产品/服务 ID，请记住以下几点：

- 客户可以在市场产品/服务和 Azure 资源管理器模板的 Web 地址中看到此 ID（若有）。
- 产品 ID 和发布者 ID 的组合长度必须为在 40 个字符以内。
- 只使用小写字母和数字。 产品/服务 ID 可以包括连字符和下划线，但不能包含空格。 例如，如果你的发布者 ID 为 `testpublisherid` ，并且你输入了 `test-offer-1` ，则 "产品/服务" 网址为 `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` 。
- 选择“创建”后，便无法更改此 ID。

### <a name="determine-your-offer-alias"></a>确定提供别名

"产品/服务" 别名是用于 "合作伙伴中心" 中的产品/服务的名称。 还需要遵循以下指导原则的适当提议：

- 此名称没有用于市场，与向客户显示的产品/服务名称和其他值不同。
- 选择“创建”后，便无法更改此名称。

## <a name="create-your-offer"></a>创建产品/服务

授权过程的第一步是创建商业 marketplace 产品/服务。 

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。
2. 在左侧导航菜单中，选择"**商业市场/概述"。**
3. 在"概述"页顶部，选择"新建产品/服务"，然后选择 **"Dynamics 365 for Customer Engagement & PowerApps"。**
4. 输入之前 **创建的"产品** /服务 **ID"和** "产品/服务别名"。
5. 选择“创建”，以生成产品/服务，并继续操作。
6. 选择许可选项。

    - 若要为产品/服务启用许可证管理，请选择 **"通过 Microsoft 启用应用许可证管理"。** 这是一次设置，发布产品/服务后，不能更改此设置。

    - 还可以让客户在没有许可证的情况下运行应用的基本功能，在购买许可证后运行高级功能。 为此，请选择 **"即使未分配许可证，也允许客户安装我的应用"。**

    - 如果不希望产品/服务启用许可证管理，请选择"立即获取 (免费 **) 免费试用"** 或"**与我联系"。** 

## <a name="create-your-plan"></a>创建计划

在这些步骤中，你将定义要为产品/服务启用的计划。

1. 在左侧导航菜单中，选择"**计划概述**"，然后选择"**创建新计划"。**
2. 输入"**计划 ID"** 和 **"计划名称"，** 然后选择"创建 **"。**
3. 在" **计划列表"** 页上，输入 **计划说明**。
4. 若要保存说明并稍后完成，请选择"**保存草稿"。**

5. 完成后，选择"查看并 **发布"。** 计划信息现在将显示在套餐列表 appsource.microsoft.com 套餐列表 (部分下) 。

6. 创建此产品/服务的所有计划后，需要复制每个计划的"服务 ID"。 选择 **"计划** 列表"页顶部的"计划概述"。 将每个计划的服务 ID 复制到安全位置。

## <a name="add-service-ids-to-your-solution"></a>将服务 ID 添加到解决方案

下一步是通过为刚复制的每个计划添加服务 D 来更新解决方案。 有关此的指导，请参阅 [为解决方案 创建 AppSource 包](/powerapps/developer/data-platform/create-package-app-appsource)。

## <a name="upload-your-package-and-publish-your-offer"></a>上传包并发布产品/服务

1. 在左侧导航窗格中，选择"**商业市场"，** 然后选择"**技术配置"。**
2. 在"**基本许可证模型"下**，选择"**用户"。**
3. 在 **"CRM 包**"下，输入包位置的 URL。
4. 使用左侧导航窗格中的其他选项卡输入任何其他必需信息。 完成后，选择"查看并 **发布"。**

发布产品/服务后，我们将查看并验证你的信息。 如果此过程存在任何问题，我们会通知你。 解决所有问题后，你可收到通知，告知产品/服务在 AppSource 中可用。 此时，可以使其上线。

## <a name="make-your-offer-live-in-partner-center"></a>使产品/服务在 合作伙伴中心

以下过程将指导你完成在 AppSource 中启用产品/服务的过程。 若要了解有关此过程的详细信息，请参阅 [列出选项 简介](/azure/marketplace/determine-your-listing-type)。

>[!NOTE]
>发布产品/服务后，需要 4-6 小时才能上台。

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。
2. 在左侧导航菜单中，选择"**商业市场/概述"。**
3. 在 **"概述** "页上，找到要查找的产品/服务。 已准备好发布的产品/服务的状态为"预览 **"。** 选择产品/服务。
4. 在"**产品/服务概述"** 页上，选择"**上一版"。**
产品/服务将在4-6 小时内推出。
5. 若要查看 AppSource 上的产品/服务列表，请选择 "**产品/服务概述**" 页底部的 " **AppSource** " 链接。

    - **对于启用许可证的产品/** 服务：如果你的产品/服务需要许可证检查，则用户将只能通过单击 " **与我联系**" 来输入潜在客户，以便可以与他们进行通信。

    - **对于启用许可证的产品/服务免费安装选项**：如果产品/服务不需要许可证检查，则除了 **与我联系**，管理员用户还将看到 "**立即获取**" 按钮。 如果用户想要尝试 "免费安装" 选项，则应单击 " **立即获取**"，这会使用户在 Power Platform 管理中心上安装产品/服务。 如果用户有任何疑问，或者他们想要升级到付费计划，用户仍然可以使用 " **联系我** "。

## <a name="register-isv-connect-deal-in-deal-registration"></a>注册 ISV Connect 交易交易注册

在将许可证分配给客户之前，需要在合作伙伴中心注册每个销售。 为此，请参阅 [注册交易](register-deals.md)。

## <a name="invite-the-customer"></a>邀请客户

使用以下过程邀请客户参与此交易。  

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。
2. 在左侧导航菜单中，选择 " **商业 Marketplace/概述**"。
3. 在左侧导航菜单中，选择 " **引用**"，然后选择 " **交易注册**"。
4. 筛选 **提交** 的交易，选择 " **正在进行** " 选项卡，然后选择所需的交易。
5. 在此交易的 "概述" 页上，选择 " **管理许可证**"。
6. 在 " **管理许可证** " 窗口中，从 " **客户详细信息** " 下拉列表中选择客户。 如果客户关系尚不存在，请选择 " **+ 邀请新客户同意**"。
7. 复制显示的链接。
8. 通过电子邮件将此链接发送到客户的帐单管理员或全局管理员，并让他们使用此链接访问 admin.microsoft.com，并接受并授权您正在建立的关系。

    >[!NOTE]
    >在客户执行此步骤之前，将不会建立关系。

## <a name="activate-manage-and-remove-your-licenses"></a>激活、管理和删除许可证

客户获得与关系的授权后，可以开始从产品/服务添加计划，并将许可证分配给每个计划。

1. 在"管理此交易的许可"窗口中，选择 **"+添加计划"。**
2. 完成"**此解决方案的计划"和****"许可证数量**"字段，然后选择"**更新许可证"。** 这些许可证将在 admin.microsoft.com 供客户管理和分配给员工。

    - 若要更改现有计划的许可证数，请在"许可证数"字段中输入新 **编号，然后选择**"**更新许可证"。**

    - 若要停用或删除交易许可证，请在"操作"字段中选择垃圾桶图标，然后选择"更新 **许可证"。**

## <a name="next-steps"></a>后续步骤

[许可资源](support-resources-licensing.md)