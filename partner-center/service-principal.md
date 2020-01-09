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
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716888"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>在合作伙伴中心添加 Azure AD 应用程序（服务主体）

在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。 （之前可以在云合作伙伴门户 (CPP) 帐户中执行此操作，但现在你已迁移到合作伙伴中心，因此 CPP 帐户为只读帐户。）请注意，服务主体与 Azure AD 应用程序同义。

## <a name="add-an-azure-ad-application-service-principal"></a>添加 Azure AD 应用程序（服务主体）

1. 从合作伙伴中心面板中，选择“设置”  ，然后选择“开发人员设置”  。

2. 选择“用户”  ，然后选择“添加 Azure AD 应用程序”  。

3. 选择现有的 Azure AD 应用程序，或者新建一个。

4. 如果要新建 Azure AD 应用程序，请提供以下信息：  

  


**回复 URL**：这是用户为了使用 Azure AD 应用程序而可登录的 URL。 

**应用 ID URI**：这是 Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。 

**安全角色**：角色“管理者”  （与 CPP 中的“所有者”角色相同）和“开发人员”  （与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。  

  
