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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="e7844-103">恢复客户的 Azure CSP 订阅的管理员权限</span><span class="sxs-lookup"><span data-stu-id="e7844-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="e7844-104">**相应的角色** 全局管理员 | 管理员代理</span><span class="sxs-lookup"><span data-stu-id="e7844-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="e7844-105">作为云解决方案提供商 (CSP) 合作伙伴，客户通常期望你为他们管理 Azure 使用情况和系统。</span><span class="sxs-lookup"><span data-stu-id="e7844-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="e7844-106">你必须具有管理员权限才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="e7844-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="e7844-107">与客户建立分销商关系后，你会获得一些权限。</span><span class="sxs-lookup"><span data-stu-id="e7844-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="e7844-108">另一部分权限由客户向你授予。</span><span class="sxs-lookup"><span data-stu-id="e7844-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="e7844-109">CSP 中的 Azure 管理员权限</span><span class="sxs-lookup"><span data-stu-id="e7844-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="e7844-110">在 CSP 中，有两种级别的 Azure 管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e7844-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="e7844-111">租户级管理员权限（委派的管理员权限）：CSP 合作伙伴在与客户建立 CSP 经销商关系时获得这些权限。</span><span class="sxs-lookup"><span data-stu-id="e7844-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="e7844-112">委派的管理员权限让 CSP 合作伙伴能够访问其客户的租户。</span><span class="sxs-lookup"><span data-stu-id="e7844-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="e7844-113">拥有此访问权限后，他们可以执行管理功能，例如添加/管理用户、重置密码和管理用户许可证。</span><span class="sxs-lookup"><span data-stu-id="e7844-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="e7844-114">订阅级管理员权限：CSP 合作伙伴在为其客户创建 Azure CSP 订阅时获取这些权限。</span><span class="sxs-lookup"><span data-stu-id="e7844-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="e7844-115">如果具有这些权限，CSP 合作伙伴便可以完全访问这些订阅，从而能够预配和管理 Azure 资源。</span><span class="sxs-lookup"><span data-stu-id="e7844-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="e7844-116">为 CSP 恢复合作伙伴的管理员权限</span><span class="sxs-lookup"><span data-stu-id="e7844-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="e7844-117">如果你向客户提供 AdminAgents 组的 `object ID`，他们就可重新创建 CSP 角色分配。</span><span class="sxs-lookup"><span data-stu-id="e7844-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="e7844-118">若要重新获得委派的管理员权限，需要通过以下步骤与客户协作。</span><span class="sxs-lookup"><span data-stu-id="e7844-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="e7844-119">登录到合作伙伴中心面板。</span><span class="sxs-lookup"><span data-stu-id="e7844-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="e7844-120">在“合作伙伴中心”菜单中，选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="e7844-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="e7844-121">选择合作中的客户，并请求建立经销商关系。</span><span class="sxs-lookup"><span data-stu-id="e7844-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="e7844-122">此操作会生成一个链接，该链接指向具有租户管理员权限的客户。</span><span class="sxs-lookup"><span data-stu-id="e7844-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="e7844-123">客户需要选择链接并批准经销商关系请求。</span><span class="sxs-lookup"><span data-stu-id="e7844-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="建立经销商关系的电子邮件示例。":::

5. <span data-ttu-id="e7844-125">你（合作伙伴）需要连接合作伙伴租户来获取 AdminAgents 组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="e7844-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="e7844-126">然后，你的客户必须使用 PowerShell 或 Azure CLI 执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="e7844-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="e7844-127">你的客户必须拥有：</span><span class="sxs-lookup"><span data-stu-id="e7844-127">Your customer must have:</span></span>

- <span data-ttu-id="e7844-128">“所有者”或“用户访问管理员”角色</span><span class="sxs-lookup"><span data-stu-id="e7844-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="e7844-129">在订阅级别创建角色分配的权限</span><span class="sxs-lookup"><span data-stu-id="e7844-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="e7844-130">a.</span><span class="sxs-lookup"><span data-stu-id="e7844-130">a.</span></span> <span data-ttu-id="e7844-131">客户必须更新 `Az.Resources` 模块（仅适用于 PowerShell）。</span><span class="sxs-lookup"><span data-stu-id="e7844-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="e7844-132">b.</span><span class="sxs-lookup"><span data-stu-id="e7844-132">b.</span></span> <span data-ttu-id="e7844-133">客户连接到 CSP 订阅所在的租户。</span><span class="sxs-lookup"><span data-stu-id="e7844-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="e7844-134">c.</span><span class="sxs-lookup"><span data-stu-id="e7844-134">c.</span></span> <span data-ttu-id="e7844-135">客户连接到订阅。</span><span class="sxs-lookup"><span data-stu-id="e7844-135">The customer connects to the subscription.</span></span> <span data-ttu-id="e7844-136">这只适用于用户对租户中的多个订阅拥有角色分配权限的情况。</span><span class="sxs-lookup"><span data-stu-id="e7844-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="e7844-137">d.</span><span class="sxs-lookup"><span data-stu-id="e7844-137">d.</span></span> <span data-ttu-id="e7844-138">然后，客户创建角色分配。</span><span class="sxs-lookup"><span data-stu-id="e7844-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="e7844-139">你可以在资源组或资源级别授予所有者权限，而不是在订阅范围内授予所有者权限。</span><span class="sxs-lookup"><span data-stu-id="e7844-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="e7844-140">在资源组级别</span><span class="sxs-lookup"><span data-stu-id="e7844-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="e7844-141">在资源级别</span><span class="sxs-lookup"><span data-stu-id="e7844-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="e7844-142">如果上述步骤不起作用，或在尝试时出现错误，请尝试执行以下“全部捕获”过程，恢复客户的管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e7844-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="e7844-143">疑难解答</span><span class="sxs-lookup"><span data-stu-id="e7844-143">Troubleshooting</span></span>

<span data-ttu-id="e7844-144">如果客户无法完成上述步骤 6，则让客户尝试执行以下命令：</span><span class="sxs-lookup"><span data-stu-id="e7844-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="e7844-145">向 Microsoft 提供生成的 `newRoleAssignment.log` 文件以供进一步分析。</span><span class="sxs-lookup"><span data-stu-id="e7844-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="e7844-146">如果 `Import-Module` 中的“全部捕获”过程失败，请尝试执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="e7844-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="e7844-147">如果导入失败是因为模块正在使用中，请关闭并重新打开所有窗口，重启 PowerShell 会话。</span><span class="sxs-lookup"><span data-stu-id="e7844-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="e7844-148">通过 `Get-Module Az.Resources -ListAvailable` 检查 `Az.Resources` 的版本。</span><span class="sxs-lookup"><span data-stu-id="e7844-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="e7844-149">如果版本 4.1.1 不在可用列表中，则必须使用 `Update-Module Az.Resources -Force`。</span><span class="sxs-lookup"><span data-stu-id="e7844-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="e7844-150">如果错误指明 `Az.Accounts` 需为特定版本，则还需更新该模块，将 `Az.Resources` 替换为 `Az.Accounts`。</span><span class="sxs-lookup"><span data-stu-id="e7844-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="e7844-151">然后必须重启 PowerShell 会话。</span><span class="sxs-lookup"><span data-stu-id="e7844-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="e7844-152">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e7844-152">Next steps</span></span>

- [<span data-ttu-id="e7844-153">管理 Azure 计划中的订阅和资源</span><span class="sxs-lookup"><span data-stu-id="e7844-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
