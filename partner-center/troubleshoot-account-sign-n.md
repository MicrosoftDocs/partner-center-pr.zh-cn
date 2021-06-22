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
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431753"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>排查帐户设置或 MPN 续订问题

**适当的角色**：全局管理员|MPN 合作伙伴管理员
 
下面是一些建议，用于排查设置帐户时出现的合作伙伴中心问题。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>如果从公司迁移Partner Membership Center无法编辑任何公司信息字段，会发生什么情况

例如，如果你的公司已在 合作伙伴中心 (，云解决方案提供商 (CSP) 帐户) - 将显示一个只读屏幕。 此屏幕将显示有关公司的所有信息，因为它存在于合作伙伴中心。

不能更改此屏幕上的详细信息。 这是设计使的，不是错误。

若要继续，请选择 **"接受"，** 然后选择"继续 **"。**


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>如果 IT 部门已关闭注册 **合作伙伴中心**

你会看到此消息，因为病毒用户被禁用，或者因为病毒性注册在 AD Azure Active Directory (上) 禁用。 帐户的全局管理员Azure AD运行以下 PowerShell 命令来启用所需的功能：

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

有关详细信息，请阅读 [自助注册](/azure/active-directory/users-groups-roles/directory-self-service-signup)。

## <a name="you-forgot-your-password"></a>忘记了密码

如果忘记了密码，请在登录页上选择"**无法访问你的帐户？"。** 此选项允许你重置密码或要求全局管理员分配新凭据。

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>在"告诉我们关于你的公司"屏幕上，你收到"出现问题"错误

如果无意中在公司电话号码中使用了特殊字符、空格或国家/地区代码，通常会显示此错误消息。 在"电话号码"字段中输入的值最多只能包含 10 个字符。


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>信用卡购买收到一条错误消息，指出"你的订单被拒绝。 请验证你的信息"


始终使用与信用卡相对应的地址，而不是法定实体。 此外，请确保邮政编码正确，并对应于你使用的地址。

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>你想要从脱机付款切换到联机付款方式 

需要取消原始订单，然后使用首选付款方式重新购买。

取消订单：

1. 在"合作伙伴中心"仪表板中，选择" **成员资格产品/服务"** 选项卡。

2. 选择 **"取消订单"**

3. 将出现一个确认窗口，必须确认才能取消初始订单。

## <a name="next-steps"></a>后续步骤

- [管理合作伙伴中心帐户](partner-center-account-setup.md)
- [如何读取帐单和对帐文件](read-your-bill.md)
