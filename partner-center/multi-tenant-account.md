---
title: 向合作伙伴中心帐户添加其他租户
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心帐户中添加、合并或管理多个 Azure AD 租户。 进一步了解你可能想要执行的一些原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105540"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="ca150-104">在合作伙伴中心帐户中添加和管理多个租户</span><span class="sxs-lookup"><span data-stu-id="ca150-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="ca150-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="ca150-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ca150-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ca150-106">Global admin</span></span>

<span data-ttu-id="ca150-107">可以通过此功能管理公司的多个租户，并将其合并到合作伙伴中心帐户中。</span><span class="sxs-lookup"><span data-stu-id="ca150-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="ca150-108">出于许多原因，你可能需要在合作伙伴中心帐户中管理多个 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="ca150-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="ca150-109">例如：</span><span class="sxs-lookup"><span data-stu-id="ca150-109">For example:</span></span>

- <span data-ttu-id="ca150-110">你的公司可能会购买其他公司，你希望新公司的员工能够使用合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ca150-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="ca150-111">但是，您希望两个公司保持独立。</span><span class="sxs-lookup"><span data-stu-id="ca150-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="ca150-112">在这种情况下，可将新公司的 Azure AD 租户与合作伙伴全局帐户 (PGA) 相关联。</span><span class="sxs-lookup"><span data-stu-id="ca150-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="ca150-113">这种关联使得两家公司的用户都可以在合作伙伴中心工作。</span><span class="sxs-lookup"><span data-stu-id="ca150-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="ca150-114">如果有多个租户运行你的业务 (例如，contoso.com、contoso.uk、contoso.in) 你可以使用多租户将它们与相同的 PC 帐户关联。</span><span class="sxs-lookup"><span data-stu-id="ca150-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="ca150-115">合并和收购要求使用多个租户 (例如，如果 Contoso 获取 Fabrikam，则需要能够同时使用 Constoso.com 和 Fabrikam.com 各自的租户) 。</span><span class="sxs-lookup"><span data-stu-id="ca150-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="ca150-116">任何租户的用户都需要能够：</span><span class="sxs-lookup"><span data-stu-id="ca150-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="ca150-117">访问合作伙伴中心进行培训、数字下载、MCP 关联</span><span class="sxs-lookup"><span data-stu-id="ca150-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="ca150-118">分配合作伙伴中心角色，如 MPN 管理员、奖励管理员等。</span><span class="sxs-lookup"><span data-stu-id="ca150-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="ca150-119">向你的帐户添加另一个 Azure AD 租户</span><span class="sxs-lookup"><span data-stu-id="ca150-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="ca150-120">作为全局管理员登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="ca150-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="ca150-121">从 " **设置** " 图标中，选择 " **帐户设置** "，然后选择 " **租户**"。</span><span class="sxs-lookup"><span data-stu-id="ca150-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="关联租户"::: 

3. <span data-ttu-id="ca150-123">选择 " **关联其他 AD 租户** " 并指示要关联的租户。</span><span class="sxs-lookup"><span data-stu-id="ca150-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="ca150-124">以全局管理员身份登录到要关联的租户，并确认关联。</span><span class="sxs-lookup"><span data-stu-id="ca150-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="确认关联租户"::: 

5. <span data-ttu-id="ca150-126">确认后，你将看到 **全部设置** 通知。</span><span class="sxs-lookup"><span data-stu-id="ca150-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="ca150-127">选择 " **返回到租户管理** "，你会看到列出的新添加的租户。</span><span class="sxs-lookup"><span data-stu-id="ca150-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="ca150-128">如果某个租户已与另一个合作伙伴中心帐户关联，则无法将其关联到该帐户。</span><span class="sxs-lookup"><span data-stu-id="ca150-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="ca150-129">从帐户中删除租户</span><span class="sxs-lookup"><span data-stu-id="ca150-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="ca150-130">作为全局管理员登录到合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="ca150-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="ca150-131">从 " **设置** " 图标中，选择 " **帐户设置** -> 租户"，然后单击 " **合作伙伴** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="ca150-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="ca150-132">对于要取消关联的租户，单击 " **删除** "。</span><span class="sxs-lookup"><span data-stu-id="ca150-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="ca150-133">租户取消关联是指租户上的用户将不再有权访问合作伙伴中心帐户，这可能会影响你的胜任度。</span><span class="sxs-lookup"><span data-stu-id="ca150-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="ca150-134">对于所有关联的租户，" **删除** " 按钮是启用的，主要租户和当前登录到的租户除外。</span><span class="sxs-lookup"><span data-stu-id="ca150-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="带有 &quot;删除&quot; 按钮的租户":::
 

## <a name="next-steps"></a><span data-ttu-id="ca150-136">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ca150-136">Next steps</span></span>

- [<span data-ttu-id="ca150-137">添加用户</span><span class="sxs-lookup"><span data-stu-id="ca150-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






