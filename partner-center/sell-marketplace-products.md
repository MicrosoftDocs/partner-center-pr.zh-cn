---
title: 向 Azure Marketplace 产品销售订阅 |合作伙伴中心
ms.topic: article
ms.date: 07/12/2019
description: 你可以使用合作伙伴中心向由独立软件供应商 (Isv) 发布到 Azure Marketplace 的软件即服务 (SaaS) 产品中销售客户订阅。
author: JnHs
ms.author: jenhayes
keywords: 订阅, Marketplace, 第三方, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 4dda776e7ebdece3a8a15c3576b64d93d3e4158c
ms.sourcegitcommit: dd961f85bc790e56c70479a5926177454dd8e855
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2019
ms.locfileid: "67854503"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>销售 Azure 市场产品的订阅

**适用于**

- 合作伙伴中心

你可以使用合作伙伴中心向由独立软件供应商 (Isv) 发布到[Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace)的软件即服务 (SaaS) 产品中销售客户订阅。 这有助于区分你的业务, 并为客户提供满足其特定业务需求的软件捆绑。 你可以像对 Microsoft 产品一样, 管理这些 Azure Marketplace SaaS 产品的许可证和订阅。

有关 Azure Marketplace 的详细信息, 请参阅[Azure Marketplace 常见问题解答](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)。

## <a name="view-marketplace-offers-and-pricing"></a>查看 Marketplace 产品/服务定价

若要查看所有可用的产品/服务, 请从左侧导航菜单中选择 " **Marketplace** "。 默认情况下, 你将看到所有类型和类别的产品。 您可以按类型和/或类别进行筛选, 或者使用 "搜索" 框搜索特定关键字。 选择产品以查看有关发布者和可用 Sku 的信息, 包括是否提供免费试用期。

> [!NOTE]
> Azure Marketplace 中提供的某些产品可能未显示在此处。 Isv 可以决定是否向合作伙伴中心的云解决方案提供商 (CSP) 合作伙伴提供产品。 如果你在 Azure Marketplace 中看到你希望通过合作伙伴中心提供给客户的产品, 请在 Azure Marketplace 中找到该发布者的联系人信息, 并让他们知道你感兴趣。

Azure Marketplace 产品的价格可能会频繁更改。 若要获取所有 Marketplace 产品的最新定价信息, 请选择 " **marketplace** " 页右上角的 "**导出价目表**"。 这将生成一个包含所有定价数据的电子表格。 定价信息每天更新一次, 因此, 你可以根据需要查看其最新价格。

> [!TIP]
> 如果此列表中的产品提供了免费试用版, 则电子表格将包括该产品的两行。 一行将显示零的价格, 表示有可用的免费试用版。 其他行将包含试用期结束后将应用的价格和条款。

## <a name="purchase-marketplace-products-for-your-customers"></a>为客户购买 Marketplace 产品

Azure Marketplace SaaS 产品的购买订阅遵循的过程与购买 Microsoft 产品的订阅相同。 为客户添加订阅时, 可以通过在**发布者**筛选器中选择 "**合作伙伴**" 来选择仅查看 isv 提供的 Marketplace 产品/服务。 有关详细信息, 请参阅[创建新订阅](create-a-new-subscription.md)。

> [!IMPORTANT]
> 你只能在合作伙伴中心购买 "软件即服务" (SaaS) 产品订阅。 其他产品/服务类型 (如 Azure 应用程序、容器或 Vm) 通过 Azure 门户进行管理, 并根据使用情况进行计费。 若要通过 Azure 门户启用即用即付解决方案, 需要现有的 Azure 订阅。

请注意, 在 " **Marketplace** " 页中看到的某些产品/服务可能不可用于特定客户。 可用性可能会受到许多因素的影响, 包括 ISV 是否支持客户的计费国家/地区。

> [!TIP]
> 你还可以使用[合作伙伴中心 api](https://docs.microsoft.com/partner-center/develop/)为你的客户创建 Azure Marketplace 订阅。 有关详细信息, 请参阅[为 Azure Marketplace 产品创建订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。

通过订阅 Azure Marketplace 产品, 你可以选择在取消期限 (每月订阅24小时, 每年订阅14天) 内[取消订阅](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription)。 你还可以[选择是否自动续订订阅](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription)。

## <a name="license-activation-for-marketplace-products"></a>Marketplace 产品的许可证激活

对于软件即服务 (SaaS) 产品/服务 (SaaS) 产品/服务类型, 通过发布该产品的独立软件供应商 (ISV) 管理许可证分配和激活。 若要完成此过程, 你将需要访问发布者的站点, 并通过授权代码使用个性化链接来识别你的特定购买情况。 你可以在购买 SaaS 产品/服务后出现的 "确认" 页上找到此链接, 并在 "**订阅**" 页上找到 (在该产品/服务的行中)。 你还可以[使用合作伙伴中心 api 检索此链接](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)。

当你使用此链接访问发布者的站点时, 你将看到预配和分配许可证所需的其他信息或操作, 或者完成安装过程。 所需的步骤可能因发布者和产品/服务而异。 你负责提交任何所需的信息 (或向客户发送 URL 以直接提供此信息)。 提供所需的信息后, 发布者将设置并分配适当的许可证。 仅在成功分配许可证后才开始订阅计费。

## <a name="access-billing-info-for-marketplace-products"></a>访问 Marketplace 产品的计费信息

对于 Marketplace 产品, 计费周期从日历月的第一天开始, 到日历月的最后一天结束。 我们将在下个月的第8天提供发票。 你可以在合作伙伴中心或使用合作伙伴中心 Api 来访问这些发票。

有关详细信息, 请参阅[了解合作伙伴中心的计费类型](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges)。

## <a name="provide-support-for-customers-using-marketplace-products"></a>为使用 Marketplace 产品的客户提供支持

与 Microsoft 产品一样, 你应该是客户的第一个联系点, 以了解有关计费和订阅管理的问题。 若要获得技术支持, 需要与发布者联系。 Microsoft 不对 Marketplace 产品提供支持, 但会向你提供发行者的支持联系人信息。

有关详细信息, 请参阅对[Azure Marketplace 产品的支持](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products)和[向客户提供支持](https://docs.microsoft.com/partner-center/customer-support)。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作伙伴中心 Api 管理订阅

你可以使用合作伙伴中心 Api 为 Azure Marketplace 产品创建订阅, 方法是获取市场产品/服务的列表, 创建并提交 Azure Marketplace 订阅的订单, 然后检索激活链接。 你还可以使用合作伙伴中心 Api 来执行生命周期管理, 并管理这些订阅的发票。

有关详细信息, 请参阅[为 Azure Marketplace 产品创建订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。