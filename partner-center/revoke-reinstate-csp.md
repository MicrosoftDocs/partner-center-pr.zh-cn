---
title: 恢复 Azure CSP 的管理员权限
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何帮助客户恢复合作伙伴的管理员权限，使合作伙伴能够帮助管理客户的 Azure CSP 订阅。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811327"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>恢复客户的 Azure CSP 订阅的管理员权限  

**适用角色**

- 全局管理员
- 管理员代理

作为 CSP 合作伙伴，客户通常期望你为他们管理 Azure 使用情况和系统。 这样做需要拥有管理员权限。 当与客户建立分销商关系后，你会获得一些权限。 另一部分权限由客户向你授予。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 中的 Azure 管理员权限

在 CSP 中，有两种级别的 Azure 管理员权限。

**租户级管理员权限**（委派的管理员权限）- 云解决方案提供商合作伙伴在与客户建立云解决方案提供商分销商关系时获得这些权限。 这样，云解决方案提供商合作伙伴便可以访问其客户的租户，从而能够执行管理职能，例如添加/管理用户、重置密码和管理用户许可证。

**订阅级管理员权限** - 云解决方案提供商合作伙伴在为其客户创建 Azure 云解决方案提供商订阅时获取这些权限。 如果具有这些权限，CSP 合作伙伴便可以完全访问这些订阅，从而能够预配和管理 Azure 资源。

## <a name="reinstate-csp-partners-admin-privileges"></a>恢复云解决方案提供商合作伙伴的管理员权限

若要重新获得委派的管理员权限，需要与客户协作。

1. 登录到合作伙伴中心面板，然后从“合作伙伴中心”菜单中选择“客户”。

2. 选择合作中的客户，并请求分销商关系。 这会生成一个链接，该链接指向具有租户管理员权限的客户。

3. 该用户需要选择链接并批准分销商关系请求。

   :::image type="content" source="images/azure/revoke4.png" alt-text="分销商关系":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>将管理员代理组添加为 Azure CSP 订阅的所有者

你的客户需要将管理员代理组添加为 Azure CSP 订阅的所有者。

1. 使用 PowerShell 控制台或 PowerShell 集成脚本环境 (ISE)。 确保已安装 AzureAD 模块。

2. 连接到 Azure AD 租户。

   ```powershell
   Connect-AzureAD
   ```

3. 获取管理员代理组的 ObjectId。

   ```powershell
   Get-AzureADGroup
   ```
   在客户公司中具有 Azure CSP 订阅所有者访问权限的用户执行以下步骤。

4. 具有 Azure CSP 订阅所有者访问权限的用户使用其凭据登录到 Azure。

   ```powershell
   Connect-AzAccount
   ```

5. 然后，她可以将管理员代理组作为所有者添加到 CSP Azure 订阅中。

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>后续步骤

[管理 Azure 计划中的订阅和资源](azure-plan-manage.md)
