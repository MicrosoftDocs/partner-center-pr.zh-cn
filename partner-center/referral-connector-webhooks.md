---
title: 使用 Webhook 获取资源更改事件
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作伙伴中心 Webhook Api 了解 Dynamics 365 CRM 或 Salesforce CRM 何时发生了引用资源更改。
author: sroy
ms.author: sroy
keywords: 引用，webhook api，资源更改事件
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ed7cad26af447302cb0ccd1d8d359ce6b7bbe87f
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949350"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a>使用 Webhook Api 为 Dynamics 365 CRM 和 Salesforce CRM 注册资源更改事件

### <a name="appropriate-roles"></a>相应的角色

- 引荐管理员
- 适用于 Dynamics 365 CRM 或 Salesforce CRM 的系统管理员或系统定制员

合作伙伴中心 Webhook Api 允许你注册资源更改事件。 这些更改事件以 HTTP post 的形式发送到你的 url。

>[!NOTE]
>本主题介绍 Dynamics 365 CRM 和 Salesforce CRM 的 Webhook Api。

## <a name="configure-the-webhook"></a>配置 Webhook

1. 若要注册 url，请选择 "**合作伙伴中心 Webhook 注册" （有问必答预览版）** "电源自动流程"。

2. 为（a）添加连接。具有引用管理员凭据的合作伙伴中心用户（b.）以下突出显示的合作伙伴中心事件

   触发器

3. 进行这些更新后，你将看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 保存更改，然后选择 **"打开"**。

   若要使合作伙伴中心 webhook 能够侦听合作伙伴中心和 CRM 系统中的 IP 共同销售/独立引用对象中的事件更改，请执行以下步骤：

5. 选择 "**合作伙伴中心到 Dynamics 365 （有问必答预览版）** " 或 "**合作伙伴中心到 Salesforce" （有问必答预览版）**。

6. 选择 "**编辑**" 图标，然后选择 "**收到 HTTP 请求时**"。

7. 选择**复制**图标以复制提供的 HTTP POST URL。

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="复制 URL":::

8. 现在，选择 "合作伙伴中心 Webhook 注册（有问必答预览版）" "电源自动流"，然后选择 "**运行**"。

9. 确保在右侧窗格中打开 "运行流" 窗口，然后单击 "**继续**"。

10. 输入以下详细信息：

    1. **Http 触发器终结点**：从前面的步骤中复制的 URL

    2. **要注册的事件**： "引用已创建" 和 "引用已更新"

    3. **覆盖现有触发器终结点（如果存在**）：是（这将覆盖任何现有终结点。）

    Webhook 现在可以侦听更改（创建和更新事件）。

11. 选择 "**运行**"，然后选择 "**完成"。**

## <a name="customize-synchronization-steps"></a>自定义同步步骤

当共同销售的引用在伙伴中心与你的 CRM 系统之间同步时，会在此处列出伙伴中心 PC 上同步的字段。

通常，CRM 系统是高度自定义的。 您可以自定义自动执行流的功能。 按照字段映射指南进行操作，如有必要，可在自动执行流程的步骤中做出适当的更改。  我们提供了 Microsoft 合作伙伴中心到 CRM 的映射，但根据你的 CRM 环境，你可以选择进一步自定义这些字段。

可根据需要自定义每个电源自动流的多个步骤。 下面是可用自定义的示例：

1. 若要自定义用于合作伙伴中心的创建或更新事件的字段以进行 CRM 引用同步，请执行以下操作：

   1. 选择 "合作伙伴中心到 Dynamics 365 （有问必答预览版）" 或 "合作伙伴中心到 Salesforce" （有问必答预览版）。

   2. 选择 "**编辑**" 以编辑/自定义电源自动流程。

   3. 选择 **（作用域）同步潜在客户或机会**。

2. 若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**如果是新的共享机会"，然后选择 "是"**。 **如果是**，请选择 "子步骤"，然后**在 CRM 中展开 "创建新机会**"。 您可以使用字段映射指南来编辑此部分中的映射。

   1. 若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请单击 "（作用域）同步潜在客户或机会" 步骤。

   2. **如果是对机会的更新，** 请选择 "是"。 **如果是 "是"** ，请选择 "子步骤"，然后展开 "**如果伙伴中心和 CRM 中的机会对象之间存在差异"，然后**展开。  

   3. **如果是，则选择 "是"** ，然后选择 "**更新现有机会**

