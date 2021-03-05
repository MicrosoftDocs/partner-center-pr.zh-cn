---
title: 将租户添加到合作伙伴中心帐户
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在合作伙伴中心帐户中添加、合并或管理多个 Azure AD 租户，并了解可能需要执行此操作的原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124799"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="a6d90-103">在合作伙伴中心帐户中添加和管理多个租户</span><span class="sxs-lookup"><span data-stu-id="a6d90-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="a6d90-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="a6d90-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a6d90-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a6d90-105">Global admin</span></span>
- <span data-ttu-id="a6d90-106">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="a6d90-106">Account admin</span></span>

<span data-ttu-id="a6d90-107">本文介绍如何将多个 Azure Active Directory (Azure AD) 租户合并为你的公司，然后在你的合作伙伴中心帐户中添加和管理它们。</span><span class="sxs-lookup"><span data-stu-id="a6d90-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="a6d90-108">这样做的原因有很多。</span><span class="sxs-lookup"><span data-stu-id="a6d90-108">There are many reasons to do so.</span></span> <span data-ttu-id="a6d90-109">例如：</span><span class="sxs-lookup"><span data-stu-id="a6d90-109">For example:</span></span>

- <span data-ttu-id="a6d90-110">假设你的公司 Contoso 收购了另一家公司 Fabrikam。</span><span class="sxs-lookup"><span data-stu-id="a6d90-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="a6d90-111">您希望两家公司保持独立，但您希望新员工能够使用合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="a6d90-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="a6d90-112">在这种情况下，可将新公司的 Azure AD 租户与合作伙伴全局帐户 (PGA) 相关联。</span><span class="sxs-lookup"><span data-stu-id="a6d90-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="a6d90-113">这种关联使得两家公司的用户都可以在合作伙伴中心工作。</span><span class="sxs-lookup"><span data-stu-id="a6d90-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="a6d90-114">如果你运行的业务包含多个租户 (例如， *contoso.com*、 *contoso.uk* 和 *contoso.in*) ，则可以使用多租户将它们分组到相同的 PC 帐户中。</span><span class="sxs-lookup"><span data-stu-id="a6d90-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="a6d90-115">如果合并和收购指导原则要求你使用两家公司的租户，则应同时使用 *constoso.com* 和 *fabrikam.com* 租户。</span><span class="sxs-lookup"><span data-stu-id="a6d90-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="a6d90-116">任何租户的用户都需要能够：</span><span class="sxs-lookup"><span data-stu-id="a6d90-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="a6d90-117">访问合作伙伴中心，了解培训、数字下载或 Microsoft 认证专家 (MCP) 关联。</span><span class="sxs-lookup"><span data-stu-id="a6d90-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="a6d90-118">将 Microsoft 合作伙伴网络 (MPN) 管理员或奖励 admin）分配给合作伙伴中心角色。</span><span class="sxs-lookup"><span data-stu-id="a6d90-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="a6d90-119">向你的帐户添加 Azure AD 租户</span><span class="sxs-lookup"><span data-stu-id="a6d90-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="a6d90-120">以全局管理员身份登录到 [Microsoft 合作伙伴中心](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a6d90-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="a6d90-121">在右上方，选择 " **设置**"，选择 " **帐户设置**"，然后选择 " **租户**"。</span><span class="sxs-lookup"><span data-stu-id="a6d90-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="&quot;Azure AD 配置文件&quot; 窗格上的 &quot;关联&quot; 按钮的屏幕截图。"::: 

1. <span data-ttu-id="a6d90-123">选择 " **关联**"，然后指定要关联的租户。</span><span class="sxs-lookup"><span data-stu-id="a6d90-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="a6d90-124">在提示符下，以全局管理员身份登录到要关联的租户，然后选择 " **确认**"。</span><span class="sxs-lookup"><span data-stu-id="a6d90-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="&quot;确认新 Azure AD 关联&quot; 窗格上的 &quot;确认&quot; 按钮的屏幕截图。"::: 

   <span data-ttu-id="a6d90-126">确认关联后，将显示 " **所有设置** " 消息。</span><span class="sxs-lookup"><span data-stu-id="a6d90-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="a6d90-127">若要查看新添加的租户，请选择 " **返回到租户管理**"。</span><span class="sxs-lookup"><span data-stu-id="a6d90-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="a6d90-128">如果某个租户已与另一个合作伙伴中心帐户相关联，则无法将其与该帐户相关联。</span><span class="sxs-lookup"><span data-stu-id="a6d90-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="a6d90-129">从帐户中删除租户</span><span class="sxs-lookup"><span data-stu-id="a6d90-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="a6d90-130">以全局管理员身份登录到 [Microsoft 合作伙伴中心](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a6d90-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="a6d90-131">在右上方，选择 " **设置** " 图标，然后选择 " **帐户设置**"。</span><span class="sxs-lookup"><span data-stu-id="a6d90-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="a6d90-132">在左侧窗格中，选择 " **租户**"。</span><span class="sxs-lookup"><span data-stu-id="a6d90-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="a6d90-133">在 " **管理 Azure AD 租户**" 下，选择 " **合作伙伴** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="a6d90-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="a6d90-134">选择要删除其关联的租户旁边的 " **删除** "。</span><span class="sxs-lookup"><span data-stu-id="a6d90-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="当前租户关联及其删除链接的屏幕截图。":::

   <span data-ttu-id="a6d90-136">如前面的屏幕截图所示，为所有关联的租户启用了 " **删除** " 链接，但主要租户和当前登录到的租户除外。</span><span class="sxs-lookup"><span data-stu-id="a6d90-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="a6d90-137">当你删除某个租户时，该租户上的用户将不再有权访问合作伙伴中心帐户，并且删除操作可能会影响你的能力。</span><span class="sxs-lookup"><span data-stu-id="a6d90-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="a6d90-138">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a6d90-138">Next steps</span></span>

- [<span data-ttu-id="a6d90-139">创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="a6d90-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






