---
title: 设置合作伙伴中心帐户或 MPN 续订问题的疑难解答
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查合作伙伴中心的注册问题
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848921"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>帐户设置或 MPN 续订问题的疑难解答

### <a name="applies-to"></a>适用于

- 合作伙伴中心
 
### <a name="appropriate-roles"></a>相应的角色

- 全局管理员
- MPN 合作伙伴管理员 
 

下面是有关在设置合作伙伴中心帐户时出现的常见问题的一些建议。

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>如果要从合作伙伴成员中心进行迁移并且无法编辑任何公司信息字段，会发生什么情况

如果你的公司已在合作伙伴中心（ (说 CSP 帐户) ）中存在，则会出现这种情况–你将显示一个只读屏幕，该屏幕将显示有关你的公司的所有信息，因为它存在于合作伙伴中心。

你无法更改此屏幕上的详细信息。 这是由设计决定的，而不是错误。

选择 " **接受** 并 **继续** " 继续。

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>你正在尝试注册或从合作伙伴成员中心迁移，但收到了一条错误消息，指出 IT 部门已关闭 " **注册合作伙伴中心**"。 

你会看到此消息，因为已禁用病毒用户或在 Azure AD 租户上禁用病毒注册。 Azure AD 帐户的全局管理员可以通过运行以下 PowerShell 命令来启用所需的功能：

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

有关详细信息，请阅读 [自助注册](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)

### <a name="you-forgot-your-password"></a>你忘记了密码

如果忘记了密码，请在登录页面上选择 " **无法访问帐户？** " 链接，以重置密码，或要求全局管理员为你分配新凭据。

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>在 "告诉我们公司的情况" 屏幕上，收到 "出现错误" 错误

如果你在公司电话号码中无意中使用特殊字符、空格或国家/地区代码，则通常会发生这种情况。 在 "电话号码" 字段中输入的值最多只能包含10个字符。

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>你正在尝试通过信用卡完成购买，但你收到一条错误消息，指出 "你的订单已被拒绝。 请验证你的信息

你应始终插入与信用卡相对应的地址，而不是与你的法律实体对应的地址。 此外，请确保邮政编码正确，并对应于所使用的地址。

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>要从脱机支付切换到联机付款方式 

您将需要使用首选付款方式取消原始订单和重新购买。

若要取消订单：

1. 在仪表板中选择 " **成员资格产品** " 选项卡。

2. 选择 **取消顺序**

3. 将显示一个确认窗口，您必须确认才能取消初始订单。
