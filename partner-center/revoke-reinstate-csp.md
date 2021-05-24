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
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855414"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="29943-103">恢复客户的 Azure CSP 订阅的管理员权限</span><span class="sxs-lookup"><span data-stu-id="29943-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="29943-104">**相应的角色** 全局管理员 | 管理员代理</span><span class="sxs-lookup"><span data-stu-id="29943-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="29943-105">作为 CSP 合作伙伴，客户通常期望你为他们管理 Azure 使用情况和系统。</span><span class="sxs-lookup"><span data-stu-id="29943-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="29943-106">这样做需要拥有管理员权限。</span><span class="sxs-lookup"><span data-stu-id="29943-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="29943-107">与客户建立分销商关系后，你会获得一些权限。</span><span class="sxs-lookup"><span data-stu-id="29943-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="29943-108">另一部分权限由客户向你授予。</span><span class="sxs-lookup"><span data-stu-id="29943-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="29943-109">CSP 中的 Azure 管理员权限</span><span class="sxs-lookup"><span data-stu-id="29943-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="29943-110">在 CSP 中，有两种级别的 Azure 管理员权限。</span><span class="sxs-lookup"><span data-stu-id="29943-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="29943-111">**租户级管理员权限**（委派的管理员权限）- 云解决方案提供商合作伙伴在与客户建立云解决方案提供商分销商关系时获得这些权限。</span><span class="sxs-lookup"><span data-stu-id="29943-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="29943-112">借助委派的管理员权限，解决方案提供商合作伙伴可访问其客户的租户，从而能够执行管理职能，例如添加/管理用户、重置密码和管理用户许可证。</span><span class="sxs-lookup"><span data-stu-id="29943-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="29943-113">**订阅级管理员权限** - 云解决方案提供商合作伙伴在为其客户创建 Azure 云解决方案提供商订阅时获取这些权限。</span><span class="sxs-lookup"><span data-stu-id="29943-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="29943-114">如果具有这些权限，CSP 合作伙伴便可以完全访问这些订阅，从而能够预配和管理 Azure 资源。</span><span class="sxs-lookup"><span data-stu-id="29943-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="29943-115">恢复云解决方案提供商合作伙伴的管理员权限</span><span class="sxs-lookup"><span data-stu-id="29943-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="29943-116">只要你向客户提供 AdminAgents 组的对象 ID，他们就可重新创建 CSP 角色分配。</span><span class="sxs-lookup"><span data-stu-id="29943-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="29943-117">若要重新获得委派的管理员权限，需要与客户协作。</span><span class="sxs-lookup"><span data-stu-id="29943-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="29943-118">登录合作伙伴中心仪表板，然后在合作伙伴中心菜单选择“客户”。</span><span class="sxs-lookup"><span data-stu-id="29943-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="29943-119">选择合作中的客户，并请求分销商关系。</span><span class="sxs-lookup"><span data-stu-id="29943-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="29943-120">此操作会生成一个链接，该链接指向具有租户管理员权限的客户。</span><span class="sxs-lookup"><span data-stu-id="29943-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="29943-121">该客户需要选择链接并批准分销商关系请求。</span><span class="sxs-lookup"><span data-stu-id="29943-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="指示创建经销商关系的电子邮件示例":::

4. <span data-ttu-id="29943-123">你（合作伙伴）需要连接合作伙伴租户来获取 AdminAgents 组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="29943-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="29943-124">拥有所有者或用户访问管理员角色且有权在订阅级别创建角色分配的客户则执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="29943-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="29943-125">连接到 CSP 订阅所在的租户。</span><span class="sxs-lookup"><span data-stu-id="29943-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="29943-126">连接到订阅（仅当用户对租户中的多个订阅具有角色分配权限时才适用）。</span><span class="sxs-lookup"><span data-stu-id="29943-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="29943-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="29943-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="29943-128">创建角色分配</span><span class="sxs-lookup"><span data-stu-id="29943-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="29943-129">如果要在资源组级别或资源级别（而不是订阅范围）授予所有者角色权限，可执行以下命令：</span><span class="sxs-lookup"><span data-stu-id="29943-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="29943-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="29943-130">Next steps</span></span>

- [<span data-ttu-id="29943-131">管理 Azure 计划中的订阅和资源</span><span class="sxs-lookup"><span data-stu-id="29943-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
