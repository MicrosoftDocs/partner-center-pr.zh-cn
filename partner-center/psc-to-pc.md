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
ms.openlocfilehash: 5be1c09a26cfcc0d038663e5814ccda7e535d4d1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551429"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>从合作伙伴销售 Connect 合作伙伴中心 (PSC) 迁移的合作伙伴在 合作伙伴中心 (PC (销售) 

**适当角色**：帐户管理员|引荐管理员|合作伙伴销售 (PSC) 卖方|合作伙伴销售 (PSC) 管理员|合作伙伴销售 (PSC) 交易经理

本文为合作伙伴提供从合作伙伴销售连接 (PSC) 迁移到 合作伙伴中心 (PC) 的指南，以便他们可以继续在 合作伙伴中心 创建和管理联合销售交易。

>[!Note]
> 如果因为在 PSC 中看到了有关迁移的横幅而在此处，则你的位置正确。 本指南不适用于在 PSC 中管理 (SA) 和 OEM 许可业务合作伙伴的解决方案评估。

>[!Important]
> 从 2021 年 4 月 1 日起，你的公司将无法在 PSC 中创建或编辑交易。 **仍可以使用 PSC 中的批量导出功能下载现有交易数据。还可以在此 [日期之后将未](psc-to-pc.md#psc-deals-migration) 合作伙伴中心交易从 PSC 迁移到另一个。** <br><br> 如果你正在积极处理包含 IP 联合销售奖励合格解决方案的交易，则有两种选择： <br><br> 1.将交易标记为"已赢得"，在 2021 年 3 月 31 日之前在 PSC 中完成交易注册。 <br> 2. [将](psc-to-pc.md#psc-deals-migration) 交易迁移到合作伙伴中心，以便你有更多的时间来处理交易并开始交易注册。

如你所知， **公司将在 2021** 年 4 月 30 日之后失去对 PSC 的访问权限。 但是，你仍然会发现你想要在 合作伙伴中心 中执行的所有工作，例如创建联合销售交易、管理交易，以及处理 Microsoft 销售人员发送给你的交易。

但是，存在差异。 以下指南可帮助你更顺畅合作伙伴中心更直接地转换。

## <a name="before-you-move-things-you-need-to-know"></a>在移动之前，需要知道的一些内容

### <a name="if-you-are-a-psc-admin"></a>如果你是 PSC 管理员

- 需要一封工作电子邮件来登录[合作伙伴中心。](https://partner.microsoft.com/)
- 在帐户管理员的帮助下设置合作伙伴中心 [帐户](permissions-overview.md)。
- 阅读本文档，了解如何合作伙伴中心联合销售。
- 在所有 PSC 用户合作伙伴中心管理员、交易 (和卖家角色设置用户帐户) 并为其分配引 [荐管理员角色](permissions-overview.md)。

>[!IMPORTANT]
> 请确保 PSC Microsoft 合作伙伴网络 (中显示的 MPN) ID 在 PSC 中的 MPN 位置列表中合作伙伴中心。

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="显示合作伙伴可在其中找到 MPN ID 的 PSC 横幅的图像。":::

 若要验证 MPN ID 是否显示为 合作伙伴中心 MPN 位置，请登录到 合作伙伴中心 仪表板，[](https://partner.microsoft.com/dashboard)然后选择"设置 **" (屏幕** 右上角的齿轮图标) ，后跟"帐户设置 **"。** 在二级左侧导航菜单中，选择"位置"以查看与帐户关联的所有 MPN 合作伙伴中心列表。

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>如果你是 PSC 交易经理或卖家

- 需要一封工作电子邮件登录到 合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。
- 如果在 PSC 中使用的是非工作帐户，或者工作电子邮件适用于与合作伙伴公司不同的公司，请联系 PSC 管理员，了解帐户设置帮助。
- 请咨询 PSC 管理员，合作伙伴中心帐户设置是否已完成，而不考虑用于登录 PSC 的帐户。
- 验证是否有权访问"合作伙伴中心和引荐"部分。
- 请阅读此文档，了解工作流和 合作伙伴中心。

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC 中的管理员将执行以下步骤

在左侧合作伙伴中心菜单中，选择" **引荐"** 选项。 确认可以访问"引荐"页。

  >[!Note]
  > 你可能必须注销合作伙伴中心重新登录，以刷新凭据以访问"引荐"页。

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

帐户管理员将在引荐指南旁边的联合销售机会页中看到 PSC 用户迁移向导链接。 他们可以通过选择链接来启动用户迁移。 若要启动用户迁移，管理员可以选择链接。 他们可以多次执行此用户迁移步骤，直到为所有用户分配适当的角色合作伙伴中心。

用户迁移表具有以下详细信息：

- 用户帐户 - 员工的电子邮件 ID
- PSC 合作伙伴帐户 - 员工在 PSC 中与之关联的帐户
- PSC 用户角色 - PSC 中分配给的三个角色之一。
- 电脑 MPN 位置 - 为用户提供与电脑角色相关的合作伙伴中心 (位置) 角色。 PSC 合作伙伴帐户 MPN 用于在角色中查找等效的 MPN 合作伙伴中心分配权限。 整个组织表示 vOrg MPN ID。
- 电脑用户角色 - 根据员工的 PSC 用户角色为员工分配角色。 PSC 中的管理员将在 合作伙伴中心 中分配引荐管理员合作伙伴中心。 卖方将在客户中分配引荐用户合作伙伴中心。 在此处了解合作伙伴中心角色以及具有这些角色的用户可以执行哪些合作伙伴中心[](permissions-overview.md#manage-referrals)
- PC AAD 租户 - Microsoft Azure Active Directory (Azure AD) 中用户分配到的租户合作伙伴中心
- 状态 - 迁移状态有三种可能的状态
    - **未迁移** - 用户未分配合作伙伴中心角色
    - **已迁移** - 用户已成功迁移，并分配了相关角色，如下表所示
    - **错误** - 由于某些错误，无法完成迁移

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

完成用户迁移后，使用联合销售机会页中的交易迁移向导，将 PSC 中所有符合条件的开放式交易合作伙伴中心。 **"交易迁移"链接将仅在"客户"中显示具有整个组织范围的引荐合作伙伴中心。** 联合销售机会页面的右上方有一个称为 **"PSC 交易** 迁移"的链接，这将打开交易迁移向导。

在开始交易迁移之前，请阅读本部分。

**符合迁移条件**

只有一些交易符合从 PSC 迁移到 合作伙伴中心。 此迁移向导可帮助合作伙伴将交易引入合作伙伴中心他们仍在积极与客户合作以完成交易。 **只有从 2020 年 1 月 1 日创建的、具有有效合作伙伴帐户详细信息（ (MPN ID) 且未进行交易注册）的交易才有资格进行迁移。**

**不符合迁移条件**

- 解决方案评估交易不符合交易迁移条件
- OEM 许可业务交易不符合交易迁移条件
- PSC 中标记为"获胜"的任何交易都不符合迁移条件。 如果符合标记为"获胜"的交易资格，则交易注册应在 PSC 中完成。

## <a name="pre-requisites-for-deal-migration"></a>交易迁移的先决条件

从 PSC 开始交易合作伙伴中心，请按照以下说明在 PSC 中设置交易，以成功迁移。

1. 公司中处理开放式交易的所有销售团队成员都获得有关此迁移的信息。
2. 销售团队成员经过培训，可以使用合作伙伴中心进行交易管理。
3. 交易包含所有必需的信息，如下所述。
    - 客户公司详细信息，包括名称和地址
    - 客户联系人详细信息（如果是联合销售交易）
    - 至少一个解决方案
    - 至少一个团队成员具有所有详细信息 - 名字、姓氏、电子邮件 ID 和电话号码
    - 交易值
    - 估计的交易关闭日期
    - 合作伙伴说明

可以使用 PSC 中的批量下载和上传功能，在所有符合条件的交易中添加交易中缺少的所有详细信息。

>[!Note]
> 即使未满足上述先决条件，交易迁移也会成功。 但是，如果上述任何必填字段在 合作伙伴中心不可用，则无法更改交易状态。 然后，必须输入交易中缺少的所有必需信息合作伙伴中心开始处理这些信息。 **强烈建议在 PSC 中清理符合条件的交易，然后再将它们迁移到合作伙伴中心。**

合作伙伴中心中的交易迁移构建为一键式体验。 只需在公司准备好迁移符合条件的交易后，选择"迁移交易"按钮。 **无法选择要从 PSC 迁移的交易。如果不希望将任何交易迁移到 合作伙伴中心，在开始迁移之前，请将它们移到 PSC 中的已关闭状态。**

>[!Note]
> 启动迁移后 **，最多可能需要 24** 小时才能迁移交易。

迁移完成后，横幅消息的状态将更改为完成，并包含指向迁移报告的链接。 下载报表以查看从 PSC 迁移到 合作伙伴中心。

该报表包含以下详细信息。

1. **合作伙伴中心 ID** - 合作伙伴中心中所有交易的唯一标识符。 有两个交易 - 一个交易针对合作伙伴，另一个交易适用于 Microsoft，共同销售合作伙伴中心。
2. **合作伙伴中心 ID** - 合作伙伴中心合作伙伴的交易的唯一标识符。
3. **交易名称** - PSC 中为交易给定的标识符。
4. **PSC 交易 ID** - PSC 中交易的唯一标识符。
5. **错误** - 指示迁移特定交易时是否有错误。

已成功迁移的所有交易在 PSC 中不可见。 你可以继续处理已迁移的交易，合作伙伴中心包括完成交易注册合作伙伴中心。 与 Microsoft 卖方之间的联合销售交易交互不会发生变化。

从 PSC 迁移的交易将基于交易源在"入站"和"出站"选项卡中提供。 公司共享的所有交易都将在"出站"选项卡中提供，Microsoft 发起的交易将在"入站"选项卡中合作伙伴中心。 迁移后将创建两种类型的交易。

1. **联合销售交易** - PSC 中标记为联合销售的交易将在 合作伙伴中心。
2. **合作伙伴引导式** 交易 - 未标记为联合销售的交易将在客户中创建为合作伙伴合作伙伴中心。 合作伙伴引导的交易对 Microsoft 销售人员可见，可以在达到终端状态之前升级为联合销售交易， (赢得、失去) 。 此外，如果交易有奖励符合条件的解决方案，则合作伙伴引导式交易符合交易注册条件。

>[!Important]
> 如果由于某些交易无法迁移而出现任何错误，可以通过单击"迁移交易"按钮来 **重新启动交易迁移**。 只有在有一些符合条件的交易尚未迁移时，才启用此功能。 如果在启动交易迁移后在 PSC 中创建一些新交易，则这也将很有帮助。

成功迁移所有交易后，将显示"无要迁移的交易"的横幅，其中"迁移交易 **"** 按钮 **被禁用**。

完成用户迁移和/或交易迁移后，使用以下指南确定迁移策略：

如果你的公司有合作伙伴开发经理 (PDM) - 设置 合作伙伴中心 帐户并且用户已迁移并拥有角色和权限时，可以将联合销售活动移到 合作伙伴中心。 通知 PDM 进行切换，而不是等到迁移完成截止时间，这将使所有新交易流入合作伙伴中心。

>[!Note]
>进行此切换后，你只能处理 PSC 中的现有活动交易。 在 PSC 中，既无法创建新交易，也无法从 Microsoft 卖方处收到任何交易。

如果你的公司没有 PDM - 请确保所有用户都设置并验证所有用户帐户。 PSC 中会通过电子邮件和横幅通知你何时可以开始联合销售合作伙伴中心。 请记住，你仍必须管理 PSC 中的现有活动交易。

>[!Important]
> 在 2021 年 4 月 30 日之前，你才能注册标记为"获胜"的交易。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC 管理员、PSC 交易经理和 PSC 销售人员的下一步步骤

了解如何在联合销售合作伙伴中心。
这是一个重要步骤，可帮助你准备好在 合作伙伴中心。 了解工作流和合作伙伴中心更改，以便可以有效地进行联合销售。 首先，请完全阅读本文档。 联合销售体验库中也提供了 [一组很好的资源](https://aka.ms/cosellexperience)。

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>PSC 与工作流合作伙伴中心差异

|**方案**|**合作伙伴销售连接**|**合作伙伴中心**|
|-----|:-----|:-----|
|用户角色|PSC 具有管理员、交易经理和卖家角色。|合作伙伴中心只有 [引荐管理员](permissions-overview.md#manage-referrals) 角色，该角色授予所有交易读取和写入权限。|
|邀请 Microsoft 进行联合销售交易|由 Microsoft 卖方发起，合作伙伴没有明确的请求。|如果交易需要 Microsoft[](manage-co-sell-opportunities.md#add-solutions)卖方帮助，合作伙伴必须提出显式请求。 Microsoft 卖方可以选择拒绝请求。|
|Expiry|没有交易到期的概念。|合作伙伴入站交易在 14 天后过期（如果合作伙伴未接受）。 与合作伙伴出站交易的情况相同，如果 Microsoft 销售人员在 14 天内未处理这些交易，则这些交易可能会进入过期状态。|
|Microsoft 卖方详细信息|创建交易后即可见。|Microsoft 卖方详细信息仅在卖方明确接受合作伙伴联合销售邀请时与合作伙伴共享。|
|[专用管道](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|不可用。|合作伙伴可以共享其管道，而无需向 Microsoft 销售人员提供可见性。|
|解决方案|只能将属于一个价目表的解决方案添加到交易。|合作伙伴可以 [添加属于](manage-co-sell-opportunities.md#add-solutions) 以下列表的解决方案。 a) 其自己的解决方案 b) Solutions from Microsoft 第一方目录 (类似于 PSC) 中的事务交易角色和 c) 联合销售来自其他第三方合作伙伴的解决方案 (类似于 PSC) 中的 ISV 交易角色。|
|交易分配|只有分配的卖方才能查看交易并采取行动。|可以将团队成员添加到交易，以指定处理交易的人，不会阻止其他引荐管理员查看或处理这些交易。|
|客户组织|自由格式文本条目。|只需键入 [几个字符](manage-co-sell-opportunities.md#select-your-customer) ，就可以根据 [D&B](https://www.dnb.com/) 数据库搜索客户组织。 根据选择自动填充法定名称和地址。|
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

- 合作伙伴中心中没有列表视图，如 PSC。  所有交易均根据客户信息和交易类型的最近接收日期或创建日期列出。 默认情况下，该视图中的第一个交易为选中状态。 在合作伙伴中心的交易的详细信息视图中提供了在 PSC 表格格式中显示的大部分值。
- 交易角色不是合作伙伴中心的必填字段。 它不会在任何工作流中显示或捕获。 它基于添加到交易中的解决方案在 Microsoft 卖方端自动派生。
- "上次修改日期" 不显示在合作伙伴中心的 "参考详细信息" 页上。 合作伙伴可以使用排序功能根据上一次更新的日期对交易进行排序。

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-已映射到合作伙伴中心的 PSC 交易详细信息视图

将顶部 (PSC) 屏幕截图的匹配、带编号的圆圈与下面的合作伙伴中心屏幕截图进行比较。 匹配数字显示了在合作伙伴中心查找 PSC 相关功能或属性的位置。 红色圆圈指示伙伴中心中没有匹配的字段或区域。

> [!NOTE]
> 屏幕截图下面会出现其他注意事项。

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="显示合作伙伴销售连接 (PSC 之间的字段映射的图像) 交易详细信息视图和合作伙伴中心交易详细信息视图。" lightbox="images/pscmigration/deal-details-expanded.png":::

**特别注意事项：**

- 合作伙伴可以通过选择合作伙伴交易详细信息视图 (6) 上的 "编辑" 按钮来编辑交易。 选择 "编辑" 按钮后，所有字段都将变为可编辑状态。 然后，您可以选择保存或取消对交易所做的编辑。
- 在合作伙伴中心，没有用于关闭交易的选项。
- 合作伙伴中心中不提供客户结果。 可以在合作伙伴中心的 "注释" 部分中更新与客户交互相关的所有详细信息。
- 预计解决方案关闭日期仅适用于合作伙伴中心的 OEM IOT 交易。 对于任何其他交易类型，不会显示此信息。
- 合作伙伴中心不需要许可计划。 此信息是根据在交易中选择的解决方案自动推断出来的。

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

你的 [帐户管理员](permissions-overview.md#manage-mpn-membership-and-your-company)可以授予你访问 "引用" 选项卡的权限。若要查找帐户管理员，请从 "合作伙伴中心"[仪表板](https://partner.microsoft.com/dashboard)右上角的齿轮图标中选择 "**帐户设置**"。 然后，从第二层的左侧导航栏中选择 " **用户管理** "。 在用户列表的顶部，选择 " **筛选器** " 下拉菜单，并将选项更改为 " **帐户管理员**"。该页将显示所有帐户管理员及其各自的电子邮件地址。 要求其中一个用户为你的工作帐户分配 "引用管理员" 角色。

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-对于我们的帐户，"+ 新建交易" 按钮将灰显。 如何开始创建交易？

只有在未将联合销售就绪解决方案附加到你正在云中使用的 MPN 组织时，才合作伙伴中心。 请联系 PDM 以更正解决方案的 MPN ID，或创建提及问题的支持票证："PSC 迁移后，新交易按钮灰暗"。

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - 能否将交易分配给组织的特定人员（如 PSC）？

可以将团队成员分配到特定交易。 它不会阻止其他引荐管理员查看或处理这些交易。

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - 是否可以查看分配给我的所有交易？

可以使用收藏夹功能，即用户级选项卡。可以将分配给你的所有交易标记为收藏项，以便快速访问交易。

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - 是否有交易只读视图？

否，引荐部分中没有交易只读视图。 所有引荐管理员都将拥有所有交易的完整读取和写入访问权限。

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - 如何在将交易标记为"获胜"后注册交易？

如果交易满足以下条件，我们将显示一个弹出窗口来启动 [交易注册](./register-deals.md)。

- 交易附带了一个符合奖励条件的解决方案。
- Microsoft 卖方受邀参与交易，或者邀请你参与交易。
- Microsoft 卡在"已接受"或"已合作伙伴中心。

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - 我在"交易注册"部分选择"+新建交易注册"按钮时收到错误消息。 如何注册交易？

**"+新建交易** 注册"按钮仅供在 ISV 连接计划中注册的合作伙伴使用，以注册交易，而该交易没有相应的联合销售合作伙伴中心。 对于通过联合销售机会注册交易，当交易标记为"已赢得"且满足交易注册条件时，将显示一个弹出窗口。

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - 是否强制添加客户组织？

是的，添加 [客户组织](./manage-co-sell-opportunities.md#select-your-customer) 在 合作伙伴中心。 首先，搜索客户的位置。 根据你拥有的详细信息;可以具体地包括确切的建筑物名称，也可以只提供城市详细信息。 组织搜索将提取与输入的名称匹配的所有法律实体，以便你不必输入任何地址详细信息。 所有详细信息都会根据所选组织自动填充。

### <a name="10---are-customer-contact-details-mandatory"></a>10 - 客户联系人详细信息是否是必需的？

取决于 [要创建的交易](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) 类型。 如果只是共享管道，并且不需要 Microsoft 销售组织的任何帮助，可以选择不提供客户联系人详细信息。 如果你正在联合销售你正在积极寻求 Microsoft 卖方的帮助，你必须提供客户联系人详细信息。 在合作伙伴中心创建联合销售请求之前，应获得客户的明确许可。

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - 我可以向交易添加多少解决方案？

可以添加最多 50 个解决方案 (PSC 中的"products"，) 交易。 与 PSC 不同，你可以混合使用自己的联合销售符合条件的解决方案、Microsoft 第一方 SKUS 和其他第三方联合销售符合条件的解决方案的解决方案。 合作伙伴中心没有要选择或可用的交易角色。 对于 Microsoft SKU，可以选择为添加到交易的每个 SKU 添加数量和价格。

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - 创建交易后，何时了解 Microsoft 卖方的详细信息？

只有在与 Microsoft 端相关卖方角色创建交易时所说明的确切帮助要求匹配后，才分配 Microsoft 卖方。 即使在分配后，Microsoft 销售人员也可以选择接受或拒绝联合销售邀请。 只有当销售人员接受联合销售邀请时，交易才使用 Microsoft 卖方联系人详细信息进行更新。 Microsoft 销售人员针对交易采取行动的 SLA 为 14 天。 在交易进入过期状态之前，合作伙伴必须对此交易采取相同的 SLA。

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - 在哪里可以找到机会 ID？

PSC 中的机会 ID 与中交易 ID 合作伙伴中心。 打开任何交易时，可以在交易名称旁找到交易 ID。

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 - PDM 如何获取对 合作伙伴中心？

合作伙伴中心 PSC 不同，你的 PDM 不能直接访问它。 有多种选项可启用该功能，下面将介绍这些选项。

- OCP 见解 - 如果 PDM 只是查看与它们相关的交易和进度，他们可以使用 One Commercial Partner (OCP) Insights 门户获取组织视图。 这是一个内部工具，仅适用于 PDM。 OCP 见解不适用于公司的用户。
- 合作伙伴中心中的来宾用户 - 可以在合作伙伴中心将 PDM 帐户添加为来宾用户，并为其分配引荐管理员角色，以便他们可以查看和 @microsoft.com 处理引荐。
- 在租户 [中](./create-user-accounts-and-set-permissions.md#add-a-new-user) 创建新用户 - 可以在自己的租户中创建新用户并与 PDM 共享这些详细信息，以便他们可以查看并处理与帐户中其他引荐用户类似的引荐。

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>如果 PSC 中的帐户未与有效的 MPN 关联，则查找正确的 MPN ID

如果因为看到 PSC 中提及"PSC MPN ID 关联问题无效"的横幅而在此处，则说明你的位置正确。 你的帐户可能由于以下原因链接到了无效的 MPN ID

- 你的公司没有一个合作伙伴中心帐户。
- 在将 PSC 帐户链接到 合作伙伴中心 帐户的内部系统中输入帐户的 MPN ID 时，PDM 出错 (MPN ID) 。
- 你的公司没有完成从 PMC Partner Membership Center (迁移到) 合作伙伴中心。

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
|管理业务配置文件的潜在顾客 |[管理潜在客户](./manage-leads.md)|

## <a name="next-steps"></a>后续步骤


- [合作伙伴销售合作伙伴中心](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) 工作簿 - 工作簿，用于通过 合作伙伴中心 与 Partner Sales Connect 使合作伙伴的销售流程和角色与新的销售流程保持一致。
- [合作伙伴中心联合销售运营指南](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) - 指导通过 合作伙伴中心 确定运营模型，以管理潜在顾客或联合销售机会并注册交易。
- [引荐管理](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) 组 - 可视化的分步说明，用于通过客户管理潜在顾客和联合销售合作伙伴中心。
- [在商业市场中发布](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) 和管理 - 可视化的分步说明，用于通过商业市场中的 合作伙伴中心创建、管理和发布产品/服务。