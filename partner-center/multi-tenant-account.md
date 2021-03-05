---
title: 将租户添加到合作伙伴中心帐户
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心帐户中添加、合并或管理多个 Azure AD 租户，并了解可能需要执行此操作的原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124799"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在合作伙伴中心帐户中添加和管理多个租户


**相应的角色**

- 全局管理员
- 帐户管理员

本文介绍如何将多个 Azure Active Directory (Azure AD) 租户合并为你的公司，然后在你的合作伙伴中心帐户中添加和管理它们。 这样做的原因有很多。 例如：

- 假设你的公司 Contoso 收购了另一家公司 Fabrikam。 您希望两家公司保持独立，但您希望新员工能够使用合作伙伴中心。 在这种情况下，可将新公司的 Azure AD 租户与合作伙伴全局帐户 (PGA) 相关联。 这种关联使得两家公司的用户都可以在合作伙伴中心工作。

- 如果你运行的业务包含多个租户 (例如， *contoso.com*、 *contoso.uk* 和 *contoso.in*) ，则可以使用多租户将它们分组到相同的 PC 帐户中。

- 如果合并和收购指导原则要求你使用两家公司的租户，则应同时使用 *constoso.com* 和 *fabrikam.com* 租户。

- 任何租户的用户都需要能够：
    * 访问合作伙伴中心，了解培训、数字下载或 Microsoft 认证专家 (MCP) 关联。
    * 将 Microsoft 合作伙伴网络 (MPN) 管理员或奖励 admin）分配给合作伙伴中心角色。

## <a name="add-an-azure-ad-tenant-to-your-account"></a>向你的帐户添加 Azure AD 租户

1. 以全局管理员身份登录到 [Microsoft 合作伙伴中心](https://partner.microsoft.com/dashboard)。

1. 在右上方，选择 " **设置**"，选择 " **帐户设置**"，然后选择 " **租户**"。
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="&quot;Azure AD 配置文件&quot; 窗格上的 &quot;关联&quot; 按钮的屏幕截图。"::: 

1. 选择 " **关联**"，然后指定要关联的租户。

1. 在提示符下，以全局管理员身份登录到要关联的租户，然后选择 " **确认**"。 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="&quot;确认新 Azure AD 关联&quot; 窗格上的 &quot;确认&quot; 按钮的屏幕截图。"::: 

   确认关联后，将显示 " **所有设置** " 消息。 若要查看新添加的租户，请选择 " **返回到租户管理**"。 
 
>[!NOTE]
>如果某个租户已与另一个合作伙伴中心帐户相关联，则无法将其与该帐户相关联。


## <a name="remove-a-tenant-from-your-account"></a>从帐户中删除租户
 
1. 以全局管理员身份登录到 [Microsoft 合作伙伴中心](https://partner.microsoft.com/dashboard)。

1. 在右上方，选择 " **设置** " 图标，然后选择 " **帐户设置**"。

1. 在左侧窗格中，选择 " **租户**"。 在 " **管理 Azure AD 租户**" 下，选择 " **合作伙伴** " 选项卡。
 
1. 选择要删除其关联的租户旁边的 " **删除** "。

   :::image type="content" source="images/disassociate.png" alt-text="当前租户关联及其删除链接的屏幕截图。":::

   如前面的屏幕截图所示，为所有关联的租户启用了 " **删除** " 链接，但主要租户和当前登录到的租户除外。 

   > [!NOTE]   
   > 当你删除某个租户时，该租户上的用户将不再有权访问合作伙伴中心帐户，并且删除操作可能会影响你的能力。 

## <a name="next-steps"></a>后续步骤

- [创建用户帐户](create-user-accounts-and-set-permissions.md)






