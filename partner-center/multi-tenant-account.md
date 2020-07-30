---
title: 向合作伙伴中心帐户添加其他租户
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 通过合作伙伴中心帐户管理多个租户
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389503"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="19a48-103">在合作伙伴中心帐户中添加和管理多个租户</span><span class="sxs-lookup"><span data-stu-id="19a48-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="19a48-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="19a48-104">**Applies to**</span></span>

- <span data-ttu-id="19a48-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="19a48-105">Partner Center</span></span>

<span data-ttu-id="19a48-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="19a48-106">**Appropriate roles**</span></span>

- <span data-ttu-id="19a48-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="19a48-107">Global admin</span></span>

<span data-ttu-id="19a48-108">出于许多原因，你可能需要在合作伙伴中心帐户中管理多个 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="19a48-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="19a48-109">例如，你的公司可以购买其他公司，你希望新公司的员工能够使用合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="19a48-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="19a48-110">但是，您希望两个公司保持独立。</span><span class="sxs-lookup"><span data-stu-id="19a48-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="19a48-111">在这种情况下，你需要将新公司的 Azure AD 租户与合作伙伴全局帐户（PNG）相关联。</span><span class="sxs-lookup"><span data-stu-id="19a48-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="19a48-112">这种关联使得两家公司的用户都可以在合作伙伴中心工作。</span><span class="sxs-lookup"><span data-stu-id="19a48-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="19a48-113">向你的帐户添加另一个 Azure AD 租户</span><span class="sxs-lookup"><span data-stu-id="19a48-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="19a48-114">作为全局管理员登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="19a48-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="19a48-115">从 "**设置**" 图标中，选择 "**帐户设置**"，然后选择 "**租户**"。</span><span class="sxs-lookup"><span data-stu-id="19a48-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="关联租户"::: 

3. <span data-ttu-id="19a48-117">选择 "**关联其他 AD 租户**" 并指示要关联的租户。</span><span class="sxs-lookup"><span data-stu-id="19a48-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="19a48-118">以全局管理员身份登录到要关联的租户，并确认关联。</span><span class="sxs-lookup"><span data-stu-id="19a48-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="确认关联租户"::: 

5. <span data-ttu-id="19a48-120">确认后，你将看到**全部设置**通知。</span><span class="sxs-lookup"><span data-stu-id="19a48-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="19a48-121">选择 "**返回到租户管理**"，你会看到列出的新添加的租户。</span><span class="sxs-lookup"><span data-stu-id="19a48-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="19a48-122">后续步骤</span><span class="sxs-lookup"><span data-stu-id="19a48-122">Next steps</span></span>

- [<span data-ttu-id="19a48-123">添加用户</span><span class="sxs-lookup"><span data-stu-id="19a48-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
