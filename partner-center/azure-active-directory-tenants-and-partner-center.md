---
title: "Azure Active Directory 租户和合作伙伴中心 | 合作伙伴中心"
description: "若要创建合作伙伴中心帐户，你的公司必须拥有 Azure Active Directory (Azure AD) 租户。 Azure AD 是 Microsoft 的基于云的目录和标识管理服务。"
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Azure Active Directory 租户和合作伙伴中心  

**适用于**

-  合作伙伴中心

## <a name="why-you-need-an-azure-ad-tenant"></a>为什么需要 Azure AD 租户

我们需要将你的组织 Azure AD 租户链接到新的合作伙伴中心帐户，以便你的租户用户可以使用其 Azure AD（Microsoft 帐户）用户名和密码登录合作伙伴中心。

如果你的公司已经拥有 Azure AD 租户，你可以将其链接到你的合作伙伴中心帐户。 

>**注意**<br> 在你决定使用现有的 Azure AD 租户之前，请考虑租户中将需要使用合作伙伴中心的用户数。 如果租户中有些用户不需要使用合作伙伴中心，请考虑只为将需要使用合作伙伴中心的那些用户创建一个新租户。

如果你的公司还没有 Azure AD 租户，则可以在注册过程中免费创建一个。 在**登录 Azure Active Directory** 页面上选择**创建新租户**。 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>不确定你的公司是否已经具有 Azure AD 租户？

如果你不确定你的公司是否具有 Azure AD 租户，请按照以下步骤进行检查。 请注意，如果你具有有效的 Microsoft Azure 或 Office 365 订阅，则你已经拥有了 Azure AD 租户。
1.  登录到 Azure 管理门户，网址为 https://ms.portal.azure.com
2.  从菜单中选择“Azure Active Directory”，然后选择“域名”。
3.  如果你已经有租户，则将列出你的域名。

### <a name="using-an-existing-tenant"></a>使用现有租户？

如果你想要使用现有的 Azure AD 租户，但在登录时遇到问题，请在下图中查找最符合你的情况的方案，然后按照推荐的步骤进行操作。 

![是具有 Azure AD 租户还是需要创建一个租户？](images/onboardingAADFlow.png)

有关在 Azure AD 中添加域的详细信息，请参阅[在 Azure AD 中添加或关联域](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>关于 Microsoft Azure

Microsoft Azure 是一个公共云平台，公司可以使用该平台在 Microsoft 管理的数据中心的全球网络中构建、部署和管理应用程序。 公司可以使用 Azure 构建一个具有虚拟功能或服务（而非物理计算机）的虚拟 IT 基础结构。 

当你购买 Azure 订阅时，你实际上是在 Azure 公共云中租用了一个专用安全空间，这与在办公楼中租用楼层为公司的实体业务提供办公场所没有太大的不同。 对于办公大楼的业主而言，公司就是租户。 

Azure AD 租户是 Azure 公共云中公司的专用独立虚拟表示形式，并且是在你订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时为你创建的。 

你的租户托管 Azure AD 用户及其相关信息 - 其密码、配置文件数据、权限等。 租户还包含组、应用程序以及关于公司及其安全性的其他信息。 

若要了解有关 Azure AD 的详细信息，请参阅 [Azure Active Directory 文档](https://docs.microsoft.com/ azure/active-directory/)。 