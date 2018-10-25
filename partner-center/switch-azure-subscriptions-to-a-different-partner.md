---
title: 转移 Azure 订阅 | 合作伙伴中心
description: 客户可以在云解决方案提供商计划中更改要用于提供 Microsoft Azure 服务的合作伙伴。 但是，这是一个手动过程，需要合作伙伴和客户双方进行操作。
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
keywords: Azure 订阅, 切换合作伙伴, 更换合作伙伴, 获得新的合作伙伴, 其他合作伙伴
ms.localizationpriority: medium
ms.openlocfilehash: 5c4f1b5df62d800f2c3ac14137dd85743e928e90
ms.sourcegitcommit: 5c8ea8aaa94f79cd2fc031b2b40a0cc363c5d3c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2018
ms.locfileid: "5511388"
---
# <a name="transfer-azure-subscriptions"></a>转移 Azure 订阅 

**适用于**

-  合作伙伴中心

客户可以决定切换到某个云解决方案提供商合作伙伴或另一合作伙伴来提供其 Microsoft Azure 服务。 但是，这是一个手动过程，需要合作伙伴和客户双方进行操作。

>[!Note]  
>这一次仅直接或间接提供商将能够传输的订阅。

>[!Note]它不是当前可以更改为 Office 365、 企业移动性套件或 Microsoft Dynamics CRM 订阅的云解决方案提供商订阅的合作伙伴。



**针对 Azure 订阅切换合作伙伴**

1.  若要将 Azure 订阅转移给新合作伙伴，则必须由客户发起该过程，然后以书面形式与当前记录的合作伙伴进行联系。 

    >[!Note]
    >当前合作伙伴负责创建发起转移过程所需的服务票证。 Microsoft 无法代表客户或新合作伙伴进行干预。 客户应该计划与当前合作伙伴密切合作，以便过渡顺利进行。

2.  订阅的合作伙伴需要执行以下任务：

    通过合作伙伴中心创建 Azure 服务票证以请求订阅传输：

    -   从合作伙伴中心菜单中，选择**客户**、 从列表中，选择你的客户，然后选择**服务管理**。 在**支持票证**部分下，选择**新票证**下拉列表，然后选择 **Microsoft Azure**。

    -   在 Azure 门户中，选择**新支持请求**。

        在步骤 1 中，选择**订阅管理**作为问题类型、指定你想要传输的订阅 ID，然后选择**云解决方案提供商**作为支持计划。

        在步骤 2 中，选择 **C–最小影响**，然后选择**其他一般问题**作为问题类型。

        下载[云解决方案提供商订阅转移表单](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip)。

3.  订阅的合作伙伴：填写[云解决方案提供商订阅转移表单](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip)、对其进行签名，然后将它发送给客户。 若要填写表单，需要以下信息：

    -   当前合作伙伴的联系人信息和 Microsoft ID。 在“合作伙伴中心”菜单中，依次选择**帐户设置** &gt; **组织配置文件**，然后使用此处所列的 **Microsoft ID**、**组织名称**和**地址**。

    -   客户的 Microsoft ID。 在“合作伙伴中心”菜单中，选择**客户**，然后展开客户列表以查看其 **Microsoft ID**。

    -   要转移的订阅 ID。 在展开的客户列表中，选择**查看订阅**，然后展开选定的订阅以查看**订阅 ID**。

     >[!Note]
     >转移订阅将导致两个订阅 ID，你将在被转移的订阅的**编辑订阅**页上看到它们：**1**-“合作伙伴中心订阅 ID”用于计费目的。 
    **2**- 原始“Azure 订阅 ID”仍保留，将显示在合作伙伴中心和 Azure 管理门户中。 此 ID 将显示在你的对帐文件中。  **记录支持票证时，你需要使用这两个 ID。**

4.  订阅的客户和新合作伙伴：

    查看该表单、填写与新合作伙伴有关的信息，然后进行签名。 确认新客户已签署合约协议。 将该表单发送回当前记录合作伙伴。

    *重要提示*：如果新云解决方案提供商合作伙伴与客户没有经销商关系，则在传输订阅前，他们必须建立这种关系。 [可在此处查找关于如何执行此操作的信息](request-a-relationship-with-a-customer.md)。

    >[!Note]
    >新的云解决方案提供商合作伙伴和客户租户必须位于同一国家/地区。 

5.  当前合作伙伴：

    确保该表单包含合作伙伴双方管理员的联系信息 - Microsoft 支持人员将联系双方管理员以验证该转移。 确保所有三个签名均已签署，然后使用**文件上载**选项将已完成的表单附加到现有的服务请求。 Microsoft 支持工程师将在 8 小时工作时间内给你回复以验证接收和完成操作。

6.  新合作伙伴：

    更新 Azure 订阅设置，以从帐户中删除旧的合作伙伴。 若要查看已预配哪些角色分配，请运行两个 Powershell Commandlet。

    -   在帐户上添加新的合作伙伴作为经销商：

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        若要查找客户域名：在“合作伙伴中心”菜单中，选择**客户**。 从客户列表中选择客户。 在“客户”菜单中，选择**帐户**，然后使用**域名**。

    -   查看帐户上的角色，包括以前的云解决方案提供商合作伙伴：

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

7. 删除已过期的访问权限

    -  在合作伙伴中心菜单中，选择**客户**。 
    -  展开客户列表，然后选择**查看订阅**。 
    -  在“客户”菜单中，选择**服务管理**。 
    -  在 **Microsoft Azure** 下，单击链接即可转到 **Microsoft Azure 管理门户**。

 

 



