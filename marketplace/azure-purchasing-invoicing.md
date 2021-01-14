---
title: 从 Azure Marketplace 购买软件和解决方案
description: 了解可在 Azure Marketplace 中简化和简化软件购买和管理的工具。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 8f7962b1b040be90f7dc1b2696a2ced3830d25b9
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182471"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace 购买

Azure Marketplace 提供了许多工具和功能，可简化和简化采购策略的购买、开票和管理过程。

## <a name="simplified-procurement"></a>简化采购

Azure 市场提供不同的购买选项，有助于你简化采购流程。 如果使用与你的 Azure 帐户关联的信用卡购买产品，则所有购买将合并到单个发票上，并按所选信用卡计费。 如果你是一家大型客户，则可以使用企业协议来购买。 使用 EA，任何购买的软件都将自动包含在 Azure 发票中。 你的发票将首先包含 Azure 使用费用，然后是 Azure 市场费用。

通过 Azure Marketplace 购买时，消除了管理单个供应商关系和发票的复杂性。 你将获得 Microsoft 的单个合并月度帐单，其中包含 Azure Marketplace 购买和 Azure 费用。

## <a name="permission-to-purchase"></a>要购买的权限

找到合适的软件应用程序后，即可完成购买。 但是，你将需要在 Azure 订阅中具有适当的权限。 由于 Azure 在 [基于角色的访问控制](/azure/role-based-access-control/overview) (RBAC) 模型上操作，因此你的帐户需要 **订阅所有者** 或 **参与者** 权限来进行购买。

在完成购买之前，请确保用户在 Azure 租户中配置正确。 这将有助于防止在购买过程中出现错误。

在 Azure 门户的 Azure Marketplace 体验中，找到要购买的应用程序，然后选择 " **创建** " 或 " **设置 + 订阅**"。 系统将提示你完成一些信息，然后才能使用新解决方案。

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="&quot;产品/服务&quot; 按钮。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="&quot;设置 + 订阅&quot; 按钮。":::

如果要从 Azure Marketplace 在线商店部署解决方案，请在 "产品描述" 页上选择 " **立即获取** "，然后使用 Azure 帐户凭据登录。

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="&quot;Azure Marketplace 登录&quot; 对话框。":::

登录后，你将被重定向到 Azure 门户中的产品来完成购买。

## <a name="purchase-policy-management"></a>购买策略管理

Microsoft 允许你通过计费配置文件以 Azure 订阅管理员的身份来管理用户购买情况。 从以下三个选项中进行选择：

- **免费 + 付费** –允许用户获取任何 Azure Marketplace 软件应用程序。
- **免费** –允许用户仅部署 Azure Marketplace 中的免费软件。
- **否** –阻止用户从 Azure Marketplace 部署任何软件。

这些设置将应用于有权访问 Azure 订阅的所有用户，这使你可以通过 Azure 门户控制 IT 采购。

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="通过 Azure 门户控制 IT 采购":::

## <a name="cost-management"></a>成本管理

当你从 Azure Marketplace 购买产品时，你希望获得有助于管理成本的见解。 Azure 成本管理是一个免费工具，可用于查看有关已购买产品的信息。 您可以使用成本管理来查看在一段时间内支出的服务的详细信息，以及这些成本如何针对您所设置的预算进行跟踪。 除了设置预算之外，您还可以计划报表和分析订阅成本。 若要详细了解 Azure 成本管理，请完成 [使用 Azure 成本管理分析成本和创建预算](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)的 Microsoft Learn 模块。

你可以在 Azure 成本管理下的成本分析工具上查看你的 Azure 市场费用和发票。

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="使用 Azure 成本管理获取所购买产品的见解。":::

## <a name="next-steps"></a>后续步骤

- [计费和开票](billing-invoicing.md)