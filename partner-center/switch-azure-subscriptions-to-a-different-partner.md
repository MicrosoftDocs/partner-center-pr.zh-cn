---
title: "将 Azure 订阅切换到其他合作伙伴 | 合作伙伴中心"
description: "客户可以在云解决方案提供商计划中更改要用于提供 Microsoft Azure 服务的合作伙伴。 但是，这是一个手动过程，需要合作伙伴和客户双方进行操作。"
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 29ced9a3a7256f86f0f8708a4c72ac75b9269ffc

---

# 将 Azure 订阅切换到其他合作伙伴


客户可以在云解决方案提供商计划中更改要用于提供 Microsoft Azure 服务的合作伙伴。 但是，这是一个手动过程，需要合作伙伴和客户双方进行操作。


            **注意** Azure 客户当前无法从 EA、开放或其他授权计划自动切换到云解决方案提供商。 这是一个手动过程，需要合作伙伴和客户双方进行操作。 此外，当前无法针对 Office 365、企业移动性套件或 Microsoft Dynamics CRM 订阅更改云解决方案提供商订阅的合作伙伴。

 

**针对 Azure 订阅切换合作伙伴**

1.  若要将 Azure 订阅传输到新合作伙伴，客户必须启动该过程，然后以书面形式与当前记录云解决方案提供商合作伙伴的合作伙伴进行联系。

2.  订阅的云解决方案提供商需要执行以下任务：

    通过合作伙伴中心创建 Azure 服务票证以请求订阅传输：

    -   在合作伙伴中心仪表板菜单中，选择“客户”、从列表中选择客户，然后选择“服务管理”。 在“支持票证”部分下，选择“新票证”下拉列表，然后选择“Microsoft Azure”。

    -   在 Azure 门户中，选择“新支持请求”。

        在步骤 1 中，选择“订阅管理”作为问题类型、指定你想要传输的订阅 ID，然后选择“云解决方案提供商”作为支持计划。

        在步骤 2 中，选择“C–最小影响”，然后选择“其他一般问题”作为问题类型。

        下载[云解决方案提供商订阅传输表单](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip)。

3.  订阅的当前云解决方案提供商合作伙伴：填写[云解决方案提供商订阅传输表单](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip)、对其进行签名，然后将它发送给客户。 若要填写表单，需要以下信息：

    -   当前合作伙伴的联系人信息和 Microsoft ID。 在“合作伙伴中心”菜单中，依次选择“帐户设置”&gt;“组织配置文件”，然后使用此处所列的“Microsoft ID”、“组织名称”和“地址”。

    -   客户的 Microsoft ID。 在“合作伙伴中心”菜单中，选择“客户”，然后展开客户列表以查看其“Microsoft ID”。

    -   要转移的订阅 ID。 在展开的客户列表中，选择“查看订阅”，然后展开选定的订阅以查看“订阅 ID”。

4.  订阅的客户和新云解决方案提供商：

    查看该表单、填写与新合作伙伴有关的信息，然后进行签名。 确认新客户已签署合约协议。 将该表单发送回当前记录合作伙伴。

    
            *重要提示*：如果新云解决方案提供商合作伙伴与客户没有经销商关系，则在传输订阅前，他们必须建立这种关系。 
            [可在此处查找关于如何执行此操作的信息](https://int.msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx)。

5.  当前的云解决方案提供商合作伙伴：

    确保该表单包含合作伙伴双方管理员的联系人信息 - Microsoft 支持将联系双方管理员以验证该传输。 确保所有三个签名均已签署，然后使用“文件上载”选项将已完成的表单附加到现有的服务请求。 Microsoft 支持工程师将在 8 小时工作时间内给你回复以验证接收和完成操作。

6.  新的云解决方案提供商合作伙伴：

    更新 Azure 订阅设置，以从帐户中删除旧的合作伙伴。 若要查看已预配哪些角色分配，请运行两个 Powershell Commandlet。

    -   在帐户上添加新的合作伙伴作为经销商：

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        若要查找客户域名：在“合作伙伴中心”菜单中，选择“客户”。 从客户列表中选择客户。 在客户菜单中，选择“帐户”，然后使用“域名”。

    -   查看帐户上的角色，包括以前的云解决方案提供商合作伙伴：

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

    通过在 Azure 门户中管理订阅，删除订阅和资源的已过时访问权限。 在“合作伙伴中心”菜单中，选择“客户”。 展开客户列表，然后选择“查看订阅”。 在客户菜单中，选择“服务管理”。 在“Microsoft Azure”下，单击链接即可转到“Microsoft Azure 管理门户”。

 

 






<!--HONumber=Nov16_HO3-->


