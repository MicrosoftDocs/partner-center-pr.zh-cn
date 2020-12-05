---
title: '从合作伙伴销售连接 (PSC) '
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 Microsoft 合作伙伴如何从合作伙伴销售连接 (PSC) 迁移到合作伙伴中心，以及如何创建或管理 Microsoft 卖方发送的交易。
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/04/2020
ms.openlocfilehash: 5a1b27f108440fc9adfc2cefefd2e4c2bf79ff48
ms.sourcegitcommit: 558533fb39b13aefc3ab2b015145a908f86f8d7d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "96612781"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>合作伙伴中心 (PC) 中的共同销售指南，适用于从合作伙伴销售连接 (PSC 迁移的合作伙伴) 

**相应的角色**

- 帐户管理员
- 引荐管理员
- 合作伙伴销售连接 (PSC) 卖方
-  (PSC) 管理员的合作伙伴销售连接
- 合作伙伴销售连接 (PSC) 交易经理

本文介绍从合作伙伴销售连接到合作伙伴中心的合作伙伴迁移，以便他们能够继续在合作伙伴中心创建和管理共同销售交易。

正如您所知，在2021年3月31日之后，您的公司将失去访问 PSC 的权限。 不过，您仍可以在合作伙伴中心找到要执行的所有操作，例如创建共同销售交易、管理您的交易，以及通过 Microsoft 卖方发送给您的交易。

但会有不同之处。 以下指南可帮助你更顺利、更简单地过渡到合作伙伴中心。

>[!Important]
> 如果你在此处看到有关迁移的关于迁移的横幅，就是正确的位置。 本指南不适用于在 PSC 中管理其交易 (SA) 和 OEM IOT 合作伙伴。

## <a name="before-you-move-things-you-need-to-know"></a>在移动之前，你需要知道

### <a name="if-you-are-a-psc-admin"></a>如果你是 PSC 管理员

- 需要使用工作电子邮件登录到 [合作伙伴中心](https://partner.microsoft.com/)。
- 通过合作伙伴中心 [帐户管理员](permissions-overview.md)的帮助设置你的帐户。
- 阅读本文档，了解如何在合作伙伴中心共同销售。
- 在合作伙伴中心设置用户帐户，使其 (管理员、交易经理和卖方角色的所有 PSC 用户) 并为他们分配 [引用管理员角色](permissions-overview.md)。

>[!IMPORTANT]
> 请确保在 "合作伙伴中心" 中的 "MPN" 位置列表中提供了 PSC 横幅中显示的 MPN ID。

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="显示 PSC 横幅的图像，合作伙伴可在其中找到 MPN ID。":::

 若要验证 MPN ID 是否显示为合作伙伴中心 MPN 位置，请登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)，然后选择 " **设置** " (屏幕右上角的齿轮图标) ，然后选择 " **帐户设置**"。 在第二级的左侧导航菜单中，选择 " **位置** " 以查看与合作伙伴中心帐户关联的所有 MPN id 和位置的列表。

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>如果你是 PSC 交易经理或卖方

- 需要使用工作电子邮件登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。
- 如果你使用的是 PSC 中的非工作帐户，或者你的工作电子邮件与合作伙伴公司的公司不同，请联系你的 PSC 管理员以获取帐户设置帮助。
- 如果你的合作伙伴中心帐户设置完成，而不考虑你用来登录到 PSC 的帐户，请咨询你的 PSC 管理员。
- 验证你是否有权访问 "合作伙伴中心" 和 "引用" 部分。
- 阅读本文档，了解合作伙伴中心的工作流和变化。

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>作为 PSC 的管理员，以下是你的后续步骤

从 "合作伙伴中心" 左侧导航菜单中，选择 " **引用** " 选项。 确认您可以访问 "引用" 页。

  >[!Note]
  > 您可能必须从合作伙伴中心注销并重新登录，以便刷新您的凭据以访问引用页面。

