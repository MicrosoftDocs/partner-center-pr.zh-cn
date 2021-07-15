---
title: Azure AD 服务主体
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将服务主体添加到 Azure AD 租户。 这样做意味着在合作伙伴中心添加 Azure AD 应用程序（服务主体）。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551548"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>在合作伙伴中心添加 Azure AD 应用程序（服务主体）

**相应的角色**：全局管理员

在合作伙伴中心的“商业市场”计划中，现在可以将 Microsoft Azure Active Directory (Azure AD) 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。 （你之前可以在云合作伙伴门户 (CPP) 帐户中执行此操作。 在你已迁移到合作伙伴中心后，CPP 帐户会是只读帐户。）
 
>[!Note] 
>服务主体与 Azure AD 应用程序同义。

## <a name="add-an-azure-ad-application-service-principal"></a>添加 Azure AD 应用程序（服务主体）

1. 从合作伙伴中心面板中，选择“设置”，然后选择“开发人员设置”。

2. 选择“用户”，然后选择“添加 Azure AD 应用程序”。

3. 选择现有的 Azure AD 应用程序，或者新建一个。

4. 如果要新建一个 Azure AD 应用程序，请提供以下信息：  

   - **回复 URL**：用户为了使用 Azure AD 应用程序而可登录的 URL。

   - **应用 ID URI**：Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。

   - **安全角色**：角色“管理者”（与 CPP 中的“所有者”角色相同）和“开发人员”（与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。  

## <a name="next-steps"></a>后续步骤

- [合作伙伴中心内的商业市场概述](csp-commercial-marketplace-overview.md)