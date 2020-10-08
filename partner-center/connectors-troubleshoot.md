---
title: 联合销售引荐连接器疑难解答
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有关如何排查共同销售连接器问题的常见问题解答。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 312ff9155ab4c2d84fb38bb6ccd093505e628832
ms.sourcegitcommit: df7643f3b7978e164e419e447a4dc3c163cb3bd2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2020
ms.locfileid: "91844651"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>联合销售引荐连接器疑难解答

**适用对象：**

- 合作伙伴中心
- Dynamics 365 CRM
- Salesforce CRM

**相应的角色**

- 引荐管理员
- CRM 上的系统管理员或系统定制员

 ## <a name="questions-and-answers-about-pre-requisites"></a>有关先决条件的问题和解答

1. 能否为你的环境使用试用共同销售引用连接器解决方案？

如果你在测试/过渡环境中，则可以选择试用版解决方案。 AppSource 的付费版连接器可在美国 $ 15/month 提供。 通过付费连接，你每天将获得 10K API 调用。 连接器是位于合作伙伴中心引用 Api 之上的包装器。 每当连接器解决方案在合作伙伴中心或 CRM 端的机会中运行 " **创建** " 或 " **更新** " 事件时，就会进行 API 调用。

2. 在 CRM 环境中创建节需要什么角色？

作为系统管理员或系统定制员的用户可以对所有人应用更改。 不过，所有应用程序用户都可以对系统进行个性化设置，甚至与他人共享某些自定义。 

3. 合作伙伴卖方是否需要特殊角色才能在合作伙伴中心工作？
 
必须为合作伙伴卖方分配 "引用管理员" 角色。 有关详细信息，请参阅以下 [权限概述) # B1 创建用户帐户) 。

4. 需要首先在 CRM 环境中设置哪些字段？ 

•确保你的货币适用于你所在的位置，并准确地在 CRM 环境中。 •销售团队应作为 CRM 用户列在 CRM 环境中。

5. 电源自动执行环境创建需要哪些先决条件？

若要使用电源自动执行环境，需要：

- 需要使用 Power 自动许可证。
- 至少需要 1 GB 的存储空间。

6.  是否需要 Dynamics 365 订阅才能使用 Salesforce 连接器解决方案？

Salesforce 连接器解决方案的类型为 "Dynamics Flow"，它支持与其他 CRM 系统同步。 此解决方案不需要你拥有 Dynamics 365 实例或订阅。 安装 Salesforce 解决方案时，可能会出现一个包含公司中现有 CD 环境的下拉状态。 需要选择该环境。 此外，如果收到 "找不到连接到已登录用户的 Dynamics 365 组织" 错误，则需要为连接器创建新的环境。

## <a name="questions-and-answers-about-configuration"></a>有关配置的问题和解答

1. 如果在 Power 自动化平台中激活流时遇到以下错误，应该怎么办？

错误：请求 Azure 资源管理器失败，出现错误： "{" 错误 "： {" 代码 "：" WorkflowTriggerNotFound "，" message "：" 找不到工作流 "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" 触发器 "manual"。 "}}"。 

请遵循以下故障排除步骤：

- 删除 CD 连接，然后重新创建 CD 连接。
- 关闭和打开子流 
- 删除解决方案，然后重新安装解决方案。 

2.  如果在 Power 自动化平台中添加合作伙伴中心连接器时遇到 "登录" 错误，该怎么办？

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="需要登录的错误消息":::

请按照以下故障排除步骤操作：

-  (flow.microsoft.com) 后，使用合作伙伴中心凭据登录到流环境。


3. 如果在 Power 自动化平台中激活合作伙伴中心到 CRM 流时收到以下错误，该怎么办？
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="需要登录的错误消息":::

请遵循以下故障排除步骤：

- 激活合作伙伴中心到 CRM 流之前，先激活以下两个子流。
      - 合作伙伴中心到 CRM-助手 (预览体验) 
      - 合作伙伴中心 Microsoft 共同销售 CRM (有问必答预览版的参考更新) 

4. 尝试编辑流时，如果无法将连接添加到流，应该怎么办？

在流运行时，将连接添加到流，并分别添加到每个流。  如果在编辑流时未自动打开用于添加连接的对话框，则可以单独编辑流的每个步骤和子步骤。

- 选择每个流并分别对其进行编辑。
- 展开流中的所有步骤 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="需要登录的错误消息":::

- 选择显示警告图标的步骤，要求关联连接，然后添加连接。 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="需要登录的错误消息" **使用连接** ，而不是 **由仅运行用户提供**"。  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="需要登录的错误消息" **运行**"。 提供从合作伙伴中心的第一个操作**到 Salesforce**流的**http url** 。 选择 **要注册的事件** 下的所有四个选项，然后选择 **"是"** 进行覆盖。

## <a name="questions-and-answers-about-runmaintenance"></a>有关运行/维护的问题和解答

1. 如果在自动执行流程的过程中出现故障，如何排查问题？

若要确保电源自动流按预期运行，并在执行过程中排除故障，请参阅 [修复流故障](/power-automate/fix-flow-failures)。

2. 如果在合作伙伴中心或 CRM 环境中看到未正确同步的引用，应该怎么办？
 
若要确定引用同步的状态，请选择 " **审核**"。 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="需要登录的错误消息" 时，需要客户联系信息。

3. 如何确保引用会双向同步？

执行以下步骤：

- 合作伙伴卖方需要确保客户在 CRM 部分启用了 **与合作伙伴中心的同步** 选项。

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="需要登录的错误消息" 或 "丢失"。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)
 
- [管理联合销售机会](manage-co-sell-opportunities.md)