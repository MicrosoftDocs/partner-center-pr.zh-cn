---
title: 向合作伙伴中心帐户添加其他租户
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心帐户中添加、合并或管理多个 Azure AD 租户。 进一步了解你可能想要执行的一些原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175160"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在合作伙伴中心帐户中添加和管理多个租户

**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员

可以通过此功能管理公司的多个租户，并将其合并到合作伙伴中心帐户中。 出于许多原因，你可能需要在合作伙伴中心帐户中管理多个 Azure AD 租户。 例如： 。

- 你的公司可能会购买其他公司，你希望新公司的员工能够使用合作伙伴中心。 但是，您希望两个公司保持独立。 在这种情况下，可将新公司的 Azure AD 租户与合作伙伴全局帐户 (PGA) 相关联。 这种关联使得两家公司的用户都可以在合作伙伴中心工作。

- 如果有多个租户运行你的业务 (例如，contoso.com、contoso.uk、contoso.in) 你可以使用多租户将它们与相同的 PC 帐户关联。

- 合并和收购要求使用多个租户 (例如，如果 Contoso 获取 Fabrikam，则需要能够同时使用 Constoso.com 和 Fabrikam.com 各自的租户) 。

- 任何租户的用户都需要能够：
    1.  访问合作伙伴中心进行培训、数字下载、MCP 关联
    2.  分配合作伙伴中心角色，如 MPN 管理员、奖励管理员等。


## <a name="add-another-azure-ad-tenant-to-your-account"></a>向你的帐户添加另一个 Azure AD 租户

1. 作为全局管理员登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。
1. 从 " **设置** " 图标中，选择 " **帐户设置** "，然后选择 " **租户**"。
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="关联租户&quot;::: 

3. 选择 &quot; **关联其他 AD 租户** " 并指示要关联的租户。

1. 以全局管理员身份登录到要关联的租户，并确认关联。 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="关联租户&quot;::: 

3. 选择 &quot; **关联其他 AD 租户** " **返回到租户管理** "，你会看到列出的新添加的租户。 
 

>[!NOTE]
>如果某个租户已与另一个合作伙伴中心帐户关联，则无法将其关联到该帐户。

 
## <a name="next-steps"></a>后续步骤

- [添加用户](create-user-accounts-and-set-permissions.md)
