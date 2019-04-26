---
title: 销售 Azure Marketplace 产品的订阅 |合作伙伴中心
ms.topic: article
ms.date: 04/04/2019
description: 可以使用合作伙伴中心销售你的客户订阅的软件即服务 (SaaS) 产品发布到 Azure Marketplace 的独立软件供应商 (Isv)。
author: JnHs
ms.author: jenhayes
keywords: 订阅 Marketplace 中，第三方 ISV
ms.localizationpriority: medium
ms.openlocfilehash: a086ab3a58e926d33c118690e7b171ba4f0fd18b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133827"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>销售 Azure 市场产品的订阅

**适用于**

- 合作伙伴中心

可以使用合作伙伴中心销售你的客户订阅的软件，如服务 (SaaS) 产品发布到[Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace)的独立软件供应商 (Isv)。 这可以帮助区分你的业务和用户提供满足其特定的业务需求的软件捆绑包。 管理许可证和这些 Azure Marketplace SaaS 产品的订阅，就像 Microsoft 产品。

有关 Azure Marketplace 的详细信息，请参阅[Azure Marketplace 常见问题](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)。

## <a name="view-marketplace-offers-and-pricing"></a>查看 Marketplace 产品/服务和定价

若要查看所有可用产品/服务，请选择**Marketplace**左侧的导航菜单中。 默认情况下，你将看到的所有类型和类别的产品。 可以按类型和/或类别中，筛选或使用搜索框搜索特定的关键字。 选择要查看关于发布服务器和可用的 Sku 的信息的产品。

> [!NOTE]
> 此处不会显示 Azure Marketplace 中提供了一些产品。 Isv 可以决定向合作伙伴中心中的云解决方案提供商 (CSP) 合作伙伴提供他们的产品。 如果你看到你想要提供给通过合作伙伴中心客户的 Azure Marketplace 中的产品，Azure Marketplace 中查找发布者的联系信息，让他们知道您感兴趣。

Azure Marketplace 产品的价格可能会频繁变动。 若要获取所有 Marketplace 产品的当前定价信息，请选择**导出的价目表**中的右上角**Marketplace**页。 这将生成所有定价数据电子的表格。 定价信息更新每一天，因此可以经常想要了解当前价格检查。

## <a name="purchase-marketplace-products-for-your-customers"></a>为客户购买 Marketplace 产品

购买 Azure Marketplace SaaS 产品的订阅作为购买订阅的 Microsoft 产品的过程相同。 当为客户添加订阅，你可以选择查看仅 Marketplace 提供从 Isv 通过选择**合作伙伴**中**发布服务器**筛选器。 有关详细信息，请参阅[创建新的订阅](create-a-new-subscription.md)。

> [!IMPORTANT]
> 仅可以在合作伙伴中心服务 (SaaS) 产品订阅作为购买软件。 其他产品/服务类型 （例如 Azure 应用程序、 容器或 Vm） 管理通过 Azure 门户，并基于使用量计费。 若要启用通过 Azure 门户的即用即付解决方案需要现有的 Azure 订阅。

请注意该部分提供了您在中看到**Marketplace**页可能不能与特定客户。 可用性可能会受到许多因素，包括是否 ISV 支持客户的帐单邮寄国家/地区。

> [!TIP]
> 此外可以使用[合作伙伴中心 Api](https://docs.microsoft.com/partner-center/develop/)创建你的客户的 Azure Marketplace 订阅。 有关详细信息，请参阅[创建 Azure Marketplace 产品订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。

与 Azure Marketplace 产品的订阅，可以选择[取消订阅](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription)取消时间段 （对于月度订阅或年度订阅只有 14 天 24 小时） 内。 此外可以[选择是否自动续订此订阅](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription)。

## <a name="access-billing-info-for-marketplace-products"></a>访问 Marketplace 产品的计费信息

Marketplace 产品的计费周期在日历月的第一天开始，在日历月的最后一天结束。 我们将使你的发票可在下个月的第 8 天。 您可以访问这些发票合作伙伴中心中或通过使用合作伙伴中心 Api。

有关详细信息，请参阅[了解在合作伙伴中心计费类型](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges)。

## <a name="provide-support-for-customers-using-marketplace-products"></a>对于使用 Marketplace 产品的客户提供支持

与 Microsoft 产品，您应联系你的客户计费和订阅管理方面的问题的第一个点。 有关技术支持，您将需要联系发布者。 Microsoft 不提供支持的 Marketplace 产品，但将向你提供的发布者支持联系信息。

有关详细信息，请参阅[支持的 Azure Marketplace 产品](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products)并[向客户提供支持](https://docs.microsoft.com/partner-center/customer-support)。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作伙伴中心 Api 管理订阅

可以创建使用合作伙伴中心 Api 获取市场的产品/服务列表中，创建和提交订单 Azure Marketplace 订阅，然后检索激活链接的 Azure Marketplace 产品的订阅。 此外可以使用合作伙伴中心 Api 执行生命周期管理和管理这些订阅的发票。

有关详细信息，请参阅[创建 Azure Marketplace 产品订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。