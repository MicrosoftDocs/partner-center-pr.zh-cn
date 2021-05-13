---
title: '从合作伙伴销售 Connect (PSC) '
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 Microsoft 合作伙伴如何从合作伙伴销售 Connect (PSC) 迁移到合作伙伴中心创建或管理 Microsoft 销售人员发送的交易。
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 584f8a7f2794cb64be49fe7f790904eff50c4c26
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855092"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>从合作伙伴销售 Connect 合作伙伴中心 (PSC) 迁移的合作伙伴在 合作伙伴中心 (PC (销售) 

**适当角色**：帐户管理员|引荐管理员|合作伙伴销售 (PSC) 卖方|合作伙伴销售 (PSC) 管理员|合作伙伴销售 (PSC) 交易经理

本文指导合作伙伴从 Partner Sales Connect 迁移到 合作伙伴中心以便他们可以继续在 合作伙伴中心 中创建和管理联合销售合作伙伴中心。

>[!Note]
> 如果因为在 PSC 中看到了有关迁移的横幅而在此处，则你的位置正确。 本指南不适用于在 PSC 中管理 (SA) 和 OEM 许可业务合作伙伴的解决方案评估。

>[!Important]
> 从 2021 年 4 月 1 日起，你的公司将无法在 PSC 中创建或编辑交易。 **仍可以使用 PSC 中的批量导出功能下载现有交易数据。还可以在此 [日期之后将未](psc-to-pc.md#psc-deals-migration) 合作伙伴中心交易从 PSC 迁移到另一个。** <br><br> 如果你正在积极处理包含 IP 联合销售奖励合格解决方案的交易，则有两种选择： <br><br> 1.将交易标记为"已赢得"，在 2021 年 3 月 31 日之前在 PSC 中完成交易注册。 <br> 2. [将](psc-to-pc.md#psc-deals-migration) 交易迁移到合作伙伴中心，以便你有更多的时间来处理交易并开始交易注册。

如你所知， **公司将在 2021** 年 4 月 30 日之后失去对 PSC 的访问权限。 但是，你仍然会发现你想要在 合作伙伴中心 中执行的所有工作，例如创建联合销售交易、管理交易，以及处理 Microsoft 销售人员发送给你的交易。

但是，存在差异。 以下指南可帮助你更顺畅合作伙伴中心更直接地转换。

## <a name="before-you-move-things-you-need-to-know"></a>在移动之前，需要知道的一些内容

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

如果在"合作伙伴中心"菜单或"引荐"相关页上看不到"引荐"选项，请联系公司的帐户管理员，并请求他们授予你[](permissions-overview.md)访问"引荐"选项和相关区域的访问权限。 

查找公司的帐户管理员：

1. 从 **仪表板** 右上角的齿轮图标中选择"帐户合作伙伴中心设置。

1. 从 **左侧导航** 菜单中选择"用户管理"。

1. 在用户列表顶部，选择" **筛选器** "下拉菜单。 将 选项更改为"**帐户管理员"。**

   页面将显示所有帐户管理员及其各自的电子邮件地址。 通过电子邮件发送其中一个帐户，并要求他们为工作帐户分配引荐管理员角色。

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="显示合作伙伴设置用户管理页中的帐户管理员的图像。":::

>[!Important]
>- 如果角色仅涉及在 PSC 中管理用户，请要求公司的帐户管理员在 PSC[](permissions-overview.md#manage-mpn-membership-and-your-company)中分配帐户管理员合作伙伴中心。 
>- 如果你的角色还包括管理联合销售机会，请要求分配引 [荐管理员](permissions-overview.md#manage-referrals) 角色。
> - 建议同时在 PSC 管理员中指定一个变更管理主管。 这样做将阻止所有 PSC 管理员单独联系合作伙伴中心管理员。 然后，变更管理主管可以是与帐户管理员合作伙伴中心的主要人员。

## <a name="user-migration"></a>用户迁移

在 合作伙伴中心 中设置帐户后，使用联合销售机会页中的用户迁移向导自动将合作伙伴中心分配给公司的员工。

>[!Note]
> 用户迁移只能由公司 [的帐户](permissions-overview.md#manage-mpn-membership-and-your-company) 管理员执行。 如果你没有帐户管理员角色，请找到一个帐户管理员，该管理员可以在用户迁移向导的帮助下帮助设置用户帐户。

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="显示用户迁移向导的图像。":::

帐户管理员将在引荐指南旁边的联合销售机会页中看到 PSC 用户迁移向导链接。 用户可以通过选择链接启动用户迁移。 若要启动用户迁移，管理员可以选择链接。 它们可以多次执行此用户迁移步骤，直到在合作伙伴中心向所有用户分配了适当的角色。

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

有时，迁移可能会失败并导致错误。 下面是迁移可能导致错误的一些原因以及解决此问题的一些方法：

1. PSC 用户可能正在使用非工作帐户。

2. PSC 用户可能正在使用域中的帐户，该帐户不同于在 合作伙伴中心。

   若要解决与方案 1 和方案 2 相关的错误，请要求用户使用附加到 合作伙伴中心 租户的工作帐户Azure AD登录。 全局 [管理员可以](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) 提供帮助。
   
   查找全局管理员： 
   - 登录到仪表板合作伙伴中心，然后从[](https://partner.microsoft.com/dashboard)右上角的齿轮图标中选择"帐户设置"。
   - 从 **左侧** 导航栏的第二级中选择"用户管理"。
   - 在用户列表顶部，选择"筛选器"下拉菜单，将选项更改为"全局 **管理员"。** 然后，该页面将显示所有全局管理员及其各自的电子邮件地址。 要求其中一个为工作帐户分配引荐管理员角色。
   
      全局管理员可以在租户中创建新的用户帐户Azure AD或将来宾用户访问权限分配给其他域帐户用户。 为所有 PSC 交易经理和用户设置帐户后，他们需要登录到 合作伙伴中心，从左侧导航菜单中选择"引荐"，并确认他们可以看到"引荐"页。 

3. 用户已在 合作伙伴中心 中分配了引荐合作伙伴中心。
    - 可以验证用户的现有角色。 在 合作伙伴中心 右上角，选择"设置 (齿轮图标) ，然后选择"帐户 **设置"。**  看到第二个左侧导航菜单时，选择" **用户管理** "并搜索用户。

## <a name="psc-deals-migration"></a>PSC Deals 迁移

完成用户迁移后，使用联合销售机会页中的交易迁移向导，将 PSC 的所有符合条件的开放式交易引入电脑。 **"交易迁移"链接将仅在"客户"中显示具有整个组织范围的引荐合作伙伴中心。** "共同销售机会" 页的右上方会出现名为 **"PSC 交易迁移"** 的链接，这将打开 "交易迁移向导"。

在开始交易迁移之前，请阅读本部分。

**符合迁移条件**

只有某些交易有资格从 PSC 迁移到 PC。 此迁移向导旨在帮助合作伙伴将自己的交易带入合作伙伴中心，在这种情况下，他们仍会积极地与客户合作来完成交易。 **仅从2020年1月1日创建的处于打开状态的交易，具有有效的合作伙伴帐户详细信息 (有效的 MPN ID) 并且未进行交易注册有资格进行迁移。**

**不符合迁移条件**

- 解决方案评估交易不适用于交易迁移
- OEM 授权业务交易不适用于交易迁移
- 在 PSC 中被标记为 "赢单" 的任何交易都不符合迁移条件。 如果有资格在 PSC 中完成标记为 "赢单" 的交易，则进行交易登记。

## <a name="pre-requisites-for-deal-migration"></a>交易迁移的先决条件

在开始从电脑进行交易之前，请按照以下说明设置 PSC 中用于成功迁移的交易。

1. 公司中处理开放式交易的所有销售团队成员都会收到有关此迁移的信息。
2. 销售团队成员训练有素地使用合作伙伴中心进行交易管理。
3. 交易包含如下所述的所有必需信息。
    - 客户公司详细信息，包括名称和地址
    - 如果是共同销售交易，则为客户联系详细信息
    - 至少一个解决方案
    - 至少一个具有所有详细信息-名字、姓氏、电子邮件 ID 和电话号码的团队成员
    - 交易值
    - 估计的交易关闭日期
    - 合作伙伴说明

可以使用 PSC 中的批量下载和上传功能，在所有符合条件的交易中添加交易中缺少的所有详细信息。

>[!Note]
> 即使未满足上述先决条件，交易迁移也会成功。 但是，如果上述任何必填字段在 合作伙伴中心不可用，则无法更改交易状态。 然后，必须输入交易中缺少的所有必需信息合作伙伴中心开始处理这些信息。 **强烈建议在 PSC 中清理符合条件的交易，然后再将它们迁移到合作伙伴中心。**

合作伙伴中心中的交易迁移构建为一键式体验。 只需在公司准备好迁移符合条件的交易后，单击"迁移交易"按钮即可。 **无法选择要从 PSC 迁移的交易。如果不希望将任何交易迁移到 合作伙伴中心，在开始迁移之前，请将它们移到 PSC 中的已关闭状态。**

>[!Note]
> 启动迁移后 **，最多可能需要 24** 小时才能迁移交易。

迁移完成后，横幅消息的状态将更改为完成，并包含指向迁移报告的链接。 下载报表以查看从 PSC 迁移到电脑的交易的详细信息。

该报表包含以下详细信息。

1. **合作伙伴中心 ID** - 合作伙伴中心中所有交易的唯一标识符。 有两个交易 - 一个交易针对合作伙伴，另一个交易适用于 Microsoft，共同销售合作伙伴中心。
2. **合作伙伴中心 ID** - 合作伙伴中心合作伙伴的交易的唯一标识符。
3. **交易名称** - PSC 中为交易给定的标识符。
4. **PSC 交易 ID** - PSC 中交易的唯一标识符。
5. **错误** -指示在迁移特定交易时是否出现任何错误。

已成功迁移的所有交易在 PSC 中都不可见。 您可以继续处理 PC 中的已迁移交易，包括完成交易注册。 对于共同销售交易，不会更改与 Microsoft 卖方的交互。

从 PSC 迁移的交易将基于交易来源在入站和出站选项卡中提供。 公司共享的所有交易都将在 "出站" 选项卡中提供，Microsoft 启动的交易将在合作伙伴中心的 "入站" 选项卡中提供。 迁移后将创建两种类型的交易。

1. **共同销售的交易** -在 PSC 中标记为共同销售的交易将创建为合作伙伴中心的共同销售交易。
2. **合作伙伴打头阵的交易** -未标记为共同销售的交易将创建为合作伙伴中心的伙伴 led 交易。 以合作伙伴为主导的交易对 Microsoft 卖方可见，并可升级到在到达终端状态 (赢得、丢失) 之前共同销售交易。 此外，如果交易中有符合激励条件的解决方案，则合作伙伴 led 的交易将符合交易注册条件。

>[!Important]
> 如果由于某些交易无法迁移而导致某些错误， **可以通过单击 "迁移交易" 按钮来重新启动交易迁移**。 仅当有一些合格的交易有待迁移时，才会启用此功能。 如果你处于转换阶段，在此阶段中，在开始进行交易迁移后，某些新交易会在 PSC 中创建。

成功迁移所有交易后，会显示 **"不进行迁移"** 的横幅，其中 **"迁移交易"** 按钮 **处于禁用状态**。

完成用户迁移和/或交易迁移后，请使用以下指南来决定迁移策略：

如果你的公司有合作伙伴开发经理 (PDM) - 设置 合作伙伴中心 帐户并且用户已迁移并拥有角色和权限时，可以将联合销售活动移到 合作伙伴中心。 通知 PDM 进行切换，而不是等到迁移完成截止时间，这将使所有新交易流入合作伙伴中心。

>[!Note]
>进行此切换后，你只能处理 PSC 中的现有活动交易。 在 PSC 中，既无法创建新交易，也无法从 Microsoft 卖方处收到任何交易。

如果你的公司没有 PDM - 请确保所有用户都设置并验证所有用户帐户。 PSC 中会通过电子邮件和横幅通知你何时可以开始联合销售合作伙伴中心。 请记住，你仍必须管理 PSC 中的现有活动交易。

>[!Important]
> 在 2021 年 4 月 30 日之前，你才能注册标记为"获胜"的交易。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC 管理员、PSC 交易经理和 PSC 销售人员的下一步步骤

了解如何在联合销售合作伙伴中心。
这是一个重要步骤，可帮助你准备好在 合作伙伴中心。 了解工作流和合作伙伴中心更改，以便可以有效地进行联合销售。 首先，请完全阅读本文档。 联合销售体验库中也提供了 [一组很好的资源](https://aka.ms/cosellexperience)。

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC 和 PC 工作流之间的主要差异

|**方案**|**合作伙伴销售连接**|**合作伙伴中心**|
|-----|:-----|:-----|
|用户角色|PSC 具有管理员、交易经理和卖家角色。|电脑只有 [引荐管理员](permissions-overview.md#manage-referrals) 角色，该角色授予所有交易读取和写入权限。|
|邀请 Microsoft 进行联合销售交易|由 Microsoft 卖方发起，合作伙伴没有明确的请求。|如果某个交易需要 Microsoft 卖方帮助，合作伙伴将不得不发出 [显式请求](manage-co-sell-opportunities.md#add-solutions) 。 Microsoft 卖方可以选择拒绝该请求。|
|Expiry|没有交易到期的概念。|如果合作伙伴不接受合作伙伴的入站交易，则该交易将在14天后过期。 对于合作伙伴出站交易，如果 Microsoft 卖方在14天内不执行此操作，则可以将其转入过期状态。|
|Microsoft 卖方详细信息|一旦创建了交易就会立即可见。|仅当卖方明确接受合作伙伴共同销售的邀请时，才会与合作伙伴共享 Microsoft 卖方详细信息。|
|[专用管道](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|不可用。|合作伙伴无需向 Microsoft 卖方提供可见性即可共享其管道。|
|解决方案|仅属于一个价目表的解决方案可以添加到交易中。|合作伙伴可以添加属于以下列表的 [解决方案](manage-co-sell-opportunities.md#add-solutions) 。 a) 自己的解决方案 b) Microsoft 第一方目录的解决方案， (类似于 PSC 中的交易交易角色) 和 c) 来自其他第三方合作伙伴的共同销售解决方案 (类似于 PSC) 中的 ISV 交易角色。|
|交易分配|只有分配的卖方才能查看和处理交易。|团队成员可以添加到交易来指定处理交易的人员，而不会阻止其他引用管理员查看或操作这些交易。|
|客户组织|自由格式的文本输入。|只需键入几个字符，就可以针对[D&B 数据库](https://www.dnb.com/)搜索[customer 组织](manage-co-sell-opportunities.md#select-your-customer)。 合法名称和地址是根据选择自动填充的。|
|客户联系人|不是必需的。|对于专用管道共享，不是必需的。 如果邀请 Microsoft 卖方参与联合销售请求，则是必需的。|
|公共 API|不可用。|[以编程](/partner/develop/referrals) 方式管理引荐合作伙伴中心 API。|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>将 PSC 中的字段映射到 PSC 中的相应合作伙伴中心

本部分将 (PSC ) 的所选屏幕截图与"联合销售机会"部分中的相应合作伙伴中心视图进行比较。

每对屏幕截图上都会显示编号、黄色或红色圆圈：

- **黄色圆圈是什么意思？** 编号的黄色圆圈首先显示在每个 PSC 屏幕截图上。 然后，你将找到一个合作伙伴中心屏幕截图，其中显示了许多相同的数字。

   若要了解 PSC 中每个字段或属性如何映射到 合作伙伴中心 中的对应字段或属性，请同时匹配两个相关屏幕截图中的带编号的圆圈。 例如，将第一个编号的黄色"1"匹配，PSC 屏幕截图与第二个屏幕截图中的编号黄色"1"匹配，合作伙伴中心下面的屏幕截图。

- **红色圆圈是什么意思？** 如果在一个屏幕截图上看到一个红色圆圈，则指示 PSC 字段在合作伙伴中心。

以下区域合作伙伴中心 PSC 到 合作伙伴中心 字段映射：

1. 映射到联合销售合作伙伴中心默认视图的 PSC 主页
1. 映射到交易视图的 PSC 合作伙伴中心视图
1. 映射到交易详细信息视图的 PSC 合作伙伴中心详细信息视图
1. PSC"添加产品"视图映射到"合作伙伴中心解决方案"视图
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
- 交易角色不是 PC 中的必填字段。 不会在任何工作流中显示或捕获它。 它根据添加到交易的解决方案在 Microsoft 卖方自动派生。
- 上次修改日期不显示在电脑的引荐详细信息页上。 合作伙伴可以使用排序功能根据上次更新日期对交易进行排序。

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - 映射到 合作伙伴中心 的 PSC 交易详细信息视图

将 PSC 顶部带编号的匹配圆圈 (PSC) 屏幕截图与合作伙伴中心屏幕截图进行比较。 匹配数字显示可在其中找到 PSC 相关功能或属性合作伙伴中心。 红色圆圈表示数据中不存在匹配的字段合作伙伴中心。

> [!NOTE]
> 屏幕截图下方显示了其他注意事项。

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="显示合作伙伴销售 Connect (PSC) 交易详细信息视图合作伙伴中心详细信息视图之间的字段映射的图像。" lightbox="images/pscmigration/deal-details-expanded.png":::

**特殊注意事项：**

- 合作伙伴可以通过选择合作伙伴交易详细信息视图上的编辑按钮来编辑交易 (6) 。 选择"编辑"按钮后，所有字段都将变为可编辑状态。 然后，可以选择保存或取消对交易进行编辑。
- 没有选项可以关闭交易，因为交易在合作伙伴中心。
- 客户成果在 合作伙伴中心。 可以在电脑的"备注"部分更新与客户交互相关的所有详细信息。
- 估计的解决方案关闭日期仅适用于 合作伙伴中心 中的 OEM IOT 交易。 对于任何其他交易类型，不会显示此信息。
- PC 中不需要许可计划。 此信息是根据在交易中选择的解决方案自动推断出来的。

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
- 在联合销售交易合作伙伴中心只有一个角色。 此角色是引荐管理员角色。

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - PSC 中的通知与合作伙伴中心

将 PSC 顶部带编号的匹配圆圈 (PSC) 屏幕截图与合作伙伴中心屏幕截图进行比较。 匹配数字显示可在其中找到 PSC 相关功能或属性合作伙伴中心。 红色圆圈表示数据中不存在匹配的字段合作伙伴中心。  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="显示合作伙伴销售 Connect (PSC) 通知和 合作伙伴中心 通知视图之间的映射的图像。"  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>从 PSC 迁移到合作伙伴中心 - 常见问题

以下部分回答有关迁移的常见问题。

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - 如果无法访问任何资源，该怎么办合作伙伴中心？

可以联系"无访问权限"页上列出的管理员，获取分配的角色。 在引荐 [部分下](permissions-overview.md#manage-referrals) ，需要具有读取和写入权限的引荐管理员角色。 如果仅管理业务配置文件，则需要合作伙伴中心的业务配置文件管理员角色。

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="显示中无访问体验的图像合作伙伴中心。":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - 谁可以授予我访问"引荐"部分的权限合作伙伴中心？

帐户[管理员可以](permissions-overview.md#manage-mpn-membership-and-your-company)授予你访问"引荐"选项卡的权限。若要查找帐户管理员，请从仪表板右上角的齿轮图标中选择"帐户合作伙伴中心[设置"](https://partner.microsoft.com/dashboard)。 然后，从 **左侧** 导航栏的第二级中选择"用户管理"。 在用户列表顶部，选择"筛选器"下拉菜单，将选项更改为帐户 **管理员**。页面将显示所有帐户管理员及其各自的电子邮件地址。 要求其中一个为工作帐户分配引荐管理员角色。

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - 帐户的"+新建交易"按钮灰度。 如何开始创建交易？

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

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - 是否强制添加客户组织？

是的，添加 [客户组织](./manage-co-sell-opportunities.md#select-your-customer) 在 合作伙伴中心。 首先，搜索客户的位置。 根据你拥有的详细信息;可以具体地包括确切的建筑物名称，也可以只提供城市详细信息。 组织搜索将提取与输入的名称匹配的所有法律实体，以便你不必输入任何地址详细信息。 所有详细信息都会根据所选组织自动填充。

### <a name="10---are-customer-contact-details-mandatory"></a>10 - 客户联系人详细信息是否是必需的？

取决于 [要创建的交易](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) 类型。 如果只是共享管道，并且不需要 Microsoft 销售组织的任何帮助，可以选择不提供客户联系人详细信息。 如果你正在联合销售你正在积极寻求 Microsoft 卖方的帮助，你必须提供客户联系人详细信息。 在合作伙伴中心创建联合销售请求之前，应获得客户的明确许可。

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - 我可以向交易添加多少解决方案？

可以添加最多 50 个解决方案 (PSC 中的"products"，) 交易。 与 PSC 不同，你可以混合使用自己的联合销售符合条件的解决方案、Microsoft 第一方 SKUS 和其他第三方联合销售符合条件的解决方案的解决方案。 合作伙伴中心没有要选择或可用的交易角色。 对于 Microsoft SKU，可以选择为添加到交易的每个 SKU 添加数量和价格。

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - 创建交易后，何时了解 Microsoft 卖方的详细信息？

只有在与 Microsoft 端相关卖方角色创建交易时所说明的确切帮助要求匹配后，才分配 Microsoft 卖方。 即使在分配后，Microsoft 销售人员也可以选择接受或拒绝联合销售邀请。 只有当销售人员接受联合销售邀请时，交易才使用 Microsoft 卖方联系人详细信息进行更新。 Microsoft 卖方针对交易的 SLA 为14天。 这与合作伙伴在进入过期状态之前应对交易的 SLA 是相同的。

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-在哪里可以找到机会 ID？

PSC 中的机会 ID 与 PC 中的交易 ID 相同。 您可以在打开任何交易时找到交易名称旁边的交易 ID。

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-我的 PDM 如何获取 PC 访问权限？

你的 Pdm 不能直接访问合作伙伴中心，这与 PSC 不同。 有多个选项可用于启用该功能，如下所述。

- OCP Insights-如果 Pdm 只是查看与它们相关的交易和进度，则他们可以使用 OCP Insights 门户获取组织视图。 这是一个内部工具，仅适用于 Pdm。 请注意，不能将 OCP 见解提供给公司的用户。
- 合作伙伴中心的来宾用户-可以 @microsoft.com 在合作伙伴中心添加 PDM 帐户作为来宾用户，并向其分配引用管理员角色，以便他们可以查看和操作引用。
- 在租户中创建 [新用户](./create-user-accounts-and-set-permissions.md#add-a-new-user) -可以在自己的租户中创建新用户，并与 PDM 共享这些详细信息，以便他们可以查看和处理与帐户中的其他引用用户类似的引用。

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>如果你在 PSC 中的帐户未与有效的 MPN 相关联，则查找正确的 MPN ID

如果你在这里看到的是 PSC 中提到 "PSC 无效 MPN ID 关联问题" 的横幅，就是正确的地方。 由于以下原因，你的帐户可能已链接到无效的 MPN ID

- 你的公司没有合作伙伴中心帐户。
- PDM 在将你的 PSC 帐户链接到合作伙伴中心帐户 (MPNID) 的内部系统中输入帐户的 MPN ID 时出错。
- 你的公司没有完成从合作伙伴成员中心的迁移 (PMC) 到 PC。

首先，按照以下步骤查找正确的 MPN ID

- 登录到 合作伙伴中心 帐户
- 使用帐户设置文档中 [提供的指导](./partner-center-account-setup.md#locate-your-mpn-id) 查找 MPN ID。

以下屏幕截图显示了可在其中找到你的 MPN 合作伙伴中心位置

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="显示合作伙伴可在其中找到其 MPN ID 的帐户设置的图像。"  lightbox="images/pscmigration/findingMPNID.png":::

下一步，

- 如果有 PDM，请要求他们从合作伙伴中心帐户使用正确的 MPN ID 更正 MPN ID。
- 如果没有 PDM，请发送电子邮件到 PSC 横幅中提供的地址，同时提供 PSC 横幅中显示的 PSC 帐户信息以及合作伙伴中心帐户中的正确 MPN ID。

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>帮助你在客户中创建和管理交易合作伙伴中心

如果尚未阅读联合销售帮助主题，以下资源将帮助你在合作伙伴中心管理交易。

|**要实现此目的，请执行以下操作**   |**阅读此文**   |
|-----------------------|:-----------------------|
|了解联合销售机会页中的选项卡和导航|[导航联合销售部分](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|从 D 和 B 列表中选择&组织 |[选择客户](./manage-co-sell-opportunities.md#select-your-customer)|
|修改交易详细信息部分中的字段|[交易详细信息](./manage-co-sell-opportunities.md#deal-details)|
|将团队成员添加到交易团队|[添加员工](./manage-co-sell-opportunities.md#add-team-members)|
|响应联合销售交易|[管理联合销售交易](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|注册已赢得的交易合作伙伴中心 |[注册新交易](./register-deals.md)
|获取引荐见解，了解引荐的进行方式 |[引荐见解](./referral-insights.md)
|创建和管理业务配置文件|[管理业务配置文件](./create-a-marketing-profile.md)
|管理业务配置文件的潜在客户 |[管理潜在客户](./manage-leads.md)|

## <a name="next-steps"></a>后续步骤


- [合作伙伴销售连接到合作伙伴中心工作簿](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -工作簿，通过合作伙伴中心与合作伙伴销售连接将合作伙伴的销售流程和角色与新的销售流程进行协调。
- [合作伙伴中心共同销售操作指南](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -通过合作伙伴中心识别运营模型以管理潜在客户或共同销售机会并注册交易的指导。
- [参考管理组](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -直观地说明了如何通过合作伙伴中心管理潜在客户和共同销售机会。
- [在商业 marketplace 中发布和管理](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -直观地说明了如何通过商用 marketplace 中的合作伙伴中心来创建、管理和发布产品/服务。