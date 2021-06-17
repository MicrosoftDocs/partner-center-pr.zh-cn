---
title: Salesforce CRM 合作伙伴中心 联合销售连接器
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将你的引荐合作伙伴中心 Salesforce CRM 同步。 然后，销售人员可以从 CRM 系统内部与 Microsoft 联合销售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276971"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>用于 Salesforce CRM 的联合销售连接器 – 概述

**适当的角色**：引荐管理员|CRM 上的系统管理员或系统定制员

合作伙伴中心联合销售连接器可让销售人员从 CRM 系统内部与 Microsoft 联合销售。 他们不需要经过训练，就可使用合作伙伴中心联合销售交易。 使用联合销售连接器，可以创建一个新的联合销售引荐来吸引 Microsoft 销售人员、接收来自 Microsoft 卖方的引荐、接受/拒绝引荐、修改交易数据（例如交易值）和结束日期。  还可以从 Microsoft 卖方处收到有关这些联合销售交易的任何更新。 可以在你选择的 CRM 中工作，而不是在自己选择的 CRM 中工作，而不是在 合作伙伴中心。 

该解决方案基于 Microsoft Power Automate 解决方案，并使用 合作伙伴中心 API。

## <a name="before-you-install---pre-requisites"></a>安装前 - 先决条件

