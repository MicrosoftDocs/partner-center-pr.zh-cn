---
title: 受限的直接计费功能
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 直接帐单合作伙伴要求，以及如何避免功能受到限制。 了解你的功能是否受到限制。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: 直接帐单，限制
ms.custom: SEOMAY.20
ms.openlocfilehash: 41db00bab2f421ca3ab0a8f828e8a72b26087ebd
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679414"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>限制直接帐单功能和 CSP 直销合作伙伴所需的要求  

## <a name="overview"></a>概述

直销合作伙伴必须满足 CSP 直销合作伙伴计划中保留的新[要求](direct-partner-new-requirements.md)。 否则，他们直接计费功能的访问权限最终将受到限制并且无法再执行某些特定任务，例如为他们的客户进行新的购买。

> [!Note]
> 如果直接帐单合作伙伴不满足 CSP 直销合作伙伴计划的新要求，Microsoft 将会在其直接帐单功能受到限制时得到通知。 这适用于所有直销合作伙伴，无论他们是否选择[从直接帐单合作伙伴过渡到间接经销商](transition-direct-to-indirect.md)。  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>如何判断您的直接帐单功能是否受到限制

若要确认是否限制了从直接帐单合作伙伴租户到直接计费功能的访问权限，请执行以下步骤。

1. 登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard)。

2. 中转到 "**合作伙伴设置**" "  ->  **合作伙伴配置文件**"。

3. 在 "**程序信息**" 下，查找**Microsoft 云解决方案提供程序状态**。

4. 如果程序状态的值为 "**受限**"，则表示直接帐单合作伙伴租户对直接帐单功能的访问受到限制。

## <a name="affected-direct-bill-capabilities"></a>受影响的直接计费功能

如果你的直接帐单功能受到限制，你将不能再为合作伙伴中心的客户购买新的购买。 此限制包括：

- Azure 订阅

- 基于座位的订阅

- 将新的外接程序添加到现有的基于座位的订阅。

- 为软件和预订产品（例如软件订阅、永久性软件和 Azure 保留虚拟机实例）进行一次性购买。

还不能使用 CSP 计划下的[Azure 合作伙伴共享服务产品/服务](shared-services.md)购买新的 azure 订阅。

现有的直接帐单订阅不受影响。 它们仍有效并且是 autorenewed 的。 在取消之前，你将继续直接向 Microsoft 收取费用。 你仍可通过以下方式管理现有订阅：

- 挂起现有订阅

- 调整现有基于座位的订阅的座位数

- 调整现有加载项对订阅的座位数。 
 
    >[!Note] 
    >不能将新的外接程序添加到现有订阅，因为它被视为新购买。

- 部署新的 Azure 资源，并管理现有 Azure 订阅下的现有 Azure 资源。 这包括通过 Azure marketplace 和 Visual Studio 订阅提供的资源。

除了新购买以外，还不能在合作伙伴中心访问以下直接帐单功能：

- 不能创建新的客户租户。 "合作伙伴中心" 下的 "**客户**" 页下的 "**创建客户**" 选项将不可用。

- 你无法为请求直接分销商关系的客户生成邀请。 合作伙伴中心的 "**客户**" 页下的 "**请求分销商关系**" 选项将不可用。

    >[!NOTE]
    >作为从直销伙伴过渡到间接经销商的一部分，如果你已将直接帐单合作伙伴租户注册为间接经销商，则可以为请求间接经销商关系的客户生成邀请。

- 无法创建新的沙盒租户。 每个直销合作伙伴租户都可以创建一个沙箱租户，用于直接计费 API 集成。 如果你以前未创建过此帐户，则在直接获得帐单合作伙伴功能限制后，不允许这样做。  

## <a name="next-steps"></a>后续步骤

- [成为间接经销商的其他信息](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [云解决方案提供商计划直接合作伙伴新要求](direct-partner-new-requirements.md)