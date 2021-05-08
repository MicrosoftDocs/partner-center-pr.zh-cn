---
title: 从公司购买软件和Azure 市场
description: 了解简化和简化软件购买和管理的工具Azure 市场。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 04/15/2021
ms.openlocfilehash: cfe37f26ad685ca723336d8559d15d4a64048f4b
ms.sourcegitcommit: 2ad9e61fa5b9941f927ebf44c459b6c1bd055b9d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/08/2021
ms.locfileid: "109630077"
---
# <a name="azure-marketplace-purchasing"></a>Azure 市场购买

Azure 市场有许多工具和功能，可简化购买、开票和管理购买策略的过程。

## <a name="simplified-procurement"></a>简化采购

Azure 市场提供不同的购买选项，有助于你简化采购流程。 如果使用与 Azure 帐户关联的信用卡购买产品，则所有购买都将合并到单个发票上，并按选择的信用卡计费。 如果你是大型客户，可以使用客户企业协议。 使用 EA 时，任何软件购买都会自动包含在 Azure 发票中。 你的发票将首先包含 Azure 使用费用，然后是 Azure 市场费用。

通过客户购买Azure 市场，可以消除管理各个供应商关系和发票的复杂性。 你从 Microsoft 获得单个合并的每月帐单，其中包含你的Azure 市场和 Azure 费用。

## <a name="permission-to-purchase"></a>购买权限

找到正确的软件应用程序后，完成购买非常简单。 但是，需要在 Azure 订阅中拥有适当的权限。 由于 Azure 对基于角色的访问控制 (RBAC) 模型进行操作，因此帐户需要订阅所有者或参与者权限才能进行购买。 [](/azure/role-based-access-control/overview)

完成购买之前，请确保用户在 Azure 租户中具有正确的配置。 这有助于防止在购买过程中出错。

在Azure 市场体验Azure 门户，找到要购买的应用程序，然后选择 **"创建或** 设置 + 订阅 **"。** 系统会提示你先完成一些信息，然后才能使用新解决方案。

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="产品/服务&quot;创建&quot;按钮。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="&quot;设置 + 订阅&quot;按钮。":::

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

## <a name="purchase-validation-checks"></a>购买验证检查

出于不同的原因，通过 Azure Marketplace 购买产品/服务可能会失败。 使用命令行界面 (适用于购买的 CLI) 更有可能会导致错误，因为你可能尝试购买在 Azure Marketplace 中不可用或不可见的产品/服务。 下面是可能导致购买失败的检查：

1. 订阅属于 EA 企业协议 (，) EA 管理员已禁用Azure 市场购买。
1. EA 管理员仅为免费产品/服务启用了购买，并且该产品/服务是付费产品/服务。
1. 在市场中找不到此产品/服务。
1. 独立软件供应商 (ISV) 已 (停止销售) 产品/服务，至少在你的区域。
1. 你使用的订阅属于产品/服务不可用的地区的计费帐户。
1. 订阅/计费帐户不与有效的付款方式 (例如有效的信用卡) 。
1. 订阅属于云解决方案提供商云解决方案提供商 (，) ISV 拒绝通过 CSP 进行销售。
1. 专用市场订阅已启用，并且套餐不在允许的套餐列表中。
1. 产品/服务是特定客户的专用/预览版，订阅不在允许的客户列表中。

## <a name="next-steps"></a>后续步骤

- [计费和开票](billing-invoicing.md)