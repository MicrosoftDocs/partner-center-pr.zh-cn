---
title: 合作伙伴中心见解-基于角色的访问控制 |合作伙伴中心
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 需要特定角色才能查看见解报告
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI，性能，客户成功，量化指标，角色
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945859"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="680dd-104">对见解仪表板的基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="680dd-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="680dd-105">Insights 仪表板使用合作伙伴中心中的两个新角色来管理员工对报表的访问-Executive 报表查看器和报表查看器。</span><span class="sxs-lookup"><span data-stu-id="680dd-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="680dd-106">Executive 报表查看器角色中的用户可以访问所有报表数据集，而报表查看器角色中的用户将无法访问敏感数据集，例如收入和客户/员工个人数据。</span><span class="sxs-lookup"><span data-stu-id="680dd-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="680dd-107">与其他合作伙伴中心角色一样，全局管理员或帐户管理员可以在用户管理页上将用户分配到这些角色。</span><span class="sxs-lookup"><span data-stu-id="680dd-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="680dd-108">这些角色可以在整个公司或特定 MPN 位置上适用。</span><span class="sxs-lookup"><span data-stu-id="680dd-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="680dd-109">分配给特定 MPN 位置的角色限制用户仅查看与所选 MPN 位置关联的报表数据。</span><span class="sxs-lookup"><span data-stu-id="680dd-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="680dd-110">合作伙伴可以从以下视图中选择一个或多个位置。</span><span class="sxs-lookup"><span data-stu-id="680dd-110">Partner can select one or multiple locations from the below view.</span></span>

![角色](images/pci/roles.png)

><span data-ttu-id="680dd-112">纪录在2020年1月20日 MPN 管理员的用户将自动添加到该租户的所有位置的公司范围的 "Executive 报表查看器" 角色。</span><span class="sxs-lookup"><span data-stu-id="680dd-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="680dd-113">因此，这些用户可以将报表作为 Executive 报表查看器访问，而不需要全局管理员或帐户管理员进行任何显式操作。全局管理员和帐户管理员可以覆盖这些用户的自动分配的角色，进一步增加或限制其功能。</span><span class="sxs-lookup"><span data-stu-id="680dd-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>