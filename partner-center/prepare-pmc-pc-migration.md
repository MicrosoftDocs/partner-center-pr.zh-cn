---
title: 准备从合作伙伴成员中心迁移到合作伙伴中心 |合作伙伴中心
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在将业务从 PMC 移动到合作伙伴中心之前，请先查看有用的信息和常见问题。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8d0e540282b3e683233c188f9258683809af510e
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004856"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="ee484-103">准备从合作伙伴成员中心（PMC）迁移到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="ee484-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="ee484-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="ee484-104">**Appropriate roles**</span></span>
-   <span data-ttu-id="ee484-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ee484-105">Global admin</span></span>
-   <span data-ttu-id="ee484-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="ee484-106">User admin</span></span>
-   <span data-ttu-id="ee484-107">销售代理</span><span class="sxs-lookup"><span data-stu-id="ee484-107">Sales agent</span></span>
-   <span data-ttu-id="ee484-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="ee484-108">Admin agent</span></span>

<span data-ttu-id="ee484-109">我们正在将成员身份管理从合作伙伴成员中心（PMC）移动到合作伙伴中心，这是用于管理与 Microsoft 的业务关系的单一目标。</span><span class="sxs-lookup"><span data-stu-id="ee484-109">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="ee484-110">我们希望移动到合作伙伴中心的工作效率更高。</span><span class="sxs-lookup"><span data-stu-id="ee484-110">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="ee484-111">我们确定了合作伙伴中心与 PMC 不同的部分，我们认为你需要在进行移动之前了解并准备好它们。</span><span class="sxs-lookup"><span data-stu-id="ee484-111">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="ee484-112">帐户和标识设置</span><span class="sxs-lookup"><span data-stu-id="ee484-112">Account and identity setup</span></span>

<span data-ttu-id="ee484-113">**什么是 Azure Active Directory （Azure AD）工作帐户？**</span><span class="sxs-lookup"><span data-stu-id="ee484-113">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="ee484-114">Azure 工作帐户是公司在 Azure 公有云中的专用独立虚拟表示形式，它是在订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时创建的。</span><span class="sxs-lookup"><span data-stu-id="ee484-114">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="ee484-115">你的工作帐户将托管你的 Azure AD 用户以及有关这些用户的信息-他们的电子邮件、密码、配置文件数据、权限等。</span><span class="sxs-lookup"><span data-stu-id="ee484-115">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="ee484-116">工作帐户还包含与公司及其安全性相关的组、应用程序和其他信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-116">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> <span data-ttu-id="ee484-117">有关详细信息，请参阅 。</span><span class="sxs-lookup"><span data-stu-id="ee484-117">For more information see ...</span></span>

