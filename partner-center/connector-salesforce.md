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
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148408"
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
|Salesforce CRM|CRM 用户角色是系统管理员或系统定制员|[在 Salesforce CRM 中分配角色](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power 自动化 Flow 帐户|CRM 系统管理员或系统定制员的有效 [电源自动完成](https://flow.microsoft.com) 帐户。 在安装之前，该用户至少应登录到一次 [电源](https://flow.microsoft.com) 。|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>为 Microsoft 自定义字段安装 Salesforce 包 

若要跨合作伙伴中心和 Salesforce CRM 同步检索，自动解决解决方案需要清楚地识别特定于 Microsoft 的引用字段。 此分界为合作伙伴卖方团队提供了决定他们要与 Microsoft 共享以共同销售的推荐的功能。

1. 在 Salesforce 中，激活 **注释** 并将其添加到机会相关列表。 
[引用](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. 按照以下步骤激活 **机会团队** ： 
    - 在安装程序中，使用 " **快速查找** " 框定位机会团队设置。
    - 根据需要定义设置。
[引用](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. 在 Salesforce 中，使用 [包安装程序](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)安装自定义字段和对象。 使用此可将包安装到任何公司。

>[!NOTE]
>如果要安装到沙盒，则必须将 URL 的初始部分替换为 http://test.salesforce.com

4. 在 Salesforce 中，将 Microsoft 解决方案添加到 **机会** 相关列表。 添加后，选择 **扳手** 图标并更新属性

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在上线之前进行测试

在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。

- 在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。

- 创建解决方案的副本，在过渡Power Automate运行配置和流自定义。

- 在过渡/CRM 实例上测试解决方案。

- 成功后，作为托管解决方案导入到生产实例。

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>安装合作伙伴中心 Salesforce CRM 的推荐同步

1. 转到 [Power Automate，](https://flow.microsoft.com)**然后选择右上角** 的"环境"。 此时会显示可用的 CRM 实例。

2. 从右上角的下拉列表中选择相应的 CRM 实例。

3. 在 **左侧** 导航栏中选择"解决方案"。

4. 选择顶部 **菜单上的"打开 AppSource"** 链接。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="打开 AppSource":::

5. 在 **合作伙伴中心屏幕中搜索 Salesforce** 的推荐连接器。  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. 选择"**现在获取"按钮**，然后选择"**继续"。**

7. 这将打开一个页面，可在其中选择要安装应用程序的 Salesforce CRM 环境。  同意条款和条件。

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用的 CRMS":::

8. 然后，你被定向到 **"管理解决方案"页** 。  使用页面底部的箭头按钮导航到"合作伙伴中心引用"。 **计划的安装** 应显示在"引荐合作伙伴中心旁边。 安装需要 10-15 分钟。

9. 安装完成后，导航回 [Power Automate左侧导航](https://flow.microsoft.com) 区域中 **选择"解决方案** "。 请注意，"解决方案" 列表中提供了 **Salesforce 的合作伙伴中心引用同步** 。

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

2. 通过选择三个点图标单独编辑每个连接。 添加相关连接。

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="编辑连接器":::

3. 按以下顺序打开流：

- 合作伙伴中心预览体验版 (Webhook 注册) 
- 创建联合销售引荐 - Salesforce 合作伙伴中心 (Insider Preview) 
- 合作伙伴中心 Microsoft 联合销售 Salesforce (Insider Preview) 
- 合作伙伴中心 Insider Preview (Salesforce) 
- Salesforce 合作伙伴中心 (Insider Preview) 
- Salesforce 预览体验合作伙伴中心 (预览版) 
- Salesforce Microsoft Solutions to 合作伙伴中心 (Insider Preview) 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook API 注册资源更改事件

使用合作伙伴中心 Webhook API 可以注册资源更改事件。 这些更改事件作为 HTTP 帖子发送到 URL。

1. 若要注册 URL，请选择"合作伙伴中心 **Webhook 注册 (预览体验) Power Automate** 流。

2. 使用引荐管理员凭据 (a.) 合作伙伴中心 用户添加连接， (b.) 合作伙伴中心 Events，如下所示

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="触发器":::

3. 进行这些更新时，你将看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 保存更改，然后选择"**启用"。**

   若要合作伙伴中心 Webhook 侦听事件更改，请执行以下步骤：

5. 选择 " **合作伙伴中心到 SALESFORCE CRM (内幕预览版")**。

6. 选择 " **编辑** " 图标，然后选择 " **收到 HTTP 请求时**"。

7. 选择 **复制** 图标以复制提供的 HTTP POST URL。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="复制 URL":::

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

   2. 选择 **"** 编辑"以编辑/自定义Power Automate流。

   3. 选择 **(范围) 同步潜在顾客或商机"**。

2. 若要自定义用于创建事件的 CRM 字段映射，请选择 **"如果是新的共享机会**"，然后选择 。 选择子步骤（**如果是），然后在** CRM 中展开"**创建新机会"。** 可以使用字段映射指南编辑本部分中的映射。

   1. 若要自定义更新事件的 CRM 字段映射，请选择"同步潜在顾客 (机会) 范围"步骤。

   2. 选择 **"如果是机会更新"，然后选择**。 选择子步骤 **（如果是），然后** 展开"如果机会对象与 CRM 中的机会对象 **合作伙伴中心差异"，然后展开**。  

   3. 选择 **"如果是"，** 然后选择" **更新现有机会"**

3. 若要自定义用于更新事件的 CRM 到电脑引荐同步的字段，请执行以下操作：

   1. 选择 **"**  编辑"以编辑/自定义Power Automate流。

   2. 选择 **(") 同步机会"。**

   3. 要根据字段映射指南 (自定义 CRM 字段映射) 更新事件，请选择"如果 合作伙伴中心 和 CRM 中的潜在顾客对象存在差异，然后选择 **""。**

   4. 选择子步骤（ **如果是）然后** 展开"使用机会数据 **更新引荐"步骤**。

   可以基于字段映射指南编辑本部分中的映射。

4. 若要为创建事件自定义 CRM 到电脑引荐同步的字段？

   1. 选择 **"**  编辑"以编辑/自定义Power Automate流。

   2. 选择 **(范围) 同步引荐" 。**

   3. 若要根据用于创建事件的字段映射 (自定义 CRM 字段映射) ，请选择"创建 Microsoft 引 **荐"。**

可以基于字段映射指南编辑本部分中的映射。


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
       - "Microsoft 如何提供帮助？"：从以下选项中进行选择：
       - 产品：产品的解决方案 ID

   4. 将机会"与合作伙伴中心同步"选项 **设置为"是**"后，请等待 10 分钟，登录到合作伙伴中心帐户。 引荐将与 Salesforce CRM 同步。

   5. 当"与 合作伙伴中心 同步"选项设置为"是"时，如果在 Salesforce CRM 中更新机会，所做的更改将与你的 合作伙伴中心 同步。

   6. 在 Salesforce CRM 中，合作伙伴中心与 ✔同步的机会。

2. 在 Microsoft 中创建或更新引荐时进行引荐同步合作伙伴中心 Salesforce CRM 环境中同步：

    1. 登录到 合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/home)。

    2. 从 **左侧菜单中** 选择"引荐"。

    3. 单击"新建交易"选项，从合作伙伴中心新建联合销售引荐。

    4. 登录到 Salesforce CRM 环境。

    5. 导航到"**打开机会"。** 在 Microsoft 合作伙伴中心创建的引荐现在在 Salesforce CRM 中同步。

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 机会屏幕":::

    6. 选择同步的引荐时，将填充卡片视图详细信息。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)

- [合作伙伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
