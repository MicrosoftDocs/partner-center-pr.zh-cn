---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将合作伙伴中心的推荐与 Salesforce CRM 同步。 然后，卖方可以在 CRM 系统中与 Microsoft 进行共同销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 68b8bdf7a88c1ca8d063cf3198fc49bf87552edb
ms.sourcegitcommit: de2ac2eea26426ae8f962d29ab50b68850318ce6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "97960945"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>用于 Salesforce CRM 的联合销售连接器 – 概述

### <a name="appropriate-roles"></a>相应的角色

- 引荐管理员
- CRM 上的系统管理员或系统定制员

合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。 他们无需定型即可使用合作伙伴中心来管理共同销售交易。 使用共同销售连接器，你可以创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用，接受/拒绝引用，修改交易数据（如交易价值）和结束日期。  你还可以从 Microsoft 卖方接收有关这些共同销售交易的任何更新。 你可以在所选的 CRM 中工作而不是在合作伙伴中心内工作时执行所有引用工作。 

此解决方案基于 Microsoft Power 自动化解决方案，并使用合作伙伴中心 Api。

## <a name="before-you-install---pre-requisites"></a>安装之前-必备组件

|**主题**   |**详细信息**   |**链接**   |
|--------------|--------------------|------|
|Microsoft 合作伙伴网络 ID |需要一个有效的 MPN ID|加入 [MPN](https://partner.microsoft.com/)|
|合作销售就绪|你的 IP/服务解决方案必须共同销售。|[与 Microsoft 一起销售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作伙伴中心帐户|与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。 在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。|[管理帐户](create-user-accounts-and-set-permissions.md)|
|合作伙伴中心用户角色|将安装和使用连接器的员工必须是推荐管理员|[为用户分配角色和权限](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 用户角色是系统管理员或系统定制员|[在 Salesforce CRM 中分配角色](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power 自动化 Flow 帐户|CRM 系统管理员或系统定制员的有效 [电源自动完成](https://flow.microsoft.com) 帐户。 在安装之前，该用户至少应登录到一次 [电源](https://flow.microsoft.com) 。|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>为 Microsoft 自定义字段安装 Salesforce 包 

若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要清楚地识别 Microsoft 特定的引用字段。 此分界为合作伙伴卖方团队提供了决定他们要与 Microsoft 共享以共同销售的推荐的功能。

1. 在 Salesforce 中，激活 **注释** 并将其添加到机会相关列表。 
[引用](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. 按照以下步骤激活 **机会团队** ： 
    - 在安装程序中，使用 " **快速查找** " 框定位机会团队设置。
    - 根据需要定义设置。
[引用](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. 在 Salesforce 中，使用下面的包安装程序安装自定义字段和对象。
  
请访问 [此处](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) ，将包安装到任何公司。


注意：如果要安装到沙盒，则必须将 URL 的初始部分替换为 http://test.salesforce.com

4. 在 Salesforce 中，将 Microsoft 解决方案添加到 **机会** 相关列表。 添加后，单击 **扳手** 图标并更新属性

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在上线之前进行测试

在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。

- 在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。

- 制作解决方案的副本，并在过渡环境中运行配置并对流自定义执行自动操作。

- 在过渡/CRM 实例上测试解决方案。

- 成功后，将作为托管解决方案导入到生产实例。

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>为 Salesforce CRM 安装合作伙伴中心引用同步

1. 请继续 [执行 "电源自动](https://flow.microsoft.com) "，并选择右上角的 " **环境** "。 这会显示可用的 CRM 实例。

2. 从右上角的下拉菜单中选择相应的 CRM 实例。

3. 选择左侧导航栏上的 " **解决方案** "。

4. 单击顶部菜单上的 " **打开 AppSource** " 链接。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. 在弹出屏幕中搜索 Salesforce 的 " **合作伙伴中心引用连接器** "。  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. 单击 " **立即获取** " 按钮，然后 **继续**。

7. 这将打开可在其中选择要安装应用程序的 Salesforce CRM 环境的页面。  同意条款和条件。

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用 CRM":::

8. 然后，你将转到 " **管理你的解决方案** " 页。  通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。 **计划的安装** 应显示在合作伙伴中心引用解决方案旁边。 安装将需要10-15 分钟。

9. 安装完成后，导航回 " [自动启动](https://flow.microsoft.com) "，并从左侧导航区域中选择 " **解决方案** "。 请注意，"解决方案" 列表中提供了 **Salesforce 的合作伙伴中心引用同步** 。

10. **为 Salesforce 选择合作伙伴中心引用同步**。 可以使用以下功能自动执行流和实体：

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 流":::



## <a name="configure-the-solution"></a>配置解决方案

1. 在 CRM 实例中安装解决方案后，请导航回 " [电源自动](https://flow.microsoft.com/)"。

2. 在右上角的 " **环境** " 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。
3. 你将需要创建关联三个用户帐户的连接：
    - 具有引用管理员凭据的合作伙伴中心用户
    - 合作伙伴中心事件
    - CRM 管理员，并在解决方案中自动执行流处理。
4. 从左侧导航栏中选择 " **连接** "，然后从列表中选择 "合作伙伴中心引用" 解决方案。

5. 通过单击 " **创建连接**" 创建连接。

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="创建连接":::

- 在右上角的搜索栏中搜索 "合作伙伴中心引用 (预览") 。

- 使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。

-  接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。

- 为 CRM 管理员用户创建 Salesforce 连接。

-  添加所有连接后，你的环境中应会显示以下连接：

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="观察连接":::

### <a name="edit-the-connections"></a>编辑连接

1. 返回 "解决方案" 页，选择 " **默认解决方案**"。  通过单击 "**全部**" **(预览) 选择 "连接引用**"。
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="开始连接器编辑":::

2. 通过选择三个点图标，逐个编辑每个连接。 添加相关连接。

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="编辑连接器":::

3. 按以下顺序打开流：

-  (内幕预览版) 合作伙伴中心 Webhook 注册
- 创建向合作伙伴中心 (内幕预览版的共同销售推荐-Salesforce) 
- 合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) 
- 合作伙伴中心到 Salesforce (预览体验) 
- Salesforce 到合作伙伴中心 (预览体验) 
- 合作机会到合作伙伴中心 (预览体验) 
- Salesforce Microsoft 解决方案到合作伙伴中心 (预览体验) 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook Api 注册资源更改事件

合作伙伴中心 Webhook Api 允许你注册资源更改事件。 这些更改事件以 HTTP post 的形式发送到你的 url。

1. 若要注册 url，请选择 " **合作伙伴中心 Webhook 注册 (内幕预览版")** Power 自动流 "。

2. 为 (a ) 合作伙伴中心用户添加连接， (b. ) 合作伙伴中心事件如下所示

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="触发器":::

3. 进行这些更新后，你将看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 保存更改，然后选择 **"打开"**。

   若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：

5. 选择 " **合作伙伴中心到 SALESFORCE CRM (内幕预览版")**。

6. 选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。

7. 选择 **复制** 图标以复制提供的 HTTP POST URL。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="复制 URL":::

8. 现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。

9. 确保在右侧窗格中打开 "运行流" 窗口，然后单击 " **继续**"。

10. 输入以下详细信息：

    1. **Http 触发器终结点**：从前面的步骤中复制的 URL

    2. **要注册的事件**： "引用已创建" 和 "引用已更新"

    3. **覆盖现有触发器终结点（如果存在**）：是 (这将覆盖任何现有终结点。 ) 

11. 选择 " **运行** "，然后选择 " **完成"。**

Webhook 现在可以侦听以创建和更新事件。

## <a name="customize-synchronization-steps"></a>自定义同步步骤

当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。

通常，CRM 系统是高度自定义的。 您可以自定义自动执行流的功能。 按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。  我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。

可根据需要自定义每个电源自动流的多个步骤。 下面是可用自定义的示例：

1. 若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：

   1. 选择 "合作伙伴中心到 Salesforce CRM (内幕预览版") 。

   2. 选择 " **编辑** " 以编辑/自定义电源自动流程。

   3. 选择 " **(范围") 同步潜在客户或机会**。

2. 若要为创建事件自定义 CRM 字段映射，请选择 **新的共享机会，然后选择 "是"**。 选择 " **是"** ，然后 **在 CRM 中展开 "创建新机会**"。 您可以使用字段映射指南来编辑此部分中的映射。

   1. 若要为更新事件自定义 CRM 字段映射，请单击步骤 " (范围) 同步潜在客户或机会"。

   2. **如果是对机会的更新，** 请选择 "是"。 **如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后** 展开。  

   3. **如果是，则选择 "是"** ，然后选择 "**更新现有机会**

3. 为更新事件自定义 CRM 到 PC 引用同步的字段：

   1. 选择 " **编辑**  " 以编辑/自定义电源自动流程。

   2. 选择 **(范围) 同步机会**。

   3. 对于 "基于字段映射 (自定义 CRM 字段映射" 指南) 对于 "更新事件"，请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。

   4. **如果是 "是"** ，请选择子步骤，然后展开 "**使用机会数据更新引用**" 步骤。

   您可以根据字段映射指南编辑此部分中的映射。

4. 为创建事件自定义 CRM 到 PC 引用同步的字段？

   1. 选择 " **编辑**  " 以编辑/自定义电源自动流程。

   2. 选择 **) 同步引用 (范围。**

   3. 对于 "基于字段映射自定义 CRM 字段映射 (" 指南) 对于创建事件，请选择 " **创建 Microsoft 引用**"。