<span data-ttu-id="ee484-118">在合作伙伴中心，你将使用工作电子邮件登录到你的帐户，而不是个人电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ee484-118">In the Partner Center you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="ee484-119">你的工作帐户： john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="ee484-119">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="ee484-120">你的个人帐户： John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="ee484-120">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="ee484-121">你的工作电子邮件属于你的 Azure active directory 租户。</span><span class="sxs-lookup"><span data-stu-id="ee484-121">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="ee484-122">若要在合作伙伴中心拥有帐户，需要具有 AAD 租户。</span><span class="sxs-lookup"><span data-stu-id="ee484-122">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="ee484-123">有关 Azure Active Directory 的详细信息，请参阅[在 Azure AD 中创建目录](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。</span><span class="sxs-lookup"><span data-stu-id="ee484-123">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="ee484-124">**当你从 PMC 移动到合作伙伴中心时，如果你有一个包含 Microsoft （例如 Office 365）的 AAD 租户，你应该使用哪个帐户登录到合作伙伴中心，并且你还拥有适用于你的 CSP 业务的租户？**</span><span class="sxs-lookup"><span data-stu-id="ee484-124">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="ee484-125">可以使用 CSP 帐户或 MPN 工作电子邮件帐户登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ee484-125">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="ee484-126">如果选择使用 CSP 工作电子邮件登录，则仪表板上的左侧导航栏将显示 MPN 和 CSP 计划信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-126">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="ee484-127">如果使用 MPN Azure AD 租户工作电子邮件登录，则只会看到 MPN 程序信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-127">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="ee484-128">用户角色在 MPN 和 CSP 之间有所不同，因此，如果对 MPN 和 CSP 企业使用同一帐户，请确保相应地分配用户角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-128">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="ee484-129">有关用户角色的详细信息，请参阅[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ee484-129">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="ee484-130">**如果你不想将现有的 Office 365 Azure AD 租户用于合作伙伴中心，则可以在从 PMC 迁移之前创建新租户。**</span><span class="sxs-lookup"><span data-stu-id="ee484-130">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="ee484-131">可能有很多原因不想使用现有的 Azure AD 租户设置合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="ee484-131">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="ee484-132">开始迁移到合作伙伴中心之前，请先前往[Azure 门户](https://ms.portal.azure.com/#home)创建新的 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="ee484-132">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="ee484-133">按照在 Azure Active Directory 中[创建新租户](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)中的指南进行操作。</span><span class="sxs-lookup"><span data-stu-id="ee484-133">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="ee484-134">创建新租户后，请在从 PMC 移动到合作伙伴中心时，使用此 AAD 租户设置合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="ee484-134">Once you have created the new tenant, use this AAD tenant to set up your Partner Center account when you move from PMC to Partner Center.</span></span> <span data-ttu-id="ee484-135">只有全局管理员才能创建租户。</span><span class="sxs-lookup"><span data-stu-id="ee484-135">You must be a global admin to create the tenant.</span></span> <span data-ttu-id="ee484-136">使用此新目录迁移到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ee484-136">Use this new directory to migrate to Partner Center.</span></span>


<span data-ttu-id="ee484-137">**AAD 全局管理员角色和 PMC MPN 全局管理员角色之间的区别是什么？**</span><span class="sxs-lookup"><span data-stu-id="ee484-137">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="ee484-138">它们是两个完全不同的角色，具有不同的权限。</span><span class="sxs-lookup"><span data-stu-id="ee484-138">These are two completely different roles with different permissions.</span></span> <span data-ttu-id="ee484-139">合作伙伴中心的 AAD 租户全局管理员管理租户-添加或删除用户、提供和管理密码、角色和权限，并且可以在合作伙伴中心访问公司的所有程序。</span><span class="sxs-lookup"><span data-stu-id="ee484-139">The AAD tenant global admin in Partner Center administers the tenant - adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company's programs in Partner Center.</span></span> 

<span data-ttu-id="ee484-140">PMC 中的 MPN 全局管理员角色可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ee484-140">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="ee484-141">查看和编辑与公司和公司所有位置相关的所有数据</span><span class="sxs-lookup"><span data-stu-id="ee484-141">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="ee484-142">在全局或本地级别添加管理员。</span><span class="sxs-lookup"><span data-stu-id="ee484-142">Add administrators at the global or local level.</span></span>  <span data-ttu-id="ee484-143">此外，全局管理员可在任何位置向其授予全局管理员访问权限，而无需考虑与它们关联的位置。</span><span class="sxs-lookup"><span data-stu-id="ee484-143">Also, Global admins can assign any person at any location Global Administrator Access which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="ee484-144">执行任何面向合作伙伴的 UI 函数，包括：</span><span class="sxs-lookup"><span data-stu-id="ee484-144">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="ee484-145">添加/删除用户</span><span class="sxs-lookup"><span data-stu-id="ee484-145">Add/remove users</span></span>

 - <span data-ttu-id="ee484-146">分配/删除角色</span><span class="sxs-lookup"><span data-stu-id="ee484-146">Assign/remove roles</span></span> 

 - <span data-ttu-id="ee484-147">添加/删除/更新位置</span><span class="sxs-lookup"><span data-stu-id="ee484-147">Add/remove/update locations</span></span> 

 - <span data-ttu-id="ee484-148">购买资格/地图</span><span class="sxs-lookup"><span data-stu-id="ee484-148">Purchase competency/maps</span></span> 

-  <span data-ttu-id="ee484-149">查看权益</span><span class="sxs-lookup"><span data-stu-id="ee484-149">View benefits</span></span>

<span data-ttu-id="ee484-150">当 MPN 全局管理员移动到合作伙伴中心时，角色称为 MPN 合作伙伴管理员，其权限和任务与合作伙伴中心全局管理员不同。有关合作伙伴中心中的角色和权限的详细信息，请参阅[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ee484-150">When the MPN global admin moves to Partner Center the role is called the MPN partner admin which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="ee484-151">**用户角色，包括合作伙伴中心的来宾用户角色**</span><span class="sxs-lookup"><span data-stu-id="ee484-151">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="ee484-152">根据需要完成的工作类型，合作伙伴中心具有不同类型的角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-152">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="ee484-153">全局管理员等角色 Azure AD 角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-153">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="ee484-154">某些角色特定于云服务提供商计划或激励等程序，并且有特定于 MPN 的角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-154">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="ee484-155">若要了解合作伙伴中心的所有角色，请阅读[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ee484-155">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="ee484-156">**当我的用户的角色从 PMC 移动到合作伙伴中心时会发生什么情况？**</span><span class="sxs-lookup"><span data-stu-id="ee484-156">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="ee484-157">如果执行迁移的 MPN 全局管理员或主要程序联系人除外，则 PMC 中的所有用户将失去其管理员角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-157">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="ee484-158">完成迁移的个人需要在合作伙伴中心分配角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-158">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="ee484-159">合作伙伴中心的角色不同于 PMC 中的角色。</span><span class="sxs-lookup"><span data-stu-id="ee484-159">The roles in Partner Center differ from those in PMC.</span></span> <span data-ttu-id="ee484-160">有关合作伙伴中心中的用户角色的详细信息，请参阅 [分配用户角色和权限] （overview.md 和[从 PMC 移动到合作伙伴中心](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)。</span><span class="sxs-lookup"><span data-stu-id="ee484-160">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="ee484-161">**我的公司配置文件和我的业务配置文件之间的区别是什么？**</span><span class="sxs-lookup"><span data-stu-id="ee484-161">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="ee484-162">公司配置文件是公司的相关信息，包括地址、位置、主要联系人、银行和税务详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-162">Your company profile is the information about your company that includes address, locations, primary contact, bank and tax details.</span></span>

<span data-ttu-id="ee484-163">你的业务配置文件是你向客户展示自己的方式，是一种显示徽标的营销页面、你的业务重点的详细信息、你的专业人员等。</span><span class="sxs-lookup"><span data-stu-id="ee484-163">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="ee484-164">**帐户合并对我的帐户有何意义？**</span><span class="sxs-lookup"><span data-stu-id="ee484-164">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="ee484-165">如果你使用相同的 Azure AD 租户将多个 MPN 帐户迁移到合作伙伴中心，系统将自动识别并要求你合并帐户。</span><span class="sxs-lookup"><span data-stu-id="ee484-165">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="ee484-166">即使有多个域关联到同一个 Azure AD 租户，也是如此。</span><span class="sxs-lookup"><span data-stu-id="ee484-166">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="ee484-167">你仍可以决定使用单独的 AAD 租户迁移到合作伙伴中心，但请注意，这会导致你的能力和额外购买成本的隔离。</span><span class="sxs-lookup"><span data-stu-id="ee484-167">You could still decide to migrate to Partner Center using separate AAD tenants, but please note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="ee484-168">**如果我有多个 AAD 租户和单个 MPN 帐户，是否可以在合作伙伴中心进行链接？**</span><span class="sxs-lookup"><span data-stu-id="ee484-168">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="ee484-169">是的，在合作伙伴中心，你可以将多个 Azure AD 租户链接到单个合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="ee484-169">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="ee484-170">单击此处可了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-170">Learn more here.</span></span> 

<span data-ttu-id="ee484-171">**是否存在将多个 Azure AD 租户添加到单个合作伙伴中心帐户的限制？**</span><span class="sxs-lookup"><span data-stu-id="ee484-171">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="ee484-172">如果 Azure AD 租户已关联到现有合作伙伴中心帐户，则不能使用多租户功能将其关联到新的合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="ee484-172">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="ee484-173">要考虑的另一种方法是，一个 Azure AD 租户只能关联到一个合作伙伴中心帐户，但合作伙伴中心帐户可以有多个关联的租户。</span><span class="sxs-lookup"><span data-stu-id="ee484-173">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="ee484-174">Microsoft 合作伙伴网络（MPN）成员身份迁移</span><span class="sxs-lookup"><span data-stu-id="ee484-174">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="ee484-175">**谁可以执行从 PMC 到合作伙伴中心的迁移？**</span><span class="sxs-lookup"><span data-stu-id="ee484-175">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="ee484-176">你的公司 MPN 全局管理员或主要计划联系人（这两个角色通常由同一个人持有）可以启动并执行移动。</span><span class="sxs-lookup"><span data-stu-id="ee484-176">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="ee484-177">**完成迁移的人员是否会成为合作伙伴中心的公司法律配置文件中的主要联系人？**</span><span class="sxs-lookup"><span data-stu-id="ee484-177">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="ee484-178">但不一定，主要联系人必须是有权签署协议的人。</span><span class="sxs-lookup"><span data-stu-id="ee484-178">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="ee484-179">**Microsoft 能否迁移我的 MPN 成员身份？**</span><span class="sxs-lookup"><span data-stu-id="ee484-179">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="ee484-180">不相同。</span><span class="sxs-lookup"><span data-stu-id="ee484-180">No.</span></span> <span data-ttu-id="ee484-181">Microsoft 无法帮助你将成员资格帐户移到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ee484-181">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="ee484-182">需要使用工作帐户登录到 PMC 来移动帐户（登录凭据），以便开始迁移过程。</span><span class="sxs-lookup"><span data-stu-id="ee484-182">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="ee484-183">完成了移动帐户的步骤后，你可以开始管理你的成员身份并向你的团队分配用户角色和权限，以便他们可以访问权益并帮助管理成员身份。</span><span class="sxs-lookup"><span data-stu-id="ee484-183">After you've completed the steps to move your account you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="ee484-184">Microsoft 将自动迁移当前的资格、权益、位置信息、银行/税务信息和</span><span class="sxs-lookup"><span data-stu-id="ee484-184">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="ee484-185">Microsoft 将自动迁移当前的资格、权益、位置信息、银行/税务信息和</span><span class="sxs-lookup"><span data-stu-id="ee484-185">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="ee484-186">**续订策略会如何变化？**</span><span class="sxs-lookup"><span data-stu-id="ee484-186">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="ee484-187">在合作伙伴中心，续订时段为你的周年纪念，截止时间为30天。</span><span class="sxs-lookup"><span data-stu-id="ee484-187">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="ee484-188">**迁移到合作伙伴中心后，我们的称职情况是否保持不变？**</span><span class="sxs-lookup"><span data-stu-id="ee484-188">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="ee484-189">是的，compentencies 不会受到 "移动到合作伙伴中心" 的影响。</span><span class="sxs-lookup"><span data-stu-id="ee484-189">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="ee484-190">如果你注意到了矛盾，请联系[支持人员](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="ee484-190">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="ee484-191">**迁移后，我的权益（包括云权益、技术支持、软件权益、Visual Studio）是否会更改？**</span><span class="sxs-lookup"><span data-stu-id="ee484-191">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="ee484-192">你的合格权益将不会更改。</span><span class="sxs-lookup"><span data-stu-id="ee484-192">Your eligible benefits will not change.</span></span> <span data-ttu-id="ee484-193">如果你注意到了矛盾，请联系[支持人员](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="ee484-193">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="ee484-194">**Microsoft 帐户是否会享有 Visual Studio 权益分配？**</span><span class="sxs-lookup"><span data-stu-id="ee484-194">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="ee484-195">是</span><span class="sxs-lookup"><span data-stu-id="ee484-195">Yes.</span></span> <span data-ttu-id="ee484-196">分配给 MSA 的 Visual Studio 权益仍将有效，会继续保留。</span><span class="sxs-lookup"><span data-stu-id="ee484-196">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="ee484-197">在合作伙伴中心续订后，仍会保留它们。</span><span class="sxs-lookup"><span data-stu-id="ee484-197">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="ee484-198">但是，如果在伙伴中心迁移后删除 MSA 分配，则不能将其重新添加到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ee484-198">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="ee484-199">在合作伙伴中心，合作伙伴可以添加特定的工作帐户和来宾用户帐户，这些帐户是同一租户的 MSA，而这些租户中的合作伙伴在 Azure AD 租户中是 MPN 管理员。</span><span class="sxs-lookup"><span data-stu-id="ee484-199">In Partner Center, a partner can add work accounts and guest user accounts which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="ee484-200">如果合作伙伴在多个 Azure AD 租户中是全局管理员，并且所有这些租户都关联到同一个合作伙伴中心帐户，则该合作伙伴可以跨所有这些租户将用户添加到 Visual Studio 权益中以及基于 Azure 使用情况的分配计划中。</span><span class="sxs-lookup"><span data-stu-id="ee484-200">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="ee484-201">虽然来宾用户可以由 MPN 管理员或全局管理员分配基于使用情况的 Visual Studio 订阅，但来宾用户不能使用其 MSA 登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ee484-201">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="ee484-202">不过，来宾用户可以登录 Azure 和 Visual Studio，以便验证和使用分配给他们的权益。</span><span class="sxs-lookup"><span data-stu-id="ee484-202">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="ee484-203">**如何管理 MCP 关联和合作伙伴大学访问？**</span><span class="sxs-lookup"><span data-stu-id="ee484-203">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="ee484-204">不会更改从 PMC 移动的 MCP 关联。</span><span class="sxs-lookup"><span data-stu-id="ee484-204">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="ee484-205">但是，在迁移到合作伙伴中心后，任何新员工都需要在合作伙伴中心内关联。</span><span class="sxs-lookup"><span data-stu-id="ee484-205">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="ee484-206">你的现有用户的所有合作伙伴大学权限都将保留，但任何新员工都应访问[培训中心](https://partner.microsoft.com/training)，以获取有关如何获取对合作伙伴大学的访问权限的信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-206">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="ee484-207">**转到合作伙伴中心后如何实现查看 MCP 信息？**</span><span class="sxs-lookup"><span data-stu-id="ee484-207">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="ee484-208">在仪表板的左侧导航栏中选择 "**胜任度**"。</span><span class="sxs-lookup"><span data-stu-id="ee484-208">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="ee484-209">从 "**称职**情况" 页，您可以下载技能报表。</span><span class="sxs-lookup"><span data-stu-id="ee484-209">From the **Competencies** page you are able to download the skills report.</span></span> <span data-ttu-id="ee484-210">技能报告将列出您的用户，他们已获得与合作伙伴中心的能力和计划相关的技能。</span><span class="sxs-lookup"><span data-stu-id="ee484-210">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="ee484-211">如果你的用户获得了技能，但这些技能与你正在努力的胜任度无关，则他们将不会在报告中列出。</span><span class="sxs-lookup"><span data-stu-id="ee484-211">If your users have gained skills but those skills are not relevant to the competencies which you are working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="ee484-212">**合作伙伴中心是否使用了客户参考？**</span><span class="sxs-lookup"><span data-stu-id="ee484-212">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="ee484-213">不可以，无需客户参考即可满足合作伙伴中心的资格要求。</span><span class="sxs-lookup"><span data-stu-id="ee484-213">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="ee484-214">**记录关联的合作伙伴是否会迁移到合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="ee484-214">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="ee484-215">是的，记录的合作伙伴不会有任何变化。</span><span class="sxs-lookup"><span data-stu-id="ee484-215">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="ee484-216">了解有关将[合作伙伴 ID 链接到客户](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee484-216">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="ee484-217">**由于迁移到合作伙伴中心，是否会对激励产生影响？**</span><span class="sxs-lookup"><span data-stu-id="ee484-217">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="ee484-218">不会，如果你已移动帐户而没有合并位置，则没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="ee484-218">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="ee484-219">如果你的企业在 PMC 中有多个帐户，当你移动到合作伙伴中心时，你决定将合并到全局帐户中时，将不会有任何损失，但激励付出的延迟可能会有延迟。</span><span class="sxs-lookup"><span data-stu-id="ee484-219">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="ee484-220">如果不移动所有 PMC 帐户，而这些帐户已包含在激励计划中，你可能会停止获得与这些帐户关联的奖励。</span><span class="sxs-lookup"><span data-stu-id="ee484-220">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="ee484-221">**合作伙伴中心的激励用户角色是什么？**</span><span class="sxs-lookup"><span data-stu-id="ee484-221">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="ee484-222">合作伙伴中心的激励角色是基于位置的，其中包括奖励管理和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="ee484-222">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="ee484-223">有关这些角色可以执行的操作的详细信息，请参阅[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="ee484-223">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="ee484-224">**奖励用户是否可以在全局和位置级别分配？**</span><span class="sxs-lookup"><span data-stu-id="ee484-224">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="ee484-225">是</span><span class="sxs-lookup"><span data-stu-id="ee484-225">Yes.</span></span> <span data-ttu-id="ee484-226">您可以分配激励管理员作为所有地点的奖励管理员，或者每个地点都有其自己的激励管理员。</span><span class="sxs-lookup"><span data-stu-id="ee484-226">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="ee484-227">**奖励是否可以在全局或位置级别支付？**</span><span class="sxs-lookup"><span data-stu-id="ee484-227">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="ee484-228">激励仅在位置级别支付。</span><span class="sxs-lookup"><span data-stu-id="ee484-228">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="ee484-229">**对于引用，我们可以创建多少个业务配置文件？**</span><span class="sxs-lookup"><span data-stu-id="ee484-229">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="ee484-230">你的公司可以创建任意数量的业务配置文件，以完全表示你公司的兴趣。</span><span class="sxs-lookup"><span data-stu-id="ee484-230">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="ee484-231">在每个业务配置文件中，最多可以列出五个位置，一个国家/地区。</span><span class="sxs-lookup"><span data-stu-id="ee484-231">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="ee484-232">每个业务配置文件都可以接收其每个位置的引用。</span><span class="sxs-lookup"><span data-stu-id="ee484-232">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="ee484-233">**如何分配引用，我需要做哪些更改？例如，如果在一个市场中有一个全球性公司，而在其他市场中有一个位置，将如何分配引用？**</span><span class="sxs-lookup"><span data-stu-id="ee484-233">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="ee484-234">引用根据客户定义的搜索参数进行分配。</span><span class="sxs-lookup"><span data-stu-id="ee484-234">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="ee484-235">因此，无论您有一个位置还是多个位置，如果客户指定了所需的位置，并且有一个满足其他参数的业务，则引用将会跳到该位置。</span><span class="sxs-lookup"><span data-stu-id="ee484-235">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








