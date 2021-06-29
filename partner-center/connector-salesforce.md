---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Salesforce CRM 同步。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029042"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>用于 Salesforce CRM 的联合销售连接器 – 概述

**适当的角色**：引用管理 |CRM 上的系统管理员或系统定制员

合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。 他们无需定型即可使用合作伙伴中心来管理共同销售交易。 使用共同销售连接器，你可以创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用，接受/拒绝引用，修改交易数据（如交易价值）和结束日期。  你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。 你可以在所选的 CRM 中工作而不是在合作伙伴中心内工作时执行所有引用工作。

此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。

## <a name="before-you-install---pre-requisites"></a>安装之前-必备组件

|**主题**|**详细信息**|**链接**|
|--------------|--------------------|------|
|Microsoft 合作伙伴网络 ID |需要一个有效的 MPN ID|加入 [MPN](https://partner.microsoft.com/)|
|已做好联合销售准备|你的 IP/服务解决方案必须共同销售。|[与 Microsoft 一起销售](https://partner.microsoft.com/membership/sell-with-microsoft)|
|合作伙伴中心帐户|与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。 在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。|[管理帐户](create-user-accounts-and-set-permissions.md)|
|合作伙伴中心用户角色|将安装和使用连接器的员工必须是推荐管理员|[为用户分配角色和权限](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 用户角色是系统管理员或系统定制员|[在 Salesforce CRM 中分配角色](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power 自动化 Flow 帐户|使用数据库创建新的生产环境，以便进行测试、过渡和生产。 如果你有一个具有数据库的现有生产环境，则可以重复使用它。 要安装连接器解决方案的用户必须具有对此环境的电源自动执行许可和访问权限。 如果安装失败，你可以监视进度并在 [电源自动执行](https://flow.microsoft.com/) 中获取详细信息。 选择 "**解决方案**" 下的 "**查看历史记录**"。|[创建或管理环境](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>为 Microsoft 自定义字段安装 Salesforce 包

若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要清楚地识别特定于 Microsoft 的引用字段。 此分界为合作伙伴卖方团队提供了决定他们要与 Microsoft 共享以共同销售的推荐的功能。

1. 在 Salesforce 中，激活 **注释** 并将其添加到机会相关列表。 [引用](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. 按照以下步骤激活 **机会团队** ：
    - 在安装程序中，使用 " **快速查找** " 框定位机会团队设置。
    - 根据需要定义设置。 [引用](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. 在 Salesforce 中，使用 [包安装程序](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)安装自定义字段和对象。 使用此安装程序将包安装到任何公司。

    >[!NOTE]
    >如果要安装到沙盒，则必须将 URL 的初始部分替换为 `http://test.salesforce.com` 。

1. 在 Salesforce 中，将 Microsoft 解决方案添加到 **机会** 相关列表。 添加后，选择 **扳手** 图标并更新属性

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在上线之前进行测试

在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。

- 在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。

- 制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。

- 在过渡/CRM 实例上测试解决方案。

- 成功后，将作为托管解决方案导入到生产实例。

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>为 Salesforce CRM 安装合作伙伴中心引用同步

1. 请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。 这会显示可用的 CRM 实例。

1. 从右上角的下拉列表中选择相应的 CRM 实例。

1. 选择左侧导航栏上的 " **解决方案** "。

1. 在顶部菜单中选择 " **打开 AppSource** " 链接。

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="打开 AppSource":::

1. 在弹出屏幕中搜索 Salesforce 的 " **合作伙伴中心引用连接器** "。  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="立即获取屏幕截图。":::

1. 选择 " **立即获取** " 按钮，然后选择 " **继续**"。

1. 在下一页中，选择 "Salesforce CRM 环境" 以安装应用程序。 同意条款和条件。

1. 然后，你将转到 " **管理你的解决方案** " 页。  通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。 **计划的安装** 应显示在合作伙伴中心引用解决方案旁边。 安装将需要10-15 分钟。

1. 安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，然后从左侧导航区域中选择 " **解决方案** "。 请注意，在 "解决方案" 列表中现在提供了 **Salesforce 的合作伙伴中心引用同步** 。

1. **为 Salesforce 选择合作伙伴中心引用同步**。 可以使用以下功能自动执行流和实体：

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce 流":::

## <a name="configure-the-solution"></a>配置解决方案

1. 在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。

1. 在右上角的 " **环境** " 下拉部分中，选择在其中安装了 Power 自动解决方案的 CRM 实例。

1. 需要创建关联三个用户帐户的连接：

   - 具有引用管理员凭据的合作伙伴中心用户
   - 合作伙伴中心事件
   - CRM 管理员，并在解决方案中自动执行流程

   1. 从左侧导航栏中选择 " **连接** "，然后从列表中选择 " **合作伙伴中心引用** " 解决方案。

   1. 通过选择 " **创建连接**" 来创建连接。

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="显示 &quot;创建连接&quot; 的屏幕截图。":::

   1. 在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。

   1. 使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。

   1. 接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。

   1. 为 CRM 管理员用户创建 Salesforce 连接。
  
   1. 为 CRM 管理员用户创建 Microsoft Dataverse 的连接。

   1. 添加所有连接后，你的环境中应会显示以下连接：

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="显示连接的屏幕截图。":::

### <a name="edit-the-connections"></a>编辑连接

1. 返回 " **解决方案** " 页，选择 " **默认解决方案**"。 通过单击 "**全部**" **(预览) 选择 "连接引用**"。

   :::image type="content" source="images/connection-reference-video.gif" alt-text="显示编辑连接的屏幕截图。":::

1. 通过选择省略号图标单独编辑每个连接。 添加相关连接。

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="显示如何编辑连接器的屏幕截图。":::

1. 按以下顺序打开流：
   - 合作伙伴中心预览体验版 (Webhook 注册) 
   - [自定义]从 Salesforce 创建或获取详细信息
   - 创建联合销售Referral-Salesforce预览合作伙伴中心 (预览) 
   - 合作伙伴中心 Microsoft 联合销售 Salesforce (Insider Preview)   
   - 合作伙伴中心 Insider Preview (Salesforce) 
   - Salesforce 合作伙伴中心 (Insider Preview) 
   - Salesforce 预览体验合作伙伴中心 (预览版) 
   - Salesforce Microsoft Solutions to 合作伙伴中心 (Insider Preview) 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook API 注册资源更改事件

可以使用 webhook 合作伙伴中心注册资源更改事件。 这些更改事件作为 HTTP 帖子发送到 URL。

1. 选择 **合作伙伴中心预览体验成员预览 (Salesforce CRM) "**。

1. 选择"**编辑"图标**，**然后选择"收到 HTTP 请求时"。**

1. 选择" **复制** "图标以复制提供的 **HTTP POST URL**。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="显示如何复制 URL 的屏幕截图。":::

1. 选择 **"合作伙伴中心预览 (预览版) Power Automate Webhook** 注册"，然后选择"运行 **"。**

1. 确保在右 **窗格中打开"运行** 流"窗口，然后选择"继续 **"。**

1. 输入以下详细信息：

   - **Http 触发器终结点**：此 URL 是从前面步骤复制的。
   - **要注册的事件**：选择所有可用事件 (引用 **创建**、引荐更新、**相关** 引荐创建以及相关引荐 **更新**) 。
   - **覆盖现有的触发器终结点（如果存在）？：** 是。 只能为给定的 Webhook 事件注册一个 URL。

1. 选择 **"运行流**"，然后选择"**完成"。**

Webhook 现在可以侦听、创建和更新事件。

## <a name="customize-synchronization-steps"></a>自定义同步步骤

CRM 系统是高度自定义的，你可以根据 CRM Power Automate自定义自定义解决方案。 当联合销售引荐在 合作伙伴中心 和 CRM 系统之间同步时，合作伙伴中心 电脑上同步的字段将列在自定义 [字段映射指南 中](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)。

按照字段映射指南操作，如有必要，在 **[自定义]** 从 Salesforce 或环境变量创建或获取详细信息中做出适当的更改。 请勿更新解决方案中任何其他Power Automate流，因为它可能会影响将来的解决方案升级。

以下自定义项可用：

- **在机会名称中** 显示选中标记：默认情况下，机会名称旁边会显示一个选中标记，指示 合作伙伴中心 与 Salesforce CRM 之间的同步已成功进行。 同样，如果同步失败，将显示交叉标记。 若要避免在机会名称中添加选中或交叉标记，请在机会名称环境变量中将"显示选中标记 **"的当前值** 设置为"否"。

- **阶段名称**：

  - **活动阶段名称**：这是 Salesforce 中商机销售管道中的阶段。  它表示活动阶段，等效于在活动状态中处于接受合作伙伴中心。 这可以是保留阶段后销售管道的下一阶段。 将机会的销售阶段从"保留"阶段移动到"活动"阶段将接受合作伙伴中心更改将开始同步。

  - **保留阶段名称**：Salesforce 中商机销售管道中的阶段名称。 它表示保留阶段。 尚未接受的 Microsoft 共享的新联合销售引荐将在 Salesforce 中设置为此阶段。 在机会处于保留阶段时对机会进行的任何更改将不会同步到合作伙伴中心。 将机会的销售阶段从此保留阶段移开将接受 合作伙伴中心 中的引荐，更改将开始同步。

- **客户帐户国家**/地区代码：创建新引荐时，必须提供两个字母 (ISO 3166) 国家/地区代码。 默认情况下，国家/地区代码将同步到 Salesforce 中帐户的 **BillingCountry 字段** ， 如果 Salesforce 中有不同的字段，用于同步国家/地区代码：

  - 对于帐户中包含双字母代码的非列表国家/地区代码字段：

    - 使用 CRM **的字段** 名称更新 Salesforce 环境变量中的"客户帐户国家/地区代码"字段名称。 请确保提供字段的名称，而不是其显示名称。

    - 编辑 **[自定义] 从 Salesforce** 创建或获取详细信息，然后转到在 **CRM** 操作中创建或获取客户帐户，以将国家/地区值分配给 CRM 中的正确字段。 此外，从 **BillingCountry** 中删除 Country 值分配。

  - 对于帐户中基于查找的国家/地区代码字段：

    - 在帐户中添加新的自定义字段，并使用两个字母的国家/地区代码 (ISO 3166) 基于基于查找的字段中选择的值自动填充该字段，反之亦然。

    - 按照 nonlookup 国家/地区代码字段的上述步骤，将新的自定义字段从 CRM 同步到和从 合作伙伴中心。

- **交易值**：默认情况下，来自 合作伙伴中心的交易值将同步到 CRM 中的 Amount 和 **Amount。** 如果 CRM 中有不同的字段，用于从以下位置同步交易值：

  - 使用 CRM **的字段** 名称更新 Salesforce 环境变量中的"交易值"字段名称。 请确保提供字段的名称，而不是其显示名称。

  - 编辑 **[自定义]** 从 Salesforce 创建或获取详细信息，转到在 CRM 中创建或更新机会，并更新"创建新机会"和"更新现有机会"操作，将 **DealValue** 分配给 Salesforce 中的正确字段。

- **交易值货币代码**：Salesforce 中交易值货币代码字段的名称。 在 Microsoft 合作伙伴中心 中创建或更新引荐时，此字段 API 名称将用于获取机会的交易值货币合作伙伴中心。 如果交易值货币代码字段不同于默认字段 **CurrencyIsoCode，** 请更新此环境变量的当前值。

  - 使用 CRM **的字段名称** 更新 Salesforce 环境变量中的"交易值货币"字段名称。 请确保提供字段的名称，而不是其显示名称。

  - 编辑 **[自定义]** 从 Salesforce 创建或获取详细信息，转到在 CRM 中创建或更新机会，并更新"创建新机会"和"更新现有机会"操作，以将 **DealValueCurrency** 分配到 Salesforce 中的正确字段。

- **同步联合销售机会**：如果设置为 **"是**"，则只有联合销售机会和管道共享机会合作伙伴中心 Salesforce。 如果设置为 **"否"，** 则潜在顾客、联合销售和管道共享机会将合作伙伴中心 Salesforce。 此变量对从 Salesforce 同步到销售合作伙伴中心。

## <a name="update-environment-variable"></a>更新环境变量

更新环境变量值：

1. 转到"解决方案 **"页**，然后选择"**默认解决方案"。** 选择 **"所有"，** 选择"环境 **变量"。**

1. 为需要更新的值选择环境变量，然后使用省略号图标选择"编辑"。

1. 更新 **当前 (** 不通过使用"新建值") 提供值来更新默认值值。  值必须与变量的数据类型匹配。 例如，"是"或"否"数据类型将接受"是"或"否"值。

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="显示&quot;更新环境变量&quot;的屏幕截图。":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>端到端双向联合销售引荐同步

安装、配置和自定义 Power Automate解决方案后，可以测试 Salesforce CRM 与 合作伙伴中心 之间的联合销售引荐同步。

### <a name="pre-requisites"></a>先决条件

若要跨 合作伙伴中心 Salesforce CRM 同步引荐，Power Automate解决方案需要明确划分特定于 Microsoft 的引荐字段。 此标识使卖方团队能够决定要与 Microsoft 共享哪些引荐进行联合销售。

一组自定义字段作为 Salesforce CRM 解决方案机会实体合作伙伴中心引荐同步的 **一** 部分提供。 CRM 管理员用户需要创建包含"机会"自定义字段 **的单独** CRM 部分。

以下自定义字段应是 CRM 部分的一部分：

- **与 合作伙伴中心** 同步：是否将商机与合作伙伴中心。 默认情况下，此字段的值为"否"，需要由卖方显式设置为"是"，以与 Microsoft 共享机会。 从 合作伙伴中心 CRM 共享的新引荐将此字段值设置为"是"。

- **引荐** 标识符：Microsoft 引用的只读合作伙伴中心字段。

- **引荐** 链接：指向 Microsoft 合作伙伴中心 中的引荐的只读合作伙伴中心。

- **Microsoft 如何提供帮助**：需要 Microsoft 提供引荐的帮助。 若要创建联合销售引荐，请选择 Microsoft 所需的相应帮助。 客户联系人必须与创建联合销售引荐的机会相关联。 若要创建非联合销售引荐，请勿选择此字段。 通过选择相应的"需要帮助"选项，可以随时将非联合销售引荐转换为联合销售引荐。

- **Microsoft 合作伙伴中心引荐可见性**：选择该引荐合作伙伴中心可见性。 通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。 如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会显示该引用。 将此字段标记为可见后，将无法还原它。

- **MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。

- **Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。 可以在商机中添加或删除一个或多个解决方案。 在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。 若要将此对象与商机关联，请在 CRM 中更新 **商机** 窗体。

- **Audit**：与合作伙伴中心引用同步的只读审核记录

### <a name="scenarios"></a>各种

1. 在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：

   1. 在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 Salesforce CRM 环境。

   1. 请确保在 Salesforce CRM 环境中创建 **新机会** 时， **Microsoft 合作伙伴中心** 出现在此部分。

   1. 与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce 环境的屏幕截图。":::

   1. 若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：

      - **Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="显示如何在卡片视图中获取相应字段的屏幕截图。":::

      - **与合作伙伴中心同步**：是
      - **客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。
      - **Microsoft 解决方案**：若要与 microsoft 共享引用，请向此机会添加有效的合作销售就绪或 Microsoft 解决方案。

   1. 将 "机会 **与合作伙伴中心同步** " 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。 你的参考将与 Salesforce CRM 同步，并将填充引用链接。 如果出现故障，则将使用错误信息填充审核字段。

   1. 同样，在 " **与合作伙伴中心同步** " 选项设置为 **"是"** 时，如果你更新了 Salesforce CRM 中的机会，则所做的更改将与你的合作伙伴中心帐户同步。

2. 引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：

    1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。

    1. 从左侧菜单中选择 " **引用** "。

    1. 单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。

    1. 登录到 Salesforce CRM 环境。

    1. 导航到 " **开放式机会**"。 Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。

    1. 选择同步的引用时，将填充卡片视图详细信息。

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce 机会页的屏幕截图。":::

>[!NOTE]
>**需要有关部署的帮助？**
>若要获得有关共同销售引用连接器部署的帮助，可以参与合作伙伴技术顾问。 他们可以为成功实现提供部署帮助和最佳实践。
>
>有关详细信息，请参阅 [如何提交技术预售和部署服务请求](technical-benefits.md)

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)

- [合作伙伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
