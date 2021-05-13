---
title: 排查设置 合作伙伴中心帐户或 MPN 续订问题
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查尝试在注册时合作伙伴中心。 解答解决了付款方式、忘记密码等难题。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854683"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>排查帐户设置或 MPN 续订问题

**适当的角色**：全局管理员|MPN 合作伙伴管理员
 
下面是一些建议，用于排查设置帐户时出现的合作伙伴中心问题。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>如果从公司迁移Partner Membership Center无法编辑任何公司信息字段，会发生什么情况

例如，如果你的公司已在 合作伙伴中心 (，则 CSP 帐户) - 将显示一个只读屏幕。 此屏幕将显示有关公司的所有信息，因为它存在于合作伙伴中心。

不能更改此屏幕上的详细信息。 这是设计使的，不是错误。

选择 **"接受** 并继续 **"** 以继续。


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>如果 IT 部门已关闭注册 **合作伙伴中心**

你会看到此消息，因为病毒用户已禁用，或者病毒性注册在租户Azure AD禁用。 帐户的全局管理员Azure AD运行以下 PowerShell 命令来启用所需的功能：

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

有关详细信息，请阅读 [自助注册](/azure/active-directory/users-groups-roles/directory-self-service-signup)。

## <a name="you-forgot-your-password"></a>忘记了密码

如果忘记了密码，请在登录页上选择"无法访问帐户？"链接。 此选项允许你重置密码或要求全局管理员分配新凭据。

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
