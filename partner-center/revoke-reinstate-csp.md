---
title: 恢复 Azure CSP 的管理员权限
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何帮助客户恢复合作伙伴的管理员权限，使合作伙伴能够帮助管理客户的 Azure CSP 订阅。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018181"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>恢复客户的 Azure CSP 订阅的管理员权限  

**相应的角色**

- 全局管理员
- 管理员代理

作为 CSP 合作伙伴，客户通常期望你为他们管理 Azure 使用情况和系统。 这样做需要拥有管理员权限。 与客户建立分销商关系后，你会获得一些权限。 另一部分权限由客户向你授予。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 中的 Azure 管理员权限

在 CSP 中，有两种级别的 Azure 管理员权限。

**租户级管理员权限**（委派的管理员权限）- 云解决方案提供商合作伙伴在与客户建立云解决方案提供商分销商关系时获得这些权限。 借助委派的管理员权限，解决方案提供商合作伙伴可访问其客户的租户，从而能够执行管理职能，例如添加/管理用户、重置密码和管理用户许可证。

**订阅级管理员权限** - 云解决方案提供商合作伙伴在为其客户创建 Azure 云解决方案提供商订阅时获取这些权限。 如果具有这些权限，CSP 合作伙伴便可以完全访问这些订阅，从而能够预配和管理 Azure 资源。

## <a name="reinstate-csp-partners-admin-privileges"></a>恢复云解决方案提供商合作伙伴的管理员权限

只要你向客户提供 AdminAgents 组的对象 ID，他们就可重新创建 CSP 角色分配。 若要重新获得委派的管理员权限，需要与客户协作。

1. 登录合作伙伴中心仪表板，然后在合作伙伴中心菜单选择“客户”。

2. 选择合作中的客户，并请求分销商关系。 此操作会生成一个链接，该链接指向具有租户管理员权限的客户。

3. 该客户需要选择链接并批准分销商关系请求。

   :::image type="content" source="images/azure/revoke4.png" alt-text="指示创建经销商关系的电子邮件示例":::

4. 你（合作伙伴）需要连接合作伙伴租户来获取 AdminAgents 组的对象 ID。

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. 拥有所有者或用户访问管理员角色且有权在订阅级别创建角色分配的客户则执行以下操作：


    1. 连接到 CSP 订阅所在的租户。
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. 连接到订阅（仅当用户对租户中的多个订阅具有角色分配权限时才适用）。
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"`


    3. 创建角色分配
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


如果要在资源组级别或资源级别（而不是订阅范围）授予所有者角色权限，可执行以下命令：


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>后续步骤

- [管理 Azure 计划中的订阅和资源](azure-plan-manage.md)
