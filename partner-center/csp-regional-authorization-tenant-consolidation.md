---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>CSP regional authorization tenant consolidation

**Applies to**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

\[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.\]

Use these instructions to consolidate tenants for different country/regions.

**注意** 必须注意在过渡帐户中为客户预配的所有订阅和席位计数。 Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process. Use the export list feature to help create a list of customers to move over to the centralized tenant. Partners choose to consolidate their tenants. Once consolidation is complete, Partners cannot revert to their previous state. Note that customer action is also be required.

 

## <a name="prepare-for-migration"></a>Prepare for migration


-   Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Migrate customer accounts


1.  使用过渡（新建）帐户登录 <https://partnercenter.microsoft.com>，然后从“合作伙伴中心”仪表板导航至“客户”列表。

2.  Select Customer.

3.  单击**请求经销商关系**。 You are presented with a default email message to present to your customers. This message contains a URL with the org ID unique to your new Partner Center account.

4.  **客户操作：**确保想要迁移的所有活动客户均访问此 URL。 When opening the URL, the customer is prompted to sign in to the Office 365 portal. The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.

5.  After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account. If they agree, the customer selects the checkbox and agrees to authorize the relationship.

The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrating Office 365 and non-Azure usage-based subscriptions


1.  Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.

2.  在“合作伙伴中心”仪表板上，单击左侧导航中的**客户**

3.  Open the company name for the customer you want to migrate.

4.  单击**添加订阅**。

5.  Add the correct subscriptions and seat counts from the catalog. 验证在**过渡源**合作伙伴帐户中提供的信息。

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  单击**提交**。

此时，服务将提供给**过渡目标**合作伙伴帐户中的客户。

Repeat these steps to migrate subscriptions for all additional customers.

Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.

**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabling the Office 365 subscriptions under the Transitioning From partner account


禁用**过渡源**合作伙伴帐户下的云解决方案提供商订阅将阻止以后的任何计费。 You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.

1.  使用**过渡源**云解决方案提供商帐户登录 <https://partnercenter.microsoft.com>，然后导航至客户列表。

2.  Open the customer with subscriptions to disable, and then select the first offer to disable.
3.  将订阅设置为**已暂停**，然后单击**提交**。

    **注意** 暂停订阅确保不会重复计费。

     

    该订阅在订阅列表上显示为**已暂停**。

4.  Repeat these steps for all subscriptions under the customer. 验证所有订阅是否显示**已暂停**。

5.  Select the next customer on the list and repeat the process of disabling all subscriptions.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrating Azure usage-based subscriptions


Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions. Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account. There will be no disruption of service to the customer during this transition.

1.  Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.
2.  Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.
3.  Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.
4.  The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.
5.  The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.

    **注意** 禁用客户下的订阅不会更改客户在“客户”列表中的外观。 There is currently no option to remove customers from the list. 合作伙伴应避免在以后从**过渡源**帐户中将订阅重新添加到这些客户。

     

6.  为所有客户下的所有订阅重复这些步骤，阻止在以后向**过渡源**帐户收费。 The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period. No future invoices will generate after that final billing period.

### <a name="notes"></a>Notes

-   Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.

-   Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.

-   There is currently no way to remove a customer from the Customers list completely.

-   **Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.

     

### <a name="simplify-migration-using-export"></a>Simplify migration using Export

使用**导出函数**，捕获要在新合并的结构中使用的订阅：

1.  单击“仪表板”上的**客户**，查看现有结构中的客户列表。

2.  Open the desired customer name.

3.  在**订阅**页上，单击**导出订阅**，将订阅的详细信息导出到 Excel 文件。

4.  Use this list to recreate the subscriptions in your new consolidated tenant.

### <a name="api-registration"></a>API registration

有关 API 注册的详细信息，[请参阅此页](https://go.microsoft.com/fwlink/?linkid=847990)。

## <a name="partner-center-activity-log"></a>Partner Center Activity log


With the Activity log, partners can view a record of all customer-affecting changes made on their tenant. This helps partners track changes on a customer tenant.

**View the Activity log**

1.  在“合作伙伴中心”仪表板上，单击**活动日志**链接。
2.  在**活动日志**页上，查看对客户帐户进行的更改。 若要按日期筛选活动日志，请在日志中选择**开始**和**结束**日期，缩小所选记录的范围。 若要在**活动日志**中按客户筛选，请使用搜索框。

**Export the Activity log**

-   单击**导出日志**，将活动日志数据导出为 CSV 文件。

    You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).

 

 



