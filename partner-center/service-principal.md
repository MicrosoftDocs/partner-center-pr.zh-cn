---
title: Azure AD 服务主体
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将服务主体添加到 Azure AD 租户。 这样做意味着在合作伙伴中心添加 Azure AD 应用程序（服务主体）。
author: dhirajgandhi
ms.author: dhgandhi
Keywords: Azure, Azure 计划, 服务主体, Azure AD 应用程序
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: bd2880f57d1ccb3c3675fef4fae7499f7ac02f4b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949624"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>在合作伙伴中心添加 Azure AD 应用程序（服务主体）

在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。 （你之前可以在云合作伙伴门户或 CPP 帐户中执行此操作。 在你已迁移到合作伙伴中心后，CPP 帐户会是只读帐户。）
 
>[!Note] 
>服务主体与 Azure AD 应用程序同义。

## <a name="add-an-azure-ad-application-service-principal"></a>添加 Azure AD 应用程序（服务主体）

1. 从合作伙伴中心面板中，选择“设置”，然后选择“开发人员设置”。

2. 选择“用户”，然后选择“添加 Azure AD 应用程序”。

3. 选择现有的 Azure AD 应用程序，或者新建一个。

4. 如果要新建 Azure AD 应用程序，请提供以下信息：  

   - **回复 URL**：用户为了使用 Azure AD 应用程序而可登录的 URL。

   - **应用 ID URI**：Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。

   - **安全角色**：角色“管理者”（与 CPP 中的“所有者”角色相同）和“开发人员”（与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。  
