---
title: 客户将管理权限委派给合作伙伴 | 合作伙伴中心
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何让客户将管理员权限委派给经销商或者删除相同的权限，以及如何使用这些权限。
author: LauraBrenner
ms.author: labrenne
keywords: 委派的管理员权限, 代表管理员, 删除权限, DAP, AOBO
ms.localizationpriority: high
ms.openlocfilehash: 9b82ed4828a112f28f3e2ef1da1a64745c9ffdc0
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340055"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>客户将管理权限委派给合作伙伴

**适用于**

- 合作伙伴中心

**相应的角色**

- 管理员代理
- 销售代理

若要代表客户管理客户的服务或订阅，客户必须授予你对该服务的管理员权限。 若要从客户处获取管理员权限，请通过电子邮件向他们发送经销商关系请求。 在客户批准你的请求后，你可以登录到该服务的门户并代表客户管理该服务。 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>邀请客户与你建立经销商关系

1.  选择“客户”，然后选择“请求经销商关系”。  

2.  在下一页上，查看草稿电子邮件。 你可以在默认电子邮件应用程序中打开草稿邮件，也可以将邮件复制到剪贴板，然后将它粘贴到电子邮件中。 

    >[!IMPORTANT]
    >你可以编辑电子邮件中的文本，但请务必包括链接，因为它进行了个性化设置，可以将客户直接链接到你的帐户。 
    
3.  完成此步骤后选择“完成”  。

4.  将电子邮件发送到客户。

5.  客户接受你的邀请后，他们会出现在“客户”页面上，你将能够从中为客户预配和管理服务。 

6.  若要管理客户的帐户、服务、用户和许可证，请选择客户名称附近的向下箭头来展开他们的记录，然后选择要管理的服务的管理门户。

>[!IMPORTANT]  
>客户可以在服务的管理门户中重新分配或删除管理员权限。 但是，除非并且直到你与客户重新达成协议，否则即使在客户重新分配或删除管理员权限之后，你仍然要负责提供客户支持并遵守“云经销商协议”的条款。 在这种情况下，如果客户需要帮助，请联系 Microsoft 支持部门以代表客户打开服务请求。

客户可以在 Office 365 管理门户中查找哪些合作伙伴具有他们租户的管理员权限。 若要实现此目的，请执行以下操作：

1. 客户需要以全局管理员身份登录到 Office 365 管理门户。

2. 选择“设置” > “合作伙伴关系”。  

3. 在“合作伙伴关系”页上，客户可以看到与他们合作的合作伙伴列表，以及被授予他们租户的委派管理权限的合作伙伴。 

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>客户可以管理合作伙伴的委派管理员权限 

客户可能决定从他们的租户删除你的委派管理员权限，但会出于订阅和许可续订目的保留与你的关系。 客户可以在 Office 365 管理中心的“合作伙伴关系”页面上管理他们 Office 365 帐户的权限。  在此页面上，客户可以：

- 查看他们已建立关系的合作伙伴以及哪些合作伙伴具有委派管理员权限

- 从租户删除合作伙伴的委派管理权限

删除合作伙伴的委派管理权限：

1. 在“合作伙伴关系”页面上，选择目标合作伙伴。 
2. 在详细信息窗格中，选择“删除委派管理员”。 
3. 在确认窗格中，选择“删除”。 

>[!IMPORTANT]  
>针对合作伙伴的 Azure AD 角色分配是隐式的。 如果你尝试使用 Azure AD 门户/PowerShell/Graph 列出 Azure AD 角色的成员，将不会返回任何合作伙伴。 若要了解合作伙伴是否被分配了 Azure AD 角色，必须参阅 Office 365 管理门户中的合作伙伴关系页面来了解是否已向该合作伙伴授予了委派管理权限。

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD 中的委派管理员权限 

合作伙伴的 Azure AD 租户中有两个用于委派管理的安全组 - 管理员代理和支持人员代理。 当客户将委派管理权限授予合作伙伴时：

- 管理员代理组在客户的 Azure AD 租户中被分配了全局管理员角色。

- 支持人员代理组在客户的 Azure AD 租户中被分配了帮助台管理员角色。

根据分配的目录角色，两个组的成员可以使用客户的合作伙伴凭据和管理员代表客户登录到他们的 Azure AD 租户和 O365 服务。

如果你的客户删除了委派管理员权限，所分配的 Azure AD 角色将被删除，你将不能再管理客户的 Azure AD 租户。

### <a name="azure-subscriptions-and-resource-management"></a>Azure 订阅和资源管理

每一 Azure 订阅都有自己的一组资源管理角色。 CSP 合作伙伴必须被分配有客户的 Azure 订阅下一个或多个角色才能管理客户的 Azure 订阅。 具体而言：

- 当客户接受经销商邀请并向合作伙伴授予委派管理权限时，合作伙伴不会自动获取对客户租户下现有 Azure 订阅的访问权限。

- 当 CSP 合作伙伴为客户预配新 Azure 订阅时，CSP 合作伙伴租户下的管理员代理组会自动被分配为订阅下的所有者角色。 根据此角色分配，组成员可以访问和管理订阅下的资源。

- 当客户通过 Office 365 门户删除合作伙伴的委派管理权限时，合作伙伴仍可以管理客户的 Azure 订阅，前提是该合作伙伴仍被分配有此订阅下的一个或多个角色。 若要阻止合作伙伴管理 Azure 订阅，客户必须删除角色分配。

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

在以下情况下，CSP 合作伙伴可以在合作伙伴中心为他们的客户管理 Autopilot 配置文件，而无需委派管理员权限： 

- 如果客户删除了委派管理权限，但保留了与你之间的经销商关系，那么你可以继续为他们管理 Autopilot 配置文件。

- 你可以管理你或其他合作伙伴已添加的客户设备。 

- 你无法管理客户通过适用于企业的 Microsoft Store、适用于教育的 Microsoft Store 或 Microsoft Intune 门户添加的设备。

若要详细了解 Autopilot，请参阅[使用 Windows Autopilot 简化设备设置](https://docs.microsoft.com/partner-center/autopilot)。

>[!IMPORTANT]  
>合作伙伴中心内当前的 Autopilot 管理体验可能会继续发生改变。 在本文发布之时，我们正在考虑以下更改：

- 合作伙伴必须被客户授予委派管理权限，随后他们才能够从客户租户的任何设备添加/更新/删除配置文件和应用/删除配置文件。

- 合作伙伴必须被客户授予委派管理权限，随后他们才能够删除客户租户中由其他合作伙伴或客户添加的设备。 否则，合作伙伴只能删除自己之前添加的设备。