您可以根据字段映射指南编辑此部分中的映射。


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>端到端双向共同销售引用同步

安装、配置和自定义电源自动解决方案后，可以测试 Salesforce CRM 与合作伙伴中心之间的共同销售引用同步。

### <a name="pre-requisites"></a>先决条件

若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要明确界定特定于 Microsoft 的引用字段。 此标识使你的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。

一组自定义字段作为 Salesforce CRM 解决方案 **机会** 实体的合作伙伴中心引用同步的一部分提供。 CRM 管理用户需要使用 **机会** 自定义字段创建一个单独的 CRM 部分。

以下自定义字段应为 CRM 部分的一部分：

- **与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步

- **引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段

- **引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接

- **Microsoft 如何帮助**： microsoft 提供的有关推荐的帮助

- **产品**：与此机会关联的产品列表

- **Audit**：与合作伙伴中心引用同步的只读审核记录

### <a name="scenarios"></a>各种

1. 在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：

   1. 在 CRM 的 " **机会** " 部分中具有可见性的用户登录到 Salesforce CRM 环境。

   2. 在 Salesforce CRM 环境中创建 "新机会" 时，请确保以下部分存在

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 环境":::

   3. 若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：

       - "与合作伙伴中心同步"：是
       - "Microsoft help 怎样？"：从以下选项中进行选择：
       - 产品：产品的解决方案 Id

   4. 将 "机会  **与合作伙伴中心同步** " 选项设置为 **"是"** 后，请等待10分钟，登录到合作伙伴中心帐户。 你的引用将与 Salesforce CRM 同步。

   5. 当 "与合作伙伴中心同步" 选项设置为 "是" 时，如果您更新了 Salesforce CRM 中的机会，则这些更改将与合作伙伴中心帐户同步。

   6. 与合作伙伴中心成功同步的机会将用 Salesforce CRM 中的✔图标标识。

2. 引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Salesforce CRM 环境中同步时的同步：

    1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。

    2. 从左侧菜单中选择 " **引用** "。

    3. 单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。

    4. 登录到 Salesforce CRM 环境。

    5. 导航到 " **开放式机会**"。 Microsoft 合作伙伴中心中创建的引用现已在 Salesforce CRM 中同步。

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 机会屏幕":::

    6. 选择同步的引用时，将填充卡片视图详细信息。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)

- [合作伙伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
