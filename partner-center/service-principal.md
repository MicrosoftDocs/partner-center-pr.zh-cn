---
title: Azure AD 服务主体 | 合作伙伴中心
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将服务主体添加到 Azure AD 租户
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure 计划, 服务主体, Azure AD 应用程序
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010378"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>在合作伙伴中心添加 Azure AD 应用程序（服务主体）

在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为 Azure AD 租户中的用户。 （之前可以在云合作伙伴门户 (CPP) 帐户中执行此操作，但现在你已迁移到合作伙伴中心，因此 CPP 帐户为只读帐户。）请注意，服务主体与 Azure AD 应用程序同义。

## <a name="add-an-azure-ad-application-service-principal"></a>添加 Azure AD 应用程序（服务主体）

1. 从合作伙伴中心面板中，选择“设置”  ，然后选择“开发人员设置”  。

2. 选择“用户”  ，然后选择“添加 Azure AD 应用程序”  。

3. 选择现有的 Azure AD 应用程序，或者新建一个。

4. 如果要新建 Azure AD 应用程序，请提供以下信息：  
  
**名称**：这类似于 CPP 门户中的“易记名称”字段。

**回复 URL**：这是用户为了使用 Azure AD 应用程序而可登录的 URL。 

**应用 ID URI**：这是 Azure AD 应用程序在向 Azure AD 发送单一登录请求时所显示的逻辑标识符。 

**安全角色**：角色“管理者”  （与 CPP 中的“所有者”角色相同）和“开发人员”  （与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。  

选择“保存”  以在合作伙伴中心创建此应用程序时，该信息也会同步回 CPP 系统。  
