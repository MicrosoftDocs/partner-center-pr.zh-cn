---
title: 客户将管理权限委派给合作伙伴 | 合作伙伴中心
ms.topic: article
ms.date: 12/18/2018
description: 作为分销商合作伙伴，你的客户可以委派你是其管理员。它们还可以删除权限。
author: LauraBrenner
ms.author: labrenne
keywords: 委派的管理员权限，管理员代表的删除特权，DAP，AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 9253bcca2d93d9f0d62d6d7241132f0c0c9bf5ec
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586150"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>客户将管理权限委派给合作伙伴

**适用于**

-  合作伙伴中心

若要代表客户管理客户的服务或订阅，客户必须授予你对该服务的管理员权限。 若要从客户那里获取管理员权限，请通过电子邮件向他们发送经销商关系请求。 在客户批准你的请求后，你将能够代表客户登录到服务管理门户并管理该服务。 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>邀请客户与你建立经销商关系

1.  选择**客户**，然后选择**请求经销商关系**。

2.  在下一页上，查看草稿电子邮件。 你可以在默认电子邮件应用程序中打开草稿邮件，或者可以将邮件复制到剪贴板并将其粘贴到电子邮件中。 

    >[!IMPORTANT]
    >你可以编辑电子邮件中的文本，但请务必包括链接，因为它进行了个性化设置以将客户直接链接到你的帐户。 
    
3.  完成此步骤后选择**完成**。

4.  将电子邮件发送到客户。

5.  客户接受你的邀请后，他们将出现在你的**客户**页面上，并且你将能够在此处为客户预配和管理服务。

6.  若要管理客户的帐户、 服务、 用户和许可证，选择其名称旁边的向下箭头，展开客户的记录，然后选择管理门户中你想要管理的服务。

>[!IMPORTANT]  
>客户可以重新分配或删除服务的管理门户中的管理员权限。 但是，除非并且直到你与客户重新达成协议，否则即使在客户重新分配或删除管理员权限之后，你仍然要负责提供客户支持并遵守“云经销商协议”的条款。 在此情况下，如果客户需要帮助，请联系 Microsoft 支持部门提出服务请求代表客户。

你的客户可以找出哪些合作伙伴具有到 Office 365 管理门户中从其租户的管理员权限。 要实现此目的，请执行以下操作：

1. 客户需要在登录到 Office 365 管理门户为全局管理员。

2. 选择**设置** → **合作伙伴关系**。

3. 上**合作伙伴关系**页上，客户将看到使用其合作伙伴的列表，并且那些已被授予委派给其租户管理权限。

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>客户可以管理合作伙伴的委派管理员权限 

客户可能会决定从其租户中删除你的委派的管理员特权，但保留与你的订阅和许可证续订的关系。 客户在 Office 365 管理中心的**合作伙伴关系**页面管理其 Office 365 帐户的权限。 在此页上，客户可以：

- 查看他们已建立关系的合作伙伴以及哪些合作伙伴具有委派管理员权限

- 从租户删除合作伙伴的委派管理权限

若要删除合作伙伴的委派管理权限：

1. 在**合作伙伴关系**页上，选择目标合作伙伴。
2. 在详细信息窗格中，选择**删除委派管理员**。
3. 在确认窗格中，选择**删除**。

>[!IMPORTANT]  
>合作伙伴的 Azure AD 角色分配是隐式的。 如果你尝试使用 Azure AD 门户/PowerShell/Graph 列出 Azure AD 角色的成员，将不会返回合作伙伴。 若要了解合作伙伴是否被分配了 Azure AD 角色，则必须参阅 Office 365 Admin 门户中的合作伙伴关系页面来了解是否已向该合作伙伴授予了委派管理权限。

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD 中的委派管理员权限 

合作伙伴的 Azure AD 租户中有两个安全组用于委派管理 - 管理员代理和支持人员代理。 当客户将委派管理权限授予合作伙伴时：

- 管理员代理组在客户的 Azure AD 租户中被分配全局管理员角色。

- 支持人员代理组在客户的 Azure AD 租户中被分配咨询台管理员角色。

根据分配的目录角色，两个组的成员可以使用其合作伙伴凭据和管理员代表客户登录到客户的 Azure AD 租户和 O365 服务。

如果你的客户删除了委派管理员权限，所分配的 Azure AD 角色将被删除，你将不能再管理客户的 Azure AD 租户。

### <a name="azure-subscriptions-and-resource-management"></a>Azure 订阅和资源管理

每个 Azure 订阅都有自己的一组资源管理角色。 CSP 合作伙伴必须在 Azure 订阅下被分配一个或多个角色才能管理客户的 Azure 订阅。 特别是：

- 当客户接受经销商邀请并向合作伙伴授予委派管理权限时，合作伙伴不会自动获取对客户租户下的现有 Azure 订阅的访问权限。

- 当 CSP 合作伙伴为客户预配新 Azure 订阅时，CSP 合作伙伴租户下的管理员代理组将在订阅下被自动分配所有者角色。 根据此角色分配，组成员可以访问和管理订阅下的资源。

- 当客户通过 Office 365 门户删除合作伙伴的委派管理权限时，合作伙伴仍可以管理客户的 Azure 订阅，前提是该合作伙伴在订阅下仍被分配有一个或多个角色。 若要阻止合作伙伴管理 Azure 订阅，客户必须删除角色分配。

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

在合作伙伴中心，CSP 合作伙伴可以管理 Autopilot 配置文件，供其客户无需在这些情况下委派的管理员权限： 

- 如果客户删除委派的管理权限，但会保留与你的经销商关系，您可以继续管理他们的 Autopilot 配置文件。

- 你可以管理您或另一个合作伙伴已添加的客户设备。 

- 不能管理通过 Microsoft Store for Business、 教育版的 Microsoft Store 或 Microsoft Intune 门户添加了您的客户的设备。

Autopilot 有关详细信息，请参阅[简化与 Windows Autopilot 设备设置](https://docs.microsoft.com/partner-center/autopilot)。

>[!IMPORTANT]  
>合作伙伴中心中的当前 Autopilot 管理体验可能会继续将更改。 在本文发布时，被视为以下更改：

- 合作伙伴必须被客户授予委派管理权限，才能够从客户租户的任何设备添加/更新/删除配置文件和应用/删除配置文件。

- 合作伙伴之前，必须授予委派的管理权限由客户合作伙伴可以添加其他合作伙伴或客户租户中的客户的设备中删除。 否则，合作伙伴可以删除以前添加的同一个合作伙伴的设备。
