---
title: 从 Partner Membership Center 迁移
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在将业务从 Partner Membership Center 迁移到合作伙伴中心之前，请先查看有用的信息和常见问题解答。
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 31da796b50e9deeb2d6256e7818e587e9bedb881
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114567"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="c725b-103">准备从 Partner Membership Center (PMC) 迁移到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="c725b-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="c725b-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="c725b-104">**Appropriate roles**</span></span>
- <span data-ttu-id="c725b-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c725b-105">Global admin</span></span>
- <span data-ttu-id="c725b-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="c725b-106">User admin</span></span>
- <span data-ttu-id="c725b-107">销售代理</span><span class="sxs-lookup"><span data-stu-id="c725b-107">Sales agent</span></span>
- <span data-ttu-id="c725b-108">管理员代理</span><span class="sxs-lookup"><span data-stu-id="c725b-108">Admin agent</span></span>

<span data-ttu-id="c725b-109">我们正在将成员资格管理从 Partner Membership Center (PMC) 迁移到合作伙伴中心- 管理与 Microsoft 的业务关系的单一目的地。</span><span class="sxs-lookup"><span data-stu-id="c725b-109">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="c725b-110">我们希望你迁移到合作伙伴中心后会尽可能实现轻松高效的管理。</span><span class="sxs-lookup"><span data-stu-id="c725b-110">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="c725b-111">我们确定了合作伙伴中心与 PMC 一些不同的部分，我们认为在你进行迁移之前需要了解这些部分并做好相应的准备。</span><span class="sxs-lookup"><span data-stu-id="c725b-111">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="c725b-112">帐户和标识设置</span><span class="sxs-lookup"><span data-stu-id="c725b-112">Account and identity setup</span></span>

