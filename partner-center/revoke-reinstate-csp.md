---
title: 恢复 Azure CSP 的管理员权限
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何帮助客户恢复合作伙伴的管理员权限，使合作伙伴能够帮助管理客户的 Azure 云解决方案提供商 (CSP) 订阅。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510170"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>恢复客户的 Azure CSP 订阅的管理员权限  

**相应的角色** 全局管理员 | 管理员代理

作为云解决方案提供商 (CSP) 合作伙伴，客户通常期望你为他们管理 Azure 使用情况和系统。 你必须具有管理员权限才能执行此操作。 与客户建立分销商关系后，你会获得一些权限。 另一部分权限由客户向你授予。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 中的 Azure 管理员权限

在 CSP 中，有两种级别的 Azure 管理员权限。

- 租户级管理员权限（委派的管理员权限）：CSP 合作伙伴在与客户建立 CSP 经销商关系时获得这些权限。 委派的管理员权限让 CSP 合作伙伴能够访问其客户的租户。 拥有此访问权限后，他们可以执行管理功能，例如添加/管理用户、重置密码和管理用户许可证。
- 订阅级管理员权限：CSP 合作伙伴在为其客户创建 Azure CSP 订阅时获取这些权限。 如果具有这些权限，CSP 合作伙伴便可以完全访问这些订阅，从而能够预配和管理 Azure 资源。

## <a name="reinstate-csp-a-partners-admin-privileges"></a>为 CSP 恢复合作伙伴的管理员权限

如果你向客户提供 AdminAgents 组的 `object ID`，他们就可重新创建 CSP 角色分配。 若要重新获得委派的管理员权限，需要通过以下步骤与客户协作。

1. 登录到合作伙伴中心面板。

2. 在“合作伙伴中心”菜单中，选择“客户”。

3. 选择合作中的客户，并请求建立经销商关系。 此操作会生成一个链接，该链接指向具有租户管理员权限的客户。

4. 客户需要选择链接并批准经销商关系请求。

   :::image type="content" source="images/azure/revoke4.png" alt-text="建立经销商关系的电子邮件示例。":::

5. 你（合作伙伴）需要连接合作伙伴租户来获取 AdminAgents 组的对象 ID。
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. 然后，你的客户必须使用 PowerShell 或 Azure CLI 执行以下步骤。 你的客户必须拥有：

- “所有者”或“用户访问管理员”角色 
- 在订阅级别创建角色分配的权限

   a. 客户必须更新 `Az.Resources` 模块（仅适用于 PowerShell）。
   ```powershell
   Update-Module Az.Resources
   ```

   b. 客户连接到 CSP 订阅所在的租户。
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. 客户连接到订阅。 这只适用于用户对租户中的多个订阅拥有角色分配权限的情况。

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. 然后，客户创建角色分配。
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

你可以在资源组或资源级别授予所有者权限，而不是在订阅范围内授予所有者权限。 

- 在资源组级别

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- 在资源级别

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

如果上述步骤不起作用，或在尝试时出现错误，请尝试执行以下“全部捕获”过程，恢复客户的管理员权限。

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>疑难解答

如果客户无法完成上述步骤 6，则让客户尝试执行以下命令：

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

向 Microsoft 提供生成的 `newRoleAssignment.log` 文件以供进一步分析。

如果 `Import-Module` 中的“全部捕获”过程失败，请尝试执行以下步骤：
- 如果导入失败是因为模块正在使用中，请关闭并重新打开所有窗口，重启 PowerShell 会话。
- 通过 `Get-Module Az.Resources -ListAvailable` 检查 `Az.Resources` 的版本。
- 如果版本 4.1.1 不在可用列表中，则必须使用 `Update-Module Az.Resources -Force`。
- 如果错误指明 `Az.Accounts` 需为特定版本，则还需更新该模块，将 `Az.Resources` 替换为 `Az.Accounts`。 然后必须重启 PowerShell 会话。


## <a name="next-steps"></a>后续步骤

- [管理 Azure 计划中的订阅和资源](azure-plan-manage.md)
