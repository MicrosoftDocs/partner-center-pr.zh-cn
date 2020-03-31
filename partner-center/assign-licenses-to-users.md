---
title: 客户帐户的用户管理任务 | 合作伙伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何为客户创建用户帐户、添加或删除用户许可证、重置用户密码、删除用户帐户或还原用户帐户。
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: jasonwhowell
ms.author: jasonh
Keywords: 客户管理，帐户，创建帐户，许可证，分配许可证，用户管理，密码，重置密码，更改密码
ms.localizationpriority: medium
ms.openlocfilehash: fcd5ebe2cb5daa5eafcd3ef56e1750225fcc9990
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2020
ms.locfileid: "80391006"
---
# <a name="user-management-tasks-for-customer-accounts"></a>客户帐户的用户管理任务

**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员
- 用户管理管理员
- 管理员代理
- 销售代理
- 支持人员代理

你可以在客户的帐户中创建和删除新用户。 你还可以还原以前在删除30天内删除的一个或多个用户帐户。 用户之前分配的订阅也将还原（假设之前的分配可用）。

为客户购买新的订阅时，客户应为你提供一个列表，其中列出了需要帐户的所有用户、用户权限以及每个用户需要的服务。  

可以一次[将订阅分配给多个用户](bulk-license-provisioning-for-multiple-users.md)，方法是使用 [Excel 兼容的 .csv 电子表格文件](adding-multiple-users-to-a-customer-account.md)导入这些名称。

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>为客户创建用户帐户

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 在“客户”菜单中，选择**用户和许可证**。

4. 对于每个用户，请选择**添加订阅**，然后填写信息，包括权限和许可证。 **保存**更改。

5. 请确保记录用户名和临时密码以发送给用户。

6. 如果要一次一个地添加多个用户，则使用**再次添加一个用户**。

7. 你还可以通过[导入 Excel 兼容的 .csv 电子表格文件](adding-multiple-users-to-a-customer-account.md)一次添加多个用户。 等到添加完所有用户后，可从确认屏幕通过电子邮件发送或打印这些名称和密码。

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>为客户添加或删除用户许可证

以下步骤适用于在 Microsoft 产品中添加或删除用户许可证。 若要在商业应用商店中添加或删除基于许可证的 SaaS 订阅的用户许可证，请参阅[添加或删除 SaaS 订阅的许可证](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)。

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3. 在“客户”菜单中，选择**用户和许可证**。

4. 从列表中选择一个或多个用户。 例如，如果客户刚刚购买了新许可证，并且你希望将它们分配给尚未拥有的人员，则可以使用**用户筛选条件**选项来找到正确的组。

5. 选择**管理许可证**。 进行更改，然后选择**保存**。

> [!NOTE]
> 对于[Azure Marketplace 产品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)，许可证分配和激活是通过发布产品的独立软件供应商（ISV）来管理的。

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>为客户重置用户密码

1. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

2. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

3.  在“客户”菜单中，选择**用户和许可证**。 从列表中选择用户。

4.  在屏幕底部，选择**重置密码**。 

5.  将新的临时密码发送给用户。

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>为客户删除用户帐户

1.  从 "**合作伙伴中心**" 菜单中，选择 "**客户**"。 从列表中选择客户。

2.  在“客户”菜单中，选择**用户和许可证**。 从列表中选择用户。

3.  在屏幕底部，选择**删除用户帐户**。

如果需要还原此帐户，可在客户的**用户和许可证**列表的**已删除用户**选项卡中找到它。 你有 30 天的时间还原已删除的用户。

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>还原删除的用户帐户

1.  从 "**合作伙伴中心**" 菜单中，选择 "**客户**"，然后从列表中选择客户。

2.  选择**用户和许可证**。

3.  选择**已删除的用户 ( )** ，当存在可以还原的已删除用户时，应读取 **(1)** 或更大。

4.  选中一个或多个已删除用户的复选框，然后选择**还原**。

    所有选定的用户帐户均将重新显示在**用户和许可证**页面中。

## <a name="related-topics"></a>相关主题


[向多个用户分配或撤消许可证](bulk-license-provisioning-for-multiple-users.md)

[为客户帐户创建多个用户](adding-multiple-users-to-a-customer-account.md)