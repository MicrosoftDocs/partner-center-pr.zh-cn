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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="5d58f-103">税务政策如何影响支付Azure 市场</span><span class="sxs-lookup"><span data-stu-id="5d58f-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="5d58f-104">**适当的角色**：全局管理员|用户管理管理员|管理员代理</span><span class="sxs-lookup"><span data-stu-id="5d58f-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="5d58f-105">简介</span><span class="sxs-lookup"><span data-stu-id="5d58f-105">Introduction</span></span>

<span data-ttu-id="5d58f-106">Microsoft 商业市场具有全球覆盖。</span><span class="sxs-lookup"><span data-stu-id="5d58f-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="5d58f-107">交易跨边界发生，根据 ISV 和客户所在的位置，税务影响可能会有所不同。</span><span class="sxs-lookup"><span data-stu-id="5d58f-107">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="5d58f-108">Microsoft AppSource Azure 市场使用合作伙伴中心税务配置文件信息来确定 ISV 的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="5d58f-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="5d58f-109">若要确定客户的国家/地区，请使用客户的计费信息，或者如果客户位于欧盟，我们将使用两个不同的信息片段。</span><span class="sxs-lookup"><span data-stu-id="5d58f-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="5d58f-110">为了更好地了解以下方案，请参阅税务详细信息表，该表[](tax-details-marketplace.md)显示 Microsoft 是代表发布者收集和支付税款，还是该责任属于发布者。</span><span class="sxs-lookup"><span data-stu-id="5d58f-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="5d58f-111">本主题中所有示例销售值和税务百分比仅用于说明目的，而不是确切的数字。</span><span class="sxs-lookup"><span data-stu-id="5d58f-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="5d58f-112">Microsoft 托管的税务国家/地区中的发布者交易</span><span class="sxs-lookup"><span data-stu-id="5d58f-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="5d58f-113">**方案 A** - 在 Microsoft 管理的税务国家/地区中发布者和客户 [之间发生的交易](tax-details-marketplace.md#microsoft-managed-countries)。</span><span class="sxs-lookup"><span data-stu-id="5d58f-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="5d58f-114">这些交易将在销售时添加适用的税款，Microsoft 会向适用的国家/地区发送该税款。</span><span class="sxs-lookup"><span data-stu-id="5d58f-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="5d58f-115">不从付款中预扣任何税款，付款计算是排他税。</span><span class="sxs-lookup"><span data-stu-id="5d58f-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="5d58f-116">有关 [非美国](#foreign-publisher-transacts-with-us-customer) 发布者与美国客户之间的事务，请参阅方案 D。</span><span class="sxs-lookup"><span data-stu-id="5d58f-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="显示付款流程方案 A 的工作流。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="5d58f-118">Microsoft 托管的税务国家/地区（其中市场费用为应税服务）中的发布者交易</span><span class="sxs-lookup"><span data-stu-id="5d58f-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="5d58f-119">方案 **B** - 在美国的发布者 (之间（由 合作伙伴中心 税务配置文件信息) 定义）与 Microsoft 托管的税务国家/地区客户之间的交易，该国家/地区对市场费用 (应税服务) 。</span><span class="sxs-lookup"><span data-stu-id="5d58f-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="5d58f-120">在这种情况下，将从发布者的支出中减去商店服务费用的税费。</span><span class="sxs-lookup"><span data-stu-id="5d58f-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="显示用于处理方案 B 的工作流。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="5d58f-122">发布者开展</span><span class="sxs-lookup"><span data-stu-id="5d58f-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="5d58f-123">**方案 C** -在发布者管理的税务国家/地区内发生的、不在客户上施加预缴税金的交易。</span><span class="sxs-lookup"><span data-stu-id="5d58f-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="5d58f-124">客户无需支付任何费用，这是发布者支付所有适用税款的义务。</span><span class="sxs-lookup"><span data-stu-id="5d58f-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="5d58f-125">若要详细了解特定于国家/地区的定价 (例如，要抵消即将到来的纳税) 请参阅 [适用于商业应用商店产品的计划和定价](/azure/marketplace/plans-pricing#custom-prices)。</span><span class="sxs-lookup"><span data-stu-id="5d58f-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="显示用于处理方案 C 的工作流。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="5d58f-127">外部发布者与美国客户开展</span><span class="sxs-lookup"><span data-stu-id="5d58f-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="5d58f-128">**方案 D** -所有外国出版商 (其在没有美国条约的国家/地区的合作伙伴中心税务配置文件信息) 定义 (参阅 [方案 E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) 向基于美国的客户进行销售 (由其客户帐户地址) 定义。</span><span class="sxs-lookup"><span data-stu-id="5d58f-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="5d58f-129">美国政府要求 Microsoft 预缴税金代表发布者。</span><span class="sxs-lookup"><span data-stu-id="5d58f-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="5d58f-130">根据产品/服务价格计算从发布的比率中预扣的税款。</span><span class="sxs-lookup"><span data-stu-id="5d58f-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="显示用于处理方案 D 的工作流。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="5d58f-132">与美国客户的条约开展的外部发布者</span><span class="sxs-lookup"><span data-stu-id="5d58f-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="5d58f-133">**方案 E** –所有外国出版商 (由其合作伙伴中心税务配置文件信息) 在国家/地区的国家/地区，由美国条约向基于美国的客户销售 (由其客户帐户地址) 定义。</span><span class="sxs-lookup"><span data-stu-id="5d58f-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="5d58f-134">美国政府不需要代表发布者进行 Microsoft 的预缴税金。</span><span class="sxs-lookup"><span data-stu-id="5d58f-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="显示用于付出处理方案 E 的工作流。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="5d58f-136">外国出版商出售到 Microsoft 托管的国家/地区 (国内) 的欧盟 VAT 注册客户</span><span class="sxs-lookup"><span data-stu-id="5d58f-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="5d58f-137">**方案 F** –在 Microsoft-Managed 国家/地区外 (国内) 以外的外部发布者和欧盟 VAT 注册客户之间的所有交易。</span><span class="sxs-lookup"><span data-stu-id="5d58f-137">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="5d58f-138">客户不支付销售款项。</span><span class="sxs-lookup"><span data-stu-id="5d58f-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="显示用于支出处理方案 F 的工作流。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="5d58f-140">在爱尔兰的 Microsoft 托管国家/地区，外 (向注册了欧盟增值税的客户) </span><span class="sxs-lookup"><span data-stu-id="5d58f-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="5d58f-141">**方案 G** - 外部发布者与欧盟增值税注册客户之间的所有 (在) 国家/地区Microsoft-Managed交易。</span><span class="sxs-lookup"><span data-stu-id="5d58f-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="5d58f-142">客户支付增值税，Microsoft 将此税款支付给爱尔兰政府。</span><span class="sxs-lookup"><span data-stu-id="5d58f-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="显示付款流程方案 G 的工作流。":::

## <a name="next-steps"></a><span data-ttu-id="5d58f-144">后续步骤</span><span class="sxs-lookup"><span data-stu-id="5d58f-144">Next steps</span></span>

- [<span data-ttu-id="5d58f-145">发布者常见问题解答</span><span class="sxs-lookup"><span data-stu-id="5d58f-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="5d58f-146">有关创建付款和税务配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="5d58f-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)