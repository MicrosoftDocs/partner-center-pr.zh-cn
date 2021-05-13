---
title: 将 Azure 订阅转移到另一个合作伙伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何更改云解决方案提供商 Azure 订阅关联的计划合作伙伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856060"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>了解如何将客户的 Azure 订阅转让给另一个合作伙伴

**适用于 ：** 合作伙伴中心 |合作伙伴中心Microsoft Cloud for US Government

**适当角色**：全局管理员

本文介绍客户如何从云解决方案提供商Microsoft Azure服务云解决方案提供商 (服务) 服务。

若要将客户的 Azure 服务或订阅切换到其他合作伙伴，请执行以下手动步骤。 合作伙伴和客户都需要完成这些步骤。

>[!Note]  
>目前，只有直接或间接提供商才能转移订阅。
>不能更改与 Azure 计划云解决方案提供商 Office 365、企业移动性套件或 Microsoft Dynamics CRM 订阅关联的订阅的合作伙伴。

## <a name="switch-partners-for-azure-subscriptions"></a>针对 Azure 订阅切换合作伙伴

1. 若要将 Azure 订阅转移给新合作伙伴，则必须由客户发起该过程，然后以书面形式与当前记录的合作伙伴进行联系。

   >[!Note]
   > 当前合作伙伴负责创建发起转移过程所需的服务票证。 Microsoft 无法代表客户或新合作伙伴进行干预。 客户应该计划与当前合作伙伴密切合作，以便过渡顺利进行。

2. 订阅的合作伙伴需要执行以下任务：

   通过合作伙伴中心创建 Azure 服务票证以请求订阅传输：

   1. 从合作伙伴中心菜单中，选择"**客户**"，从列表中选择你的客户，然后选择"服务 **管理"。**

   2. 在" **支持票证** "部分下，选择" **新建票证** "下拉列表 **，然后选择** Microsoft Azure" 。
   
   3. 从"Azure 门户"，选择"**新建支持请求"。** [](https://portal.azure.com)
   
   4. 在"步骤 1"中，选择"订阅管理 **"** 作为问题类型，指定要转移的订阅 ID，然后选择云解决方案提供商作为支持计划。 
   
   5. 在步骤 2 中，选择 **"C-最小影响** "，然后选择"其他 **常规问题** "作为问题类型。
   
   6. 下载[“CSP 订阅转让”表](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)。

3. 订阅的合作伙伴：填写[云解决方案提供商订阅转移表单](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)、对其进行签名，然后将它发送给客户。 

   若要填写表单，需要以下信息：

   - 当前合作伙伴的联系人信息和 Microsoft ID。 在"合作伙伴中心"菜单中，选择"帐户设置""组织配置文件 &gt; "，并使用列出的 **"Microsoft ID"、"** 组织名称"和"地址"。  

   - 客户的 Microsoft ID。 在合作伙伴中心菜单中，选择" **客户"，** 然后展开客户列表以查看其 **Microsoft ID**。

   - 要转移的订阅 ID。 在展开的客户列表中，选择 **"查看订阅"，** 然后展开所选订阅以查看"订阅 **ID"。**

   >[!Note]
   >转移订阅将导致两个订阅 ID，你将在被转移的订阅的 **编辑订阅** 页上看到它们：**1**-“合作伙伴中心订阅 ID”用于计费目的。 **2**- 原始“Azure 订阅 ID”仍保留，将显示在合作伙伴中心和 Azure 管理门户中。 此 ID 将显示在你的对帐文件中。  **记录支持票证时，你需要使用这两个 ID。**

4. 订阅的客户和新合作伙伴：

   查看该表单、填写与新合作伙伴有关的信息，然后进行签名。 确认新客户已签署合约协议。 将该表单发送回当前记录合作伙伴。

   *重要提示*：如果新的 CSP 合作伙伴没有与客户的分销商关系，则必须在传输订阅之前建立订阅。 [可在此处查找关于如何执行此操作的信息](request-a-relationship-with-a-customer.md)。

   >[!Note]
   >新的 CSP 合作伙伴和客户租户必须位于同一国家/地区。 

5. 当前合作伙伴：

   请确保此窗体包含合作伙伴管理员的联系信息。 Microsoft 支持部门将与这两个管理员联系以验证传输。 请确保具有所有三个签名。 然后，使用 " **文件上传** " 选项将完成的窗体附加到现有的服务请求。 Microsoft 支持工程师将在8个工作时间内返回给你，以验证接收和完成情况。

6. 新合作伙伴：

   更新 Azure 订阅设置，以从帐户中删除旧的合作伙伴。 若要查看预配了哪些角色分配，请运行两个 PowerShell Commandlet。

   - 在帐户上添加新的合作伙伴作为经销商：

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > 客户的 **租户 id** 显示在合作伙伴中心中作为客户的 **Microsoft id**。 若要查找特定客户的 Microsoft ID (租户 ID) ，请登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。 然后从菜单中选择 " **客户** "。 找到列表上的客户。 选择向下箭头以展开客户的列表。 你将看到有关客户 *域名* 和客户的 **Microsoft ID** 的信息。 在 PowerShell commandlet 中使用16位 **MICROSOFT ID** 。

   - 查看帐户上的角色，包括以前的云解决方案提供商合作伙伴：

     ```powershell
     Get-AzRoleAssignment
     ```

7. 删除过时的访问权限：

   - 在 "合作伙伴中心" 菜单中，选择 " **客户**"。
   - 找到列表上的客户。 选择 (双击其公司名称) 。 此操作将打开 "客户 **订阅** " 页。
   - 在客户详细信息菜单中，选择"**服务管理"。**
   - 在 **Microsoft Azure"** 下，选择链接以 **转到Microsoft Azure 管理门户。**

## <a name="next-steps"></a>后续步骤

- 下载[“CSP 订阅转让”表](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)。

- 了解 [多合作伙伴支持](multipartner.md)。

- [多合作伙伴支持](multipartner.md)。
- [多通道支持](multichannel.md)。
- [转移 Azure 订阅](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)