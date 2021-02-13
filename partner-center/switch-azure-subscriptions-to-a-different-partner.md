---
title: 将 Azure 订阅转移到另一个合作伙伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何更改与客户的 Azure 订阅关联的云解决方案提供商计划合作伙伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/29/2020
ms.openlocfilehash: 94df138eb94d79fb0e472744f19337ad536eb90d
ms.sourcegitcommit: 64b43ad8fb7bb56628450bea06b9cd2606c36b03
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2021
ms.locfileid: "100281263"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>了解如何将客户的 Azure 订阅转让给另一个合作伙伴

**适用于**

- Microsoft Cloud for US Government 合作伙伴中心
- Microsoft 全球云合作伙伴中心
- 云解决方案提供商 (CSP) 计划中的合作伙伴

本文介绍了如何将 Microsoft Azure 服务从一个云解决方案提供商 (CSP) 切换到另一个云解决方案提供商。

若要将客户的 Azure 服务或订阅切换到其他合作伙伴，请执行以下手动步骤。 合作伙伴和客户都需要完成这些步骤。

>[!Note]  
>目前，只有直接或间接提供程序可以传输订阅。
>不能更改与 Azure 计划、Office 365、企业移动性套件或 Microsoft Dynamics CRM 订阅关联的云解决方案提供商订阅的合作伙伴。

## <a name="switch-partners-for-azure-subscriptions"></a>针对 Azure 订阅切换合作伙伴

1. 若要将 Azure 订阅转移给新合作伙伴，则必须由客户发起该过程，然后以书面形式与当前记录的合作伙伴进行联系。

   >[!Note]
   > 当前合作伙伴负责创建发起转移过程所需的服务票证。 Microsoft 无法代表客户或新合作伙伴进行干预。 客户应该计划与当前合作伙伴密切合作，以便过渡顺利进行。

2. 订阅的合作伙伴需要执行以下任务：

   通过合作伙伴中心创建 Azure 服务票证以请求订阅传输：

   1. 从 "合作伙伴中心" 菜单中，选择 " **客户**"，从列表中选择你的客户，然后选择 " **服务管理**"。 

   2. 在 " **支持票证** " 部分下，选择 " **新票证** " 下拉列表，然后选择 " **Microsoft Azure**"。
   
   3. 在 [Azure 门户](https://portal.azure.com)中，选择 " **新建支持请求**"。
   
   4. 在步骤1中，选择 " **订阅管理** " 作为 "问题类型"，指定要传输的订阅 ID，然后选择 " **云解决方案提供商** " 作为支持计划。
   
   5. 在步骤2中，选择 " **最小影响** "，并选择 **其他一般问题** 作为问题类型。
   
   6. 下载[“CSP 订阅转让”表](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)。

3. 订阅的合作伙伴：填写[云解决方案提供商订阅转移表单](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)、对其进行签名，然后将它发送给客户。 

   若要填写表单，需要以下信息：

   - 当前合作伙伴的联系人信息和 Microsoft ID。 在 "合作伙伴中心" 菜单中，选择 " **帐户设置**" " &gt; **组织配置文件**"，并使用其中列出的 **Microsoft ID**、 **组织名称** 和 **地址** 。

   - 客户的 Microsoft ID。 在 "合作伙伴中心" 菜单中，选择 " **客户**"，然后展开客户的列表以查看其 **Microsoft ID**。

   - 要转移的订阅 ID。 在展开的客户列表中，选择 " **查看订阅**"，然后展开所选订阅以查看 **订阅 ID**。

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

7. 删除已过期的访问权限

   - 在 "合作伙伴中心" 菜单中，选择 " **客户**"。
   - 找到列表上的客户。 选择 (双击其公司名称) 。 这将打开 "客户 **订阅** " 页。
   - 在 "客户详细信息" 菜单中，选择 " **服务管理**"。
   - 在 " **Microsoft Azure**" 下，单击链接以中转到 **Microsoft Azure 管理门户**。

## <a name="next-steps"></a>后续步骤

- 下载[“CSP 订阅转让”表](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)。

- 了解 [多合作伙伴支持](multipartner.md)。

- [多合作伙伴支持](multipartner.md)。
- [多通道支持](multichannel.md)。
- [转移 Azure 订阅](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)