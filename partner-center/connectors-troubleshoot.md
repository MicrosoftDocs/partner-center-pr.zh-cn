---
title: 联合销售引荐连接器疑难解答
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解有关使用共同销售连接器的常见问题的解答。 阅读有关如何排查共同销售连接器问题的常见问题解答。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354536"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>联合销售引荐连接器疑难解答

**适用对象：**

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
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="需要更新的错误消息":::

请遵循以下故障排除步骤：

- 激活合作伙伴中心到 CRM 流之前，先激活以下两个子流。
      - 合作伙伴中心到 CRM-助手 (预览体验) 
      - 合作伙伴中心 Microsoft 共同销售 CRM (有问必答预览版的参考更新) 

4. 尝试编辑流时，如果无法将连接添加到流，应该怎么办？

在流运行时，将连接添加到流，并分别添加到每个流。  如果在编辑流时未自动打开用于添加连接的对话框，则可以单独编辑流的每个步骤和子步骤。

- 选择每个流并分别对其进行编辑。
- 展开流中的所有步骤 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="需要连接的步骤":::

- 选择显示警告图标的步骤，要求关联连接，然后添加连接。 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="逐步骤编辑流":::


5. 如果共同销售引用连接器解决方案的流未打开，应该怎么办？

A. 在 "自动启动" 中，需要按以下顺序编辑流，并将其更新为使用正确的连接：

-  (内幕预览版) 合作伙伴中心 Webhook 注册
- 创建向合作伙伴中心 (内幕预览版的共同销售推荐-Salesforce) 
- 合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) 
- 合作伙伴中心到 Salesforce (预览体验) 
- Salesforce 到合作伙伴中心 (预览体验) 
- 合作机会到合作伙伴中心 (预览体验) 
- Salesforce Microsoft 解决方案到合作伙伴中心 (预览体验) 

 B. 对于每个 flow，选择 " **仅运行用户** " 选项。 选择 " **使用连接** ，而不是 **由仅运行用户提供**"。  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="激活流":::


C. 激活以下所述的流：

 - 合作伙伴中心 Microsoft 共同销售对 Salesforce (内幕预览版的推荐更新) 

- Salesforce 到合作伙伴中心 (预览体验) 

    
D. 激活所有剩余流。

E. 在流伙伴中心 Webhook 注册中，选择 " **运行**"。 提供从合作伙伴中心的第一个操作 **到 Salesforce** 流的 **http url** 。 选择 **要注册的事件** 下的所有四个选项，然后选择 **"是"** 进行覆盖。

## <a name="questions-and-answers-about-runmaintenance"></a>有关运行/维护的问题和解答

1. 如果在自动执行流程的过程中出现故障，如何排查问题？

若要确保电源自动流按预期运行，并在执行过程中排除故障，请参阅 [修复流故障](/power-automate/fix-flow-failures)。

2. 如果在合作伙伴中心或 CRM 环境中看到未正确同步的引用，应该怎么办？
 
若要确定引用同步的状态，请选择 " **审核**"。 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="如何同步引用":::

确保满足以下条件：

- 解决方案 ID 作为机会的一部分提供。

- 需要两个字母的国家/地区代码。

- 为此机会选择了 "Microsoft 帮助" 时，需要客户联系信息。

3. 如何确保引用会双向同步？

执行以下步骤：

- 合作伙伴卖方需要确保客户在 CRM 部分启用了 **与合作伙伴中心的同步** 选项。

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="确保已启用同步":::

- 卖方需要在确认潜在客户时提供收入和结束日期。

- 如果在共同销售机会的 **创建** 或 **更新** 阶段提供 CRM ID，但 crm 中找不到具有该 id 的潜在顾客机会，则将忽略 update 或 create。

- 确保在 Salesforce 环境中配置了参考货币字段。 

4. 如果连接器断开连接并且错过了引用同步，应该怎么做。 

下面是一些你可以尝试的选项：

- 通过引用管理员角色检查伙伴中心用户的用户名或密码是否已过期。

- 您可以使用未同步的机会，进行次要更新，并观察引用是否已同步。

- 如果流已运行并失败，请选择该流，并重新提交失败的运行。

5. 收到拒绝访问错误后，应该怎么办？

请确保存在适当的角色

- 合作伙伴中心卖方的引用管理员角色 
 
- CRM 实例上的系统管理员或系统定制员角色

- 确保自动将流量帐户用户登录 https://flow.microsoft.com 至少一次

6. 如果在创建共同销售机会时看到 **客户帐户国家/地区代码** 缺失，你应该怎么办？

需要将 ISO 双字母国家/地区代码添加到 CRM 中的客户帐户。

7. 如果在创建共同销售机会时看到 **需要解决方案 ID** 的错误，该怎么办？

若要创建共同销售引用，你需要一个 Microsoft 共同销售好的解决方案。 

8. 当你看到在合作伙伴中心创建的共同销售机会（即使没有流错误）时，你应该怎么办：

请执行以下操作：

- 在合作伙伴中心创建新的共同销售交易后，请检查是否调用了 "合作伙伴中心到 Dynamics 365" 流 (它可能会) 调用多次。

- 如果调用了流，请检查所有调用的流，并识别将更新 CRM 的流运行。 你可以执行这些操作，并验证其是否更新了 CRM 或遇到了问题。

- 请查看合作伙伴中心的 *新交易**，查看其是否已用 CRM ID 填充。

- 请确保在合作伙伴中心，交易不会意外地被视为 "赢单" 或 "丢失"。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)
 
- [管理联合销售机会](manage-co-sell-opportunities.md)
