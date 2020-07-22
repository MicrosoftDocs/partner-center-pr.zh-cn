---
title: 合作伙伴赚取的托管服务返点
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何计算和支付 Microsoft 合作伙伴赚取的托管服务返点 (PEC)，以及如何确保你有资格赚取它们。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 8c42916c253d1ff2497f47c11c640f2805fc0a86
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436736"
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

## <a name="important-eligibility-and-calculation-information"></a>重要的资格和计算信息

- 合作伙伴应已签署有效的 MPN 协议并具有有效的 RBAC 角色，才能赚取 Azure 资产管理工作的返点。 

- 对于间接提供商及其间接经销商，如果间接提供商或/和间接经销商为云解决方案提供商中的客户 Azure 资源提供全天候运营控制和管理，则间接提供商有资格赚取 PEC。

- PEC 与云解决方案提供商中由合作伙伴管理的客户 Azure 资产的计费（可收费）消耗量相关联。 PEC 仅适用于 CSP 中由 Microsoft 计费的合作伙伴（间接提供商和直接计费合作伙伴）。 

- 符合条件的服务：合作伙伴赚取的返点适用于 Azure 计划消费定价（合作伙伴可从 [Azure 计划定价](https://partner.microsoft.com/commerce/sales)页将其导出）中列出的服务。 注意，例外情况包括但不限于，Azure 计划消费定价表和 Azure 计划预留项“标记”列中标识为“第三方”的第三方产品和“市场”定价表中的产品。 。

- PEC 每日计算，可在每日使用情况文件和每月发票对帐文件中查看。 合作伙伴（间接提供商或间接经销商）必须拥有全天 (24x7) 的访问权限，才可确保赚取 PEC。  

- 可赚取 PEC 的最低级别为 Azure 资源级别。 如果合作伙伴在订阅或资源组级别拥有有效的访问权限，则他们可以赚取该角色直到更高一级实体的资源的 PEC。  

- [Azure 成本管理](https://go.microsoft.com/fwlink/?linkid=2106482)中也提供了 PEC 详细信息

## <a name="azure-cost-management"></a>Azure 成本管理

 使用成本分析的 Azure 成本管理 (ACM) 能够让你以合作伙伴的身份查看已享有 PEC 权益的费用。  

1. 在 Azure 门户中，登录到合作伙伴租户，并选择“成本管理”+“计费”。
2.  选择“成本管理”
3.  选择“成本分析”

成本分析视图将显示计费帐户的成本，即以你支付给 Microsoft 的价格购买和使用的所有服务的成本。

4.  在数据透视图的下拉菜单中选择 PartnerEarnedCreditApplied，以查看应用了 PEC 的成本。 如果 PartnerEarnedCreditApplied 属性为 True，则表示关联的成本享有合作伙伴赚取的返点的权益。 

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

