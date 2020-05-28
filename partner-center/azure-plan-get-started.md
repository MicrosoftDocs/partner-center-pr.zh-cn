---
title: 开始迁移到 Azure 计划
description: 了解你和你的客户需要知道的有关使用 Azure 即用即付计划的信息，包括首要步骤、安全预防措施以及入门方式。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: Azure、Azure 计划、购买订阅、订阅
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 849b205d8a889659647ba8a9cf788428b6b25e21
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394191"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a><span data-ttu-id="9bc94-104">开始将即用即付费率与 Azure 计划配合使用</span><span class="sxs-lookup"><span data-stu-id="9bc94-104">Begin using pay-as-you-go-rates with the Azure plan</span></span>

<span data-ttu-id="9bc94-105">Microsoft 在合作伙伴中心引入了新的商务体验。</span><span class="sxs-lookup"><span data-stu-id="9bc94-105">Microsoft has introduced a new commerce experience in Partner Center.</span></span>  <span data-ttu-id="9bc94-106">使用此新商务体验，合作伙伴可以访问对签署了 Microsoft 客户协议的客户采用即用即付费率的客户的 Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="9bc94-106">With this new commerce experience, partners will gain access to Azure services at pay-as-you-go rates for customers under the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="9bc94-107">此计划简化了购买体验 - 可以在一个 Azure 计划中包含多个 Azure 订阅。</span><span class="sxs-lookup"><span data-stu-id="9bc94-107">This plan simplifies the purchase experience - you can have multiple Azure subscriptions in an Azure plan.</span></span> <span data-ttu-id="9bc94-108">不再需要为每个 Azure 订阅单独提交订单。</span><span class="sxs-lookup"><span data-stu-id="9bc94-108">You no longer need to submit a separate order per Azure subscription.</span></span> <span data-ttu-id="9bc94-109">在 Azure 的此新商务体验中，我们遵守全球一种定价的原则，使 CSP 合作伙伴能够以已发布的价格供应 Azure 产品。</span><span class="sxs-lookup"><span data-stu-id="9bc94-109">And in this new commerce experience for Azure, we have aligned to a single global pricing principle enabling CSP partners to offer Azure at the published prices.</span></span>

<span data-ttu-id="9bc94-110">客户的数字变革要求需要合作伙伴提供新的技能。</span><span class="sxs-lookup"><span data-stu-id="9bc94-110">The digital transformation needs of our customers require new skills from partners.</span></span> <span data-ttu-id="9bc94-111">许多客户希望合作伙伴提供的服务超越交易的价值，使其云旅程变得更平稳，同时帮助他们有效使用 Azure 服务。</span><span class="sxs-lookup"><span data-stu-id="9bc94-111">Many customers look for partners to provide services above and beyond the transaction to make their cloud journey smoother and help consume Azure services efficiently.</span></span> <span data-ttu-id="9bc94-112">Microsoft 合作伙伴在客户生命周期的各个阶段发挥着关键的作用。</span><span class="sxs-lookup"><span data-stu-id="9bc94-112">Microsoft partners play a critical role in all stages of the customer lifecycle.</span></span> <span data-ttu-id="9bc94-113">这些类型的合作伙伴服务实际上在不断发展，其中包括 Azure 资产监视、策略和监管、设置和配置精细调整、技术支持和其他各种服务。</span><span class="sxs-lookup"><span data-stu-id="9bc94-113">These kinds of partner services are on-going in nature and include Azure estate monitoring, policy and governance management, set up and configuration fine-tuning, technical support and a variety of other services.</span></span> <span data-ttu-id="9bc94-114">它们要求合作伙伴非常熟悉客户的 Azure 环境，并能够对其管理的底层资源进行持续适当的监管和控制。</span><span class="sxs-lookup"><span data-stu-id="9bc94-114">They require a partner to be intimately familiar with the customer's Azure environment and have continuous and appropriate governance and control of the underlying resources they manage.</span></span> <span data-ttu-id="9bc94-115">提供这种全天候云运营管理的计费合作伙伴有资格**赚取托管服务的返点**。</span><span class="sxs-lookup"><span data-stu-id="9bc94-115">Billing partners who provide this 24 X 7 cloud-operations management will become eligible for a **Partner earned credit for services managed** for that work.</span></span>

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a><span data-ttu-id="9bc94-116">请确保客户已签署 Microsoft 客户协议</span><span class="sxs-lookup"><span data-stu-id="9bc94-116">Make sure your customers have signed the Microsoft Customer Agreement</span></span>

