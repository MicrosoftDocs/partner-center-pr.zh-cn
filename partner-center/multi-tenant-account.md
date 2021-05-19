---
title: 将租户添加到合作伙伴中心帐户
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在 合作伙伴中心 帐户中添加、合并或Azure AD多个租户，并了解如何这样做的原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151196"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="f3ff8-103">在帐户中添加和管理合作伙伴中心租户</span><span class="sxs-lookup"><span data-stu-id="f3ff8-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="f3ff8-104">**适当的角色**：全局管理员|帐户管理员</span><span class="sxs-lookup"><span data-stu-id="f3ff8-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="f3ff8-105">本文讨论如何为公司合并Azure Active Directory (Azure AD) 租户，然后在客户帐户中添加和管理合作伙伴中心租户。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="f3ff8-106">这样做的原因有很多。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-106">There are many reasons to do so.</span></span> <span data-ttu-id="f3ff8-107">例如：</span><span class="sxs-lookup"><span data-stu-id="f3ff8-107">For example:</span></span>

- <span data-ttu-id="f3ff8-108">假设你的公司 Contoso 收购了另一家公司 Fabrikam。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="f3ff8-109">希望这两家公司保持独立，但希望新员工能够使用合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="f3ff8-110">在这种情况下，将新公司的 Azure AD 租户与 PGA (合作伙伴全局帐户) 。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="f3ff8-111">通过此关联，这两家公司的用户可以在合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="f3ff8-112">如果通过多个租户运行业务 (例如 *contoso.com、contoso.uk* 和 *contoso.in*) ，可以使用多租户将它们分组到同一电脑帐户中。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="f3ff8-113">如果合并和收购准则要求你与这两家公司的租户合作，则同时使用 constoso.com 租户fabrikam.com *租户。*</span><span class="sxs-lookup"><span data-stu-id="f3ff8-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="f3ff8-114">任何租户的用户都需要能够：</span><span class="sxs-lookup"><span data-stu-id="f3ff8-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="f3ff8-115">访问合作伙伴中心培训、数字下载或 Microsoft 认证专家 (MCP) 关联。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="f3ff8-116">分配一合作伙伴中心角色，例如Microsoft 合作伙伴网络 (MPN) 管理员或奖励管理员。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="f3ff8-117">将Azure AD租户添加到帐户</span><span class="sxs-lookup"><span data-stu-id="f3ff8-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="f3ff8-118">以全局管理员角色登录到[Microsoft 合作伙伴中心。](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="f3ff8-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="f3ff8-119">在右上角，选择"设置 **"，** 选择"**帐户设置**"，然后选择"**租户"。**</span><span class="sxs-lookup"><span data-stu-id="f3ff8-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="&quot;配置文件&quot;窗格上&quot;关联&quot;Azure AD屏幕截图。"::: 

1. <span data-ttu-id="f3ff8-121">选择 **"** 关联"，然后指示要关联的租户。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="f3ff8-122">在提示符下，以全局管理员身份登录到要关联的租户，然后选择 " **确认**"。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="&quot;确认新 Azure AD 关联&quot; 窗格上的 &quot;确认&quot; 按钮的屏幕截图。"::: 

   <span data-ttu-id="f3ff8-124">确认关联后，将显示 " **所有设置** " 消息。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="f3ff8-125">若要查看新添加的租户，请选择 " **返回到租户管理**"。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="f3ff8-126">如果某个租户已与另一个合作伙伴中心帐户相关联，则无法将其与该帐户相关联。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="f3ff8-127">从帐户中删除租户</span><span class="sxs-lookup"><span data-stu-id="f3ff8-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="f3ff8-128">以全局管理员身份登录到 [Microsoft 合作伙伴中心](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="f3ff8-129">在右上方，选择 " **设置** " 图标，然后选择 " **帐户设置**"。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="f3ff8-130">在左侧窗格中，选择 " **租户**"。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="f3ff8-131">在 " **管理 Azure AD 租户**" 下，选择 " **合作伙伴** " 选项卡。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="f3ff8-132">选择要删除其关联的租户旁边的 " **删除** "。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="当前租户关联及其删除链接的屏幕截图。":::

   <span data-ttu-id="f3ff8-134">如前面的屏幕截图所示，为所有关联的租户启用了 " **删除** " 链接，但主要租户和当前登录到的租户除外。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="f3ff8-135">当你删除某个租户时，该租户上的用户将不再有权访问合作伙伴中心帐户，并且删除操作可能会影响你的能力。</span><span class="sxs-lookup"><span data-stu-id="f3ff8-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f3ff8-136">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f3ff8-136">Next steps</span></span>

- [<span data-ttu-id="f3ff8-137">创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="f3ff8-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






