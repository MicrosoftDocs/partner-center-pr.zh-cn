---
title: 客户将管理权限委派给合作伙伴 | 合作伙伴中心
ms.topic: article
ms.date: 12/18/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 作为经销商合作伙伴，你的客户可以将你作为其管理员。它们还可以删除权限。
author: LauraBrenner
ms.author: labrenne
keywords: 委派的管理员权限，代表的管理员，删除权限，AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 35777dbdaa8ce77f4a1e7154447b37cd62772bc6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653424"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>客户将管理权限委派给合作伙伴

**适用于**

-  合作伙伴中心

若要代表客户管理客户的服务或订阅，客户必须授予你对该服务的管理员权限。 若要从客户那里获取管理员权限，请通过电子邮件向他们发送经销商关系请求。 在客户批准你的请求后，你将能够代表客户登录到服务管理门户并管理该服务。 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>邀请客户与你建立经销商关系

1.  选择 "**客户**"，然后选择 "**请求分销商关系**"。

2.  在下一页上，查看草稿电子邮件。 你可以在默认电子邮件应用程序中打开草稿邮件，或者可以将邮件复制到剪贴板并将其粘贴到电子邮件中。 

    >[!IMPORTANT]
    >你可以编辑电子邮件中的文本，但请务必包括链接，因为它进行了个性化设置，可以将客户直接链接到你的帐户。 
    
3.  完成此步骤后，请选择 "**完成**"。

4.  将电子邮件发送到客户。

5.  客户接受你的邀请后，他们将出现在你的**客户**页面上，并且你将能够在此处为客户预配和管理服务。

6.  若要管理客户的帐户、服务、用户和许可证，请通过在其名称旁选择向下箭头，然后选择要管理的服务的管理门户，来展开客户的记录。

>[!IMPORTANT]  
>客户可以在服务的管理门户中重新分配或删除管理员权限。 但是，除非并且直到你与客户重新达成协议，否则即使在客户重新分配或删除管理员权限之后，你仍然要负责提供客户支持并遵守“云经销商协议”的条款。 在这种情况下，如果客户需要帮助，请与 Microsoft 支持部门联系，以代表客户打开服务请求。

你的客户可以从 Office 365 管理门户中了解他们的哪些合作伙伴对其租户拥有管理员权限。 要实现此目的，请执行以下操作：

1. 客户需要以全局管理员身份登录到 Office 365 管理门户。

2. 选择 "**设置**" > **合作伙伴关系**"。

3. 在 "**合作伙伴关系**" 页上，客户将看到他们工作的合作伙伴的列表，以及已向其租户授予委派管理权限的合作伙伴的列表。

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>客户可以管理合作伙伴的委派管理员权限 

你的客户可以决定从其租户中删除委派的管理员权限，但保留与你的关系，以便进行订阅和许可证续订。 客户在 Office 365 管理中心的**合作伙伴关系**页面管理其 Office 365 帐户的权限。 在此页上，客户可以：

- 查看他们已建立关系的合作伙伴以及哪些合作伙伴具有委派管理员权限

- 从租户中删除合作伙伴的委派管理权限

若要删除合作伙伴的委派管理权限：

1. 在**合作伙伴关系**页上，选择目标合作伙伴。
2. 在详细信息窗格中，选择**删除委派管理员**。
3. 在确认窗格中，选择**删除**。

>[!IMPORTANT]  
>合作伙伴的 Azure AD 角色分配是隐式的。 如果你尝试使用 Azure AD 门户/PowerShell/Graph 列出 Azure AD 角色的成员，将不会返回合作伙伴。 若要了解合作伙伴是否被分配了 Azure AD 角色，则必须参阅 Office 365 Admin 门户中的合作伙伴关系页面来了解是否已向该合作伙伴授予了委派管理权限。

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD 中的委派管理员权限 

在合作伙伴的 Azure AD 租户中，有两个安全组 "管理代理" 和 "支持者" 代理用于委派管理。 当客户将委派管理权限授予合作伙伴时：

- 管理代理组分配给客户的 Azure AD 租户中的全局管理员角色。

- 支持人员代理组分配给客户 Azure AD 租户中的 "支持人员" 管理员角色。

根据所分配的目录角色，这两个组的成员可以使用其合作伙伴凭据和代表客户的管理员登录到客户的 Azure AD 租户和 O365 服务。

如果客户删除了委派的管理员权限，则会删除 Azure AD 角色分配，并且你将无法再管理客户的 Azure AD 租户。

### <a name="azure-subscriptions-and-resource-management"></a>Azure 订阅和资源管理

每个 Azure 订阅都有自己的一组资源管理角色。 在 CSP 合作伙伴可以管理客户的 Azure 订阅之前，必须在 Azure 订阅下将合作伙伴分配到一个或多个角色。 特别是：

- 当客户接受经销商邀请并向合作伙伴授予委派管理权限时，合作伙伴不会自动获取对客户租户下的现有 Azure 订阅的访问权限。

- 当 CSP 合作伙伴为客户预配新 Azure 订阅时，CSP 合作伙伴租户下的管理员代理组将在订阅下被自动分配所有者角色。 根据此角色分配，组成员可以访问和管理订阅下的资源。

- 当客户使用 Office 365 门户从合作伙伴中删除委派的管理权限时，只要合作伙伴仍分配给订阅下的一个或多个角色，伙伴仍可管理客户的 Azure 订阅。 若要阻止合作伙伴管理 Azure 订阅，客户必须删除角色分配。

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

在以下情况下，CSP 合作伙伴可以在合作伙伴中心为其客户管理 Autopilot 配置文件，而无需委派管理员权限： 

- 如果客户删除了委派的管理权限，但与你一起保留了分销商关系，你可以继续为他们管理 Autopilot 配置文件。

- 你可以管理你或其他合作伙伴添加的客户设备。 

- 你无法管理客户通过 Microsoft Store for Business、Microsoft Store 教育或 Microsoft Intune 门户添加的设备。

有关 Autopilot 的详细信息，请参阅[通过 Windows Autopilot 简化设备设置](https://docs.microsoft.com/partner-center/autopilot)。

>[!IMPORTANT]  
>合作伙伴中心的当前 Autopilot 管理体验可能会继续改变。 发布本文时，将考虑以下更改：

- 合作伙伴必须被客户授予委派管理权限，才能够从客户租户的任何设备添加/更新/删除配置文件和应用/删除配置文件。

- 合作伙伴必须被客户授予委派的管理权限，然后合作伙伴才能删除其他合作伙伴或客户租户中的客户添加的设备。 否则，合作伙伴只能删除同一合作伙伴先前添加的设备。