|**主题**   |**详细信息**   |**链接**   |
|--------------|--------------------|------|
|Microsoft 合作伙伴网络 ID |需要有效的 MPN ID|加入 [MPN](https://partner.microsoft.com/)|
|已做好联合销售准备|IP/服务解决方案必须可供联合销售。|[与 Microsoft 一起销售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作伙伴中心帐户|与联合销售合作伙伴中心关联的 MPN ID 必须与与联合销售解决方案关联的 MPN ID 相同。 在部署连接器之前，请验证是否可在 合作伙伴中心门户中查看联合销售引荐。|[管理帐户](create-user-accounts-and-set-permissions.md)|
|合作伙伴中心用户角色|将安装和使用连接器的员工必须是引荐管理员|[为用户分配角色和权限](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 用户角色为"系统管理员"或"系统定制员"|[在 Salesforce CRM 中分配角色](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow 帐户|CRM [Power Automate](https://flow.microsoft.com) 或系统定制员的活动帐户。 该用户应在安装 [Power Automate](https://flow.microsoft.com) 至少登录一次。|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>安装 Microsoft 自定义字段的 Salesforce 包 

若要跨 合作伙伴中心 Salesforce CRM 同步引荐，Power Automate解决方案需要明确标识 Microsoft 特定的引荐字段。 合作伙伴销售人员团队能够决定要与 Microsoft 共享哪些引荐进行联合销售。

1. 在 Salesforce 中，激活 **"** 备注"，并将其添加到与商机相关的列表中。 
[引用](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. 按照 **以下步骤** 激活机会团队： 
    - 在"设置"中，使用" **快速查找** "框查找"机会团队设置"。
    - 根据需要定义设置。
[引用](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. 在 Salesforce 中，使用包安装程序 安装 [自定义字段和对象](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)。 使用此包将包安装到任何公司。

>[!NOTE]
>如果要安装到沙盒中，则必须将 URL 的初始部分替换为 http://test.salesforce.com

4. 在 Salesforce 中，将 Microsoft Solutions 添加到 **"机会相关"** 列表。 添加后，选择 **手部** 图标并更新属性

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在上台之前进行测试

在生产环境中安装、配置Power Automate自定义解决方案之前，请务必在过渡 CRM 实例上测试该解决方案。

- 在Power Automate/CRM 实例上安装 Microsoft Power Automate 解决方案。

- 创建解决方案的副本，在过渡Power Automate运行配置和流自定义。

- 在过渡/CRM 实例上测试解决方案。

- 成功后，作为托管解决方案导入到生产实例。

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>安装合作伙伴中心 Salesforce CRM 的推荐同步

1. 转到 [Power Automate，](https://flow.microsoft.com)**然后选择右上角** 的"环境"。 此时会显示可用的 CRM 实例。

2. 从右上角的下拉列表中选择相应的 CRM 实例。

3. 在 **左侧** 导航栏中选择"解决方案"。

4. 选择顶部 **菜单上的"打开 AppSource"** 链接。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource。":::

5. 在 **合作伙伴中心屏幕中搜索 Salesforce** 的推荐连接器。  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce。":::

6. 选择"**现在获取"按钮**，然后选择"**继续"。**

7. 这将打开一个页面，可在其中选择要安装应用程序的 Salesforce CRM 环境。  同意条款和条件。

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用的 CRMS。":::

8. 然后，你被定向到 **"管理解决方案"页** 。  使用页面底部的箭头按钮导航到"合作伙伴中心引用"。 **计划的安装** 应显示在"引荐合作伙伴中心旁边。 安装需要 10-15 分钟。

9. 安装完成后，导航回 [Power Automate左侧导航](https://flow.microsoft.com) 区域中 **选择"解决方案** "。 请注意 **，合作伙伴中心解决方案列表中提供了 Salesforce** 的推荐同步。

10. 选择 **合作伙伴中心 Salesforce 的引荐同步"**。 以下Power Automate流和实体可用：

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 流。":::



## <a name="configure-the-solution"></a>配置解决方案

1. 在 CRM 实例中安装解决方案后，导航回[Power Automate。](https://flow.microsoft.com/)

2. 从 **右上角** 的"环境"下拉列表中，选择安装了 Power Automate 解决方案的 CRM 实例。
3. 需要创建关联三个用户帐户的连接：
    - 合作伙伴中心管理员凭据的用户
    - 合作伙伴中心事件
    - 具有解决方案Power Automate流的 CRM 管理员。
4. 从 **左侧** 导航栏中选择"连接"，然后从列表中选择"合作伙伴中心推荐"解决方案。

5. 通过单击"创建连接 **"创建连接**。

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="创建连接。":::

- 在合作伙伴中心的 (搜索) 搜索"中，搜索"引荐"和"预览版"。

- 使用引荐管理员合作伙伴中心为用户创建连接。

-  接下来，使用合作伙伴中心管理员的凭据为合作伙伴中心用户创建一个事件连接。

- 为 CRM 管理员用户创建 Salesforce 连接。

-  添加所有连接后，应在环境中看到以下连接：

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="观察连接。":::

### <a name="edit-the-connections"></a>编辑连接

1. 返回到"解决方案"页，然后选择"**默认解决方案"。**  单击 **"所有" (") "****连接引用**"。
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="开始连接器编辑。":::

2. 通过选择三个点图标单独编辑每个连接。 添加相关连接。

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="编辑连接器。":::

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

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="界限.":::

3. 进行这些更新后，你将看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook.":::

4. 保存更改，然后选择 **"打开"**。

   若要启用合作伙伴中心 webhook 来侦听事件更改，请执行以下步骤：

5. 选择 " **合作伙伴中心到 SALESFORCE CRM (内幕预览版")**。

6. 选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。

7. 选择 **复制** 图标以复制提供的 HTTP POST URL。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="复制 URL。":::

8. 现在，选择 "合作伙伴中心 Webhook 注册 (内幕预览版") "Power 自动流"，然后选择 " **运行**"。

9. 确保在右侧窗格中打开 "运行流" 窗口，并选择 " **继续**"。

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

   1. 若要为更新事件自定义 CRM 字段映射，请选择步骤 " (范围) 同步潜在客户或机会"。

   2. **如果是对机会的更新，** 请选择 "是"。 选择 " **是"** ，然后展开 " **如果合作伙伴中心和 CRM 中的机会对象之间的差异"，然后** 展开。  

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

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 环境。":::

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

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 机会屏幕。":::

    6. 选择同步的引用时，将填充卡片视图详细信息。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)

- [合作伙伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
