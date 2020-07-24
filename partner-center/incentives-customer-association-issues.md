---
title: 客户关联问题
description: 了解如何解决在使用声明的记录合作伙伴（CPOR）客户关联时遇到的问题。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: 63138dd6eaa16534cb73f41655ba728cb0c7a430
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114530"
---
# <a name="customer-association-issues"></a>客户关联问题

适用于：

- 合作伙伴中心

以下内容将帮助你解决在使用客户关联时可能出现的问题。

适当的角色：

- 计费管理员
- 全局管理员
- 奖励管理员

## <a name="domain-tenant-mismatch"></a>域-租户不匹配

在声明的记录合作伙伴（CPOR）关联声明流中，系统将要求你提供客户租户 ID 和子域。 如果收到指出不匹配的错误，请与客户联系以确保具有正确的详细信息。

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR 关联声明流中的订阅错误

在 CPOR 关联声明流中，系统可能会要求你通过 Business Applications （Dynamics 365）为你要尝试声明的产品提供订阅。 我们要求提供订阅，因为我们要动态检查产品和订阅是否属于所申请的租户。 我们还检查订阅是否处于活动/已宽限状态。

如果收到错误，则可能是由于以下几个原因：

- 客户的租户上不存在所选产品
- 提供的订阅不适用于 Dynamics
- 提供的订阅适用于 CSP
- 客户尚未激活/预配该订阅的产品
- 已声明订阅
- 提供的标识符不是订阅 ID

如果对订阅准确性有疑问，请与客户合作，确保订阅正确并使用正确的租户 ID。

如果此路由尚未解决你的问题，请联系[支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="when-subscriptions-will-be-available-to-claim"></a>订阅将可用于声明

在为订阅申报时，如果尚未预配订阅，你将会收到错误。 客户需要执行几个步骤，以便 CPOR 平台可以选择订阅并使其可供声明使用。 如果你在尝试声明订阅时收到错误，请与你的客户联系，以确保它已预配，并且你所申报的订阅是正确的。 如果已创建此路由，请联系[支持人员](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)。

## <a name="which-activity-do-i-choose"></a>我应选择哪种活动？

CPOR 声明平台允许与 Business Applications 和 Microsoft 365 解决方案区域相关的 CPOR 关联声明。 下面是适用于每个解决方案区域的活动。 根据说明选择正确的活动，以避免将来需要回收。 如果申报的活动不正确，可能会导致缺少合格和激励收益。


| 解决方案领域 | 活动 | 适用于 |
| ------ | ----------- | ----------- |
| 业务应用程序      | 前   | 如果你影响其对符合条件的产品的购买，并想要申请售前奖励，请选择此项。 仅当客户通过批量许可协议或 Web 直接购买这些产品时，此选项才适用。 |
|    |  用法  | 如果你推动其采用和使用符合条件的工作负荷，并想要应用以实现使用奖励，请选择。 仅当客户通过批量许可协议或 Web 直接购买这些产品时，此选项才适用。 |
|    | 收入关联   | 如果影响其对符合业务影响的产品，请选择此项。 此选项仅适用于收入协会，不适用于激励支付。 仅当客户通过批量许可协议或 Web 直接购买这些产品时，此选项才适用。   |
| Microsoft 365   | 用法   | 如果你推动其采用和使用符合条件的工作负荷，并想要应用以实现使用奖励，请选择。 |

## <a name="which-mpn-do-i-choose"></a>我 MPN 选择哪一种？

在 CPOR 关联声明流中，系统将要求你选择一个公司 MPN，该公司应该与你在最终客户申报的工作相关联。 你的公司可能有许多 MPNs，其中一些可能在激励计划中注册，另一些则与合作伙伴类型（如 FRP FastTrack）相关联。 CPOR 关联声明流将确定哪些 MPNs 在激励计划中注册，但它不会告诉您它是否为特定的合作伙伴类型 MPN。 选择正确的 MPN，以避免将来不得不回收，这一点很重要。 如果申报的 MPN 不正确，可能会导致缺少资格和激励收益。

如果你不知道要使用哪种 MPN，请联系你的全局管理员。

如果你想要使用的 MPN 未注册，你可以在[激励概述选项卡](https://partner.microsoft.com/dashboard/incentives/enrollment/summary)中对其进行管理。

## <a name="choosing-a-product-vs-entering-a-subscription"></a>选择产品与输入订阅

当要求和批准 Dynamics 产品时，合作伙伴可以在 CPOR 关联声明自身中查看订阅 ID。 当声明此订阅时，该订阅处于活动状态或处于宽限状态，但可能会有时间结束，并且需要在单独的 CPOR 关联声明中声明新的订阅。

## <a name="competing-claims"></a>竞争声明

如果要为已与另一个合作伙伴关联的客户及其产品创建 CPOR 关联声明，则声明将通过仲裁：

1. 创建新的客户关联后，Microsoft 将验证关联的详细信息以及提供的执行证明，以确保其准确性。

2. 如果你和其他合作伙伴声称了相同的客户和产品/工作负荷，Microsoft 将查看每个合作伙伴的执行证明文档，以确定要批准的合作伙伴。

3. 可能会从两个伙伴请求其他信息，这可能会导致延迟处理您的关联请求。

4. 你_的 CPOR_关联声明仍将在五个工作日内查看，但其状态可能会持续很长一段时间。 当 Microsoft 与当前拥有产品/工作负载的合作伙伴合作时，可能会发生这种情况。 如果出现这种情况，你将在声明的 "评论" 部分中收到通知。 

>[!IMPORTANT]
>如果我们需要其他信息来验证你的 CPOR 关联 PoE，我们将通过 CPOR 关联声明评论部分与你联系。
