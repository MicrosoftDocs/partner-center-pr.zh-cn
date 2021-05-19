---
title: 奖励的客户关联问题
description: 了解如何解决在使用声称的记录 (CPOR) 客户关联的合作伙伴时遇到的问题。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152165"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a> (CPOR) 客户关联的声明合作伙伴的问题

**适当的角色**：计费管理员 |全局管理员 |奖励管理

以下内容将帮助你解决在使用客户关联时可能出现的问题。

## <a name="domain-tenant-mismatch"></a>域-租户不匹配

在请求的记录合作伙伴 (CPOR) 关联声明流中，系统将要求你提供客户租户 ID 和子域。 如果收到指出不匹配的错误，请与客户联系以确保具有正确的详细信息。

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR 关联声明流中的订阅错误

在 CPOR 关联声明流中，系统可能会要求你通过 Business Applications (Dynamics 365) 为你试图声明的产品提供订阅。 我们要求提供订阅，因为我们要动态检查产品和订阅是否属于所申请的租户。 我们还检查订阅是否处于活动/已宽限状态。

如果收到错误，则可能是由于以下几个原因：

- 客户的租户上不存在所选产品
- 提供的订阅不适用于 Dynamics
- 提供的订阅适用于 CSP
- 客户尚未激活/预配该订阅的产品
- 已声明订阅
- 提供的标识符不是订阅 ID

如果对订阅准确性有疑问，请与客户合作，确保订阅正确并使用正确的租户 ID。

如果此路由尚未解决你的问题，请联系 [支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="when-subscriptions-will-be-available-to-claim"></a>订阅将可用于声明

在为订阅申报时，如果尚未预配订阅，你将会收到错误。 客户需要执行几个步骤，以便 CPOR 平台可以选择订阅并使其可供声明使用。 如果在尝试申请订阅时收到错误，请联系客户，确保已预配该订阅，并且所声明的订阅正确无误。 如果已采取此路由，请联系 [支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="which-activity-do-i-choose"></a>我选择哪种活动？

CPOR 声明平台允许 CPOR 关联声明，这些声明Business Applications和Microsoft 365方面。 下面列出了适用于每个解决方案领域的活动。 根据说明选择正确的活动，以避免将来必须回收。 使用不正确的活动进行声明可能会导致错过资格和奖励收益。


| 解决方案领域 | 活动 | 适用于 |
| ------ | ----------- | ----------- |
| 业务应用程序      | 售前   | 选择是否影响他们购买符合条件的产品，并想要申请预售奖励。 只有在客户通过批量许可协议或 Web-Direct 购买这些产品时，此选项才适用。 |
|    |  使用情况  | 选择是否推动其采用和使用符合条件的工作负载，并想要申请使用奖励。 只有在客户通过批量许可协议或 Web-Direct 购买这些产品时，此选项才适用。 |
|    | 收入关联   | 选择是否影响他们选择符合条件的产品作为业务影响因素。 此选项仅适用于收入关联，不用于奖励付款。 只有在客户通过批量许可协议或 Web-Direct 购买这些产品时，此选项才适用。   |
| Microsoft 365   | 使用情况   | 选择是否推动其采用和使用符合条件的工作负载，并想要申请使用奖励。 |

## <a name="which-mpn-do-i-choose"></a>我选择哪个 MPN？

在 CPOR 关联声明流中，将要求你选择一个公司 MPN，该 MPN 应关联到最终客户要申请的工作。 你的公司可能有许多 MPNs，其中一些可能在激励计划中注册，另一些则与合作伙伴类型（如 FRP FastTrack）相关联。 CPOR 关联声明流将确定哪些 MPNs 在激励计划中注册，但它不会告诉您它是否为特定的合作伙伴类型 MPN。 选择正确的 MPN，以避免将来不得不回收，这一点很重要。 如果申报的 MPN 不正确，可能会导致缺少资格和激励收益。

如果你不知道要使用哪种 MPN，请联系你的全局管理员。

如果要使用的 MPN 未注册，可以在 " [激励概述" 选项卡](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) 中进行管理， (登录所需) 。

## <a name="choosing-a-product-vs-entering-a-subscription"></a>选择产品与输入订阅

当要求和批准 Dynamics 产品时，合作伙伴可以在 CPOR 关联声明自身中查看订阅 ID。 当声明此订阅时，该订阅处于活动状态或处于宽限状态，但可能会有时间结束，并且需要在单独的 CPOR 关联声明中声明新的订阅。

## <a name="competing-claims"></a>竞争声明

如果要为客户创建 CPOR 关联声明，并为已与另一个合作伙伴关联的产品 () ，则声明将通过仲裁：

1. 创建新的客户关联后，Microsoft 将验证关联的详细信息以及提供的执行证明，以确保其准确性。

2. 如果你和其他合作伙伴声称了相同的客户和产品/工作负荷，Microsoft 将查看每个合作伙伴的执行证明文档，以确定要批准的合作伙伴。

3. 可能会从两个伙伴请求其他信息，这可能会导致延迟处理您的关联请求。

4. 你 _的 CPOR_ 关联声明仍将在五个工作日内查看，但其状态可能会持续很长一段时间。 当 Microsoft 与当前拥有产品/工作负载的合作伙伴合作时，可能会发生这种情况。 如果出现这种情况，你将在声明的 "评论" 部分中收到通知。 

>[!IMPORTANT]
>如果我们需要其他信息来验证你的 CPOR 关联执行证明 (PoE) ，我们将通过 CPOR 关联声明注释部分联系你。

## <a name="next-steps"></a>后续步骤

- [即刻体验奖励](incentives-get-started-intro.md)