<span data-ttu-id="9bc94-117">从 2019 年 10 月 1 日起，Microsoft 客户协议已成为永久性的协议，它提供一个全数字化流程，从而简化了客户购买体验。</span><span class="sxs-lookup"><span data-stu-id="9bc94-117">Since October 1, 2019, the Microsoft Customer Agreement, a perpetual agreement that simplifies and streamlines the customer purchasing experience with a fully digital process, is available.</span></span> <span data-ttu-id="9bc94-118">希望利用 Azure 的 CSP 新商务体验的所有客户必须签署 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="9bc94-118">All customers who want to take advantage of the new commerce experience in CSP for Azure must sign the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="9bc94-119">希望在新的 Azure 计划下交易并进行订购的合作伙伴应在生产环境中使用合作伙伴中心面板和 API 确认客户接受 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="9bc94-119">Partners who want to transact under the new Azure plan and make a new order should confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span>

<span data-ttu-id="9bc94-120">从 2020 年 2 月 1 日开始，将从云解决方案提供商计划中删除现有 Microsoft 云协议。</span><span class="sxs-lookup"><span data-stu-id="9bc94-120">Starting February 1, 2020, the existing Microsoft Cloud Agreement is removed from the CSP program.</span></span> <span data-ttu-id="9bc94-121">从那一时间开始，所有其他产品/服务（包括 Microsoft 365、Dynamics 365 和现有 Azure）都需要合作伙伴确认（证明）客户接受新的 Microsoft 客户协议。</span><span class="sxs-lookup"><span data-stu-id="9bc94-121">From that time, partner confirmation (attestation) of the customer acceptance for the new Microsoft Customer Agreement will be required for all other offers including Microsoft 365, Dynamics 365, and existing Azure.</span></span> <span data-ttu-id="9bc94-122">云解决方案提供商中的合作伙伴将无法在没有 Microsoft 客户协议证明的情况下为客户进行订购。</span><span class="sxs-lookup"><span data-stu-id="9bc94-122">Partners in the CSP will not be able to make a new order for the customer without attestation of the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="9bc94-123">有关完整详细信息，请参阅[确认客户接受 Microsoft 客户协议](confirm-customer-agreement.md)</span><span class="sxs-lookup"><span data-stu-id="9bc94-123">For full details, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md)</span></span>

## <a name="security-and-access-control-practices"></a><span data-ttu-id="9bc94-124">安全性和访问控制做法</span><span class="sxs-lookup"><span data-stu-id="9bc94-124">Security and access control practices</span></span>

<span data-ttu-id="9bc94-125">为了保护合作伙伴和客户，我们引入了一系列强制性安全要求，针对那些参与云解决方案提供商计划的顾问、控制面板供应商和合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="9bc94-125">To help safeguard partners and customers, we are introducing a set of mandatory security requirements for Advisors, Control Panel Vendors, and partners participating in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="9bc94-126">一旦我们强制实施这些安全要求，不实施这些强制性要求的合作伙伴将不能在云解决方案提供商计划中进行事务处理，也不能利用委托管理权限来管理客户租户。</span><span class="sxs-lookup"><span data-stu-id="9bc94-126">Partners who do not implement the mandatory security requirements will not be able to transact in the Cloud Solution Provider program or manage customer tenants leveraging delegate admin rights, once these requirements are enforced.</span></span> <span data-ttu-id="9bc94-127">我们准备针对这些要求确定一个严格的强制实施日期，并且会将该日期和相关详细信息告知合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="9bc94-127">We are in the process of establishing a technical enforcement date for the requirements and will notify partners of the date with detailed information.</span></span>

## <a name="actions-to-take-to-implement-mfa"></a><span data-ttu-id="9bc94-128">采取实施 MFA 的措施</span><span class="sxs-lookup"><span data-stu-id="9bc94-128">Actions to take to implement MFA</span></span>

<span data-ttu-id="9bc94-129">考虑到合作伙伴会有很高的特权，因此我们需要确保在每位用户每次进行身份验证时都对其进行 MFA 质询。</span><span class="sxs-lookup"><span data-stu-id="9bc94-129">Given the highly privileged nature of being a partner we need to ensure that each user has an MFA challenge for every single authentication.</span></span> <span data-ttu-id="9bc94-130">可以通过下述方式之一来实现这一点：</span><span class="sxs-lookup"><span data-stu-id="9bc94-130">This can be accomplished through one of the following ways:</span></span>

