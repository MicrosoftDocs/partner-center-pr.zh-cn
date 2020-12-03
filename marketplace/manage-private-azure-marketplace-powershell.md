---
title: 快速入门：使用 PowerShell 管理专用 Azure Marketplace
description: 本快速入门介绍如何使用 Azure PowerShell 在专用 Azure Marketplace 中管理产品/服务。
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536074"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="85d5b-103">快速入门：使用 PowerShell 管理专用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="85d5b-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="85d5b-104">本文介绍如何使用 [Az](/powershell/module/az.marketplace) PowerShell 模块在专用 Azure Marketplace 中管理产品/服务。</span><span class="sxs-lookup"><span data-stu-id="85d5b-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="85d5b-105">私有 Azure Marketplace 目前处于公共预览版中。</span><span class="sxs-lookup"><span data-stu-id="85d5b-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="85d5b-106">此预览版本未提供服务级别协议。</span><span class="sxs-lookup"><span data-stu-id="85d5b-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="85d5b-107">对于生产型工作负荷，不建议使用该预览版。</span><span class="sxs-lookup"><span data-stu-id="85d5b-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="85d5b-108">某些功能可能不受支持或者受限。</span><span class="sxs-lookup"><span data-stu-id="85d5b-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="85d5b-109">有关详细信息，请参阅 [Microsoft Azure 预览版补充使用条款](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)。</span><span class="sxs-lookup"><span data-stu-id="85d5b-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="85d5b-110">要求</span><span class="sxs-lookup"><span data-stu-id="85d5b-110">Requirements</span></span>

* <span data-ttu-id="85d5b-111">如果没有 Azure 订阅，请在开始之前创建一个[免费](https://azure.microsoft.com/free/)帐户。</span><span class="sxs-lookup"><span data-stu-id="85d5b-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="85d5b-112">如果选择在本地使用 Azure PowerShell：</span><span class="sxs-lookup"><span data-stu-id="85d5b-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="85d5b-113">[安装 Az PowerShell 模块](/powershell/azure/install-az-ps)。</span><span class="sxs-lookup"><span data-stu-id="85d5b-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="85d5b-114">使用 [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet 连接到 Azure 帐户。</span><span class="sxs-lookup"><span data-stu-id="85d5b-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="85d5b-115">如果选择使用 Azure Cloud Shell：</span><span class="sxs-lookup"><span data-stu-id="85d5b-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="85d5b-116">有关详细信息，请参阅 [Azure Cloud Shell 概述](https://docs.microsoft.com/azure/cloud-shell/overview)。</span><span class="sxs-lookup"><span data-stu-id="85d5b-116">See [Overview of Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="85d5b-117">尽管 **Az** PowerShell 模块处于预览阶段，但你必须使用 cmdlet 单独安装它 `Install-Module` 。</span><span class="sxs-lookup"><span data-stu-id="85d5b-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="85d5b-118">此 PowerShell 模块正式发布后，它会包含在将来的 Az PowerShell 模块发行版中，并在 Azure Cloud Shell 中默认提供。</span><span class="sxs-lookup"><span data-stu-id="85d5b-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="85d5b-119">如果有多个 Azure 订阅，请选择应当计费的资源所在的相应订阅。</span><span class="sxs-lookup"><span data-stu-id="85d5b-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="85d5b-120">使用 [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet 选择特定订阅。</span><span class="sxs-lookup"><span data-stu-id="85d5b-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="85d5b-121">列出专用商店</span><span class="sxs-lookup"><span data-stu-id="85d5b-121">List private stores</span></span>

<span data-ttu-id="85d5b-122">若要检索专用存储的列表，请使用 [AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85d5b-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="85d5b-123">下面的示例列出了在租户范围下创建的专用存储。</span><span class="sxs-lookup"><span data-stu-id="85d5b-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="85d5b-124">将产品/服务添加到专用 marketplace</span><span class="sxs-lookup"><span data-stu-id="85d5b-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="85d5b-125">若要将产品/服务添加到专用商店，请使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85d5b-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="85d5b-126">下面的示例将指定的提议添加到在租户范围下创建的专用商店的私有 marketplace。</span><span class="sxs-lookup"><span data-stu-id="85d5b-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="85d5b-127">获取专用应用商店产品</span><span class="sxs-lookup"><span data-stu-id="85d5b-127">Get private store offers</span></span>

<span data-ttu-id="85d5b-128">若要获取一个或多个私有存储区，请使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85d5b-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="85d5b-129">下面的示例获取与已添加到租户范围下的指定专用存储关联的提供程序。</span><span class="sxs-lookup"><span data-stu-id="85d5b-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="85d5b-130">删除产品/服务</span><span class="sxs-lookup"><span data-stu-id="85d5b-130">Remove an offer</span></span>

<span data-ttu-id="85d5b-131">若要从专用商店中删除产品/服务，请使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85d5b-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="85d5b-132">下面的示例从已在租户范围中创建的私有存储区中删除一个产品/服务。</span><span class="sxs-lookup"><span data-stu-id="85d5b-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="85d5b-133">后续步骤</span><span class="sxs-lookup"><span data-stu-id="85d5b-133">Next steps</span></span>

<span data-ttu-id="85d5b-134">[创建和管理私有 Azure Marketplace](create-manage-private-azure-marketplace.md)。</span><span class="sxs-lookup"><span data-stu-id="85d5b-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>
