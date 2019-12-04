---
title: 如何计算合作伙伴盈余合作伙伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何计算 Azure 计划的合作伙伴获得信用（PEC）方面的情况。 这包括合作伙伴和间接提供商的资格要求。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: aee60449a31cf1908912cc1fa62e2bf2c003f998
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721729"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a>如何计算合作伙伴获得的信用额度（PEC）

**相应的角色**

- 全局管理员
- 帐单管理员

在 CSP 中，对部件或其客户的整个 Azure 环境拥有全天候 IT 运营管理的合作伙伴将获得 PEC 奖励。 PEC 作为发票的一部分提供给与 Microsoft 直接计费关系的合作伙伴。 该信用额度每天计算，并反映在月度发票中。 默认情况下，在 CSP 中，为合作伙伴授予了对客户订阅所需的访问权限，使其能够对订阅上的资源进行24X7 操作管理和控制。 下一节介绍了客户可用于预配约束力合作伙伴访问权限的其他方法。


## <a name="important-eligibility-and-calculation-requirements"></a>重要的资格和计算要求：

- 合作伙伴应具有有效的 MPN 协议和基于规则的有效帐户控制（RBAC）角色，以接收他们所管理的 azure 资产的获得的信用额度。 了解有关 [有效 RBAC 角色] 的详细信息

- 如果间接提供程序或其间接经销商，或者两者都具有对 CSP 中客户的 Azure 资源的全天候运营控制和管理，则该提供程序适用于 PEC。

- PEC 与云解决方案提供商中由合作伙伴管理的客户 Azure 资产的计费（可收费）消耗量相关联。 

- PEC 仅适用于由 Microsoft （间接提供商和直接帐单合作伙伴）计费的 CSP 中的合作伙伴。

- 符合条件的服务：合作伙伴获得的信用额度适用于价格列表中提供的所有 Azure 1PP Azure 使用量。 存在例外，包括但不限于3PP 和 Azure 预订。

- PEC 每日计算一次，可以在每日侦测文件中查看。 合作伙伴（通过其提供商提供的提供商或经销商）必须有整天（24x7）的访问权限，以确保他们获得 PEC。

- 可赚取 PEC 的最低级别为 Azure 资源级别。 如果合作伙伴在订阅或资源组级别具有有效的访问权限，则具有更高实体的角色的每个资源将获得 PEC。 

- PEC 将包含在合作伙伴的月度发票中。 发票是收费的。 详细信息显示在 invoice 侦测文件中。

若要了解如何获取管理 Azure 订阅的访问权限，以及如何将 MPN ID 链接到 RBAC 角色，请阅读[Azure 计划下的管理订阅和资源](azure-plan-manage.md)。

有关详细信息

- [Azure 计划-计费](azure-plan-billing.md)

- [CSP 新商务体验的价目表](azure-plan-price-list.md)