- <span data-ttu-id="9bc94-131">实施 Azure AD Premium，确保对每位用户强制实施多重身份验证 (MFA)</span><span class="sxs-lookup"><span data-stu-id="9bc94-131">Implementing Azure AD Premium and ensure that multi-factor authentication (MFA) is enforced for each user</span></span>
- <span data-ttu-id="9bc94-132">实施 [Azure AD 安全性默认设置](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="9bc94-132">Implementing the [Azure AD security defaults](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)</span></span>
- <span data-ttu-id="9bc94-133">实现第三方解决方案，确保为每位用户强制实施 MFA</span><span class="sxs-lookup"><span data-stu-id="9bc94-133">Implementing a third-party solution and ensure MFA is enforced for each user</span></span>

<span data-ttu-id="9bc94-134">从 2019 年 8 月 1 日开始，所有合作伙伴都必须对其合作伙伴租户中的所有用户（包括服务帐户）强制实施多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="9bc94-134">Starting August 1, 2019, all partners are required to enforce multi-factor authentication for all users, including service accounts, in their partner tenant.</span></span> <span data-ttu-id="9bc94-135">有关这些安全要求的详细信息，请参阅[合作伙伴安全要求](https://docs.microsoft.com/partner-center/partner-security-requirements)。</span><span class="sxs-lookup"><span data-stu-id="9bc94-135">Detailed information on these security requirements can be found at [Partner security requirements](https://docs.microsoft.com/partner-center/partner-security-requirements).</span></span>

<span data-ttu-id="9bc94-136">Microsoft 建议合作伙伴遵循通过 [Azure Active Directory Privileged Identity Management 资源](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)实现的最佳做法来积极使用 RBAC。</span><span class="sxs-lookup"><span data-stu-id="9bc94-136">Microsoft recommends partners make use of RBAC diligently, following best practices enabled through [Azure Active Directory Privileged Identity Management resources](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>

## <a name="read-more-about-the-azure-plan"></a><span data-ttu-id="9bc94-137">详细了解 Azure 计划</span><span class="sxs-lookup"><span data-stu-id="9bc94-137">Read more about the Azure plan</span></span>

- [<span data-ttu-id="9bc94-138">购买 Azure 计划</span><span class="sxs-lookup"><span data-stu-id="9bc94-138">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

- [<span data-ttu-id="9bc94-139">比较 Azure 套餐</span><span class="sxs-lookup"><span data-stu-id="9bc94-139">Compare Azure offers</span></span>](compare-azure-offers.md)

- [<span data-ttu-id="9bc94-140">合作伙伴赚取的返点 - 概述</span><span class="sxs-lookup"><span data-stu-id="9bc94-140">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="9bc94-141">合作伙伴中心仪表板价目表中提供了合作伙伴赚取的返点 (PEC) 的计算方式，以及有资格赚取合作伙伴返点的角色和所需权限（需要登录）。</span><span class="sxs-lookup"><span data-stu-id="9bc94-141">The partner earned credit (PEC) calculations and the roles and permissions that are eligible to earn partner earned credits are available from your Partner Center Dashboard price list (sign-in required).</span></span>

## <a name="next-steps"></a><span data-ttu-id="9bc94-142">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9bc94-142">Next steps</span></span> 

- [<span data-ttu-id="9bc94-143">如何确定合作伙伴赚取的返点 - 详细信息</span><span class="sxs-lookup"><span data-stu-id="9bc94-143">How the partner earned credit is determined - details</span></span>](partner-earned-credit-explanation.md)
- [<span data-ttu-id="9bc94-144">Azure 计划价目表说明</span><span class="sxs-lookup"><span data-stu-id="9bc94-144">Azure plan price list explained</span></span>](azure-plan-price-list.md)
- [<span data-ttu-id="9bc94-145">将客户过渡到 Azure 计划</span><span class="sxs-lookup"><span data-stu-id="9bc94-145">Transition your customer to Azure plan</span></span>](azure-plan-transition.md)
- [<span data-ttu-id="9bc94-146">管理 Azure 计划中的订阅和资源</span><span class="sxs-lookup"><span data-stu-id="9bc94-146">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
- [<span data-ttu-id="9bc94-147">Azure 计划的上市国家/地区完整列表</span><span class="sxs-lookup"><span data-stu-id="9bc94-147">The full list of countries/regions where Azure plan is available</span></span>](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)
