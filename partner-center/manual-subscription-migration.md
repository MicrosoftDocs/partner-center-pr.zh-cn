---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. 作为新产品的一部分，Microsoft 在 2016 年 11 月 1 日为客户引进了新 Microsoft Dynamics 订阅计划，该计划与当前计划类似但不相同。

本文档中的说明介绍了间接提供商如何将客户的现有 Microsoft Dynamics AX 订阅和 Microsoft Dymanics CRM Online 订阅转换为 Microsoft Dynamics 365。 The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

Microsoft Dynamics CRM Online 和 AX 计划已停用。  2017 年 7 月 1 日生效，你可以不再续订这些旧计划，此外，现有 E4 订阅在到期时将不会自动续订。

当 CRM Online 和 AX 订阅结束时，它们将会被取消。 为确保客户服务连续性，将具有即将到期订阅的客户过渡到下列支持的 SKU 选项。 建议在订阅年度结束日期之前将客户转移到新订阅，以避免出现任何客户服务中断。 

在订阅详细信息页面上，即将到期的订阅的状态会从“[日期] 自动续订”更改为“[日期] 过期”。 

如果你使用 API（CREST 或合作伙伴中心），则可以通过评估订阅的结束日期以及“自动续订 = False”属性来发现即将到期的订阅。2017 年 7 月 1 日，这些订阅已被设置为“自动续订 = False”。 你可以随时将客户移到新计划中。 

**Microsoft Dynamics AX 授权更改**

Microsoft Dynamics AX 产品线于 2016 年 11 月 1 日停用。 若要了解关于 Dynamics 365 的新授权选项的更多信息，请参阅[授权指南](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)。

 请参考下表，了解关于许可证映射的详细信息：

|**已停用的 SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|企业版 SKU|针对 Unified Operations 或 Microsoft Dynamics 365 计划的 Microsoft Dynamics 365 |
|任务|Microsoft Dynamics 365 for Activity
|任务/自助服务|Microsoft Dynamics 365 for Team Members|
|设备|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Microsoft Dynamics CRM Online 授权更改 

**Microsoft Dynamics CRM Online**

当前的 Microsoft Dynamics CRM Online 计划于 2016 年 11 月 1 日停用 若要了解关于 microsoft Dynaics 365 的新授权选项的更多信息，请参阅[授权指南](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)。 若要了解有关新授权选项的详细信息，请参阅[面向 CRM Online 客户的重要信息](https://go.microsoft.com/fwlink/?linkid=831667)。

请参考下表，了解关于许可证映射的详细信息：

|**已停用的 SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Dynamics 365 企业客户参与度计划 |
|Professional|Dynamics 365 企业客户参与度计划计划、Dynamics 365 for Sales 或 Dynamics 365 for Customer Service|
|Basic|Dynamics 365 for Team Members、Dynamics 365 for Sales、Dynamics 365 for Customer Service 或 Dynamics 365 企业客户参与度计划|
|Essential|Dynamics 365 for Team Members|
|现场服务加载项|Dynamics 365 企业客户参与度计划或 Dynamics 365 for Field Service|
|项目服务自动化加载项|Dynamics 365 企业客户参与度计划或 Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>将客户过渡到新产品计划


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [取消旧订阅](#manual-subscription-migration-cancelsubscriptions)。

以下过程将客户从 Microsoft Dynamics AX 或 CRM Online 移动到 Dynamics 365。

在该示例中，经销商需要将具有现有 Dynamics AX Enterprise 订阅的客户移至 Dynamics 365 for Operations。 第一步是购买 Dynamics 365 for Operations。  对于将移至 Microsoft Dynamics 365 的 CRM Online 客户，重复这些步骤。

<a href="" id="purchasenewsubsc"></a>

**购买新订阅**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



