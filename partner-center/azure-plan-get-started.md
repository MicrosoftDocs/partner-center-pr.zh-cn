---
title: 开始迁移到 Azure 计划
description: 了解你和你的客户需要知道的有关使用 Azure 即用即付计划的信息，包括首要步骤、安全预防措施以及入门方式。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: Azure、Azure 计划、购买订阅、订阅
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 849b205d8a889659647ba8a9cf788428b6b25e21
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394191"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>开始将即用即付费率与 Azure 计划配合使用

Microsoft 在合作伙伴中心引入了新的商务体验。  使用此新商务体验，合作伙伴可以访问对签署了 Microsoft 客户协议的客户采用即用即付费率的客户的 Azure 服务。

此计划简化了购买体验 - 可以在一个 Azure 计划中包含多个 Azure 订阅。 不再需要为每个 Azure 订阅单独提交订单。 在 Azure 的此新商务体验中，我们遵守全球一种定价的原则，使 CSP 合作伙伴能够以已发布的价格供应 Azure 产品。

客户的数字变革要求需要合作伙伴提供新的技能。 许多客户希望合作伙伴提供的服务超越交易的价值，使其云旅程变得更平稳，同时帮助他们有效使用 Azure 服务。 Microsoft 合作伙伴在客户生命周期的各个阶段发挥着关键的作用。 这些类型的合作伙伴服务实际上在不断发展，其中包括 Azure 资产监视、策略和监管、设置和配置精细调整、技术支持和其他各种服务。 它们要求合作伙伴非常熟悉客户的 Azure 环境，并能够对其管理的底层资源进行持续适当的监管和控制。 提供这种全天候云运营管理的计费合作伙伴有资格**赚取托管服务的返点**。

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>请确保客户已签署 Microsoft 客户协议

从 2019 年 10 月 1 日起，Microsoft 客户协议已成为永久性的协议，它提供一个全数字化流程，从而简化了客户购买体验。 希望利用 Azure 的 CSP 新商务体验的所有客户必须签署 Microsoft 客户协议。

希望在新的 Azure 计划下交易并进行订购的合作伙伴应在生产环境中使用合作伙伴中心面板和 API 确认客户接受 Microsoft 客户协议。

从 2020 年 2 月 1 日开始，将从云解决方案提供商计划中删除现有 Microsoft 云协议。 从那一时间开始，所有其他产品/服务（包括 Microsoft 365、Dynamics 365 和现有 Azure）都需要合作伙伴确认（证明）客户接受新的 Microsoft 客户协议。 云解决方案提供商中的合作伙伴将无法在没有 Microsoft 客户协议证明的情况下为客户进行订购。

有关完整详细信息，请参阅[确认客户接受 Microsoft 客户协议](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>安全性和访问控制做法

为了保护合作伙伴和客户，我们引入了一系列强制性安全要求，针对那些参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴。

一旦我们强制实施这些安全要求，不实施这些强制性要求的合作伙伴将不能在云解决方案提供商计划中进行事务处理，也不能利用委托管理权限来管理客户租户。 我们准备针对这些要求确定一个严格的强制实施日期，并且会将该日期和相关详细信息告知合作伙伴。

## <a name="actions-to-take-to-implement-mfa"></a>采取实施 MFA 的措施

考虑到合作伙伴会有很高的特权，因此我们需要确保在每位用户每次进行身份验证时都对其进行 MFA 质询。 可以通过下述方式之一来实现这一点：

- 实施 Azure AD Premium，确保对每位用户强制实施多重身份验证 (MFA)
- 实施 [Azure AD 安全性默认设置](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- 实现第三方解决方案，确保为每位用户强制实施 MFA

从 2019 年 8 月 1 日开始，所有合作伙伴都必须对其合作伙伴租户中的所有用户（包括服务帐户）强制实施多重身份验证。 有关这些安全要求的详细信息，请参阅[合作伙伴安全要求](https://docs.microsoft.com/partner-center/partner-security-requirements)。

Microsoft 建议合作伙伴遵循通过 [Azure Active Directory Privileged Identity Management 资源](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)实现的最佳做法来积极使用 RBAC。

## <a name="read-more-about-the-azure-plan"></a>详细了解 Azure 计划

- [购买 Azure 计划](purchase-azure-plan.md)

- [比较 Azure 套餐](compare-azure-offers.md)

- [合作伙伴赚取的返点 - 概述](partner-earned-credit.md)

- 合作伙伴中心仪表板价目表中提供了合作伙伴赚取的返点 (PEC) 的计算方式，以及有资格赚取合作伙伴返点的角色和所需权限（需要登录）。

## <a name="next-steps"></a>后续步骤 

- [如何确定合作伙伴赚取的返点 - 详细信息](partner-earned-credit-explanation.md)
- [Azure 计划价目表说明](azure-plan-price-list.md)
- [将客户过渡到 Azure 计划](azure-plan-transition.md)
- [管理 Azure 计划中的订阅和资源](azure-plan-manage.md)
- [Azure 计划的上市国家/地区完整列表](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)
