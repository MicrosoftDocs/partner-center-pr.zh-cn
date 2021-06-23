---
title: 受限的直接计费功能
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解云云解决方案提供商 (CSP) 直接计费合作伙伴要求，以及为避免功能受限而该怎么办。 了解功能是否受到限制。
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551412"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>CSP 直接计费合作伙伴所需的受限直接计费功能和要求

**相应的角色**：全局管理员

## <a name="overview"></a>概述

直接计费合作伙伴必须满足 [新要求](direct-partner-new-requirements.md) ，云解决方案提供商 (CSP) 直接计费合作伙伴计划。 否则，他们直接计费功能的访问权限最终将受到限制并且无法再执行某些特定任务，例如为他们的客户进行新的购买。

> [!Note]
> 不满足 CSP 直接计费合作伙伴计划新要求的直接计费合作伙伴将在直接计费功能受限时告知 Microsoft。 这适用于所有直接计费合作伙伴，无论他们是否已选择从直接计费合作伙伴过渡到 [间接](transition-direct-to-indirect.md) 经销商。  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>如何判断直接计费功能是否受限

若要确认是否已限制从直接计费合作伙伴租户访问直接计费功能，请执行以下步骤。

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard)。

2. 转到"**帐户设置""**  >  **法律配置文件"。**

3. 在 **"程序信息**"下 **，Microsoft 云解决方案提供商状态**。

4. 如果计划状态的值 **受限**，则意味着直接计费合作伙伴租户对直接计费功能的访问权限受到限制。

## <a name="affected-direct-bill-capabilities"></a>受影响的直接计费功能

如果直接计费功能受到限制，则无法再在 合作伙伴中心 中为客户进行新的合作伙伴中心。 此限制包括：

- Azure 订阅

- 基于许可证的订阅

- 将新的加载项添加到现有的基于许可证的订阅。

- 一次购买软件和预留产品，例如 (订阅、永久性软件和 Azure 虚拟机预留) 。

也不能使用 CSP 计划下的 Azure 合作伙伴 [共享](shared-services.md) 服务产品/服务购买新的 Azure 订阅供自己使用。

现有直接计费订阅不受影响。 它们保持有效并自动进行。 Microsoft 将继续直接向你计费，直到取消它们。 仍可以通过以下方式管理现有订阅：

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