<span data-ttu-id="c725b-113">**什么是 Azure Active Directory (Azure AD) 工作帐户？**</span><span class="sxs-lookup"><span data-stu-id="c725b-113">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="c725b-114">Azure 工作帐户是公司在 Azure 公有云中的专用独立虚拟表示形式，它是在订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时创建的。</span><span class="sxs-lookup"><span data-stu-id="c725b-114">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="c725b-115">工作帐户托管 Azure AD 用户及其相关信息 - 他们的密码、个人资料数据和权限等。</span><span class="sxs-lookup"><span data-stu-id="c725b-115">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="c725b-116">工作帐户还包含组、应用程序以及有关公司及其安全性的其他信息。</span><span class="sxs-lookup"><span data-stu-id="c725b-116">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="c725b-117">你的工作电子邮件属于你 Azure Active Directory 租户的一部分。</span><span class="sxs-lookup"><span data-stu-id="c725b-117">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="c725b-118">若要在合作伙伴中心中拥有帐户，你需要拥有 AAD 租户。</span><span class="sxs-lookup"><span data-stu-id="c725b-118">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="c725b-119">有关 Azure Active Directory 的详细信息，请参阅[在 Azure AD 中创建目录](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。</span><span class="sxs-lookup"><span data-stu-id="c725b-119">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="c725b-120">在合作伙伴中心，你将使用工作电子邮件来登录你的帐户，而不是使用个人电子邮件。</span><span class="sxs-lookup"><span data-stu-id="c725b-120">In Partner Center, you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="c725b-121">你的工作帐户：john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="c725b-121">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="c725b-122">你的个人帐户：John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="c725b-122">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="c725b-123">**如果你有一个 Microsoft （例如 Office 365）的 AAD 租户并且还有适用于你的 CSP 业务的租户，你应该使用哪个帐户登录到合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="c725b-123">**What account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="c725b-124">可以使用 CSP 帐户或 MPN 工作电子邮件帐户登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="c725b-124">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="c725b-125">如果选择使用 CSP 工作电子邮件登录，面板上的左侧导航则将显示 MPN 和 CSP 计划信息。</span><span class="sxs-lookup"><span data-stu-id="c725b-125">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="c725b-126">如果使用 MPN Azure AD 租户工作电子邮件登录，则只会看到 MPN 计划信息。</span><span class="sxs-lookup"><span data-stu-id="c725b-126">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> 

<span data-ttu-id="c725b-127">**如果不想将现有的 Office 365 Azure AD 租户用于合作伙伴中心，则可以在从 PMC 迁移之前创建新租户。**</span><span class="sxs-lookup"><span data-stu-id="c725b-127">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="c725b-128">可能有很多原因导致你不想使用现有的 Azure AD 租户来设置合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="c725b-128">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="c725b-129">在开始迁移到合作伙伴中心之前，请先转至 [Azure 门户](https://ms.portal.azure.com/#home)以创建新的 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="c725b-129">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="c725b-130">按照[在 Azure Active Directory 中创建新租户](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)中的指南进行操作。</span><span class="sxs-lookup"><span data-stu-id="c725b-130">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="c725b-131">使用新的 AAD 租户设置合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="c725b-131">Use the new AAD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="c725b-132">只有全局管理员才能创建租户。</span><span class="sxs-lookup"><span data-stu-id="c725b-132">You must be a global admin to create the tenant.</span></span> 


<span data-ttu-id="c725b-133">**用户角色，包括合作伙伴中心中的来宾用户角色**</span><span class="sxs-lookup"><span data-stu-id="c725b-133">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="c725b-134">合作伙伴中心具有不同类型的角色，具体取决于需要完成的工作类型。</span><span class="sxs-lookup"><span data-stu-id="c725b-134">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="c725b-135">有属于 Azure AD 角色的全局管理员等角色。</span><span class="sxs-lookup"><span data-stu-id="c725b-135">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="c725b-136">某些角色特定于云服务提供商计划或奖励等计划，并且有特定于 MPN 的角色。</span><span class="sxs-lookup"><span data-stu-id="c725b-136">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="c725b-137">若要了解所有的合作伙伴中心角色，请参阅[为用户分配角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="c725b-137">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="c725b-138">**当我用户的角色从 PMC 迁移到合作伙伴中心时会发生什么情况？**</span><span class="sxs-lookup"><span data-stu-id="c725b-138">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="c725b-139">除了 MPN 全局管理员或执行迁移的主要计划联系人外，PMC 中的所有用户将失去他们的管理员角色。</span><span class="sxs-lookup"><span data-stu-id="c725b-139">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="c725b-140">完成迁移的个人需要在合作伙伴中心中分配角色。</span><span class="sxs-lookup"><span data-stu-id="c725b-140">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="c725b-141">合作伙伴中心中的角色不同于 PMC 中的角色。</span><span class="sxs-lookup"><span data-stu-id="c725b-141">The roles in Partner Center differ from the roles in PMC.</span></span> <span data-ttu-id="c725b-142">若要详细了解合作伙伴中心中的用户角色，请参阅 [为用户分配角色和权限](permissions-overview.md 以及[从 PMC 迁移到合作伙伴中心](move-pmc-pc-map.md#user-roles)。</span><span class="sxs-lookup"><span data-stu-id="c725b-142">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](move-pmc-pc-map.md#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="c725b-143">**我的公司配置文件和我的业务配置文件之间有什么区别？**</span><span class="sxs-lookup"><span data-stu-id="c725b-143">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="c725b-144">公司配置文件是公司的相关信息，包括地址、位置、主要联系人、银行和税务详细信息。</span><span class="sxs-lookup"><span data-stu-id="c725b-144">Your company profile is the information about your company that includes address, locations, primary contact, bank, and tax details.</span></span>

<span data-ttu-id="c725b-145">你的业务配置文件是你像客户展示自己的方式，并且是显示你的徽标、业务重心的详细信息，以及你的专长等信息的一个营销页面。</span><span class="sxs-lookup"><span data-stu-id="c725b-145">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="c725b-146">**帐户合并对我的帐户而言有什么意义？**</span><span class="sxs-lookup"><span data-stu-id="c725b-146">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="c725b-147">如果你使用相同的 Azure AD 租户将多个 MPN 帐户迁移到合作伙伴中心，系统将自动识别出来并要求你合并帐户。</span><span class="sxs-lookup"><span data-stu-id="c725b-147">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="c725b-148">这也适用于你有多个关联到同一 Azure AD 租户的域。</span><span class="sxs-lookup"><span data-stu-id="c725b-148">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="c725b-149">你仍然可以决定使用单独的 ADD 租户迁移到合作伙伴中心，但请注意，这会导致对你的资格进行单独评估并且会产生额外的购买成本。</span><span class="sxs-lookup"><span data-stu-id="c725b-149">You could still decide to migrate to Partner Center using separate AAD tenants, but note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> <span data-ttu-id="c725b-150">有关帐户合并的详细信息，请参阅[合并公司帐户](consolidate-accounts.md)</span><span class="sxs-lookup"><span data-stu-id="c725b-150">For more information about account consolidation, read [Consolidate your company accounts](consolidate-accounts.md)</span></span>

<span data-ttu-id="c725b-151">**如果我有多个 ADD 租户和一个 MPN 帐户，是否可以在合作伙伴中心中链接它们？**</span><span class="sxs-lookup"><span data-stu-id="c725b-151">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="c725b-152">是的，可以在合作伙伴中心中将多个 Azure AD 租户链接到一个合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="c725b-152">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="c725b-153">有关帐户合并的详细信息，请参阅[合并公司帐户](consolidate-accounts.md)</span><span class="sxs-lookup"><span data-stu-id="c725b-153">For more information about account consolidation, read [Consolidate your company accounts](consolidate-accounts.md)</span></span>

<span data-ttu-id="c725b-154">**将多个 Azure AD 租户添加到一个合作伙伴中心帐户有什么限制吗？**</span><span class="sxs-lookup"><span data-stu-id="c725b-154">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="c725b-155">如果 Azure AD 租户已与一个现有的合作伙伴中心帐户相关联，则不能使用多租户功能将它关联到新的合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="c725b-155">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="c725b-156">另一种思考方向是，一个 Azure AD 租户只能关联到一个合作伙伴中心帐户，但一个合作伙伴中心帐户可以有多个与之关联的租户。</span><span class="sxs-lookup"><span data-stu-id="c725b-156">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="c725b-157">Microsoft 合作伙伴网络 (MPN) 成员资格迁移</span><span class="sxs-lookup"><span data-stu-id="c725b-157">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="c725b-158">**谁可以执行从 PMC 到合作伙伴中心的迁移？**</span><span class="sxs-lookup"><span data-stu-id="c725b-158">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="c725b-159">公司 MPN 全局管理员或主要计划联系人（这两个角色通常由同一人持有）可以发起和执行迁移。</span><span class="sxs-lookup"><span data-stu-id="c725b-159">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="c725b-160">**完成迁移的人员是否会成为合作伙伴中心中公司法定配置文件上的主要联系人？**</span><span class="sxs-lookup"><span data-stu-id="c725b-160">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="c725b-161">不一定，然而，主要联系人需要是有权签署协议的人员。</span><span class="sxs-lookup"><span data-stu-id="c725b-161">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="c725b-162">**Microsoft 能否为我迁移我的 MPN 成员资格？**</span><span class="sxs-lookup"><span data-stu-id="c725b-162">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="c725b-163">不能。</span><span class="sxs-lookup"><span data-stu-id="c725b-163">No.</span></span> <span data-ttu-id="c725b-164">Microsoft 无法帮助你将成员资格帐户移到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="c725b-164">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="c725b-165">你需要使用你的工作帐户（登录凭据）登录 PMC 来迁移你的帐户，以便开始进行迁移。</span><span class="sxs-lookup"><span data-stu-id="c725b-165">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="c725b-166">完成迁移帐户的步骤后，可以开始管理你的成员资格并向你的团队分配用户角色和权限，使他们可以访问权益并帮助管理成员资格。</span><span class="sxs-lookup"><span data-stu-id="c725b-166">After you've completed the steps to move your account, you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> 

<span data-ttu-id="c725b-167">Microsoft 将自动迁移当前的资格、权益、位置信息、用于奖励的银行/税务信息，以及 MCP 关联，包括 Partner University 访问权限。</span><span class="sxs-lookup"><span data-stu-id="c725b-167">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="c725b-168">**续订策略会如何变化？**</span><span class="sxs-lookup"><span data-stu-id="c725b-168">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="c725b-169">在合作伙伴中心，续订时段自你的周年日期起到接下来的 30 天内。</span><span class="sxs-lookup"><span data-stu-id="c725b-169">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="c725b-170">**在迁移到合作伙伴中心后，我们的资格是否保持不变？**</span><span class="sxs-lookup"><span data-stu-id="c725b-170">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="c725b-171">是的，资格不会受迁移到合作伙伴中心的影响。</span><span class="sxs-lookup"><span data-stu-id="c725b-171">Yes, competencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="c725b-172">如果出现不相符的情况，请联系[支持部门](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="c725b-172">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="c725b-173">**我的权益（包括云权益、技术支持、软件权益、Visual Studio）是否会在迁移后更改？**</span><span class="sxs-lookup"><span data-stu-id="c725b-173">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="c725b-174">你符合使用资格的权益将不会更改。</span><span class="sxs-lookup"><span data-stu-id="c725b-174">Your eligible benefits will not change.</span></span> <span data-ttu-id="c725b-175">如果出现不相符的情况，请联系[支持部门](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="c725b-175">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="c725b-176">**我们的 Microsoft 帐户是否会享有已有的 Visual Studio 权益分配？**</span><span class="sxs-lookup"><span data-stu-id="c725b-176">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="c725b-177">是的。</span><span class="sxs-lookup"><span data-stu-id="c725b-177">Yes.</span></span> <span data-ttu-id="c725b-178">分配给 MSA 的 Visual Studio 权益仍将有效，会继续保留。</span><span class="sxs-lookup"><span data-stu-id="c725b-178">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="c725b-179">在合作伙伴中心续订后，仍会保留它们。</span><span class="sxs-lookup"><span data-stu-id="c725b-179">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="c725b-180">不过，如果你在迁移到合作伙伴中心以后删除了某个 MSA 分配，则不能将它重新添加到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="c725b-180">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="c725b-181">在合作伙伴中心，合作伙伴可以添加特定的工作帐户和来宾用户帐户，这些帐户是同一租户的 MSA，而这些租户中的合作伙伴在 Azure AD 租户中是 MPN 管理员。</span><span class="sxs-lookup"><span data-stu-id="c725b-181">In Partner Center, a partner can add work accounts and guest user accounts, which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="c725b-182">如果合作伙伴在多个 Azure AD 租户中是全局管理员，并且所有这些租户都关联到同一个合作伙伴中心帐户，则该合作伙伴可以跨所有这些租户将用户添加到 Visual Studio 权益中以及基于 Azure 使用情况的分配计划中。</span><span class="sxs-lookup"><span data-stu-id="c725b-182">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="c725b-183">虽然来宾用户可以由 MPN 管理员或全局管理员分配基于使用情况的 Visual Studio 订阅，但来宾用户不能使用其 MSA 登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="c725b-183">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="c725b-184">不过，来宾用户可以登录 Azure 和 Visual Studio，以便验证和使用分配给他们的权益。</span><span class="sxs-lookup"><span data-stu-id="c725b-184">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="c725b-185">**我们应如何管理 MCP 关联和 Partner University 访问权限？**</span><span class="sxs-lookup"><span data-stu-id="c725b-185">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="c725b-186">从 PMC 迁移的 MCP 关联不会有什么更改。</span><span class="sxs-lookup"><span data-stu-id="c725b-186">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="c725b-187">然而，需要在合作伙伴中心将迁移到合作伙伴中心后的任何新员工进行关联。</span><span class="sxs-lookup"><span data-stu-id="c725b-187">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="c725b-188">你所有针对现有用户的 Partner University 权限将保留，不过，任何新员工都应该访问[培训中心](https://partner.microsoft.com/training)获取有关如何获取对 Partner University 的访问权限的信息。</span><span class="sxs-lookup"><span data-stu-id="c725b-188">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="c725b-189">**迁移到合作伙伴中心后如何查看 MCP 信息？**</span><span class="sxs-lookup"><span data-stu-id="c725b-189">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="c725b-190">在面板的左侧导航栏中选择“资格”。</span><span class="sxs-lookup"><span data-stu-id="c725b-190">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="c725b-191">在“资格”页面中，你可以下载技能报告。</span><span class="sxs-lookup"><span data-stu-id="c725b-191">From the **Competencies** page, you are able to download the skills report.</span></span> <span data-ttu-id="c725b-192">技能报告将列出合作伙伴中心中已获得了与资格相关的技能以及计划的用户。</span><span class="sxs-lookup"><span data-stu-id="c725b-192">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="c725b-193">如果你的用户获得了技能，但这些技能与你所围绕展开工作的资格无关，这些用户则不会在报告中列出。</span><span class="sxs-lookup"><span data-stu-id="c725b-193">If your users have gained skills but those skills are not relevant to the competencies you're working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="c725b-194">**合作伙伴中心中是否使用了客户证明？**</span><span class="sxs-lookup"><span data-stu-id="c725b-194">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="c725b-195">否，无需客户证明即可满足合作伙伴中心的资格要求。</span><span class="sxs-lookup"><span data-stu-id="c725b-195">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="c725b-196">**记录合作伙伴关联是否将迁移到合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="c725b-196">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="c725b-197">是的，记录合作伙伴不会有任何更改。</span><span class="sxs-lookup"><span data-stu-id="c725b-197">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="c725b-198">了解[将合作伙伴 ID 链接到客户](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c725b-198">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="c725b-199">**奖励计划是否会因迁移到合作伙伴中心而受到影响？**</span><span class="sxs-lookup"><span data-stu-id="c725b-199">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="c725b-200">不会，如果你迁移了帐户但没有合并位置，奖励计划则不会受到任何影响。</span><span class="sxs-lookup"><span data-stu-id="c725b-200">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="c725b-201">如果你的企业在 PMC 中有多个帐户，但你迁移到合作伙伴中心并决定合并到一个全局帐户时，不会对奖励造成任何损失，不过可能会稻城奖励付款出现延迟的情况。</span><span class="sxs-lookup"><span data-stu-id="c725b-201">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="c725b-202">如果不迁移所有涉及到奖励计划的 PMC 帐户，你可能会停止获得与这些帐户相绑定的奖励。</span><span class="sxs-lookup"><span data-stu-id="c725b-202">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="c725b-203">**合作伙伴中心中的奖励角色是什么？**</span><span class="sxs-lookup"><span data-stu-id="c725b-203">**What are the incentive roles in Partner Center?**</span></span> 

<span data-ttu-id="c725b-204">合作伙伴中心中的奖励用户是基于位置的角色，并且包含奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="c725b-204">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="c725b-205">有关这些角色可以执行的操作的详细信息，请参阅[为用户分配角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="c725b-205">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="c725b-206">**是否可以在全局和位置级别分配奖励管理员？**</span><span class="sxs-lookup"><span data-stu-id="c725b-206">**Can incentives admins be assigned at the global and location level?**</span></span>

 <span data-ttu-id="c725b-207">是的。</span><span class="sxs-lookup"><span data-stu-id="c725b-207">Yes.</span></span> <span data-ttu-id="c725b-208">你可以将奖励管理员分配为所有位置的奖励管理员，或者每一位置可以有自己的奖励管理员。</span><span class="sxs-lookup"><span data-stu-id="c725b-208">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="c725b-209">**奖励是否可以在全局或本地级别支付？**</span><span class="sxs-lookup"><span data-stu-id="c725b-209">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="c725b-210">奖励仅在位置级别支付。</span><span class="sxs-lookup"><span data-stu-id="c725b-210">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="c725b-211">**就引荐而言，我们可以创建多少个业务配置文件？**</span><span class="sxs-lookup"><span data-stu-id="c725b-211">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="c725b-212">你的公司可以按需创建任意数量的业务配置文件，以完全代表你公司的兴趣。</span><span class="sxs-lookup"><span data-stu-id="c725b-212">Your company can create as many business profiles as you need to fully represent your company's interests.</span></span> <span data-ttu-id="c725b-213">在每一业务配置文件中，你可以列出多达五个位置，每国家/地区一个位置。</span><span class="sxs-lookup"><span data-stu-id="c725b-213">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="c725b-214">每一业务配置文件都可以接收每一相关位置的引荐。</span><span class="sxs-lookup"><span data-stu-id="c725b-214">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="c725b-215">**引荐将如何分配，会出现什么更改？例如，如果我在某一市场中有一个全球公司并且在其他市场中有多个位置，引荐将如何分配？**</span><span class="sxs-lookup"><span data-stu-id="c725b-215">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="c725b-216">引荐是根据客户定义的搜索参数分配的。</span><span class="sxs-lookup"><span data-stu-id="c725b-216">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="c725b-217">无论你有一个还是多个位置，如果客户定义了一个所需位置并且你在此位置有满足其他参数的业务，那么引荐则将转至此位置。</span><span class="sxs-lookup"><span data-stu-id="c725b-217">Regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








