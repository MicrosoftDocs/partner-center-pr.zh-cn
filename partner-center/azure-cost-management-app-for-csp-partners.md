---
title: Cloudyn for Csp 的 Azure 成本管理
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心注册 Cloudyn web 应用并使用它的密钥，以便可以使用该应用来跟踪客户的 Azure 使用情况和成本。
author: aparnagkrishnan
ms.author: aparnag
Keywords: Azure 成本管理应用，管理成本，web 应用
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 521501f9a979c0993d299ab30443168408656a44
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390444"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>使用适用于 CSP 合作伙伴的 Azure 成本管理应用跟踪客户的 Azure 使用情况和成本  

**适用于**

- 合作伙伴中心
- 云解决方案提供商计划合作伙伴

**相应的角色**

- 全局管理员
- 管理员代理

[获取有关 Azure Cost Management 的详细信息](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>开始之前
为能够使用 Azure Cost Management，请确保你满足以下要求：

- 你是参与云解决方案提供商计划的合作伙伴。
- 你具备创建合作伙伴中心 API Web 应用的能力。

## <a name="overview"></a>概述

Cloudyn 是一个 web 应用，可用于跟踪和管理你的客户使用 Azure 的量和该使用量的成本。 你可以通过合作伙伴中心 API 使用 Azure Cost Management。

## <a name="register-your-web-app-in-the-partner-center"></a>在合作伙伴中心注册你的 Web 应用
在合作伙伴中心注册一款 Azure Active Directory Web 应用即可获得合作伙伴中心 API 的访问权限。 
1.  使用[全局管理员或管理员代理帐户](create-user-accounts-and-set-permissions.md)登录到[合作伙伴中心](https://partnercenter.microsoft.com/pcv/dashboard/overview)。
2.  从 "**合作伙伴中心**"，选择 "**帐户设置**" " &gt; **[应用管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**"。
3.  在 **Web 应用**部分中，单击**添加新的 Web 应用**。
<br> **注意**：如果此前已创建 Web 应用，你可以跳过第 3 步。
4.  复制并保存你的 Web 应用的**商业 ID** GUID 和**应用 ID** GUID。 你必须拥有这两个 ID，才能使用为期 30 天的 Azure Cost Management 应用免费试用版。

## <a name="add-a-secret-key-to-your-app"></a>为应用添加密钥
1. 在**添加密钥**按钮旁的下拉列表中，选择 1 年或 2 年有效期。
2. 单击 "**添加密钥**"。 
3. 复制并保存密钥值。 你将需要借助此密钥使用为期 30 天的免费试用版。<br>
   > [!NOTE]  
   > 应用程序密钥类似于密码，具有较长的到期日期。 请将密钥值保存在安全的位置以供今后使用。

## <a name="next-steps"></a>后续步骤
开始使用[为期 30 天的免费试用版](https://go.microsoft.com/fwlink/?linkid=857895)。
你需要提供以下详细信息以开始试用：
- 合作伙伴中心登录凭据
- 商业 ID GUID
- 应用 ID GUID
- 应用程序密钥值
