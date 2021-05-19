---
title: 联合销售引荐连接器疑难解答
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解有关使用联合销售连接器的常见问题的解答。 阅读此常见问题解答，了解如何排查联合销售连接器问题。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148340"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>联合销售引荐连接器疑难解答

**适用于：Dynamics** 365 CRM |Salesforce CRM

**适当的角色**：引荐管理员|CRM 上的系统管理员或系统定制员

 ## <a name="questions-and-answers-about-pre-requisites"></a>有关先决条件的问题和解答

1. 能否为环境使用试用联合销售引荐连接器解决方案？

如果位于测试/过渡环境中，可以选择试用解决方案。 AppSource 中提供的连接器付费版本为 15 美元/月。 使用付费连接时，你每天将收到 10，000 个 API 调用。 连接器是引用 API 合作伙伴中心包装器。 每当连接器解决方案在客户端或CRM端针对合作伙伴中心创建或更新事件运行时，都会进行 API 调用。

2. 在 CRM 环境中创建节需要哪些角色？

作为系统管理员或系统定制员的用户可以针对每个人应用更改。 但是，所有应用用户可以对系统进行个性化设置，甚至可以与他人共享一些自定义项。 

3. 合作伙伴销售人员是否需要特殊角色来处理合作伙伴中心？
 
合作伙伴销售人员必须分配有"引荐管理员"角色。 有关详细信息，请参阅 [权限概述](create-user-accounts-and-set-permissions.md)。

4. 首先需要在 CRM 环境中设置哪些字段？ 

• 确保你的货币适合你的位置，并且准确位于 CRM 环境中。 • 你的销售团队应作为 CRM 用户列在 CRM 环境中。

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

- 使用合作伙伴中心凭据登录流环境后 (flow.microsoft.com) 。


3. 如果在 Power Automate Platform 中激活 合作伙伴中心 CRM 流时收到以下错误，应Power Automate操作？
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="需要更新的错误消息":::

请按照以下故障排除步骤操作：

- 先激活以下两个子流，然后再激活合作伙伴中心 CRM 流。
      - 合作伙伴中心 CRM - Helper (Insider Preview) 
      - 合作伙伴中心 Microsoft 联合销售 CRM 引荐更新 (Insider Preview) 

4. 尝试编辑流时，如果无法向流添加连接，该怎么办？

在流运行时向流添加连接，并单独添加到每个流。  如果在编辑流时用于添加连接的对话框未自动打开，可以单独编辑流的每个步骤和子步骤。

- 选择每个流并单独编辑它们。
- 展开流中的所有步骤 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="需要连接的步骤":::

- 选择一些步骤，其中会显示一个警告图标，要求关联连接并添加连接。 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="分步编辑流":::


5. 如果联合销售引荐连接器解决方案流没有打开，该怎么办？

A. 在Power Automate中，需要按以下顺序编辑流，并更新流以使用正确的连接：

- 合作伙伴中心预览体验版 (Webhook 注册) 
- 创建联合销售引荐 - Salesforce 合作伙伴中心 (Insider Preview) 
- 合作伙伴中心 Microsoft 联合销售 Salesforce (Insider Preview) 
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

1. 如何排查电源自动流执行过程中的故障？

若要确保电源自动流按预期运行，并在执行过程中排除故障，请参阅 [修复流故障](/power-automate/fix-flow-failures)。

2. 如果在合作伙伴中心或 CRM 环境中看到未正确同步的引用，应该怎么办？
 
若要确定引用同步的状态，请选择 " **审核**"。 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="如何同步引用":::

确保满足以下条件：

- 解决方案 ID 作为机会的一部分提供。

- 需要两个字母的国家/地区代码。

- 选择 Microsoft 的帮助作为机会时，需要客户联系信息。

3. 如何确保引荐双向同步？

执行以下步骤：

- 合作伙伴销售人员需要确保他们已启用 CRM 部分 **中的"合作伙伴中心** 同步"选项。

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="确保已启用 Synch":::

- 在限定潜在客户时，销售人员需要提供收入和结束日期。

- 如果在联合销售机会的创建或更新阶段中提供了 CRM ID，但在 CRM 中找不到具有该 ID 的潜在顾客机会，则更新或创建将被忽略。

- 确保在 Salesforce 环境中配置引荐货币字段。 

4. 如果连接器断开连接并错过引荐同步，该怎么办？。

下面是可以尝试的一些选项：

- 检查具有引荐管理员角色的用户的用户名合作伙伴中心密码是否已过期。

- 可以转到未同步的机会，进行次要更新，并观察引荐是否已同步。

- 如果流已运行且失败，请选择流，然后重新提交失败的运行。

5. 出现访问被拒绝错误时，应该怎么办？

确保存在适当的角色

- 卖方的引荐合作伙伴中心管理员角色 
 
- CRM 实例上的系统管理员或系统定制员角色

- 确保Power Automate帐户用户事先至少 https://flow.microsoft.com 登录一次

6. 如果在创建联合销售机会 **时** 发现缺少客户帐户国家/地区代码，该怎么办？

需要将 ISO 双字母国家/地区代码添加到 CRM 中的客户帐户。

7. 如果在创建联合销售机会时看到"解决方案 **ID** 是必需的"错误，该怎么办？

若要创建联合销售引荐，需要 Microsoft 联合销售就绪解决方案。 

8. 如果看到在云中创建的联合销售机会合作伙伴中心即使没有流错误，也未同步到 CRM 时，应该怎么办？

请执行以下操作：

- 在 合作伙伴中心 中创建了新的联合销售交易后，请检查是否调用了 合作伙伴中心 到 Dynamics 365 流的 (它可能会多次) 。

- 如果调用了流，请检查所有调用的流，并确定将更新 CRM 的流运行。 可以按照操作操作并验证它是否更新了 CRM 或遇到了问题。

- 检查 **"新建** 合作伙伴中心，查看其是否填充了 CRM ID。

- 确保交易不会意外以"赢得"或"丢失"状态在合作伙伴中心。

## <a name="next-steps"></a>后续步骤

- [管理潜在客户](manage-leads.md)
 
- [管理联合销售机会](manage-co-sell-opportunities.md)
