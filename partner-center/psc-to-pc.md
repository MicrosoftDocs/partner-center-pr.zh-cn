---
title: '从合作伙伴销售连接 (PSC) '
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 Microsoft 合作伙伴如何从合作伙伴销售连接 (PSC) 迁移到合作伙伴中心，以及如何创建或管理 Microsoft 卖方发送的交易。
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3dd511f455c24d7fa3193d6a99efd786eb3c34da
ms.sourcegitcommit: 561db5fabdebcd369f456007e5061f15d4ab781d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "90848259"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>合作伙伴中心 (PC) 中的共同销售指南，适用于从合作伙伴销售连接 (PSC 迁移的合作伙伴) 

**适用于**

- 合作伙伴中心

**相应的角色**

- 帐户管理员
- 引荐管理员
- 合作伙伴销售连接 (PSC) 卖方
-  (PSC) 管理员的合作伙伴销售连接
- 合作伙伴销售连接 (PSC) 交易经理

如你所知，你的公司将无法访问 PSC，2020年12月31日。 不过，你会发现你要创建共同销售交易所要做的一切，管理你的交易，并对 Microsoft 卖方发送到合作伙伴中心的交易进行操作。 但有一些区别，以下指南可帮助你将过渡过渡到合作伙伴中心。

>[!Important]
> 如果你在此处看到有关迁移的关于迁移的横幅，就是正确的位置。 本指南不适用于在 PSC 中管理其交易 (SA) 和 OEM IOT 合作伙伴。

## <a name="before-you-move-things-you-need-to-know"></a>在移动之前，你需要知道

### <a name="if-you-are-psc-admin"></a>如果你是 PSC 管理员