3. 为更新事件自定义 CRM 到 PC 引用同步的字段：

   1. 选择 "**编辑**" 以编辑/自定义电源自动流程。

   2. 选择 **（范围）同步机会**。

   3. 若要为更新事件自定义 CRM 字段映射（基于字段映射指南），请选择 **"合作伙伴中心和 CRM 中的潜在顾客对象之间是否存在差异"，然后**。

   4. **如果是 "是"** ，请选择 "子步骤"，然后展开 "**使用机会数据更新引用**" 步骤。

   您可以根据字段映射指南编辑此部分中的映射。

4. 为创建事件自定义 CRM 到 PC 引用同步的字段？

   1. 选择 "**编辑**" 以编辑/自定义电源自动流程。

   2. 选择 **（作用域）同步引用。**

   3. 若要为创建事件自定义 CRM 字段映射（基于字段映射指南），请选择 "**创建 Microsoft 引用**"。

您可以根据字段映射指南编辑此部分中的映射。

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>端到端双向共同销售引用同步

安装、配置和自定义电源自动解决方案后，可以测试 Dynamics 365 或 Salesforce 与合作伙伴中心之间的共同销售引用同步。

### <a name="pre-requisites"></a>先决条件

若要跨伙伴中心和 Dynamics 365 CRM 或跨合作伙伴中心和 Salesforce CRM 同步检索，自动完成解决方案需要明确界定特定于 Microsoft 的引用字段。 这使您的卖方团队能够确定他们要与 Microsoft 共享哪些推荐以共同销售。

对于 Dynamics 365 解决方案**机会**实体，合作伙伴中心引用同步中提供了一组自定义字段。 CRM 管理用户需要使用**机会**自定义字段创建一个单独的 CRM 部分。

以下自定义字段应为 CRM 部分的一部分：

- **与合作伙伴中心同步**：是否要将此机会与 Microsoft 合作伙伴中心同步

- **引用标识符**： Microsoft 合作伙伴中心引用的只读标识符字段

- **引用链接**：指向 Microsoft 合作伙伴中心中的引用的只读链接

- **Microsoft 如何帮助？**： microsoft 提供的有关引用的帮助

- **产品**：与此机会关联的产品列表

- **Audit**：与合作伙伴中心引用同步的只读审核记录

### <a name="scenarios"></a>各种

1. 在 CRM 中创建或更新引用并在伙伴中心同步时的引用同步：

   1. 在 CRM 的 "**机会**" 部分中具有可见性的用户登录到 DYNAMICS 365 CRM 环境。

   2. 在 Dynamics 365 环境中创建 "新机会" 时，请确保以下部分存在

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="机会":::

   3. 若要将此机会与 Microsoft 合作伙伴中心同步，请确保在卡片视图中设置以下字段：

      - **与合作伙伴中心同步**：是

      - **Microsoft Help 如何？**：选择以下各项：

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="帮助选择":::

      - **产品**：产品的解决方案 id

   4. 一旦在 Dynamics 365 中创建了商机，并将 "**伙伴中心同步**" 选项设置为 **"是"**，请等待10分钟，登录到合作伙伴中心帐户。 你的引用将与 Dynamics 365 同步。

   5. 因此，对于将 "与合作伙伴中心同步" 选项设置为 "是" 的机会，如果您更新 Dynamics 365 CRM 中的机会，则这些更改将在你的合作伙伴中心帐户中同步。

   6. 与合作伙伴中心成功同步的机会将用 Dynamics 365 中的✔图标标识。

2. 引用同步在 Microsoft 合作伙伴中心创建或更新引用并在 Dynamics 365 环境中同步时的同步：

   1. 登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。

   2. 从左侧菜单中选择 "**引用**"。

   3. 单击 "新建交易" 选项，从合作伙伴中心创建新的联销售引用。

   4. 登录到 Dynamics 365 CRM 环境。

   5. 导航到 "**开放式机会**"。 现在，在 Microsoft 合作伙伴中心创建的引用同步到 Dynamics 365 CRM 中。

   6. 选择同步的引用时，将填充卡片视图详细信息。

## <a name="next-steps"></a>后续步骤

- [有关 Microsoft Power 自动化平台的详细信息？](https://docs.microsoft.com/power-automate/)

- [合作伙伴中心 webhook 事件](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)
