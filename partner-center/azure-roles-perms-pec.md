---
title: 角色，针对合作伙伴获得的信用额度的权限
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解合作伙伴可以获得合作伙伴获得的信用额度（PEC）的角色和权限。 这些角色不同于合作伙伴中心的角色。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: af21fe17afdab07ef259634d9df18d65ae072d5d
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908268"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>符合合作伙伴获得的信用额度的角色和权限

以下角色映射到用于确定合作伙伴是否有资格获得合作伙伴获得信用额度的权限级别。

>[!Important]
>这些角色和权限不同于用户在合作伙伴中心工作时所需的角色和权限。

|**Role**   |**说明**   |**可用 PEC**   |
|-----------------|:------------------|:--------------|
|“所有者”  |您可以管理所有内容，包括对资源的访问权限。|是|
|参与者 |除授予资源访问权限外，你还可以管理所有内容。|是|
|读取器|您可以查看所有内容，但不能进行任何更改|否|
|ACRDelete|acr delete|是|
|ACRImageSigner|ACR 映像签名程序|是|
|ACRPull|acr 拉取|是|
|AcrPush|acr 推送|是|
|AcrQuarantineReader|ACR 隔离数据读取器|否|
|AcrQuarantineWriter| ACR 隔离数据编写器|是|
|API 管理服务参与者|可以管理服务和 API|是|
|API 管理服务操作员角色|可以管理服务，但不可管理 API|是|
|API 管理服务读者角色|对服务和 API 的只读访问权限|否|
|Application Insights 组件参与者|管理 Application Insights 组件|是|
|Application Insights 快照调试器|授予用户查看和下载使用 Application Insights Snapshot Debugger 收集的调试快照的权限。 请注意，所有者或参与者角色中未包括这些权限。|是|
|