如果在 "合作伙伴中心" 菜单或 "与引用相关的页面" 中看不到 " **引用** " 选项，请联系你的公司的 [全局管理员](permissions-overview.md) ，并请求他们为你授予对 " **引用** " 选项和相关区域的访问权限。 

查找公司的全局管理员：

1. 从 "合作伙伴中心" 仪表板右上角的齿轮图标中选择 " **帐户设置** "。

1. 从二级的左侧导航菜单中选择 " **用户管理** "。 

1. 在用户列表的顶部，选择 " **筛选器** " 下拉菜单。 将选项更改为 **全局管理员**。

   页面将显示所有全局管理员及其各自的电子邮件地址。 通过电子邮件发送其中一项，并要求他们为你的工作帐户分配 "引用管理员" 角色。

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="显示 &quot;合作伙伴设置&quot; 用户管理页中的 &quot;帐户管理员&quot; 的图像。":::

>[!Important]
>- 如果你的角色仅涉及在 PSC 中管理用户，则要求你的公司的全局管理员向你分配合作伙伴中心的 [帐户管理员](permissions-overview.md#manage-mpn-membership-and-your-company) 角色。 
>- 如果你的角色还包括管理共同销售机会，则要求分配有 " [引用管理员](permissions-overview.md#manage-referrals) " 角色。
> - 最好还是在 PSC 管理员中提名一项变更管理线索。 这样做将阻止所有 PSC 管理员必须单独联系到合作伙伴中心帐户管理员。 改为使用合作伙伴中心帐户管理员的主要人员可以使用更改管理线索。

## <a name="user-migration"></a>用户迁移

在合作伙伴中心设置帐户后，使用 "共同销售机会" 页中的 "用户迁移向导" 将合作伙伴中心角色自动分配给公司的员工。

>[!Note]
> 用户迁移只能由公司的 [帐户管理员](permissions-overview.md#manage-mpn-membership-and-your-company) 执行。 如果你没有帐户管理员角色，请使用 "用户迁移向导" 查找可帮助设置用户帐户的帐户管理员。 用户迁移功能将在2020年11月18日开始推出。

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="显示用户迁移向导的映像。":::

帐户管理员将在 "参考指南" 旁边的 "共同销售机会" 页中看到 "PSC 用户迁移向导" 链接。 用户可以通过选择链接启动用户迁移。 若要启动用户迁移，管理员可以选择链接。 它们可以多次执行此用户迁移步骤，直到在合作伙伴中心向所有用户分配了适当的角色。

用户迁移表具有以下详细信息：

- 用户帐户-员工的电子邮件 ID
- PSC 合作伙伴帐户-员工与 PSC 关联的帐户
- PSC 用户角色-在 PSC 中分配给的三个角色之一。
- PC MPN location-用户将获得相关 PC 角色的位置。 PSC 合作伙伴帐户 MPN 用于在伙伴中心查找要分配权限的等效 MPN 位置。 整个组织表示 vOrg MPN ID。
- PC 用户角色-根据用户的 PSC 用户角色为员工分配角色。 PSC 中的管理员将被分配到 PC 中的 "引用管理员" 角色。 卖方将在 PC 中分配 "引用用户" 角色。 若要详细了解 PC 角色以及具有这些角色的用户可在[合作伙伴中心执行](permissions-overview.md#manage-referrals)的操作
- PC AAD 租户-在合作伙伴中心将用户分配到的租户
- 状态-迁移状态有三个可能的状态
    - **未迁移** -用户未分配任何电脑引用角色
    - 已 **迁移**-已成功迁移用户，并已分配相关角色，如下表所示
    - **错误** -由于出现一些错误，无法完成迁移

有时，迁移可能会失败并导致错误。 下面是迁移可能导致错误的几个原因，以及解决此问题的一些方法：

1. PSC 用户可能在使用非工作帐户。

2. PSC 用户使用的帐户可能不同于在合作伙伴中心使用的域。

   若要解决与方案1和2相关的错误，请要求用户使用附加到 Azure AD 租户的工作帐户登录到合作伙伴中心。 [全局管理员](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles)可以帮助。
   
   查找全局管理员： 
   - 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard) ，并选择右上角的齿轮图标中的 " **帐户设置** "。
   - 从二级左侧导航栏中选择 " **用户管理** "。
   - 在用户列表的顶部，选择 " **筛选器** " 下拉菜单，并将选项更改为 " **全局管理员**"。然后，该页将显示所有全局管理员及其各自的电子邮件地址。 要求其中一个用户为你的工作帐户分配 "引用管理员" 角色。
   
      全局管理员可以在 Azure AD 租户中创建新的用户帐户，也可以为来宾用户分配对其他域帐户用户的访问权限。 为所有 PSC 交易经理和用户设置帐户后，他们需要登录到合作伙伴中心，从左侧导航菜单中选择 " **引用** "，然后确认他们可以看到 "引用" 页面。

3. 用户已在合作伙伴中心分配了引用角色。
    - 可以验证用户的现有角色。 在 "合作伙伴中心" 的右上角，选择 " **设置** " (齿轮图标) ，然后选择 " **帐户设置**"。 显示第二个左导航菜单时，请选择 " **用户管理** " 并搜索用户。

完成用户迁移后，请使用以下指南来决定迁移策略：

如果你的公司具有 PDM-当你的合作伙伴中心帐户已设置并且你的用户已移动并拥有角色和权限时，你可以将共同销售活动移动到合作伙伴中心。 通知 PDM 进行切换，而不是等到迁移完成截止时间，这会使所有新交易都流动到合作伙伴中心。

>[!Note]
>一旦您进行了此项切换，您将只能采取 PSC 中现有的活动交易。 您既不能创建新的交易，也不能从 PSC 的 Microsoft 卖方获得任何交易。

如果你的公司没有 PDM，请确保所有用户帐户均已设置并由所有用户进行验证。 当你可以在合作伙伴中心开始共同销售时，会通过电子邮件通知你的相关电子邮件和有关准确日期的版权。 请记住，你仍需要管理 PSC 中现有的活动交易。

>[!Important]
>活动交易不会迁移到 PC。 在2020年12月31日之前，请先关闭并注册交易。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC 管理员、PSC 交易经理和 PSC 卖方的后续步骤

了解如何在合作伙伴中心共同销售。
这是一个重要步骤，可帮助你为合作伙伴中心的共同销售做好准备。 了解合作伙伴中心的工作流和更改，以便有效地共同销售。 首先阅读本文档。 [共同销售体验库](https://aka.ms/cosellexperience)中也提供了一组良好的资源。

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC 和 PC 工作流之间的主要差异

|**方案**|**合作伙伴销售连接**|**合作伙伴中心**|
|-----|:-----|:-----|
|用户角色|PSC 具有管理员、交易经理和卖方角色。|PC 仅具有 [引用管理员](permissions-overview.md#manage-referrals) 角色，该角色提供所有交易的读取和写入权限。|
|邀请 Microsoft 共同销售交易|由 Microsoft 卖方发起，伙伴没有明确的 ask。|如果某个交易需要 Microsoft 卖方帮助，合作伙伴将不得不发出 [显式请求](manage-co-sell-opportunities.md#add-solutions) 。 Microsoft 卖方可以选择拒绝该请求。|
|Expiry|没有交易到期的概念。|如果合作伙伴不接受合作伙伴的入站交易，则该交易将在14天后过期。 对于合作伙伴出站交易，如果 Microsoft 卖方在14天内不执行此操作，则可以将其转入过期状态。|
|Microsoft 卖方详细信息|一旦创建了交易就会立即可见。|仅当卖方明确接受合作伙伴共同销售的邀请时，才会与合作伙伴共享 Microsoft 卖方详细信息。|
|[专用管道](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|不可用。|合作伙伴无需向 Microsoft 卖方提供可见性即可共享其管道。|
|解决方案|仅属于一个价目表的解决方案可以添加到交易中。|合作伙伴可以添加属于以下列表的 [解决方案](manage-co-sell-opportunities.md#add-solutions) 。 a) 自己的解决方案 b) Microsoft 第一方目录的解决方案， (类似于 PSC 中的交易交易角色) 和 c) 来自其他第三方合作伙伴的共同销售解决方案 (类似于 PSC) 中的 ISV 交易角色。|
|交易分配|只有分配的卖方才能查看和处理交易。|团队成员可以添加到交易来指定处理交易的人员，而不会阻止其他引用管理员查看或操作这些交易。|
|客户组织|自由格式的文本输入。|只需键入几个字符，就可以针对[D&B 数据库](https://www.dnb.com/)搜索[customer 组织](manage-co-sell-opportunities.md#select-your-customer)。 合法名称和地址是根据选择自动填充的。|
|客户联系人|不是必需的。|对于专用管道共享，不是必需的。 如果邀请 Microsoft 卖方加入共同销售请求，则需要此项。|
|公共 API|不可用。|用于以编程方式管理合作伙伴中心引用的[公共 API](/partner/develop/referrals) 。|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>将 PSC 中的字段映射到合作伙伴中心中的相应字段

本部分将针对 PSC 显示的 (或 "地图" ) 所选屏幕截图与 "合作伙伴中心共同销售机会" 部分中的相应视图进行比较。

你将在每对屏幕截图上看到数字、黄色或红色圆圈：

- **黄色圆圈的含义是什么？** 编号，每个 PSC 屏幕截图首先显示黄色圆圈。 然后，你将在其下面找到具有多个相同数字的同伴伙伴中心屏幕截图。

   若要查看 PSC 中的每个字段或属性如何映射到合作伙伴中心中的相应字段 例如，匹配第一个中编号为黄色 "1" 的第二个，PSC 屏幕截图指向第二个编号为黄色 "1" 的第二个 "合作伙伴中心" 屏幕截图。

- **红色圆圈的含义是什么？** 如果在一台屏幕截图上看到一个红色圆圈，则表明 PSC 字段在合作伙伴中心不可用。

针对以下领域显示了 PSC 到合作伙伴中心字段映射：

1. 映射到合作伙伴中心联销售商机默认视图的 PSC 主页
1. 已映射到合作伙伴中心交易视图的 PSC 网格视图
1. 已映射到合作伙伴中心交易详细信息视图的 PSC 交易详细信息视图
1. PSC 添加映射到合作伙伴中心的产品视图添加解决方案视图
1. 已映射到合作伙伴中心用户管理视图的 PSC 用户管理视图
1. 已映射到合作伙伴中心角色分配视图的 PSC 用户角色分配视图
1. 已映射到合作伙伴中心通知视图的 PSC 通知视图

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-已映射到合作伙伴中心联销售商机默认视图的 PSC 主页

比较顶级 PSC 屏幕截图和其下的合作伙伴中心屏幕截图之间的匹配、带编号的圆圈。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈表示没有匹配的合作伙伴中心字段。  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="显示合作伙伴销售连接主页与合作伙伴中心的共同销售机会的默认视图之间的字段映射的图像。" lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-被映射到合作伙伴中心交易视图的 PSC 网格视图

比较顶级 PSC 屏幕截图和其下的合作伙伴中心屏幕截图之间的匹配、带编号的圆圈。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈表示没有匹配的合作伙伴中心字段。  

> [!NOTE]
> 屏幕截图下面会出现其他注意事项。

:::image type="content" source="images/pscmigration/gridview.png" alt-text="此图像显示合作伙伴销售连接 (PSC) 网格视图和合作伙伴中心交易视图之间的字段映射。" lightbox="images/pscmigration/grid-view-expanded.png":::

**特别注意事项：**

- 合作伙伴中心中没有列表视图，如 PSC。  所有交易均根据客户信息和交易类型的最近接收日期或创建日期列出。 默认情况下，该视图中的第一个交易为选中状态。 在该交易的详细信息视图中，可在该交易的详细信息视图中找到以 PSC 表格格式显示的大多数值。
- 交易角色不是 PC 中的必填字段。 它不会在任何工作流中显示或捕获。 它基于添加到交易中的解决方案在 Microsoft 卖方端自动派生。
- 上次修改日期不显示在 PC 的 "参考详细信息" 页上。 合作伙伴可以使用排序功能根据上一次更新的日期对交易进行排序。

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-已映射到合作伙伴中心的 PSC 交易详细信息视图

将顶部 (PSC) 屏幕截图的匹配、带编号的圆圈与下面的合作伙伴中心屏幕截图进行比较。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈指示伙伴中心中没有匹配的字段或区域。

> [!NOTE]
> 屏幕截图下面会出现其他注意事项。

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="显示合作伙伴销售连接 (PSC 之间的字段映射的图像) 交易详细信息视图和合作伙伴中心交易详细信息视图。" lightbox="images/pscmigration/deal-details-expanded.png":::

**特别注意事项：**

- 合作伙伴可以通过选择合作伙伴交易详细信息视图 (6) 上的 "编辑" 按钮来编辑交易。 选择 "编辑" 按钮后，所有字段都将变为可编辑状态。 然后，您可以选择保存或取消对交易所做的编辑。
- 在合作伙伴中心，没有用于关闭交易的选项。
- 合作伙伴中心中不提供客户结果。 所有与客户交互相关的详细信息都可以在 PC 的 "说明" 部分中更新。
- 预计解决方案关闭日期仅适用于合作伙伴中心的 OEM IOT 交易。 对于任何其他交易类型，不会显示此信息。
- PC 不需要许可计划。 此信息是根据在交易中选择的解决方案自动推断出来的。

>[!Note]
>标记为赢单或失去损失的任何交易都不能之后编辑。 在将交易移入其中一种终端状态时要格外小心。

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-PSC "添加产品" 视图映射到合作伙伴中心的 "添加解决方案" 视图

将顶部 (PSC) 屏幕截图的匹配、带编号的圆圈与下面的合作伙伴中心屏幕截图进行比较。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈指示伙伴中心中没有匹配的字段或区域。
  
:::image type="content" source="images/pscmigration/products.png" alt-text="显示合作伙伴销售连接 (PSC 之间的字段映射的图像) 添加产品视图和合作伙伴中心添加解决方案视图。" lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-PSC 与合作伙伴中心之间的用户管理

将顶部 (PSC) 屏幕截图的匹配、带编号的圆圈与下面的合作伙伴中心屏幕截图进行比较。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈指示伙伴中心中没有匹配的字段或区域。  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="显示合作伙伴销售连接 () PSC 之间的字段映射的图像 &quot;帐户设置&quot; 区域中的 &quot;用户管理&quot; 主页和 &quot;合作伙伴中心&quot; 用户管理页视图。"  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-PSC 与合作伙伴中心之间的用户角色分配

将顶部 (PSC) 屏幕截图的匹配、带编号的圆圈与下面的合作伙伴中心屏幕截图进行比较。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈指示伙伴中心中没有匹配的字段或区域。  

:::image type="content" source="images/pscmigration/roles.png" alt-text="此图像显示合作伙伴销售连接 (PSC) 角色分配视图和合作伙伴中心角色分配视图之间的字段映射。" lightbox="images/pscmigration/roles-expanded.png":::

**特别注意事项：**

- PSC 管理员的等效角色是合作伙伴中心的帐户管理员角色。
- 合作销售交易管理在合作伙伴中心只有一个角色。 此角色是 "引用管理员" 角色。

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-PSC 与合作伙伴中心的通知

将顶部 (PSC) 屏幕截图的匹配、带编号的圆圈与下面的合作伙伴中心屏幕截图进行比较。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈指示伙伴中心中没有匹配的字段或区域。  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="显示合作伙伴销售连接 (PSC 之间的映射的图像) 通知和合作伙伴中心通知视图。"  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>从 PSC 迁移到合作伙伴中心-常见问题

以下部分回答了有关迁移的常见问题。

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-如果我无权访问合作伙伴中心，我该怎么办？

您可以与 "无法访问" 页上列出的管理员联系，以获取分配的角色。 对于 "引用" 部分下的 "读取" 和 "写入" 权限，你将需要 " [引用管理员](permissions-overview.md#manage-referrals) " 角色。 如果只管理业务配置文件，则需要合作伙伴中心的业务配置文件管理员角色。

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="显示合作伙伴中心的 &quot;无访问体验&quot; 的图像。":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-谁有权访问 "合作伙伴中心" 中的 "引用" 部分？

你的 [帐户管理员](permissions-overview.md#manage-mpn-membership-and-your-company)可以授予你访问 "引用" 选项卡的权限。若要查找全局管理员，请从合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)右上角的齿轮图标中选择 "**帐户设置**"。 然后，从第二层的左侧导航栏中选择 " **用户管理** "。 在用户列表的顶部，选择 " **筛选器** " 下拉菜单，并将选项更改为 " **全局管理员**"。页面将显示所有全局管理员及其各自的电子邮件地址。 要求其中一个用户为你的工作帐户分配 "引用管理员" 角色。

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-对于我们的帐户，"+ 新建交易" 按钮将灰显。 如何开始创建交易？

仅当不存在附加到合作伙伴中心中所使用的 MPN 组织的共同销售准备解决方案时，才会发生这种情况。 联系你的 PDM 以获取你的解决方案的 MPN ID，或创建提及问题的支持票证 "新的交易按钮在 PSC 迁移后灰显。"

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-是否可以将交易分配给我们的组织中的特定人员，如 PSC？

您可以将团队成员分配给特定交易。 它不会阻止其他引用管理员查看或操作这些交易。

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-是否有分配给我的所有交易的视图？

您可以使用 "收藏夹" 功能，它是用户级选项卡。你可以将分配给你的所有交易标记为收藏夹，以快速访问交易。

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-是否有用于交易的只读视图？

不，"引用" 部分中没有任何交易的只读视图。 所有的引用管理员都将对所有交易都具有完全读写访问权限。

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-如何在将交易标记为赢单后进行注册？

如果交易符合以下条件，则会显示一个弹出窗口，用于开始 [交易注册](./register-deals.md)。

- 有一种激励资格解决方案附加到交易。
- Microsoft 卖方邀请参加交易，或邀请参加交易。
- Microsoft 卡处于合作伙伴中心的 "已接受" 或 "赢" 状态。

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-我在交易注册部分选择 "+ 新交易注册" 按钮时收到一条错误消息。 如何注册我的交易？

" **+ 新建交易注册** " 按钮仅由在 ISV connect 计划中注册的合作伙伴使用，用于注册交易，而合作伙伴中心没有相应的共同销售机会。 为了向共同销售机会注册交易，当交易标记为 "赢单" 时，将显示一个弹出窗口，如果该交易符合交易注册条件，则会显示一个弹出窗口。

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-是否强制添加客户组织？

是的，在合作伙伴中心，添加 [客户组织](./manage-co-sell-opportunities.md#select-your-customer) 是必需的。 首先，搜索客户所在位置的位置。 根据所拥有的详细信息，您可以指定具体的建筑物名称，也可以只是给出城市细节。 组织搜索将提取与你输入的名称相匹配的所有法律实体，这样你就不必输入任何地址详细信息。 系统会根据所选组织自动填充所有详细信息。

### <a name="10---are-customer-contact-details-mandatory"></a>10-客户联系详细信息是否是必需的？

取决于要创建的 [交易类型](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) 。 如果你只是共享你的管道，而不需要 Microsoft 销售组织的任何帮助，则可以选择不为客户联系详细信息。 如果你正在积极地从 Microsoft 卖方寻求帮助，你将需要提供客户联系详细信息。 在合作伙伴中心创建共同销售请求之前，你应该获得客户的明确同意。

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-可以添加到交易中的解决方案有多少？

你最多可以添加50个解决方案 (类似于 PSC) 的 "产品"。 与 PSC 不同，你可以将解决方案与你自己共同销售的符合条件的解决方案、Microsoft 第一方 Sku 和其他第三方共同销售的符合条件的解决方案组合在一起。 没有要在合作伙伴中心选择或使用的交易角色。 对于 Microsoft Sku，你可以选择为添加到交易中的每个 SKU 添加数量和价格。

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-在创建交易后，我将如何了解 Microsoft 卖方的详细信息？

只有在与 Microsoft 的相关卖方角色一起创建交易后，才会为 microsoft 卖方分配具体的帮助要求。 即使在分配后，Microsoft 卖方也可以选择接受或拒绝共同销售邀请。 只有卖方接受共同销售邀请时，才会使用 Microsoft 卖方联系详细信息更新交易。 Microsoft 卖方针对交易的 SLA 为14天。 这与合作伙伴在进入过期状态之前应对交易的 SLA 是相同的。

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-在哪里可以找到机会 ID？

PSC 中的机会 ID 与 PC 中的交易 ID 相同。 您可以在打开任何交易时找到交易名称旁边的交易 ID。

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-我的 PDM 如何获取 PC 访问权限？

你的 Pdm 不能直接访问合作伙伴中心，这与 PSC 不同。 有多个选项可用于启用该功能，如下所述。

- OCP Insights-如果 Pdm 只是查看与它们相关的交易和进度，则他们可以使用 OCP Insights 门户获取组织视图。 这是一个内部工具，仅适用于 Pdm。 请注意，不能将 OCP 见解提供给公司的用户。
- 合作伙伴中心的来宾用户-可以 @microsoft.com 在合作伙伴中心添加 PDM 帐户作为来宾用户，并向其分配引用管理员角色，以便他们可以查看和操作引用。
- 在租户中创建 [新用户](./create-user-accounts-and-set-permissions.md#add-a-new-user) -可以在自己的租户中创建新用户，并与 PDM 共享这些详细信息，以便他们可以查看和处理与帐户中的其他引用用户类似的引用。

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>帮助你在合作伙伴中心创建和管理你的交易的资源

如果尚未阅读共同销售帮助主题，可通过以下资源来管理合作伙伴中心的交易。

|**要实现此目的，请执行以下操作**   |**阅读此文**   |
|-----------------------|:-----------------------|
|了解 "共同销售机会" 页中的选项卡和导航|[导航共同销售部分](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|从 D&B 列表选择客户组织 |[选择客户](./manage-co-sell-opportunities.md#select-your-customer)|
|修改 "交易详细信息" 部分中的字段|[交易详细信息](./manage-co-sell-opportunities.md#deal-details)|
|将团队成员添加到交易团队|[添加员工](./manage-co-sell-opportunities.md#add-team-members)|
|响应共同销售交易|[管理共同销售交易](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|注册在合作伙伴中心赢得的交易 |[注册新交易](./register-deals.md)
|获取参考见解并了解你的引用的工作方式 |[引荐见解](./referral-insights.md)
|创建和管理业务配置文件|[管理业务配置文件](./create-a-marketing-profile.md)
|管理业务配置文件的潜在客户 |[管理潜在客户](./manage-leads.md)|

## <a name="next-steps"></a>后续步骤

请遵循以下其他资源：

- [合作伙伴销售连接到合作伙伴中心工作簿](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -工作簿，通过合作伙伴中心与合作伙伴销售连接将合作伙伴的销售流程和角色与新的销售流程进行协调。
- [合作伙伴中心共同销售操作指南](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -通过合作伙伴中心识别运营模型以管理潜在客户或共同销售机会并注册交易的指导。
- [参考管理组](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -直观地说明了如何通过合作伙伴中心管理潜在客户和共同销售机会。
- [在商业 marketplace 中发布和管理](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -直观地说明了如何通过商用 marketplace 中的合作伙伴中心来创建、管理和发布产品/服务。