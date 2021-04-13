---
title: 无法登录到合作伙伴中心
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 解决可能的原因并了解无法登录到合作伙伴中心时的解决方案-详细了解重置密码、检查角色和检查凭据。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266565"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>合作伙伴中心的登录问题疑难解答

**相应的角色**

- 所有对合作伙伴中心感兴趣的合作伙伴

本文包含合作伙伴中心常见登录问题的解决方案。

## <a name="youve-forgotten-your-password-for-partner-center"></a>你忘记了合作伙伴中心的密码

如果你忘记了密码，但无法登录到合作伙伴中心，请联系支持人员。 在 [支持业务产品](/microsoft-365/admin/contact-support-for-business-products)时查找相应的联系人。

如果你是 MPN 合作伙伴，请让你的全局管理员为你创建新密码。 如果你是一个 CSP 间接经销商，请向你的间接提供商要求你为你的 Azure AD 租户创建新的全局管理员，或者使用其委派的管理员权限创建新密码。

若要详细了解如何重置密码和重新获得工作帐户的访问权限，请阅读 [使用安全信息重置工作或学校密码](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)。

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>你无法在合作伙伴中心查看或管理预期的页面或功能

对合作伙伴中心中的页面的访问权限由你分配的角色控制。 若要查看分配的角色，请在 "合作伙伴中心" 中选择 "设置" 图标，选择 " **帐户设置**"，然后在 "帐户设置" 中选择 " **用户管理**"。 在 "搜索" 中，键入您的姓名，然后查看结果。

如果无法查看或管理预期的能力、客户、奖励或用户，请尝试以下解决方案：

- 若要访问 MPN、CSP 和引用的功能，请联系你的全局管理员或帐户管理员。若要详细了解角色以及他们在合作伙伴中心启用的任务，请参阅向 [用户分配角色 & 权限](permissions-overview.md)。
- 若要访问商业市场和 Windows & Xbox、Office 应用商店、Microsoft Edge 和硬件开发人员计划的功能，请与组织中的 "所有者" 或 "经理" 角色联系。 若要了解有关角色和权限的详细信息，请参阅 [如何在 Microsoft 合作伙伴中心管理商业 marketplace 帐户](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)。

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>你无法在合作伙伴中心看到你的产品/服务或权益

确认使用正确的凭据进行登录。 例如，您的工作帐户和个人帐户可能看起来像是相同的 (abc@contoso.com ，如) ，而另一个帐户可能是您创建的个人帐户，而另一个帐户可能是代表您设置的企业帐户。 在这种情况下，如果你已登录，但无法查看与 MPN、CSP 和商用 Marketplace 相关的预期功能，请尝试选择你的工作帐户。

## <a name="next-steps"></a>后续步骤

- [验证帐户信息](verification-responses.md)
- [重置我的密码](reset-my-pasword.md)
- [重置用户密码](reset-a-user-password.md)