---
title: 工作帐户与合作伙伴中心 | 合作伙伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解为何需要使用工作帐户来创建合作伙伴中心帐户，以及是否已有工作帐户。
author: LauraBrenner
ms.author: labrenne
Keywords: 工作帐户, 电子邮件, 租户, Azure 租户, 创建帐户, 域名
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: c309cd4f79bcc92fa54c903b4517fd5a1b8399fd
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721352"
---
# <a name="your-company-work-account-and-partner-center"></a>公司的工作帐户与合作伙伴中心  

**适用于**

-  合作伙伴中心

**相应的角色**

- 全局管理员
- 用户管理管理员

## <a name="why-you-need-a-work-account"></a>需要工作帐户的原因

我们需要将你所在公司的工作帐户链接到新的合作伙伴中心帐户，以便你的帐户用户可以使用其工作帐户用户名和密码登录到合作伙伴中心。

## <a name="the-work-account-email-address"></a>工作帐户电子邮件地址

工作帐户或工作电子邮件是你的公司提供给你的电子邮件地址。 工作帐户电子邮件通常采用 you@yourcompany.com 格式。 个人电子邮件地址（例如 Hotmail、Gmail 等）不属于工作电子邮件，无法用于合作伙伴中心帐户。 

如果你有多个有效的工作电子邮件地址，请使用与企业总部（而不是区域部门）关联的电子邮件地址，例如，应使用 contoso.com 电子邮件地址，而不要使用 contoso.uk。

> [!NOTE]  
> 在决定使用现有的工作帐户之前，请考虑该工作帐户中需要使用合作伙伴中心的用户数。 如果工作帐户中有些用户不需要使用合作伙伴中心，请考虑只为那些需要使用合作伙伴中心的用户创建一个新帐户。


## <a name="not-sure-if-your-company-already-has-a-work-account"></a>不确定公司是否已有工作帐户？

如果你不确定公司是否有工作帐户，请遵循以下步骤进行检查。 请注意，如果你有有效的 Microsoft Azure 或 Office 365 订阅，则已经有了一个工作帐户。

1. 登录到 Azure 管理门户 (https://ms.portal.azure.com )。

2. 从菜单中选择“Azure Active Directory”，然后选择“域名”。

3. 如果你已有工作帐户，门户将列出你的域名。

如果公司还没有工作帐户，可以在注册过程中创建一个。

下图提供了适用于几个典型场景的步骤：

- 确定是否有工作帐户 
- 确定如何登录到工作帐户 
- 确定是否需要创建新的工作帐户


![是否有工作帐户，或者是否需要创建一个工作帐户？](images/onboardingAADFlow.png)

有关在 Azure AD 中添加域的详细信息，请参阅[在 Azure AD 中添加或关联域](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>关于 Microsoft Azure

Microsoft Azure 是一个公有云平台，公司可以使用该平台在 Microsoft 管理的数据中心的全球网络中构建、部署和管理应用程序。 公司可以使用 Azure 构建一个具有虚拟功能或服务（而非物理计算机）的虚拟 IT 基础结构。 

当你购买 Azure 订阅时，实际上是在 Azure 公有云中租用了一个专用安全空间，这与在办公楼中租用楼层为公司的实体业务提供办公场所没有太大的不同。 对于办公大楼的业主而言，公司就是租户。 

Azure 工作帐户是公司在 Azure 公有云中的专用独立虚拟表示形式，它是在订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时创建的。 

工作帐户托管 Azure AD 用户及其相关信息 - 其密码、个人资料数据、权限等。 工作帐户还包含组、应用程序以及有关公司及其安全性的其他信息。 
