---
title: 从公司购买软件和Azure 市场
description: 了解简化和简化软件购买和管理的工具Azure 市场。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 0e79674825f8ab28fa4b0e68dd01c9c1b7e8c27a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565179"
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

> [!CAUTION]
> 批准专用市场并不表示已采购解决方案。

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="产品/服务&quot;创建&quot;按钮。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="&quot;设置 + 订阅&quot;按钮。":::

如果要从在线商店部署Azure 市场，请在产品说明页上选择"立即获取"，然后使用 Azure 帐户凭据登录。

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="&quot;Azure 市场登录&quot;对话框。":::

登录后，你将被重定向到Azure 门户完成购买。

## <a name="purchase-policy-management"></a>购买策略管理

Microsoft 允许以 Azure 订阅管理员角色通过计费配置文件管理用户购买。 从三个选项中进行选择：

- **免费 +** 付费 - 允许用户获取任何Azure 市场应用程序。
- **免费** - 允许用户仅从 Azure 市场。
- **否** – 阻止用户部署任何软件Azure 市场。

这些设置适用于有权访问 Azure 订阅的所有用户，这让你能够通过门户控制 IT Azure 门户。

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="通过 IT 部门控制AZURE 门户。":::

## <a name="cost-management"></a>成本管理

从公司购买Azure 市场时，需要获取有助于管理成本的见解。 Azure 成本管理是一个免费工具，用于查看已购买产品的信息。 可以使用成本管理来查看在一段时间花费哪些服务的详细信息，以及这些成本如何根据你设置的预算进行跟踪。 除了设置预算，还可以计划报表和分析订阅成本。 若要详细了解Azure 成本管理，请完成有关使用 Microsoft Learn 分析成本和创建预算上的[Azure 成本管理。](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

你可以在 Azure 成本管理下的成本分析工具上查看你的 Azure 市场费用和发票。

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="使用Azure 成本管理获取所购买产品的见解。":::

## <a name="purchase-validation-checks"></a>购买验证检查

通过产品/服务Azure 市场可能会出于不同原因失败。 将命令行接口 (CLI) 更有可能导致错误，因为你可能尝试购买的产品/服务在 Azure 市场 中不可用或不可见。 下面是可能导致购买失败的检查：

1. 订阅属于 EA 企业协议 (，) EA 管理员已禁用Azure 市场购买。
1. EA 管理员仅为免费产品/服务启用了购买，并且该产品/服务是付费产品/服务。
1. 在市场中找不到此产品/服务。
1. 独立软件供应商 (ISV) 停止销售产品/服务，至少在你的区域。
1. 你使用的订阅属于产品/服务不可用的地区的计费帐户。
1. 订阅/计费帐户不与有效的付款方式 (例如有效的信用卡) 。
1. 订阅属于云解决方案提供商云解决方案提供商 (，) ISV 拒绝通过 CSP 进行销售。
1. 专用市场订阅已启用，并且套餐不在允许的套餐列表中。
1. 产品/服务是特定客户的专用/预览版，订阅不在允许的客户列表中。

如果市场产品/服务与组织中 Azure 管理员定义的Azure Policy冲突，则购买市场产品/服务可能会失败。 例如，如果 Microsoft.SaaS 不在组织的允许列表中，则不能 **购买** 它。 有关详细信息，请参阅Azure Policy [文档](/azure/governance/policy/)。

## <a name="next-steps"></a>后续步骤

- [计费和开票](billing-invoicing.md)