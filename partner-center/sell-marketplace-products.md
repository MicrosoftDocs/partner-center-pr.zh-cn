---
title: 销售商业市场产品的订阅 | 合作伙伴中心
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 可以使用合作伙伴中心向客户销售由独立软件供应商 (ISV) 发布到商业市场的软件即服务 (SaaS) 产品的订阅。
author: JnHs
ms.author: jenhayes
keywords: 订阅, 市场, 第三方, ISV
ms.localizationpriority: medium
ms.openlocfilehash: bf3ad75f4bac84163efb4a67009a5d4d7f2261d5
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651638"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>销售商业市场产品的订阅

**适用于**

- 合作伙伴中心

可以使用合作伙伴中心向客户销售由独立软件供应商 (ISV) 发布到商业市场（[Microsoft AppSource](https://appsource.microsoft.com/) 和 [Azure 市场](https://azuremarketplace.microsoft.com/)）的软件即服务 (SaaS) 产品的订阅。 这样可以让你的业务脱颖而出并提供给客户解决其特定业务需求的软件捆绑包。 可以为这些市场 SaaS 产品管理许可证和订阅，就像为 Microsoft 产品管理一样。

有关商业市场的详细信息，请参阅[市场常见问题解答](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)。

> [!IMPORTANT]
> 在合作伙伴中心只能购买软件即服务 (SaaS) 商业市场订阅。 其他商业市场套餐类型（例如 Azure 应用程序、容器或 VM）通过 Azure 门户进行管理，按使用量计费。 必须有现有的 Azure 订阅才能通过 Azure 门户启用即用即付解决方案。

## <a name="view-marketplace-offers-and-pricing"></a>查看市场套餐和定价

若要查看所有可用的商业市场套餐，请从左侧导航菜单中选择“市场”。 默认情况下，你将看到所有类型和类别的产品。 可以按类型和/或类别进行筛选，也可以使用搜索框来搜索特定关键字。 选择一个产品即可查看发布者和可用 SKU 的相关信息，包括是否提供免费试用期。

> [!NOTE]
> 某些在商业市场中提供的产品可能不会显示在这里。 ISV 可以决定是否将其产品提供给合作伙伴中心的云解决方案提供商 (CSP) 合作伙伴。 如果你希望通过合作伙伴中心向你的客户提供商业 marketplace 产品，请在产品列表中找到发布者的联系人信息，并让他们知道你感兴趣。

商业市场产品的价格可能会频繁变化。 若要获取所有商业市场产品的当前定价信息，请在“市场”页的右上角选择“导出价目表”。 这将生成一个包含所有定价数据的电子表格。 此定价信息每日进行更新，因此若要获取当前价格，你可以尽量多查看。

> [!TIP]
> 如果此价目表中的某个产品提供免费试用版，则电子表格会为该产品提供两行内容。 其中一行显示的价格为零，表示提供免费试用版。 另一行包含试用期完后会应用的价格和期限。
>
> 如果此价目表中的某个产品使用[按流量计费](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing)，则期限字段为空。

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>为客户购买商业市场产品

为商业市场 SaaS 产品购买订阅所遵循的流程与为 Microsoft 产品购买订阅所遵循的流程相同。 在购买订阅之前，必须选择一位客户，或者添加一位新客户。

为客户添加订阅时，可以在“发布者”筛选器中选择“合作伙伴”，这样就可以选择只看 ISV 提供的市场套餐。 有关详细信息，请参阅[创建新订阅](create-a-new-subscription.md)。

请注意，在“市场”页中看到的某些套餐也许不能供特定的客户使用。 可用性可能会受到许多因素的影响，包括 ISV 是否支持客户的计费国家/地区。

> [!TIP]
> 也可使用[合作伙伴中心 API](https://docs.microsoft.com/partner-center/develop/) 为客户创建商业市场订阅。 有关详细信息，请参阅[为商业市场产品创建订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。

订阅商业市场产品后，可以选择在取消期（按月订阅为 24 小时，按年订阅为 14 天）内[取消订阅](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription)。 也可[选择是否自动续订订阅](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription)。

## <a name="license-activation-for-commercial-marketplace-products"></a>商业市场产品的许可证激活

对于软件即服务 (SaaS) 套餐类型，许可证的分配和激活由发布产品的独立软件供应商 (ISV) 管理。 若要完成此过程，你将需要访问发布者的站点，并通过授权代码使用个性化链接来识别你的特定购买情况。 可以在购买 SaaS 套餐后显示的确认页上以及在“订阅”页上（在该套餐所在的行中）找到此链接。 也可[使用合作伙伴中心 API 来检索此链接](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)。

当你使用此链接访问发布者的站点时，你将看到预配和分配许可证所需的其他信息或操作，或者完成安装过程。 所需步骤可能因发布者和套餐而异。 你负责提交任何必需信息（或向客户发送用于直接提供此信息的 URL）。 在你提交必需信息以后，发布者会预配并分配相应的许可证。 只有在成功分配许可证后，订阅计费才会开始。

## <a name="access-billing-info-for-commercial-marketplace-products"></a>访问商业市场产品的计费信息

商业市场产品的计费周期从日历月的第一天开始，在日历月的最后一天结束。 我们将在下个月的第8天提供发票。 可以通过合作伙伴中心或合作伙伴中心 API 访问这些发票。

有关详细信息，请参阅[了解合作伙伴中心的计费类型](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges)。

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>为使用商业市场产品的客户提供支持

客户遇到计费和订阅管理问题时，你应该是客户的第一联系点，这一点与使用 Microsoft 产品一样。 有关技术支持，需联系发布者。 Microsoft 不提供对商业 marketplace 产品的支持，但会向你提供发行者的支持联系人信息。

有关详细信息，请参阅[对商业市场产品的支持](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products)和[向客户提供支持](https://docs.microsoft.com/partner-center/customer-support)。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作伙伴中心 API 管理订阅

可以使用合作伙伴中心 API 为商业市场产品创建订阅。 为此，请先获取某个市场的套餐的列表，然后针对特定的商业市场订阅创建并提交一个订单。 最后，检索该订阅的激活链接。

也可使用合作伙伴中心 API 对这些订阅进行生命周期管理和发票管理。

有关详细信息，请参阅[为商业市场产品创建订阅](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。