- 需要使用工作电子邮件登录到 [合作伙伴中心](https://partner.microsoft.com/)。
- 通过合作伙伴中心 [帐户管理员](https://docs.microsoft.com/partner-center/permissions-overview)的帮助设置你的帐户。
- 阅读本文档，了解如何在合作伙伴中心共同销售。
- 在合作伙伴中心设置用户帐户，使其 (管理员、交易经理和卖方角色) 的所有 PSC 用户，并为他们分配 [引用管理员角色](https://docs.microsoft.com/partner-center/permissions-overview)。

>[!Important]
> 请确保在 "合作伙伴中心" 中的 MPN 位置列表中提供了 PSC 横幅中所示的 MPN ID。 可以通过转到 "帐户设置" 和 "位置" 来验证合作伙伴中心中的 "帐户设置" 和 "[位置](https://docs.microsoft.com/partner-center/manage-locations)"，以查找与合作伙伴中心帐户关联的所有 MPNs 列表。

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="显示 PSC 横幅的图像，合作伙伴可在其中找到 MPN ID。":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>如果是 PSC 交易经理或卖方

- 需要使用工作电子邮件登录到 [合作伙伴中心](https://partner.microsoft.com/)。
- 如果你使用的是 PSC 中的非工作帐户，或者你的工作电子邮件与合作伙伴公司的公司不同，请联系你的 PSC 管理员以获取帐户设置帮助。
- 如果你的合作伙伴中心帐户设置完成，而不考虑你用来登录到 PSC 的帐户，请咨询你的 PSC 管理员。
- 验证你是否有权访问 "合作伙伴中心" 和 "引用" 部分。
- 阅读本文档，了解合作伙伴中心的工作流和变化。

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>作为 PSC 的管理员，以下是你的后续步骤

如果看不到 "引用" 选项卡：

- 贵公司的 [全局管理员](https://docs.microsoft.com/partner-center/permissions-overview) 可授予你访问 "引用" 选项卡的权限。若要查找全局管理员，请从合作伙伴中心右上方的齿轮图标中转到 "合作伙伴设置"。 选择左侧导航栏中第二级的 "用户管理" 页。 单击页面右上方的 "所有用户" 下拉箭头，然后更改为 "全局管理员"。 然后，该页将显示具有各自电子邮件 Id 的所有全局管理员。 请与他们联系以获取工作帐户的 "引用管理员" 访问权限。

>[!Important]
> 如果你的角色仅管理 PSC 中的用户，你可以在合作伙伴中心获得 [帐户管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) 角色。 如果你的角色还包括管理共同销售机会，你应该获得 " [引用管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) " 角色。 另外，还提名了一项更改管理线索，以与合作伙伴中心帐户管理员合作，而不是由所有 PSC 管理员单独使用。

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="显示 "合作伙伴设置" 用户管理页中的 "帐户管理员" 的图像。":::

- 在左侧导航窗格中转到 "引用" 选项卡，并检查是否可以访问这些页面。

>[!Note]
> 您可能必须从合作伙伴中心注销并重新登录，以便刷新您的凭据以访问引用页面。

在合作伙伴中心设置帐户后，

- 下一步，邀请 PSC 中具有角色 "交易经理" 或 "卖方" 的所有用户作为下一步。
- 帮助你使用引用访问权限的 [帐户管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) 可以邀请所有用户。
- 邀请用户时，要求帐户管理员将 " [引用管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) " 角色分配给他们。
- 一些 PSC 用户可能使用的是非工作帐户，或者使用的是合作伙伴中心以外的域中的帐户。 所有此类用户都需要使用附加到 Azure AD 租户的工作帐户登录到合作伙伴中心。 你的 [全局管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) 可对此有帮助。 若要查找全局管理员，请从合作伙伴中心右上方的齿轮图标中转到 "合作伙伴设置"。 单击左侧导航栏中第二级的 "用户管理" 页。 单击页面右上方的 "所有用户" 下拉箭头，然后更改为 "全局管理员"。
- 全局管理员可以在 Azure AD 租户中创建新的用户帐户，也可以为来宾用户分配对其他域帐户用户的访问权限。
- 为所有 PSC 交易经理和用户设置帐户后，他们需要登录到合作伙伴中心，在左侧导航栏中转到 "引用" 选项卡，然后检查以确保他们可以看到 "引用" 页面。

如果你的公司具有 PDM-当你的合作伙伴中心帐户已设置并且你的用户已移动并拥有角色和权限时，你可以将共同销售活动移动到合作伙伴中心。 通知 PDM 进行切换，而不是等到迁移完成截止时间，这会使所有新交易都流动到合作伙伴中心。
>[!Note]
>一旦您进行了此项切换，您将只能采取 PSC 中现有的活动交易。 您既不能创建新的交易，也不能从 PSC 的 Microsoft 卖方获得任何交易。

如果你的公司没有 PDM，请确保所有用户帐户均已设置并由所有用户进行验证。 当你可以在合作伙伴中心开始共同销售时，会通过电子邮件通知你的相关电子邮件和有关准确日期的版权。 请记住，你仍需要管理 PSC 中现有的活动交易。

>[!Important]
>活动交易不会迁移到 PC。 在2020年12月31日之前，请先关闭并注册交易。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC 管理员、PSC 交易经理和 PSC 卖方的后续步骤

了解如何在合作伙伴中心共同销售。
这是一个重要步骤，可帮助你为合作伙伴中心的共同销售做好准备。 了解合作伙伴中心的工作流和更改，以便能够有效地从第一天进行共同销售。 首先阅读本文档。 [共同销售体验库](https://aka.ms/cosellexperience)中也提供了一组良好的资源。

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC 和 PC 工作流之间的主要差异

|**方案**|**合作伙伴销售连接**|**合作伙伴中心**|
|-----|:-----|:-----|
|用户角色|PSC 具有管理员、交易经理和卖方角色。|PC 仅具有 [引用管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) 角色，该角色提供所有交易的读取和写入权限。|
|邀请 Microsoft 共同销售交易|由 Microsoft 卖方发起，伙伴没有明确的 ask。|如果某个交易需要 Microsoft 卖方帮助，合作伙伴将不得不发出 [显式请求](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) 。 Microsoft 卖方可以选择拒绝该请求。|
|Expiry|没有交易到期的概念。|如果合作伙伴不接受合作伙伴的入站交易，则该交易将在14天后过期。 对于合作伙伴出站交易，如果 Microsoft 卖方在14天内不执行此操作，则可以将其转入过期状态。|
|Microsoft 卖方详细信息|一旦创建了交易就会立即可见。|仅当卖方明确接受合作伙伴共同销售的邀请时，才会与合作伙伴共享 Microsoft 卖方详细信息。|
|[专用管道](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities)|不可用。|合作伙伴无需向 Microsoft 卖方提供可见性即可共享其管道。|
|解决方案|仅属于一个价目表的解决方案可以添加到交易中。|合作伙伴可以添加属于以下列表的 [解决方案](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) 。 a) 自己的解决方案 b) Microsoft 第一方目录的解决方案， (类似于 PSC 中的交易交易角色) 和 c) 来自其他第三方合作伙伴的共同销售解决方案 (类似于 PSC) 中的 ISV 交易角色。|
|交易分配|只有分配的卖方才能查看和处理交易。|团队成员可以添加到交易来指定处理交易的人员，而不会阻止其他引用管理员查看或操作这些交易。|
|客户组织|自由格式的文本输入。|只需键入几个字符，就可以针对[D&B 数据库](https://www.dnb.com/)搜索[customer 组织](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer)。 合法名称和地址是根据选择自动填充的。|
|客户联系人|不是必需的。|对于专用管道共享，不是必需的。 如果邀请 Microsoft 卖方加入共同销售请求，则需要此项。|
|公共 API|不可用。|用于以编程方式管理合作伙伴中心引用的[公共 API](https://docs.microsoft.com/partner/develop/referrals) 。|

## <a name="psc-and-partner-center-field-mapping"></a>PSC 和合作伙伴中心字段映射

本部分介绍了 PSC 与合作伙伴中心之间的确切属性映射。 与 "合作伙伴中心共同销售机会" 一节中的相关视图相比，PSC 中的每个屏幕。 

>[!Note]
>按照 PSC 屏幕截图中的黄色气泡上的数字，在 "合作伙伴中心" 中找到等效的属性。 红色气泡表明 "存档" 在 "合作伙伴中心" 中不可用。

**合作伙伴中心的 PSC 和共同销售机会的默认视图的主页**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="显示合作伙伴销售连接主页与合作伙伴中心的共同销售机会的默认视图之间的字段映射的图像。":::

**PSC 网格视图和合作伙伴中心交易视图**

- 合作伙伴中心中没有列表视图，如 PSC。  所有交易均根据客户信息和交易类型的最近接收日期或创建日期列出。 默认情况下，该视图中的第一个交易为选中状态。 在该交易的详细信息视图中，可在该交易的详细信息视图中找到以 PSC 表格格式显示的大多数值。
- 交易角色不是 PC 中的必填字段。 它既不显示也不在任何工作流中捕获。 它基于添加到交易中的解决方案在 Microsoft 卖方端自动派生。
- 上次修改日期不显示在 PC 的 "参考详细信息" 页上。 合作伙伴可以使用排序功能根据上一次更新的日期对交易进行排序。

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="此图像显示合作伙伴销售连接 (PSC) 网格视图和合作伙伴中心交易视图之间的字段映射。":::

**PSC 和合作伙伴中心的交易详细信息视图**

- 合作伙伴可以通过单击伙伴交易详细信息视图 (6) 上的 "编辑" 按钮来编辑交易。 单击 "编辑" 按钮后，所有字段都将变为可编辑的字段，并可选择保存或取消对该交易所做的编辑。
- 在合作伙伴中心，没有用于关闭交易的选项。
- 合作伙伴中心中不提供客户结果。 所有与客户交互相关的详细信息都可以在 PC 的 "说明" 部分中更新。
- 预计解决方案结束日期仅适用于合作伙伴中心的 OEM IOT 交易。 它不会显示任何其他交易类型。
- PC 不需要许可计划。 它基于在交易中选择的解决方案自动推断。

>[!Note]
>不能编辑标记为赢单或丢失的任何交易。 在将交易转到其中一种终端状态时要格外小心。

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="显示合作伙伴销售连接 (PSC 之间的字段映射的图像) 交易详细信息视图和合作伙伴中心交易详细信息视图。":::

**PSC "添加产品" 视图和合作伙伴中心的 "添加解决方案" 视图**

 :::image type="content" source="images/pscmigration/products.png" alt-text="显示合作伙伴销售连接 (PSC 之间的字段映射的图像) 添加产品视图和合作伙伴中心添加解决方案视图。":::

**PSC 和合作伙伴中心的用户管理**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="显示合作伙伴销售连接 (PSC 之间的字段映射的图像) 用户管理主页和 "帐户设置" 视图中的 "合作伙伴中心用户管理"。":::

**PSC 和合作伙伴中心的用户角色分配**

- PSC 管理员的等效角色是合作伙伴中心的帐户管理员角色。
- 合作伙伴中心中只有一个角色，共同销售交易管理是推荐管理员角色。

 :::image type="content" source="images/pscmigration/roles.png" alt-text="此图像显示合作伙伴销售连接 (PSC) 角色分配视图和合作伙伴中心角色分配视图之间的字段映射。":::

**PSC 和合作伙伴中心的通知**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="显示合作伙伴销售连接 (PSC 之间的映射的图像) 通知和合作伙伴中心通知视图。":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>从 PSC 迁移到合作伙伴中心-常见问题

**第.如果我没有访问合作伙伴中心的权限，我该怎么办？**

您可以与 "无法访问" 页上列出的管理员联系，以获取分配的角色。 在 "引用" 部分下，你将需要 "[引用管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals)" 角色才能读取和写入权限。 如果你只管理业务配置文件，则在合作伙伴中心需要 "业务配置文件管理员" 角色。

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="显示合作伙伴中心的 "无访问体验" 的图像。":::

**Q2.谁有权访问合作伙伴中心的 "引用" 部分？**

你的 [帐户管理员](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) 可以授予你访问 "引用" 选项卡的权限。若要查找帐户管理员，请从合作伙伴中心右上方的齿轮图标中转到 "合作伙伴设置"。 单击左侧导航栏中第二级的 "用户管理" 页。 单击显示页面右上方的 "所有用户" 的下拉箭头，然后更改为 "帐户管理员"。 然后，该页将显示所有帐户管理员及其各自的电子邮件 Id。 请与他们联系以获取工作帐户的 "引用管理员" 访问权限。

**又.对于我们的帐户，"+ 新建交易" 按钮将灰显。如何开始创建交易？**

仅当不存在附加到合作伙伴中心中所使用的 MPN 组织的共同销售准备解决方案时，才会发生这种情况。 联系你的 PDM 以获取你的解决方案的 MPN ID，或创建一个支持票证，其中提及 "新交易" 按钮在 PSC 迁移后灰显。

**四.我是否可以将交易分配给我们的组织中的特定人员，如 PSC？**

您可以将团队成员分配给特定交易。 它不会阻止其他引用管理员查看或操作这些交易。 

**Q5.是否有所有分配给我的交易的视图？**

你可以使用 "收藏夹" 功能，它是 "用户级别" 选项卡。你可以将分配给你的所有交易标记为收藏夹，以快速访问交易。

**Q6.是否有用于交易的只读视图？**

不，"引用" 部分中没有任何交易的只读视图。 所有的引用管理员都将对所有交易都具有完全读写访问权限。

**问题7.如何在使交易成为赢后进行注册？**

如果交易符合以下条件，则会显示一个弹出窗口，用于开始 [交易注册](https://docs.microsoft.com/partner-center/register-deals)。

- 有一种激励资格解决方案附加到交易。
- Microsoft 卖方邀请参加交易，或邀请参加交易。
- Microsoft 卡处于合作伙伴中心的 "已接受" 或 "赢" 状态。

**问题8.在交易注册部分中单击 "+ 新交易注册" 按钮时，会收到一条错误消息。如何注册我的交易？**

"+ 新交易注册" 仅供在 ISV 连接计划中注册的合作伙伴使用，用于注册交易，而合作伙伴中心没有相应的共同销售机会。 为了向共同销售机会注册交易，当交易标记为 "赢单" 时，将显示一个弹出窗口，如果该交易符合交易注册条件，则会显示一个弹出窗口。

**Q9.是否要求添加客户组织？**

是的，在合作伙伴中心，添加 [客户组织](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer) 是必需的。 首先，搜索客户所在位置的位置。 根据所拥有的详细信息，您可以指定具体的建筑物名称，也可以只是给出城市细节。 组织搜索将提取与你输入的名称相匹配的所有法律实体，这样你就不必输入任何地址详细信息。 系统会根据所选组织自动填充所有详细信息。

**Q10.客户联系详细信息是否是必需的？**

取决于要创建的 [交易类型](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities) 。 如果你只是共享你的管道，而不需要 Microsoft 销售组织的任何帮助，则可以选择不为客户联系详细信息。 如果你正在积极地从 Microsoft 卖方寻求帮助，你将需要提供客户联系详细信息。 在合作伙伴中心创建共同销售请求之前，你应该获得客户的明确同意。

**Q11.可以向交易添加多少个解决方案？**

你最多可以添加50个解决方案 (类似于 PSC) 的 "产品"。 与 PSC 不同，你可以将解决方案与你自己共同销售的符合条件的解决方案、Microsoft 第一方 Sku 和其他第三方共同销售的符合条件的解决方案组合在一起。 没有要在合作伙伴中心选择或使用的交易角色。 对于 Microsoft Sku，你可以选择为添加到交易中的每个 SKU 添加数量和价格。

**Q12.在创建交易后，我将如何了解 Microsoft 卖方的详细信息？**

只有在与 Microsoft 的相关卖方角色一起创建交易后，才会为 microsoft 卖方分配具体的帮助要求。 即使在分配后，Microsoft 卖方也可以选择接受或拒绝共同销售邀请。 只有卖方接受共同销售邀请时，才会使用 Microsoft 卖方联系详细信息更新交易。 Microsoft 卖方针对交易的 SLA 为14天。 这与合作伙伴在进入过期状态之前应对交易的 SLA 是相同的。

**Q13.在哪里可以找到机会 ID？**

PSC 中的机会 ID 与 PC 中的交易 ID 相同。 您可以在打开任何交易时找到交易名称旁边的交易 ID。

**Q14.PDM 如何可以访问 PC？**

你的 Pdm 不能直接访问合作伙伴中心，这与 PSC 不同。 有多个选项可用于启用该功能，如下所述。

- OCP Insights-如果 Pdm 只是查看 & 相关的交易进度，则可以使用 OCP Insights 门户获取组织视图。 这是一个内部工具，仅适用于 Pdm。 请注意，不能将 OCP 见解提供给公司的用户。
- 合作伙伴中心的来宾用户-可以 @microsoft.com 在合作伙伴中心添加 PDM 帐户作为来宾用户，并向其分配引用管理员角色，以便他们可以查看和操作引用。
- 在租户中创建 [新用户](https://docs.microsoft.com/partner-center/create-user-accounts-and-set-permissions#add-a-new-user) -可以在自己的租户中创建新用户，并与 PDM 共享这些详细信息，以便他们可以查看和处理与帐户中的其他引用用户类似的引用。

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>帮助你在合作伙伴中心创建和管理你的交易的资源

如果尚未阅读共同销售帮助主题，可通过以下资源来管理合作伙伴中心的交易。

|**要实现此目的，请执行以下操作**   |**阅读此文**   |
|-----------------------|:-----------------------|
|了解 "共同销售机会" 页中的选项卡和导航|[导航共同销售部分](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#navigating-the-co-sell-section)|
|从 D&B 列表选择客户组织 |[选择客户](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer)|
|修改 "交易详细信息" 部分中的字段|[交易详细信息](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#deal-details)|
|将公司员工添加到交易团队|[添加员工](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-your-employees)|
|响应共同销售交易|[管理共同销售交易](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#responding-to-a-co-sell-opportunity)
|注册在合作伙伴中心赢得的交易 |[注册新交易](https://docs.microsoft.com/partner-center/register-deals)
|获取参考见解并了解你的引用的工作方式 |[引荐见解](https://docs.microsoft.com/partner-center/referral-insights)
|创建和管理业务配置文件|[管理业务配置文件](https://docs.microsoft.com/partner-center/create-a-marketing-profile)
|管理业务配置文件的潜在客户 |[管理潜在客户](https://docs.microsoft.com/partner-center/manage-leads)|

## <a name="additional-resources"></a>其他资源

- [合作伙伴销售连接到合作伙伴中心工作簿](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -工作簿，通过合作伙伴中心与合作伙伴销售连接将合作伙伴的销售流程和角色与新的销售流程进行协调。
- [合作伙伴中心共同销售操作指南](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -通过合作伙伴中心识别运营模型以管理潜在客户或共同销售机会并注册交易的指导。
- [参考管理组](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -直观地说明了如何通过合作伙伴中心管理潜在客户和共同销售机会。
- [在商业 marketplace 中发布和管理](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -直观地说明了如何通过商用 marketplace 中的合作伙伴中心来创建、管理和发布产品/服务。
