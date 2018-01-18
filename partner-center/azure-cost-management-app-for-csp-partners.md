---
title: "Azure Cost Management by Cloudyn（面向云解决方案提供商合作伙伴）| 合作伙伴中心"
description: "Azure Cost Management by Cloudyn 需要对合作伙伴中心 API 的访问权限进行预配。"
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: 
ms.openlocfilehash: 3d122e0f88867d16df3713f79e735126b7f40dd4
ms.sourcegitcommit: 628443b08dde9d2f02553b46e669504c620c3da4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/21/2017
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>面向 Azure 云解决方案提供商合作伙伴的 Azure Cost Management  

**适用范围**

-  合作伙伴中心

[获取有关 Azure Cost Management 的详细信息](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>开始之前
为能够使用 Azure Cost Management，请确保你满足以下要求：
- 你是参与云解决方案提供商计划的合作伙伴。
- 你具备创建合作伙伴中心 API Web 应用的能力。

## <a name="overview"></a>概述

Azure Cost Management by Cloudyn 是一款 Web 应用，用于跟踪和管理客户使用 Azure 的程度以及该使用情况所产生的成本。 你可以通过合作伙伴中心 API 使用 Azure Cost Management。

## <a name="register-your-web-app-in-partner-center"></a>在合作伙伴中心注册你的 Web 应用
在合作伙伴中心注册一款 Azure Active Directory Web 应用即可获得合作伙伴中心 API 的访问权限。 
1.  使用[全局管理员或管理员代理帐户](create-user-accounts-and-set-permissions.md)登录到[合作伙伴中心](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)。
2.  在**仪表板**中，选择**帐户设置** &gt; **[应用管理](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**。
3.  在 **Web 应用**部分中，单击**添加新的 Web 应用**。
<br> **注意**：如果此前已创建 Web 应用，你可以跳过第 3 步。
4.  复制并保存你的 Web 应用的**商业 ID** GUID 和**应用 ID** GUID。 你必须拥有这两个 ID，才能使用为期 30 天的 Azure Cost Management 应用免费试用版。

## <a name="add-a-secret-key-to-your-app"></a>为应用添加密钥
1.  在**添加密钥**按钮旁的下拉列表中，选择 1 年或 2 年有效期。
2.  单击**添加密钥**。 
3.  复制并保存密钥值。 你将需要借助此密钥使用为期 30 天的免费试用版。
<br>**注意**：应用程序密钥类似于密码，不过有效期更久。 请将密钥值保存在安全的位置以供今后使用。

## <a name="next-steps"></a>后续步骤
开始使用[为期 30 天的免费试用版](https://go.microsoft.com/fwlink/?linkid=857895)。
你需要提供以下详细信息以开始试用：
- 合作伙伴中心登录凭据
- 商业 ID GUID
- 应用 ID GUID
- 应用程序密钥值
