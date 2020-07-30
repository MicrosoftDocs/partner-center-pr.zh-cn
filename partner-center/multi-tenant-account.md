---
title: 向合作伙伴中心帐户添加其他租户
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 通过合作伙伴中心帐户管理多个租户
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389503"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在合作伙伴中心帐户中添加和管理多个租户

**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员

出于许多原因，你可能需要在合作伙伴中心帐户中管理多个 Azure AD 租户。 例如，你的公司可以购买其他公司，你希望新公司的员工能够使用合作伙伴中心。 但是，您希望两个公司保持独立。 在这种情况下，你需要将新公司的 Azure AD 租户与合作伙伴全局帐户（PNG）相关联。 这种关联使得两家公司的用户都可以在合作伙伴中心工作。

## <a name="add-another-azure-ad-tenant-to-your-account"></a>向你的帐户添加另一个 Azure AD 租户

1. 作为全局管理员登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard)。
1. 从 "**设置**" 图标中，选择 "**帐户设置**"，然后选择 "**租户**"。
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="关联租户"::: 

3. 选择 "**关联其他 AD 租户**" 并指示要关联的租户。

1. 以全局管理员身份登录到要关联的租户，并确认关联。 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="确认关联租户"::: 

5. 确认后，你将看到**全部设置**通知。  选择 "**返回到租户管理**"，你会看到列出的新添加的租户。
 
## <a name="next-steps"></a>后续步骤

- [添加用户](create-user-accounts-and-set-permissions.md)
