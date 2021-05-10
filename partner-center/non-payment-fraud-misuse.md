---
title: 管理拒不付款、欺诈或滥用
description: 了解联机事务中涉及的各种风险，以及在合作伙伴中心管理和缓解这些风险的最佳实践。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686290"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>合作伙伴中心中管理拒不付款、欺诈或误用

**适用于**

- Microsoft Cloud for US Government 合作伙伴中心

**相应的角色**

- 全局管理员
- “用户管理”管理员
- 管理员代理
- 计费管理员

你对客户的欺诈性购买和/或客户对所购服务拒不付款的行为负有财务责任。 因此， *我们强烈建议您设置防欺诈防护和检测风险缓解* 措施。

若要避免和/或应对欺诈活动或滥用问题，请务必了解潜在风险并制定可以降低风险的策略和做法。

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>强制实施 Microsoft 可接受的使用策略

如果 Microsoft 检测到我们确认或怀疑违反了可接受的使用策略的合作伙伴或客户活动，我们将采取强制措施。 客户可以立即挂起。 你将收到有关强制操作的通知，或你的请求已由 Microsoft 请求更新。

## <a name="abuse-of-service-risks"></a>滥用服务风险

**滥用服务** 风险意味着使用云服务的客户违反了 Microsoft 的可接受的使用策略。

### <a name="examples-of-abuse-of-service"></a>服务滥用的示例

Microsoft 的可接受使用策略违反的示例可能包括：

- 垃圾邮件
- 黑客攻击
- 分布式拒绝服务 (DDoS) 攻击
- 比特币开采
- 恶意软件传播
- 转售盗版订阅

## <a name="theft-of-service-risks"></a>服务风险的盗窃

**服务风险的盗窃** 意味着不打算支付所使用服务的客户。 此盗窃可能涉及使用盗用的付款方式，提供假计费信息，并/或对未付余额使用默认值。

### <a name="examples-of-service-theft"></a>服务盗用示例

这些在线交易风险的示例包括：

- 不在 person ( "不存在信用卡" 事务中发生的事务) 
- 虚假身份
- 在接收初始付款之前预配和使用的服务
- 针对在线欺诈的新兴市场和/或高风险区域
- 使用不良参与者自动创建和购买帐户

## <a name="managing-online-risk"></a>管理联机风险

可以使用以下建议来帮助制定策略和做法，以减少在客户关系生命周期中遭受联机事务风险的风险。

### <a name="onboarding-new-customers"></a>加入新客户

加入新客户时降低联机风险的建议包括：

- 在可能的情况下与客户建立 (关系，例如，通过电话呼叫) 。
- 通过更好的方法验证客户的凭据和背景， (如使用信用机构或商业商业报表) 。
- 使用多重身份验证 (例如注册期间) 短信验证功能，以最大程度地减少创建和购买机器人帐户的风险。
- 使用数字标识服务等服务 (和跟踪标识) 。
- 通过严格的信用卡欺诈检测系统评估客户的财务能力。
- 建立明确的集合策略。 详细说明你的集合过程以及何时对订阅的访问将受非付款的影响。  (可以禁用访问或 [暂停](create-a-new-subscription.md#suspend-a-subscription) 客户的非付款订阅。) 

### <a name="managing-customer-accounts"></a>管理客户帐户

有关在购买后管理客户帐户的建议包括：

- 实施一个快速接收、查看、处理和响应 Microsoft 通知的过程。
- 与客户合作，了解其云使用情况业务需求，同时设置适当的监视阈值。  (例如，可以在门户中设置每月 [Azure](set-an-azure-spending-budget-for-your-customers.md) 支出合作伙伴中心。 通过这种了解，可以监视当月的客户使用情况，并当客户接近其预算时收到通知。) 
- 定期 [监视客户](activity-logs.md) 活动日志，以帮助尽早检测欺诈。
- 检测到可疑活动时快速采取措施。
- 避免在未先实施风险缓解控制的情况下为客户提供对订阅的完全管理访问权限。

### <a name="managing-customer-billing"></a>管理客户帐单

有关管理客户帐单购买后的建议包括：

- 在初始交易和计费之前请求预付款。
- 不要接受高风险支付仪器 (例如预支付卡或存储的价值卡) 。
- 监视客户付款并应收帐款。 主动强制实施标准化的纠缠流程，以应付延期或非支付费用。

有关可以降低在线风险的更多详细策略，请参阅[在线交易风险管理指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)。
