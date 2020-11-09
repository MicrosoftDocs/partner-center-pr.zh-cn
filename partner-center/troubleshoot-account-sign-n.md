---
title: 设置合作伙伴中心帐户或 MPN 续订问题的疑难解答
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查试图注册伙伴中心时遇到的问题。 通过支付方法、忘记密码等解决问题。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381403"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>帐户设置或 MPN 续订问题的疑难解答

**适用于**

- 合作伙伴中心
 
**相应的角色**

- 全局管理员
- MPN 合作伙伴管理员 
 
下面是有关在设置合作伙伴中心帐户时出现的常见问题的一些建议。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>如果要从合作伙伴成员中心进行迁移并且无法编辑任何公司信息字段，会发生什么情况

如果你的公司已在合作伙伴中心中存在， (说 CSP 帐户) ，你会看到一个只读屏幕。 此屏幕将显示在合作伙伴中心存在的有关公司的所有信息。

无法更改此屏幕上的详细信息。 这是由设计决定的，而不是错误。

选择 " **接受** 并 **继续** " 继续。


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>如果 IT 部门已关闭 **合作伙伴中心的注册** ，

你会看到此消息，因为已禁用病毒用户，或者是因为 Azure AD 租户上禁用了病毒注册。 Azure AD 帐户的全局管理员可以通过运行以下 PowerShell 命令来启用所需的功能：

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

有关详细信息，请阅读 [自助注册](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>你忘记了密码

如果忘记了密码，请在登录页上选择 " **无法访问帐户？** " 链接。 此选项可让你重置密码或请求全局管理员为你分配新凭据。

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>在 "告诉我们你的公司" 屏幕上，你会看到 "出现错误" 错误

如果你无意中在公司电话号码中使用特殊字符、空格或国家/地区代码，则会出现此错误消息。 在 "电话号码" 字段中输入的值最多只能包含10个字符。


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>你的信用卡购买将收到一条错误消息，指出 "你的订单已被拒绝。 请验证你的信息


始终使用与您的信用卡相对应的地址，而不是您的法律实体。 此外，请确保邮政编码正确，并对应于所使用的地址。

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>要从脱机支付切换到联机付款方式 

您将需要使用首选付款方式取消原始订单和重新购买。

若要取消订单：

1. 在仪表板中选择 " **成员资格产品** " 选项卡。

2. 选择 **取消顺序**

3. 将显示一个确认窗口，您必须确认才能取消初始订单。

## <a name="next-steps"></a>后续步骤

- [管理合作伙伴中心帐户](partner-center-account-setup.md)
- [如何读取帐单和侦测文件](read-your-bill.md)
