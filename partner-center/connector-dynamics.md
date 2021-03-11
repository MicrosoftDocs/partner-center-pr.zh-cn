---
title: Dynamics 365 CRM 合作伙伴中心的共同销售连接器
description: 将合作伙伴中心中的引用与 Dynamics 365 CRM 的共同销售连接器同步。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 1b0f8f12cf60db0dcc03aae24316e869cbf34376
ms.sourcegitcommit: d7fbaff51c7ac29fbf700d7f7fdef798fd97c6fa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "102619403"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>用于 Dynamics 365 CRM 的共同销售连接器–概述

### <a name="appropriate-roles"></a>相应的角色

- 引荐管理员
- CRM 上的系统管理员或系统定制员

合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。 他们无需定型即可使用合作伙伴中心来管理共同销售交易。 使用共同销售连接器，可以创建新的共同销售的引用，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受/拒绝引用、修改交易数据（如交易价值和结束日期）。 你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。 你可以在所选的 CRM 中（而不是在合作伙伴中心）管理你的所有引用。 

此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。

## <a name="before-you-install---pre-requisites"></a>安装之前-必备组件

|**主题**   |**详细信息**   |**链接**   |
|--------------|--------------------|------|
|Microsoft 合作伙伴网络 ID |需要一个有效的 MPN ID|加入 [MPN](https://partner.microsoft.com/)|
|合作销售就绪|你的 IP/服务解决方案必须共同销售。|[与 Microsoft 一起销售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作伙伴中心帐户|与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。 在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。|[管理帐户](create-user-accounts-and-set-permissions.md)|
|合作伙伴中心用户角色|将安装和使用连接器的员工必须是推荐管理员|[为用户分配角色和权限](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|CRM 用户角色是系统管理员或系统定制员|[在 Dynamics 365 中分配角色](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power 自动化 Flow 帐户|创建新的生产环境，其中包含用于测试/过渡和生产的数据库。 如果你有包含数据库的现有生产环境，则可以重复使用它。 要安装连接器解决方案的用户需要具有对此环境的电源自动许可证和访问权限。可以通过单击 "解决方案" [下的 "](https://flow.microsoft.com/) 查看历史记录"，来监视进度并获得更多详细信息。|[创建或管理环境](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>安装适用于 Dynamics 365 (Power 自动化解决方案的合作伙伴中心引用同步) 

1. 请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。 此步骤将显示可用的 CRM 实例。

2. 从右上角的下拉菜单中选择相应的 CRM 实例。

3. 选择左侧导航栏上的 " **解决方案** "。

4. 单击顶部菜单上的 " **打开 AppSource** " 链接。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. 在弹出屏幕中搜索 **Dynamics365 的合作伙伴中心引用连接器** 。  

6. 单击 " **立即获取** " 按钮，然后 **继续**。

7. 这将打开一个页面，可在其中选择 CRM (Dynamics 365) 环境以安装应用程序。  同意条款和条件。

8. 可以通过单击 "**解决方案**" 下的 "**查看历史记录**"，来监视进度并获得更多详细信息。
 

9. 安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。 请注意，"解决方案" 列表中提供了 **Dynamics 365 的合作伙伴中心引用同步** 。

10. 选择 **Dynamics 365 的伙伴中心引用同步**。 可以使用以下功能自动执行流和实体：

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用 CRM":::

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在上线之前进行测试

在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。

- 在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。
- 在过渡环境中配置和自定义 Microsoft Power 自动化解决方案。
- 在过渡/CRM 实例上测试解决方案。 
- 成功后，将作为托管解决方案导入到生产实例。 

## <a name="configure-the-solution"></a>配置解决方案

1. 在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。


2. 在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。

3. 需要创建关联三个用户帐户的连接：

   - 具有引用管理员凭据的合作伙伴中心用户

   - 合作伙伴中心事件

   - CRM 管理员，并在解决方案中自动执行流处理。

      1. 从左侧导航栏中选择 " **连接** "，然后从列表中选择 " **合作伙伴中心引用** " 解决方案。

      2. 通过单击 " **创建连接**" 创建连接。

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="创建连接":::

      3. 在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。

      4. 使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。

      5. 接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。

      6. 为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。
     
      7. 添加所有连接后，你的环境中应会显示以下连接：

         :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="连接":::
   
## <a name="edit-the-connections"></a>编辑连接

1. 返回 " **解决方案** " 页，选择 " **默认解决方案**"。 通过单击 "**全部**" **(预览) 选择 "连接引用**"。

   :::image type="content" source="images/connection-reference-video.gif" alt-text="编辑连接":::

2. 通过选择三个点图标，逐个编辑每个连接。 添加相关连接。

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="列出的连接"::: 

3.  返回到 "解决方案" 页，为 Dynamics 365 选择 "合作伙伴中心引用同步"，然后单击以下序列中每个流旁边的三个点图标，打开流。 如果在打开流时遇到任何问题，请参阅 [自定义步骤](connector-dynamics.md#customize-synchronization-steps) 和 [故障排除步骤](connectors-troubleshoot.md)。 

按以下顺序打开流：

-  (内幕预览版) 合作伙伴中心 Webhook 注册
- 创建共同销售引用– Dynamics 365 到合作伙伴中心 (预览体验中心) 
- 来自创建或获取 Dynamics 365 流中的详细信息 
- 合作伙伴中心到 Dynamics 365-Helper (预览体验中心) 
- 合作伙伴中心 Microsoft 共同销售对 Dynamics 365 (预览体验的引用更新) 
- 合作伙伴中心到 Dynamics 365 (预览体验体验) 
- Dynamics 365 到合作伙伴中心 (预览体验) 
- Dynamics 365 到合作伙伴中心 (有问必答预览版的机会) 
- Dynamics 365 的 Microsoft 解决方案到合作伙伴中心 (预览体验) 
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook Api 注册资源更改事件

合作伙伴中心 Webhook Api 允许你注册资源更改事件。 这些更改事件以 HTTP post 的形式发送到你的 url。

1. 选择 " **合作伙伴中心到 Dynamics 365 (预览体验预览")**。

2. 选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。

3. 选择 **复制** 图标以复制提供的 HTTP POST URL。

   :::image type="content" source="images/webhook-video.gif" alt-text="使用 webhook 注册资源更改":::

4. 选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。

5. 确保在右侧窗格中打开 "运行流" 窗口，然后单击 " **继续**"。

6. 输入以下详细信息：

   - **Http 触发器终结点**：从前面的步骤中复制的 URL

   - **要注册的事件**：选择所有可用事件 ( "引用已创建"、"引用已更新"、"相关-引用已创建"、"相关引用-已更新" ) 

   -**覆盖现有触发器终结点（如果存在**）：是重要的，请务必注意，只能为给定 webhook 事件注册一个 URL。 请务必注意，只能为给定 webhook 事件注册一个 URL。 

7. 选择 " **运行** "，然后选择 " **完成"。**

Webhook 现在可以侦听以创建和更新事件。

## <a name="customize-synchronization-steps"></a>自定义同步步骤

CRM 系统经过高度自定义，你可以基于 CRM 设置自定义电源自动化解决方案。  当共同销售的引用在合作伙伴中心与你的 CRM 系统之间同步时，在 " [自定义字段映射指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)" 中列出了在合作伙伴中心电脑上同步的字段。

按照字段映射指南进行操作，如有必要，请在 **[自定义] 创建或获取 Dynamics 365 flow**  或环境变量的详细信息。 建议不要更新 Power 自动解决方案中的任何其他流，因为它可能会影响将来的解决方案升级。 

可用的自定义如下：

- "复选标记出现机会名称"：默认情况下，将在 "机会名称" 旁显示一个复选标记，指示合作伙伴中心与 Dynamics 365 CRM 之间的同步已成功完成。 同样，如果同步失败，将显示交叉标记。 若要避免在 "机会名称" 中添加复选标记或交叉标记，请将机会 name 环境变量中显示复选标记的当前值设置为 "否"。

- 交易价值：默认情况下，来自合作伙伴中心的交易值将与 CRM 中的 **estimatedvalue** 同步。 如果 CRM 中有不同的字段要从中同步值，请执行以下操作：

  a. 在 Dynamics 365 环境变量中，用 CRM 的字段名称更新交易值字段名称。 请注意，应提供字段名称，而不是其显示名称。

  b. 编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**  ，并导航到 crm 中的 " **创建或更新** 机会" 和 "更新" " **创建新机会** 并 **更新现有机会** 操作"，将 **DealValue** 值分配到 CRM 中的正确字段。 同时，从 "**估计收入**" 字段中删除 **DealValue 分配**。

- 客户帐户国家/地区代码：创建新引用时，必须提供两个字母的国家/地区代码 (ISO 3166) 。 默认情况下，国家/地区代码将同步到 CRM 中的帐户 address1_country 字段。 如果 CRM 中的 "国家/地区代码" 字段不同，则：

   a. 对于包含两个字母代码的帐户的非查找国家/地区代码字段：

   - 用 CRM 的字段名称更新 Dynamics 365 环境变量中的客户帐户国家/地区代码字段名称。 请注意，应提供字段名称，而不是其显示名称。

   - 编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息**  ，并导航到 "创建或获取 crm 中的客户帐户" 操作，以将国家/地区值分配到 crm 中的正确字段。 同时，从地址1：国家/地区字段中删除国家/地区值分配。

   b. 对于帐户中的基于查找的国家/地区代码字段：

   - 在帐户中添加新的自定义字段并使用两个字母的国家/地区代码自动填充它 (ISO 3166) 基于基于查找的字段中选择的值，反之亦然。

   - 对于非查找国家/地区代码字段，请按照上述步骤将新的自定义字段从 CRM 同步到合作伙伴中心。

- 机会字段：如果存在需要填充的商机中的必填字段，则编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息**  ，并导航到 "在 CRM 中 **创建或更新机会** " 和 "更新" " **创建新机会" 操作** ，以根据业务要求向必填字段分配值。

- 潜在客户字段：如果潜在顾客需要填充，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息**  ，并导航到 **创建或更新** CRM 中的潜在客户，并更新 **创建新的潜在客户操作** ，根据业务需求将值分配到必填字段。

- 客户帐户：如果新的引用从合作伙伴中心同步到 CRM，则 Power 自动解决方案将尝试使用客户公司名称和邮政编码搜索 CRM 中的现有帐户。 如果找不到，将在 CRM 中创建新的客户帐户。 若要更新搜索条件和创建新帐户的详细信息，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息** ，然后导航到 **创建或获取** CRM 中的客户帐户并 **创建客户帐户操作**。

## <a name="update-environment-variable"></a>更新环境变量

更新环境变量值：

1. 单击 " **解决方案** " 页，然后选择 " **默认解决方案**"。 通过单击 "全部" 选择 **环境变量** 。

2. 为需要更新的值选择环境变量，然后单击 "使用三个点图标 **编辑** " 图标。

3. 更新 **当前值** (不要使用 **新值** 选项更新默认值) 并提供值。 值必须与变量的数据类型相匹配，例如 Yes/No 数据类型将接受 Yes 或 No 值。

   :::image type="content" source="images/environment-variables-video.gif" alt-text="更新环境变量":::

- 端到端双向共同销售引用同步

安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 和合作伙伴中心之间的共同销售引用同步。

### <a name="pre-requisites"></a>先决条件

若要跨伙伴中心和 Dynamics 365 CRM 同步引用，Power 自动化解决方案可以清晰地划分 Microsoft 特定的引用字段。 此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。

一组自定义字段和对象将作为解决方案安装的一部分添加。 CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。

以下自定义字段应为 CRM 部分的一部分：

- **与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步。 默认情况下，此字段的值为 "否"，并且你的卖方需要将其显式设置为 "是"，以便与 Microsoft 共享机会。 从合作伙伴中心到 CRM 共享的新引用将此字段值设置为 "是"。

- **引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段

- **引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接
- **Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助。 若要创建共同销售引用，请选择 Microsoft 所需的适当帮助。 必须将客户联系人关联到创建共同销售引用的机会。 若要创建非共同销售引用，请将此字段取消选中状态。 通过选择相应的 "必需帮助" 选项，可以随时将非共同销售引用转换为共同销售引用。

- **Microsoft 合作伙伴中心引用可见性**：选择 Microsoft 合作伙伴中心引用的可见性。 通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。 如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会看到引用。 标记为可见后，此字段将无法还原。

- **MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。

- **产品：已过时** –不要使用此字段或将其添加到 CRM 部分，仅可用于向后兼容性。 改为使用 Microsoft 合作伙伴中心解决方案。

- **Audit**：与合作伙伴中心引用同步的只读审核记录

- **Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。 可以在商机中添加和/或删除一个或多个解决方案。 在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。 若要将此对象与商机关联，请在 CRM 中更新商机窗体：

  选择 "机会窗体" 中适当的选项卡，并添加子网格，如下所示：

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="机会窗体":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::

- 添加 Microsoft 解决方案后，你可以预先填充联合销售就绪解决方案的详细信息，以便你的卖方不必添加它们。 若要添加新的解决方案详细信息，请前往 CRM 中的 Microsoft 解决方案详细信息对象，然后单击 " **添加记录** " 添加一个条目或使用 **Excel 上传** 添加多个条目。

  :::image type="content" source="images/dynamic-1a.png" alt-text="解决方案详细信息":::

### <a name="scenarios"></a>方案：

1. 在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：

   1. 在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。

   2. 确保在 Dynamics 365 环境中创建 "新机会" 时出现 Microsoft 合作伙伴中心部分

   :::image type="content" source="images/dynamic-2a.png" alt-text="新机会"::: 

   3. 若要将此机会与合作伙伴中心同步，请确保在卡片视图中设置以下字段：

      - **Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。

         :::image type="content" source="images/dynamic-3a.png" alt-text="如何在卡片视图中获取相应的字段":::

      - **客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。

      - **与合作伙伴中心同步**：是

      - Microsoft 解决方案：若要与 Microsoft 共享引用，请向商机添加有效的合作销售就绪或 Microsoft 解决方案。
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="解决方案 ID":::

   4. 一旦在 Dynamics 365 中创建了商机，并将 "伙伴中心同步" 选项设置为 "是"，请等待10分钟，然后登录到合作伙伴中心帐户。 你的引用将与 Dynamics 365 和引用标识符同步。 将填充引用链接。 如果失败，将使用错误信息填充审核字段。
     
    5. 同样，如果将 "与合作伙伴中心同步" 选项设置为 "是"，则在 Dynamics 365 CRM 中更新此机会时，所做的更改将在你的合作伙伴中心帐户中同步。

    6. 与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。

2. 引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：

   1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。

   2. 从左侧菜单中选择 " **引用** "。

   3. 通过选择 "  **新建交易** " 选项，从合作伙伴中心创建新的共同销售引用。

   4. 登录到 Dynamics 365 CRM 环境。

   5. 导航到 " **开放式机会**"。 现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。

   6. 选择同步的引用时，将填充卡片视图详细信息。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)

- [有关 Microsoft Power 自动化平台的详细信息？](/power-automate/)

- [合作伙伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
