---
title: 合作伙伴赚取的托管服务返点
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何计算和支付 Microsoft 合作伙伴赚取的托管服务返点 (PEC)，以及如何确保你有资格赚取它们。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182403"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>合作伙伴赚取的返点的计算与支付方式

**相应的角色**

- 全局管理员
- 用户管理员
- 管理员代理
- 计费管理员
- 销售代理

合作伙伴赚取的托管服务返点 (PEC) 是对合作伙伴为客户的部分或整个 Azure 环境提供全天候 IT 运营控制和管理所做努力给予的认可和奖励。 默认情况下，在云解决方案提供商中，合作伙伴对客户订阅拥有必要的访问权限，以便能够对订阅中的资源进行全天候的运营管理和控制。 下一部分将会介绍客户为交易合作伙伴预配访问权限的其他方法。 每月发票金额是合作伙伴赚取的返点净额。 合作伙伴可以在其每月对帐文件中查看 PEC 详细信息。 有关客户可为交易合作伙伴预配访问权限的其他方法，请参阅[管理 Azure 计划中的订阅和资源](azure-plan-manage.md)。

另请参阅[恢复 Azure CSP 订阅的管理员权限](revoke-reinstate-csp.md)

## <a name="eligibility"></a>资格

必须满足以下要求才能收到合作伙伴赚取的返点 (PEC)： 

- 你应已签署有效的 MPN 协议并具有有效的基于角色的访问控制 (RBAC) 角色，才能收到为你管理的 Azure 资产赚取的返点。

- 你必须对客户的 CSP 中的 Azure 资源具有全天候运营控制和管理权限。 这意味着，你必须对客户的 Azure 订阅、Azure 资源组和 Azure 资源具有管理员权限。 对于间接提供商及其间接经销商，如果间接提供商或间接经销商，或者这两者都具有此运营控制，则间接提供商有资格赚取 PEC。 如需了解详细信息，请参阅[恢复 Azure CSP 订阅的管理员权限](./revoke-reinstate-csp.md)。

- 除了上述要求，合作伙伴赚取的返点仅适用于 Azure 计划消费定价中列出的服务，可从[Azure 计划定价](https://partner.microsoft.com/commerce/sales)页面导出此定价。

- PEC 并不适用于以下服务：
    - Azure 计划预留
    - 在 Azure 计划消费定价的“标记”列中被识别为“第三方”的第三方产品
    - 市场价格列表中的产品
    - [Azure 现成虚拟机](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- 可赚取 PEC 的最低级别为 Azure 资源级别。 如果你在订阅或资源组级别拥有有效的访问权限，则每个资源（包括更高一级的实体）都可以赚取 PEC。

- 有关 PEC 的详细信息，请参阅 [Azure 成本管理](/azure/cost-management-billing/costs/get-started-partners)页面。

### <a name="calculation"></a>计算

PEC 每日计算，可在每日使用情况文件和每月发票对帐文件中查看。 合作伙伴（间接提供商或间接经销商）必须拥有全天 (24x7) 的访问权限，才可确保赚取 PEC。 PEC 根据所管理的 Azure 资产每日计算一次。 给定计费周期（月份）的 PEC 不超过 15%。 如果合作伙伴针对所有符合条件的资源（访问范围）保留持久性特权访问一整月（范围跨度），他们将赚取全部 PEC (15%)。 范围和跨度变小将导致当月 PEC 比率变低。 无论是否应用了 PEC，针对 Azure 资产，每天都会显示按每日计费的使用量文件。 合作伙伴还可以注册接收警报，以监视对持久性特权访问的更改。

## <a name="azure-cost-management"></a>Azure 成本管理

使用成本分析的 Azure 成本管理 (ACM) 能够让你以合作伙伴的身份查看已享有 PEC 权益的费用。  

1. 在 [Azure 门户](https://portal.azure.com)中，登录到合作伙伴租户，并选择“成本管理”+“计费”。

2. 选择“成本管理”

3. 选择“成本分析”

   成本分析视图将显示计费帐户的成本，即以你支付给 Microsoft 的价格购买和使用的所有服务的成本。

4. 在数据透视图的下拉菜单中选择 PartnerEarnedCreditApplied，以查看应用了 PEC 的成本。 如果 PartnerEarnedCreditApplied 属性为 True，则表示关联的成本享有合作伙伴赚取的返点的权益。 

   如果 PartnerEarnedCreditApplied 属性为 False，则表示关联的成本不满足所需的返点条件，或者购买的服务不符合合作伙伴赚取的返点条件。

   >[!NOTE] 
   >通常情况下，服务的使用情况在 8-24 小时后才会出现在“成本管理”中，PEC 额度自访问时间起 48 小时内显示在“Azure 成本管理”中。

5. 还可以使用“分组依据和添加”筛选器功能按 PartnerEarnedCreditApplied 属性进行分组和筛选，从而深入分析享有 PEC 权益的成本以及没有应用 PEC 的成本 。

## <a name="next-steps"></a>后续步骤

- [合作伙伴赚取的返点 - 概述](partner-earned-credit.md)

- 在可通过合作伙伴中心仪表板访问（需要登录）的价目表中，提供了合作伙伴赚取的返点的计算方式的详细示例。

- [转移到 Azure 计划 - 入门](azure-plan-get-started.md)

- [管理 Azure 计划中的订阅和资源](azure-plan-manage.md)

- [撤销或恢复 Azure CSP 订阅的管理员权限](revoke-reinstate-csp.md)