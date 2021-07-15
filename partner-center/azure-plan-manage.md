---
title: Azure 计划 - 管理订阅和资源
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解合作伙伴如何使用不同基于角色的访问控制 (RBAC) 选项来获得对客户 Azure 资源的操作控制和管理。
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a885d8bbbd7541e199365a7c732aba0b67128053
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277141"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>管理 Azure 计划中的订阅和资源

相应的角色：管理员代理


本文介绍了 CSP 合作伙伴如何使用不同的基于角色的访问控制 (RBAC) 选项对客户的 Azure 资源进行操作控制和管理。 将客户过渡到 Azure 计划时，默认你会获得 Azure 中的特权管理员权限（由管理员代表授予的订阅所有者权限）。

 > [!NOTE]
 > 客户可以在订阅、资源组或工作负荷级别删除 Azure 订阅的管理员权限。 

 合作伙伴可以使用通过基于角色的访问控制功能 (RBAC) 提供的不同选项，获取对客户在云解决方案提供商中的 Azure 资源的全天候操作控制和管理权限。 

- 管理员代表 (AOBO) - 借助 [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)，在合作伙伴租户中具有“管理员代理”角色的任何用户将对你通过云解决方案提供商计划创建的 Azure 订阅拥有 RBAC 所有者访问权限。

- **Azure Lighthouse**：使用 AOBO 不能灵活地创建处理不同客户的不同组，或者为组或用户启用不同的角色。 使用 Azure Lighthouse 可将不同的组分配到不同的客户或角色。 由于用户将通过 Azure 委托的资源管理获取适当的访问级别，因此你可以减少具有“管理员代理”角色的用户数量（因此拥有完全 AOBO 访问权限）。 这有助于通过限制对客户资源的不必要访问权限来提高安全性。 此外，它还可以让你更灵活地大规模管理多个客户。 有关详细信息，请参阅 [Azure Lighthouse 和云解决方案提供商计划](/azure/lighthouse/concepts/cloud-solution-provider)。

- **目录用户、来宾用户或 [服务主体](/azure/active-directory/develop/app-objects-and-service-principals)** ：可以通过将用户添加到客户目录，或者添加来宾用户并分配特定的 RBAC 角色，来委托对 CSP 订阅的精细访问权限。

Microsoft 建议为用户分配最低的权限，使他们能够履行自己的职责即可，这是一种安全做法。 请参阅 [Azure Active Directory Privileged Identity Management 资源](/azure/active-directory/privileged-identity-management/pim-configure)。

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>将合作伙伴 ID (MPN ID) 关联到用于管理客户 Azure 资源的凭据

下表显示了用于将合作伙伴 ID 关联到各种 RBAC 访问选项的方法。

|**类别**   |**方案**   |**MPN ID 关联**|
|-----------------|:------------------------|:------------------|
|AOBO   |CSP 直接合作伙伴或间接提供商为客户创建订阅，并使用 AOBO 将 CSP 直接伙伴或间接提供商指定为该订阅的默认所有者；CSP 直接合作伙伴或间接提供商使用 AOBO 向间接经销商授予对该订阅的访问权限。|自动（无需合作伙伴的干预）|
|Azure Lighthouse|合作伙伴[在市场中创建新的托管服务套餐](/azure/lighthouse/concepts/managed-services-offers)。 此套餐在 CSP 订阅中接受，合作伙伴获取对该 CSP 订阅的访问权限。|自动（无需合作伙伴的干预）|
|Azure Lighthouse|合作伙伴在 Azure 订阅中部署 [ARM 模板](/azure/lighthouse/how-to/onboard-customer)|合作伙伴需要将 MPN ID 关联到合作伙伴租户中的用户或服务主体。 有关详细信息，请参阅[链接合作伙伴 ID](/azure/billing/billing-partner-admin-link-started)。|
|目录或来宾用户|合作伙伴在客户目录中创建新的用户或服务主体，并向用户授予对 CSP 订阅的访问权限。 合作伙伴在客户目录中创建新的用户或服务主体。 伙伴将用户添加到某个组，并向该组授予对 CSP 订阅的访问权限。|合作伙伴需要将 MPN ID 关联到客户租户中的用户或服务主体。 有关详细信息，请参阅[链接合作伙伴 ID](/azure/billing/billing-partner-admin-link-started)。|

## <a name="confirm-that-you-have-admin-access"></a>确认你拥有管理员访问权限

你需要拥有管理员访问权限才能管理客户的服务和接收赚取的返点。 有关赚取的返点的详细信息，请阅读[合作伙伴赚取的返点](partner-earned-credit.md) 可通过两种方式来确认你是否拥有管理员访问权限。

- 查看每日使用情况文件 - 可以通过查看每日使用情况文件中的单价和有效单价，并确认当前是否应用了某种折扣，来确定你是否拥有管理员访问权限。 如果收到了折扣，则你是管理员。

- 创建 Azure Monitor 警报 - 可以创建 Azure Monitor 活动日志[警报](/azure/azure-monitor/platform/alerts-activity-log)，如果从 CSP 订阅中删除了你的 RBAC 访问权限，你将收到通知。

### <a name="create-an-azure-monitor-alert"></a>创建 Azure Monitor 警报

1. 创建警报

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure 警报。":::

2. 选择需要警报执行的操作类型。 例如，如果指定需要电子邮件，则发生任何角色分配删除操作时，你会收到一封通知电子邮件。

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="配置警报。":::

### <a name="aobo-removal"></a>AOBO 删除

客户可以在 Azure 门户上的“访问控制”中管理对其订阅的访问权限。 在“角色分配”选项卡中，选择“删除访问权限”即可。  如果发生这种情况，你可以：

- 与客户沟通，看看是否可以恢复管理访问权限。

- 使用通过[基于角色的访问控制 (RBAC)](/azure/role-based-access-control/overview) 提供的访问权限。

- 使用通过 [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) 提供的访问权限。

基于角色的访问权限不同于管理员访问权限。 角色精确界定你可以和不可以执行的操作。 管理员访问权限更广泛。

若要查看有资格赚取 PEC 的角色，请阅读[可赚取返点的合作伙伴的角色和权限](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)。

## <a name="next-steps"></a>后续步骤

- [撤销和恢复 Azure CSP 订阅的管理员权限](revoke-reinstate-csp.md)

- [合作伙伴赚取的返点 - 概述](partner-earned-credit.md)

- [合作伙伴赚取的托管服务返点](partner-earned-credit-explanation.md)