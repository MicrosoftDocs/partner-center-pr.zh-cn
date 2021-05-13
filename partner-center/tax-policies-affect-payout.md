---
title: 税务政策如何影响支付Azure 市场
description: 了解税务政策如何影响个人Azure 市场。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856009"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>税务政策如何影响支付Azure 市场

**适当的角色**：全局管理员|用户管理管理员|管理员代理

## <a name="introduction"></a>简介

Microsoft 商业市场具有全球覆盖。 交易跨边界发生，根据 ISV 和客户所在的位置，税务影响可能会有所不同。 Microsoft AppSource Azure 市场使用合作伙伴中心税务配置文件信息来确定 ISV 的国家/地区。 若要确定客户的国家/地区，请使用客户的计费信息，或者如果客户位于欧盟，我们将使用两个不同的信息片段。

为了更好地了解以下方案，请参阅税务详细信息表，该表[](tax-details-marketplace.md)显示 Microsoft 是代表发布者收集和支付税款，还是该责任属于发布者。

> [!NOTE]
> 本主题中所有示例销售值和税务百分比仅用于说明目的，而不是确切的数字。

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Microsoft 托管的税务国家/地区中的发布者交易

**方案 A** - 在 Microsoft 管理的税务国家/地区中发布者和客户 [之间发生的交易](tax-details-marketplace.md#microsoft-managed-countries)。 这些交易将在销售时添加适用的税款，Microsoft 会向适用的国家/地区发送该税款。 不从付款中预扣任何税款，付款计算是排他税。

有关 [非美国](#foreign-publisher-transacts-with-us-customer) 发布者与美国客户之间的事务，请参阅方案 D。

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="显示付款流程方案 A 的工作流。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Microsoft 托管的税务国家/地区（其中市场费用为应税服务）中的发布者交易

方案 **B** - 在美国的发布者 (之间（由 合作伙伴中心 税务配置文件信息) 定义）与 Microsoft 托管的税务国家/地区客户之间的交易，该国家/地区对市场费用 (应税服务) 。 在这种情况下，将从发布者的支出中减去商店服务费用的税费。

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="显示用于处理方案 B 的工作流。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>发布者开展

**方案 C** -在发布者管理的税务国家/地区内发生的、不在客户上施加预缴税金的交易。 客户无需支付任何费用，这是发布者支付所有适用税款的义务。

若要详细了解特定于国家/地区的定价 (例如，要抵消即将到来的纳税) 请参阅 [适用于商业应用商店产品的计划和定价](/azure/marketplace/plans-pricing#custom-prices)。

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="显示用于处理方案 C 的工作流。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>外部发布者与美国客户开展

**方案 D** -所有外国出版商 (其在没有美国条约的国家/地区的合作伙伴中心税务配置文件信息) 定义 (参阅 [方案 E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) 向基于美国的客户进行销售 (由其客户帐户地址) 定义。 美国政府要求 Microsoft 预缴税金代表发布者。 根据产品/服务价格计算从发布的比率中预扣的税款。

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="显示用于处理方案 D 的工作流。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>与美国客户的条约开展的外部发布者

**方案 E** –所有外国出版商 (由其合作伙伴中心税务配置文件信息) 在国家/地区的国家/地区，由美国条约向基于美国的客户销售 (由其客户帐户地址) 定义。 美国政府不需要代表发布者进行 Microsoft 的预缴税金。

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="显示用于付出处理方案 E 的工作流。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>外国出版商出售到 Microsoft 托管的国家/地区 (国内) 的欧盟 VAT 注册客户

**方案 F** –在 Microsoft-Managed 国家/地区外 (国内) 以外的外部发布者和欧盟 VAT 注册客户之间的所有交易。 客户不支付销售款项。

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="显示用于支出处理方案 F 的工作流。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>在爱尔兰的 Microsoft 托管国家/地区，外 (向注册了欧盟增值税的客户) 

**方案 G** - 外部发布者与欧盟增值税注册客户之间的所有 (在) 国家/地区Microsoft-Managed交易。 客户支付增值税，Microsoft 将此税款支付给爱尔兰政府。

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="显示付款流程方案 G 的工作流。":::

## <a name="next-steps"></a>后续步骤

- [发布者常见问题解答](/azure/marketplace/marketplace-faq-publisher-guide)
- [有关创建付款和税务配置文件的说明](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)