---
title: 转让资格–在帐单帐户、Azure Marketplace 之间传输订阅的准则
description: 在 Azure 门户中的计费帐户之间传输订阅之前的商业检查准则。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412550"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>传输计费帐户之间的订阅的资格

可以在 Azure 门户的 "计费" 部分中将订阅从一个计费帐户 [转移](/azure/cost-management-billing/understand/subscription-transfer) 到另一个。 在传输之前，会扫描订阅以获取第三方产品。 仅当清除 *所有* 产品进行传输时才允许传输 (请参阅下面的 [条件](#criteria-for-transfer-approval-or-denial)) 。 系统将为未能清除的应用生成相关的错误消息，以帮助你确定后续步骤。

> [!NOTE]
> 本文不适用于 SaaS 产品，因为 SaaS 资源附加到租户，而不是订阅。 SaaS 资源可从一个计费帐户转移到另一个计费帐户，但这是根据资源和 Azure 支持作为支持请求来完成的。

## <a name="criteria-for-transfer-approval-or-denial"></a>传输批准或拒绝的条件

如果任何第三方应用满足以下任一条件，则无法传输订阅：

- 目标帐户是商业的，应用可以选择退出，通过合作伙伴进行销售。
- 对于所选的合作伙伴，此应用将处于选中状态，并且目标帐户不在允许列表中。
- 产品/服务是过去对于所选订阅的预览提议，或者是专用产品/服务，并且订阅不再处于允许列表中。
- 新的计费帐户所在的区域与产品/服务的销售区域不同，该产品/服务不会出售到该区域。

在从订阅中删除资源之前，阻止的传输将一直有效，之后可以再次尝试传输。

## <a name="next-steps"></a>后续步骤

[获取 Microsoft AppSource 和 Azure Marketplace 的支持](get-support.md)

