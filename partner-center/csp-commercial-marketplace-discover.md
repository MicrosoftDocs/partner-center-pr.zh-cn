---
title: 发现产品/服务-商业应用商店
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 合作伙伴如何使用合作伙伴中心来查看或搜索 marketplace，以获取 SaaS 产品/服务的市场，或从独立软件供应商处 (Isv) 的定价。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147966"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>在合作伙伴中心商业市场中发现产品/服务和定价

**适当的角色**：全局管理员 |管理代理

当独立的软件供应商 (Isv) 选择在商业应用商店中发布产品/服务时，他们还可以决定是否要在 CSP 计划中提供该产品/服务。 如果他们选择通过 CSP 计划销售该产品/服务，则 CSP 合作伙伴应在合作伙伴中心市场领域看到该产品/服务。

如果 ISV 产品/服务未按预期显示在合作伙伴中心，原因可能是：

- ISV 决定不通过 CSP 计划出售产品/服务。 例如，某些 ISV 产品可能已在商业市场 (的其他区域中提供，例如 [Microsoft AppSource](https://appsource.microsoft.com/) 和 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) ，但可能不会在合作伙伴中心 marketplace 中的 CSP 计划中显示为合作伙伴。

- ISV 决定为仅选择数量的 CSP 合作伙伴提供产品/服务。 有关专用产品/服务的详细信息，请参阅本帮助主题后面的。

- 产品/服务类型可能无法通过合作伙伴中心或 Azure 门户 (例如容器或某些基于使用情况的产品/服务的) 。

- 此 ISV 产品/服务可能不支持关联客户 (s) 的计费国家/地区。

## <a name="view-marketplace-offers-in-partner-center"></a>在合作伙伴中心查看 Marketplace 产品/服务

若要查看 CSP 计划中的可用商业 marketplace 产品/服务：

1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)，然后从左侧导航菜单中选择 " **CSP** "。

2. 选择 " **销售**"，再选择 " **Marketplace**"。 默认情况下，你将看到所有类型和类别的产品。

3. 按类型或类别选择筛选器。 你还可以使用 **搜索** 来查找特定的关键字，提供名称或 ISV 发布者的名称。

4. 从列表中选择特定的产品/服务。 这会将你打开产品"概述"选项卡，可在其中了解有关产品/服务的信息。 此选项卡上的信息可能包括： 

    - 产品或产品/服务的说明

    - 有关 ISV 发布服务器详细信息

    - 指向 ISV 发布者上传的文档或营销材料的链接

    - 其他可能的 ISV 联系人，用于客户支持、工程或 CSP 计划的联系人

5. 若要详细了解套餐的可用计划、SKUS 或定价，请选择"计划 + 定价 **"** 选项卡。此选项卡将显示：

    - 提供此产品/服务的市场

    - 产品/服务可用的 SKUS 或计划列表

    - 每个可用的 SKU 或计划的定价

## <a name="view-marketplace-offers-via-partner-center-apis"></a>通过 API 查看合作伙伴中心产品/服务

CSP 计划合作伙伴还可使用 API 返回符合条件的产品/服务列表。 符合条件的产品/服务仅包括合作伙伴可通过市场销售的 SaaS ISV 合作伙伴中心产品/服务。 对于使用 API 在目录中标识产品/服务的合作伙伴，请参阅获取市场 [产品/服务列表的指南](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)。

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>查看最新的市场产品/服务定价合作伙伴中心

按照以下步骤获取与产品/服务关联的最新定价详细信息：

1. 登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)，然后从左侧导航菜单中选择 **"CSP"。**

2. 选择 **"销售**"，然后选择 **"定价和产品/服务"。**

3. 向下滚动到"市场 **"** 部分，选择一个位置并下载 **"市场定价"。** 这会生成一个电子表格，其中包含来自 ISV 发布者提供的 SaaS、基于许可证的产品/服务和计量服务的最新定价数据。 此处还可能会显示一些 Azure 应用程序定价。 此信息每日更新，因此，你可以在选择时查看其最新价格。

4. 如果 ISV 产品包含免费试用期，则电子表格将为该产品显示两行：

    - 一行显示免费试用价格为零。 这意味着有一个免费试用期。

    - 另一行显示了在免费试用期结束后将应用的价格和条款。

作为 CSP 计划合作伙伴，你可能有资格享受与特定商业 marketplace 产品/服务相关的其他奖励。 有关其他奖励的详细信息，请参阅 [csp 激励指南](https://aka.ms/partnerincentives) (需要 csp 登录) 。

## <a name="learn-about-marketplace-exclusive-offers"></a>了解 marketplace 专用产品/服务

Isv 可以选择仅向 CSP 计划中的特定合作伙伴提供其产品/服务。 这称为独家提议。 CSP 计划中的所有合作伙伴仍可查看合作伙伴中心商用 marketplace 中的所有 ISV 产品/服务，包括标记为独占的产品/服务。

如果产品/服务 **未** 标记为 "专用"，则所有合作伙伴都可以购买该产品/服务， (假设所选客户的计费国家/地区与 ISV 产品/服务的国家/地区可用性) 。

但对于标记为 "独占" 的任何产品/服务，只有 ISV 选择的合作伙伴才能购买该产品/服务。

> [!NOTE]
> 如果你看到一个标记为 "独占" 的产品/服务要销售给客户，请直接联系 ISV 并要求提供销售独家产品/服务的权限。 查看专用产品/服务的详细信息时，可能会看到可供选择的 " **联系人 ISV** " 链接。

若要了解有关商业应用商店中的 ISV 体验的详细信息，请参阅 [云解决方案提供商](/azure/marketplace/cloud-solution-providers)。

有关 marketplace 中的 CSP 体验的详细信息，请阅读 [商业市场概述](csp-commercial-marketplace-overview.md)。

## <a name="next-steps"></a>后续步骤

- [购买商业市场优惠](csp-commercial-marketplace-purchase.md)