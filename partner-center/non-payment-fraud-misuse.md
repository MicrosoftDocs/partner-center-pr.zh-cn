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
ms.openlocfilehash: ba5fe60234c002ad2696de348a1b3b9b1284c149
ms.sourcegitcommit: eef446698ed4e21afee7fe091fe9c2664767755c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "89280505"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>合作伙伴中心中管理拒不付款、欺诈或误用

适用于：

- 合作伙伴中心
- Microsoft Cloud for US Government 合作伙伴中心

**相应的角色**
- 全局管理员
- 用户管理员
- 管理员代理
- 计费管理员

你对客户的欺诈性购买和/或客户对所购服务拒不付款的行为负有财务责任。 因此， *我们强烈建议您设置防欺诈防护和检测风险缓解*措施。

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

## <a name="managing-online-risk"></a>管理在线风险

你可以使用以下建议来帮助你制定策略和做法，以降低你的客户关系生命周期内的联机事务风险的暴露程度。

### <a name="onboarding-new-customers"></a>加入新客户

在加入新客户时降低在线风险的建议包括：

- 例如，与客户建立个人关系 (例如，通过电话) 与客户联系。
- 通过更好的方法来验证客户的凭据和背景 (如使用信用报告机构或商业商业报表机构) 。
- 在注册期间使用多重身份验证 (如 SMS 验证) ，以最大程度地减少向机器人帐户创建和购买的风险。
- 使用服务 (例如数字标识服务) 管理和跟踪标识。
- 通过严格的信用卡欺诈检测系统对客户的财务强度进行评估。
- 建立清晰的集合策略。 详细说明你的集合流程，以及何时对订阅的访问会受到非支付影响。  (你可以禁用访问或 [暂停客户的](suspend-a-subscription.md) 非付款订阅。 ) 

### <a name="managing-customer-accounts"></a>管理客户帐户

在购买后管理客户帐户的建议包括：

- 实施一个过程来快速接收、查看、操作和响应 Microsoft 通知。
- 与客户合作，在设置适当的监视阈值时了解云使用情况业务需求。 例如，可以在合作伙伴中心 [设置每月 Azure 支出预算](set-an-azure-spending-budget-for-your-customers.md) ， (例如。 通过这种了解，你可以监视当月的客户使用情况，并在客户接近预算时收到通知。 ) 
- 定期监视 [客户活动日志](activity-logs.md) 以帮助及早检测欺诈行为。
- 当检测到可疑活动时，请执行快速操作。
- 不要首先实施风险缓解控制，避免向客户提供对订阅的完全管理访问权限。

### <a name="managing-customer-billing"></a>管理客户帐单

有关管理客户帐单购买后的建议包括：

- 在初始交易和计费之前请求预付款。
- 不要接受高风险支付仪器 (例如预支付卡或存储的价值卡) 。
- 监视客户付款并应收帐款。 主动强制实施标准化的纠缠流程，以应付延期或非支付费用。

有关可以降低在线风险的更多详细策略，请参阅[在线交易风险管理指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)。
