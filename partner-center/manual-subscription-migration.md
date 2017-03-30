---
title: "将 Dynamics AX 订阅迁移到 Dynamics 365 | 合作伙伴中心"
description: "Microsoft 引入了 Dynamics 365，这是下一代智能业务应用程序，可使组织成长、发展和转型，满足客户需求并抓住新机遇。"
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: f19e46da31a7e479ebd3b1cd368ca7646c3c55b7
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>将 Dynamics AX 订阅迁移到 Dynamics 365

**适用于**

-  合作伙伴中心

Microsoft 引入了 Dynamics 365，这是下一代智能业务应用程序，可使组织成长、发展和转型，满足客户需求并抓住新机遇。 作为新产品的一部分，Microsoft 在 2016 年 11 月 1 日为客户引进了新 Microsoft Dynamics 订阅计划，该计划与当前计划类似但不相同。

本文档中的说明介绍了间接提供商如何将客户的现有 Microsoft Dynamics AX 订阅转换为新的 Microsoft Dynamics 365。 这些说明也适用于其他更新到新版本的 Microsoft 产品，需要提供商将客户订阅迁移到新 SKU。

**Microsoft Dynamics AX 授权更改**

Microsoft Dynamics AX 产品线将于 2016 年 11 月 1 日停用。 若要了解关于 Dynamics 365 的新授权选项的详细信息，请参阅即将发布的“授权指南”。 请参考下表，了解关于许可证映射的详细信息：

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>停用的 Dynamics AX 许可证</strong></p></td>
<td><p><strong>Dynamics 365 许可证</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Dynamics 365 Enterprise edition Plan 2</p>
<p>或 Dynamics 365 for Operations</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Task</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Functional</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Device</p></td>
<td><p>Dynamics 365 for Operations Device</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

当前的 Microsoft Dynamics CRM Online 计划将于 2016 年 11 月 1 日停用 若要了解有关新授权选项的详细信息，请参阅[面向 CRM Online 客户的重要信息](https://go.microsoft.com/fwlink/?linkid=831667)。

## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划


Microsoft 不断向经销商和提供商提供新产品和服务。 在这些情况下，经销商可能需要将客户升级到新服务，或将他们的订阅从最终将关闭的 SKU 中迁出。 将客户从旧 SKU 中迁移到新 SKU 需要按照以下顺序操作：

-   [购买新订阅](#manual-subscription-migration-purchasenewsubsc)；
-   [重新分配当前用户许可证](#manual-subscription-migration-reassignlicenses)；
-   [取消旧订阅](#manual-subscription-migration-cancelsubscriptions)。

以下过程将客户从 Dynamics AX7 Enterprise 移动到 Dynamics 365 for Operations。

<a href="" id="purchasenewsubsc"></a>经销商需要将具有现成 Dynamics AX Enterprise 订阅的客户移动到 Dynamics 365 for Operations。 第一步是购买 Dynamics 365 for Operations。

**购买新订阅**

1.  在**仪表板**菜单中，选择**客户**、选择要移动的客户，然后选择**添加订阅**。
2.  选择要从目录中购买的订阅（在此情况下是 Dynamics 365 for Operations 企业版）、输入许可证编号，然后选择**提交**。

    此时客户应该具有新旧两个订阅：在此示例中是旧的 Dynamics AX Enterprise 和新的“目标”订阅，即 Dynamics 365 for Operations 企业版。

<a href="" id="reassignlicenses"></a>下一步是将所有现有用户许可证重新分配到新订阅。

**重新分配用户许可证**

1.  在**仪表板**菜单中，选择**客户**、选择要移动的客户，然后选择**用户和许可证**。 将打开客户的“用户和许可证”页。
2.  若要重新分配用户许可证，选择要重新分配的用户，然后选择**管理许可证**。
3.  在**管理许可证**页上，清除 **Dynamics AX Enterprise** 许可证复选框，然后选择 **Dynamics 365 for Operations** 许可证。
4.  选择**提交**。 确认页面列出了新的许可证分配。
5.  对其他任何需要重新分配许可证的客户用户继续执行相同的步骤。

<a href="" id="cancelsubscriptions"></a>在将用户许可证移动至新服务后，可安全取消最高“客户”级别的旧订阅。

**取消旧订阅**

1.  在**仪表板**菜单中，选择**客户**、选择要移动的客户，然后选择要取消的订阅。
2.  在订阅详细信息页面中，将订阅**状态**设置为**已暂停**。
3.  选择**提交**。

旧订阅已暂停，新订阅将激活。 暂停的订阅在 120 天后将自动取消预配。 不会向客户收取旧订阅的任何额外成本。

## <a name="additional-considerations"></a>其他注意事项


如果客户从“开放渠道”移动至“云服务计划”以进一步预配订阅，还需要迁移他们的现有订阅：

-   如果客户通过“开放渠道”接收旧订阅，可直接移动到新 SKU 上的云解决方案提供商。
-   如果客户尚未成为你的客户，可向他们发出邀请。 有关信息，请参阅[请求与客户建立关系](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx)帮助主题。

在客户接受你成为他们的间接提供商后，预配步骤与上述步骤大致相同：购买新订阅，然后分配用户许可证。 唯一的区域是取消旧订阅。 新提供商无法暂停/取消通过其他渠道获取的订阅。 如果客户在其他销售渠道（例如开放渠道）获取了以前的订阅，需要通过该渠道自行取消。

 

 



