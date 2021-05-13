---
title: 受限的直接计费功能
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 直接帐单合作伙伴要求，以及如何避免功能受到限制。 了解你的功能是否受到限制。
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855482"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>限制直接帐单功能和 CSP 直销合作伙伴所需的要求

**适当的角色**：全局管理员

## <a name="overview"></a>概述

直销合作伙伴必须满足 CSP 直销合作伙伴计划中保留的新 [要求](direct-partner-new-requirements.md) 。 否则，他们直接计费功能的访问权限最终将受到限制并且无法再执行某些特定任务，例如为他们的客户进行新的购买。

> [!Note]
> 如果直接帐单合作伙伴不满足 CSP 直销合作伙伴计划的新要求，Microsoft 将会在其直接帐单功能受到限制时得到通知。 这适用于所有直销合作伙伴，无论他们是否选择 [从直接帐单合作伙伴过渡到间接经销商](transition-direct-to-indirect.md) 。  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>如何判断您的直接帐单功能是否受到限制

若要确认是否限制了从直接帐单合作伙伴租户到直接计费功能的访问权限，请执行以下步骤。

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard)。

2. 中转到 "**帐户设置**" "  ->  **法律配置文件**"。

3. 在 " **程序信息**" 下，查找 **Microsoft 云解决方案提供程序状态**。

4. 如果程序状态的值为 " **受限**"，则表示直接帐单合作伙伴租户对直接帐单功能的访问受到限制。

## <a name="affected-direct-bill-capabilities"></a>受影响的直接计费功能

如果你的直接帐单功能受到限制，你将不能再为合作伙伴中心的客户购买新的购买。 此限制包括：

- Azure 订阅

- 基于许可证的订阅

- 将新的外接程序添加到现有的基于许可证的订阅。

- 将软件和预订产品的一次性购买 (例如，软件订阅、永久性软件和 Azure 保留虚拟机实例) 。

还不能使用 CSP 计划下的 [Azure 合作伙伴共享服务产品/服务](shared-services.md) 购买新的 azure 订阅。

现有的直接帐单订阅不受影响。 它们保持有效并且自动续订。 Microsoft 将继续直接向你计费，直到取消它们。 仍可以通过以下方式管理现有订阅：

- 挂起现有订阅

- 调整现有基于许可证的订阅的许可证计数

- 调整订阅中现有加载项的许可证计数。 

    >[!Note]
    >无法将新的加载项添加到现有订阅，因为它被视为新购买。

- 部署新的 Azure 资源，并管理现有 Azure 订阅下的现有 Azure 资源。 这包括通过订阅和订阅Azure 市场Visual Studio资源。

除了新购买项外，你也无法访问以下直接计费功能：合作伙伴中心：

- 无法创建新的客户租户。 "**客户"****页下的**"创建合作伙伴中心选项将不可用。

- 无法生成客户请求建立直接经销商关系的邀请。 "**客户"页** 下的"合作伙伴中心经销商关系"选项将不可用。

    >[!NOTE]
    >在从直接计费合作伙伴过渡到间接经销商过程中，如果已将直接计费合作伙伴租户注册为间接经销商，可以改为生成客户请求间接经销商关系的邀请。

- 无法创建新的沙盒租户。 每个直接计费合作伙伴租户可以创建一个沙盒租户，用于直接计费 API 集成。 如果以前尚未创建一个，则不允许在直接计费合作伙伴功能受到限制后创建一个。  

## <a name="next-steps"></a>后续步骤

- [成为间接经销商的其他信息](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [云解决方案提供商计划直接合作伙伴新要求](direct-partner-new-requirements.md)
