---
title: Dynamics 365 CRM 合作伙伴中心的共同销售连接器
description: 将合作伙伴中心中的引用与 Dynamics 365 CRM 的共同销售连接器同步。 然后，你可以在 CRM 系统中与 Microsoft 进行共同销售。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 035a819020097ddee2230b5541e1b477d4b34c14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148459"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>用于 Dynamics 365 CRM 概述的共同销售连接器

**适当的角色**：引用管理 |CRM 上的系统管理员或系统定制员

合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。 他们无需定型即可使用合作伙伴中心来管理共同销售交易。 使用共同销售连接器创建新的共同销售的参考，以与 Microsoft 卖方联系、接收来自 Microsoft 卖方的引用、接受或拒绝推荐，并修改交易数据（如交易价值和结束日期）。 你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。 你可以在所选的 CRM 中（而不是在合作伙伴中心）管理你的所有引用。

此解决方案基于电源自动化，并使用合作伙伴中心 Api。

## <a name="prerequisites"></a>先决条件

在安装解决方案之前，请确保满足以下先决条件。

|**主题**   |**详细信息**   |**链接**   |
|--------------|--------------------|------|
|Microsoft 合作伙伴网络 (MPN) ID |需要一个有效的 MPN ID。|[加入合作伙伴网络](https://partner.microsoft.com/)|
|已做好联合销售准备|你的 IP/服务解决方案必须共同销售。|[与 Microsoft 一起销售](https://partner.microsoft.com/membership/sell-with-microsoft)|
|合作伙伴中心帐户|与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。 在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。|[管理帐户](create-user-accounts-and-set-permissions.md)|
|合作伙伴中心用户角色|将安装和使用连接器的员工必须是推荐管理员。|[为用户分配角色和权限](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|CRM 用户角色是"系统管理员"或"系统定制员"。|[在 Dynamics 365 中分配角色](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate流帐户|使用数据库创建新的生产环境，用于测试、暂存和生产。 如果有包含数据库的现有生产环境，可以重复使用它。 要安装连接器解决方案的用户必须具有此Power Automate和访问权限。 如果安装失败，可以监视进度 [，Power Automate](https://flow.microsoft.com/) 获取详细信息。 在"**解决方案"下选择"** 查看 **历史记录"。**|[创建或管理环境](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>安装合作伙伴中心 Dynamics 365 (Power Automate解决方案) 

1. 转到[Power Automate"，](https://flow.microsoft.com)然后选择右上角的"环境"。 此步骤将显示可用的 CRM 实例。

1. 从右上角的下拉列表中选择相应的 CRM 实例。

1. 选择 **左侧** 的"解决方案"。

1. 选择顶部 **菜单上的"打开 AppSource"** 链接。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="显示 Open AppSource 的屏幕截图。":::

1. 在合作伙伴中心屏幕中搜索 **Dynamics 365** 的推荐连接器。  

1. 选择"**现在获取"** 按钮，然后选择"继续 **"。**

1. 将出现一个页面，可在其中选择 DYNAMICs 365 (环境) CRM 应用程序。 同意条款和条件。

1. 可以监视进度，如果安装失败，可以通过选择"解决方案"下的"查看历史记录Power Automate **获取详细信息****。**

1. 安装完成后，返回到"Power Automate [并选择左侧](https://flow.microsoft.com)**的"** 解决方案"。 合作伙伴中心解决方案列表中现提供 **Dynamics 365** 的推荐 **同步**。

1. 选择 **合作伙伴中心 Dynamics 365 的推荐同步"**。 以下Power Automate流和实体可用。

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="显示可用 CCR 的屏幕截图。":::

## <a name="test-before-you-go-live"></a>上台前进行测试

在生产环境中安装、配置Power Automate自定义解决方案之前，请务必在过渡 CRM 实例上测试该解决方案。 你将需要：

- 在Power Automate CRM 实例上安装 Power Automate 解决方案。
- 在过渡Power Automate配置和自定义解决方案。
- 在过渡 CRM 实例上测试解决方案。
- 成功测试后，作为托管解决方案导入到生产实例。

## <a name="configure-the-solution"></a>配置解决方案

1. 在 CRM 实例中安装解决方案后，返回到[Power Automate。](https://flow.microsoft.com/)

1. 从 **右上角** 的"环境"下拉列表中，选择安装了 Power Automate 解决方案的 CRM 实例。

1. 需要创建关联三个用户帐户的连接：

   - 合作伙伴中心引荐管理员凭据的用户
   - 合作伙伴中心事件
   - 具有解决方案中Power Automate流的 CRM 管理员

   1. 选择 **左侧** 的"连接"，然后从 **合作伙伴中心选择"** 引荐"解决方案。

   1. 通过选择"创建连接 **"创建连接**。

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="显示&quot;创建连接&quot;的屏幕截图。":::

   1. 在右上角的搜索栏中搜索 " **合作伙伴中心引用 (预览")** 。

   1. 使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。

   1. 接下来，使用 "引用管理员" 凭据为合作伙伴中心用户创建合作伙伴中心事件连接。

   1. 为 CRM 管理员用户的 Common Data Service (当前环境) 创建连接。
     
   1. 添加所有连接后，你的环境中应会显示以下连接。

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="显示连接的屏幕截图。":::

## <a name="edit-the-connections"></a>编辑连接

1. 返回 " **解决方案** " 页，选择 " **默认解决方案**"。 通过选择 "**全部**" **(预览) 选择 "连接引用**"。

   :::image type="content" source="images/connection-reference-video.gif" alt-text="显示编辑连接的屏幕截图。":::

1. 通过选择省略号图标，分别编辑每个连接。 添加相关连接。

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="显示连接的屏幕截图。":::

1.  返回到 " **解决方案** " 页，选择 **Dynamics 365 的 "合作伙伴中心引用同步**"，并通过选择以下序列中每个流旁边的省略号图标来打开流。 如果在打开流时遇到任何问题，请参阅 [自定义步骤](connector-dynamics.md#customize-synchronization-steps) 和 [故障排除步骤](connectors-troubleshoot.md)。

按以下顺序打开流：

-  (内幕预览版) 合作伙伴中心 Webhook 注册
- 创建共同销售引用– Dynamics 365 到合作伙伴中心 (预览体验中心) 
- 来自创建或获取 Dynamics 365 流中的详细信息
- 合作伙伴中心到 Dynamics 365-Helper (预览体验中心) 
- 合作伙伴中心 Microsoft 联合销售 Dynamics 365 (Insider Preview) 
- 合作伙伴中心 Dynamics 365 (Insider Preview) 
- Dynamics 365 合作伙伴中心 (Insider Preview) 
- Dynamics 365 预览体验合作伙伴中心 (预览版) 
- Dynamics 365 Microsoft Solutions to 合作伙伴中心 (Insider Preview) 
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook API 注册资源更改事件

可以使用 webhook 合作伙伴中心注册资源更改事件。 这些更改事件作为 HTTP 帖子发送到 URL。

1. 选择 **合作伙伴中心 Dynamics 365 (Insider Preview) "**。

1. 选择"**编辑"** 图标，然后选择 **"收到 HTTP 请求时"。**

1. 选择" **复制"** 图标以复制提供的 HTTP POST URL。

   :::image type="content" source="images/webhook-video.gif" alt-text="显示使用 Webhook 注册资源更改的屏幕截图。":::

1. 选择 **"合作伙伴中心预览 (预览版) Power Automate Webhook** 注册"，然后选择"运行 **"。**

1. 确保在右 **窗格中打开"运行** 流"窗口，然后选择"继续 **"。**

1. 输入以下详细信息：

   - **Http 触发器终结点**：此 URL 是从前面步骤复制的。
   - **要注册的事件**：选择所有可用事件 (引用 **创建**、引荐更新、**相关** 引荐创建以及相关引荐 **更新**) 。
   - **覆盖现有的触发器终结点（如果存在）？：** 是。 只能为给定的 Webhook 事件注册一个 URL。

1. 选择 **"运行流**"，然后选择" **完成"。**

Webhook 现在可以侦听、创建和更新事件。

## <a name="customize-synchronization-steps"></a>自定义同步步骤

CRM 系统经过高度自定义，你可以基于 CRM 设置自定义电源自动化解决方案。 当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，在 " [自定义字段映射指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)" 中列出了在合作伙伴中心电脑上同步的字段。

按照字段映射指南进行操作，如有必要，请在 **[自定义] 创建或获取 Dynamics 365 flow** 或环境变量的详细信息。 请勿更新 Power 自动化解决方案中的任何其他流，因为它可能会影响将来的解决方案升级。

提供下列自定义项：

- **显示机会名称中的复选标记**：默认情况下，机会名称旁边将显示一个复选标记，指示在合作伙伴中心与 DYNAMICS 365 CRM 之间的同步成功发生。 同样，如果同步失败，将显示交叉标记。 若要避免在机会名称中添加复选标记或交叉标记，请将 **机会 name 环境变量中显示复选标记** 的当前值设置为 "否"。
- **交易价值**：默认情况下，来自合作伙伴中心的交易值将与 CRM 中的 **estimatedvalue** 同步。 如果 CRM 中有其他字段要从中同步交易值：

  - 用 CRM 的字段名称更新 Dynamics 365 环境变量中的 " **交易值** " 字段名称。 请确保提供字段名称，而不是其显示名称。
  - 编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**，转到 **创建或更新** crm 中的机会，更新 **创建新机会** 并 **更新现有机会** 操作，将 **DealValue** 值分配到 CRM 中的正确字段。 同时，从 "**估计收入**" 字段中删除 **DealValue** 分配。

- **客户帐户国家/地区代码**：创建新引用时，必须提供两个字母的国家/地区代码 (ISO 3166) 。 默认情况下，国家/地区代码将与 CRM 中帐户的 **address1_country** 字段同步。 如果 CRM 中的 "国家/地区代码" 字段不同，则：

   - 对于包含两个字母代码的帐户中的 nonlookup "国家/地区代码" 字段：
     - 将 Dynamics 365 环境变量中的 **客户帐户 "国家/地区代码** " 字段名称更新为 CRM 的字段名称。 请确保提供字段名称，而不是其显示名称。
     - 编辑 **[自定义] 创建或获取 Dynamics 365 flow 的详细信息**，然后转到 **创建或获取** crm 操作中的客户帐户，将 **国家/地区** 值分配给 crm 中的正确字段。 同时，从 "**地址1：国家/地区**" 字段中删除 **国家**/地区值分配。

   - 对于帐户中的基于查找的国家/地区代码字段：
     - 在帐户中添加新的自定义字段，并使用两个字母的国家/地区代码自动填充该字段 (ISO 3166) 基于在查找字段中选择的值，反之亦然。
     - 按照前面的步骤为 nonlookup "国家/地区代码" 字段，将新的自定义字段从 CRM 同步到合作伙伴中心。

- **机会字段**：如果存在需要填充的 **机会** 中的必填字段，请编辑 **[自定义] 创建或获取来自 Dynamics 365 flow 的详细信息** ，然后转到 CRM 中的 " **创建" 或 "更新机会** "，然后根据您的业务要求，"更新 **创建新的机会" 操作** 以将值分配到必填字段。
- **潜在顾客字段**：如果 **lead** 中有需要填充的必填字段，请编辑 **[自定义] 创建或获取 Dynamics 365 流中的详细信息** ，然后转到 **创建或更新** CRM 中的潜在客户，并更新 **创建新的潜在客户操作** ，根据业务需求将值分配到必填字段。
- **客户帐户**：将新引荐从 合作伙伴中心 同步到 CRM 时，Power Automate 解决方案会尝试使用客户公司名称和邮政编码在 CRM 中搜索现有帐户。 如果找不到帐户，将在 CRM 中创建一个新的客户帐户。 若要更新搜索条件以及新帐户创建详细信息，请编辑 **[自定义] 从 Dynamics 365** 流创建或获取详细信息，然后转到在 CRM 中创建或获取客户帐户和 **创建客户帐户操作**。

## <a name="update-environment-variable"></a>更新环境变量

更新环境变量值：

1. 转到"解决方案 **"页**，然后选择"**默认解决方案"。** 选择 **"所有"，** 选择"环境 **变量"。**

1. 为需要更新的值选择环境变量，然后使用省略号图标选择"编辑"。

1. 更新 **当前 (** 不通过使用"新建值") 提供值来更新默认值值。  值必须与变量的数据类型匹配。 例如，"是"或"否"数据类型将接受"是"或"否"值。

   :::image type="content" source="images/environment-variables-video.gif" alt-text="显示&quot;更新环境变量&quot;的屏幕截图。":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>端到端双向联合销售引荐同步

安装、配置和自定义 Power Automate 解决方案后，可以测试 Dynamics 365 和 合作伙伴中心 之间的联合销售引荐同步。

### <a name="prerequisites"></a>先决条件

为了跨 合作伙伴中心 和 Dynamics 365 CRM 同步引荐，Power Automate解决方案明确划分了特定于 Microsoft 的引荐字段。 此标识使卖方团队能够决定要与 Microsoft 共享哪些引荐进行联合销售。

将在解决方案安装过程中添加一组自定义字段和对象。 CRM 管理员用户需要创建包含"机会"自定义字段 **的单独** CRM 部分。

以下自定义字段应是 CRM 部分的一部分：

- **与合作伙伴中心同步**：是否要将此机会与合作伙伴中心同步。 默认情况下，此字段的值为 "否"，并且你的卖方需要将其显式设置为 "是"，以便与 Microsoft 共享机会。 从合作伙伴中心到 CRM 共享的新引用将此字段值设置为 "是"。
- **引用标识符**：合作伙伴中心引用的只读标识符字段。
- **引用链接**：指向合作伙伴中心中的引用的只读链接。
- **Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助。 若要创建共同销售引用，请选择 Microsoft 所需的适当帮助。 必须将客户联系人关联到创建共同销售引用的机会。 若要创建非共同销售引用，请不要选择此字段。 通过选择适当的帮助-必需选项，可以随时将非共同销售引用转换为共同销售引用。
- **Microsoft 合作伙伴中心引用可见性**：选择合作伙伴中心引用的可见性。 通过使其对 Microsoft 卖方可见，非共同销售的引用可能会转换为共同销售。 如果需要 Microsoft 帮助，则默认情况下，Microsoft 卖方会显示该引用。 将此字段标记为可见后，将无法还原它。
- **MICROSOFT CRM 标识符**：当 microsoft 创建并接受共同销售引用时，此字段将填充 MICROSOFT 的 CRM 标识符。
- **产品：已过时**：请勿使用此字段或将其添加到 CRM 部分。 它仅可用于向后兼容。 请改用合作伙伴中心解决方案。
- **Audit**：与合作伙伴中心引用同步的只读审核记录。
- **Microsoft 合作伙伴中心解决方案**：一个自定义对象，用于将共同销售的现成解决方案或 Microsoft 解决方案与机会关联起来。 可以在商机中添加或删除一个或多个解决方案。 在与 Microsoft 共享之前，必须至少向此机会添加一个共同销售就绪或 Microsoft 解决方案。 若要将此对象与商机关联，请在 CRM 中更新 **商机** 窗体。

  选择 " **机会** " 窗体上的相应选项卡，并添加子网格，如下所示。

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="显示机会窗体的屏幕截图。":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="显示 Microsoft 解决方案的屏幕截图。":::

- 添加 Microsoft 解决方案后，你可以预填充联合销售就绪解决方案详细信息，以便你的卖方不必添加它们。 若要添加新的解决方案详细信息，请前往 CRM 中的 Microsoft 解决方案详细信息对象，然后选择 " **添加记录** " 以添加一个条目或使用 **Excel 上传** 添加多个条目。

  :::image type="content" source="images/dynamic-1a.png" alt-text="显示新的 Microsoft 解决方案详细信息的屏幕截图。":::

### <a name="scenarios"></a>方案

1. 在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：

   1. 在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。

   1. 在 Dynamics 365 环境中创建新机会时，请确保 **Microsoft 合作伙伴中心** 部分存在。

      :::image type="content" source="images/dynamic-2a.png" alt-text="显示新机会的屏幕截图。":::

   1. 若要将此机会与合作伙伴中心同步，请确保在卡片视图中设置以下字段：

      - **Microsoft 如何帮助？**：若要创建共同销售引用，请选择适当的帮助选项。

         :::image type="content" source="images/dynamic-3a.png" alt-text="显示如何在卡片视图中获取相应字段的屏幕截图。":::

      - **客户联系人**：若要创建共同销售引用，请将客户联系人添加到机会。
      - **与合作伙伴中心同步**：是。
      - **Microsoft 解决方案**：若要与 microsoft 共享引用，请向此机会添加有效的合作销售就绪或 Microsoft 解决方案。
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="显示解决方案 ID 的屏幕截图。":::

   1. 在 Dynamics 365 中创建机会后，将"与 合作伙伴中心 同步"选项设置为 **"是** ，等待 10 分钟"。 然后登录到你的合作伙伴中心帐户。 引荐将与 Dynamics 365 和引 **荐标识符 同步**。 **将填充** 引荐链接。 如果失败，"审核"字段将填充错误信息。
     
    1. 同样，对于将"与 **合作伙伴中心** 同步"选项设置为"是"的机会，如果在 Dynamics 365 CRM 中更新机会，所做的更改将在 合作伙伴中心 帐户中同步。

    1. 成功与 合作伙伴中心 同步的机会将在 Dynamics 365 ✔通过 ✔icon 进行标识。

1. 在 Dynamics 365 环境中合作伙伴中心或更新引荐时进行引荐同步：

   1. 登录到 合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。

   1. 从 **左侧菜单中** 选择"引荐"。

   1. 通过选择"新建交易"合作伙伴中心新建联合 **销售** 引荐。

   1. 登录到 Dynamics 365 CRM 环境。

   1. 转到"**打开机会"。** 现在，在 合作伙伴中心 中创建的引荐在 Dynamics 365 CRM 中同步。

   1. 选择同步的引荐时，将填充卡片视图详细信息。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)
- [管理联合销售机会](manage-co-sell-opportunities.md)
- [有关 Microsoft Power Automate 平台](/power-automate/)
- [合作伙伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
