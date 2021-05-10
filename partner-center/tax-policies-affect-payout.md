---
title: 税务策略如何影响 Azure Marketplace 的支出
description: 了解税务政策如何影响 Azure Marketplace 的支出。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686307"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>税务策略如何影响 Azure Marketplace 的支出

**相应的角色**

- 全局管理员
- “用户管理”管理员
- 管理员代理

## <a name="introduction"></a>简介

Microsoft 商业市场的全球覆盖范围。 交易跨边框发生，并且根据 ISV 和客户所在的位置，税务含义可能有所不同。 Microsoft AppSource 和 Azure Marketplace 使用合作伙伴中心税务分析信息来确定 ISV 的国家/地区。 若要确定客户所在的国家/地区，请使用客户的计费信息，或者，如果客户位于欧盟，我们将使用两条不同的信息。

为了更好地了解以下方案，请参阅 [税务详细信息](tax-details-marketplace.md) 表，其中显示 Microsoft 是代表发布者收集和支付税款，还是属于该发布者。

> [!NOTE]
> 本主题中的所有示例销售值和税百分比仅用于说明目的，而不是精确的数字。

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Microsoft 托管税收国家/地区的发布者开展

**方案 A** –在 [Microsoft 管理的税务国家/地区](tax-details-marketplace.md#microsoft-managed-countries)的发布者和客户之间发生的事务。 这些交易将在销售时添加适用的税收，Microsoft 将该税款发送到适用的国家/地区。 不会从付出的支出中预扣税金，而付出的比率则为税收。

请参阅非美国出版社和美国客户之间的交易 [方案 D](#foreign-publisher-transacts-with-us-customer) 。

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="显示用于付出处理方案 A 的工作流。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Microsoft 托管税收国家/地区的发布者开展，其中 Marketplace 费用为应缴税服务

**方案 B** -在基于美国的出版商 (按其合作伙伴中心税务配置文件信息定义的交易) 到 Microsoft 托管的税务国家/地区的客户，国家/地区按 (应缴税的服务) 的 Marketplace 费用收费。 在这种情况下，将从发布者的支出中减去商店服务费用的税费。

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="显示用于处理方案 B 的工作流。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>发布者管理的税务国家/地区中的发布者交易

**方案 C** - 发布者和客户在发布者管理的税务国家/地区内进行的交易，不为客户施加预扣税。 客户在销售时不支付任何税款，发布者有责任支付所有适用的税款。

有关特定于国家/地区定价 (例如，若要偏移即将推出的) ，请参阅商业市场套餐的计划 [和定价](/azure/marketplace/plans-pricing#custom-prices)。

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="显示付款流程方案 C 的工作流。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>外方发布者与美国客户的事务处理

方案 **D** - (在未获得美国税款的国家/地区合作伙伴中心税务配置文件信息) 定义的所有外方发布者 (请参阅方案 [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer))  (通过客户帐户地址) 定义向美国客户进行销售。 美国政府要求 Microsoft 代表发布者扣税。 从付款到发布者的税款是根据产品/服务价格计算的。

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="显示付款流程方案 D 的工作流。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>具有美国客户的 Transacts 的外商发布者

**方案 E** – 所有 (美国合作伙伴中心税务配置文件信息) 所定义的所有外方发布者均按照其客户帐户地址) 的定义向美国客户销售 (。 美国政府不要求 Microsoft 代表发布者扣税。

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="显示付款流程方案 E 的工作流。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>在爱尔兰以外的 Microsoft 托管国家/地区，外 (向注册了欧盟增值税的客户) 

**方案 F** - 外部发布者与欧盟增值税注册客户之间的所有 (在) 国家/地区Microsoft-Managed交易。 客户不支付销售税。

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="显示付款流程方案 F 的工作流。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>在爱尔兰的 Microsoft 托管国家/地区，外 (向注册了欧盟增值税的客户) 

**方案 G** –国外出版商和欧盟 VAT 注册客户之间的所有交易都 (Microsoft-Managed 国家/地区的爱尔兰) 内。 客户支付爱尔兰增值税和 Microsoft 向爱尔兰政府支付这一税款。

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="显示用于处理方案 G 的工作流。":::

## <a name="next-steps"></a>后续步骤

- [发布者常见问题](/azure/marketplace/marketplace-faq-publisher-guide)
- [创建付款和税务配置文件的说明](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)