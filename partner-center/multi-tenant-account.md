---
title: 向合作伙伴中心帐户添加其他租户
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心帐户中添加、合并或管理多个 Azure AD 租户。 进一步了解你可能想要执行的一些原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105540"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在合作伙伴中心帐户中添加和管理多个租户


**相应的角色**

- 全局管理员

可以通过此功能管理公司的多个租户，并将其合并到合作伙伴中心帐户中。 出于许多原因，你可能需要在合作伙伴中心帐户中管理多个 Azure AD 租户。 例如：

- 你的公司可能会购买其他公司，你希望新公司的员工能够使用合作伙伴中心。 但是，您希望两个公司保持独立。 在这种情况下，可将新公司的 Azure AD 租户与合作伙伴全局帐户 (PGA) 相关联。 这种关联使得两家公司的用户都可以在合作伙伴中心工作。

- 如果有多个租户运行你的业务 (例如，contoso.com、contoso.uk、contoso.in) 你可以使用多租户将它们与相同的 PC 帐户关联。

- 合并和收购要求使用多个租户 (例如，如果 Contoso 获取 Fabrikam，则需要能够同时使用 Constoso.com 和 Fabrikam.com 各自的租户) 。

- 任何租户的用户都需要能够：
    1.  访问合作伙伴中心进行培训、数字下载、MCP 关联
    2.  分配合作伙伴中心角色，如 MPN 管理员、奖励管理员等。


## <a name="add-another-azure-ad-tenant-to-your-account"></a>向你的帐户添加另一个 Azure AD 租户

1. 作为全局管理员登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。
1. 从 " **设置** " 图标中，选择 " **帐户设置** "，然后选择 " **租户**"。
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="关联租户"::: 

3. 选择 " **关联其他 AD 租户** " 并指示要关联的租户。

1. 以全局管理员身份登录到要关联的租户，并确认关联。 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="确认关联租户"::: 

5. 确认后，你将看到 **全部设置** 通知。  选择 " **返回到租户管理** "，你会看到列出的新添加的租户。 
 

>[!NOTE]
>如果某个租户已与另一个合作伙伴中心帐户关联，则无法将其关联到该帐户。


## <a name="remove-a-tenant-from-your-account"></a>从帐户中删除租户
 
1. 作为全局管理员登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。

1. 从 " **设置** " 图标中，选择 " **帐户设置** -> 租户"，然后单击 " **合作伙伴** " 选项卡。
 
3. 对于要取消关联的租户，单击 " **删除** "。

4. 租户取消关联是指租户上的用户将不再有权访问合作伙伴中心帐户，这可能会影响你的胜任度。 

对于所有关联的租户，" **删除** " 按钮是启用的，主要租户和当前登录到的租户除外。

:::image type="content" source="images/disassociate.png" alt-text="带有 &quot;删除&quot; 按钮的租户":::
 

## <a name="next-steps"></a>后续步骤

- [添加用户](create-user-accounts-and-set-permissions.md)






