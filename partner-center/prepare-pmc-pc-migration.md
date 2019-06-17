---
title: 准备从 Partner Membership Center 将移动到合作伙伴中心 |合作伙伴中心
ms.topic: article
ms.date: 06/13/2019
description: 将你的业务从 PMC 移到合作伙伴中心之前需要考虑的事项
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 16c29bdccd4c4853fcc28ed4f2752270415449b1
ms.sourcegitcommit: 8305d8d1da404d75ce3120085724fe67da733eec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "67145348"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="34415-103">准备移动从伙伴成员身份 Center (PMC) 到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="34415-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="34415-104">我们要将成员身份管理从伙伴成员身份 Center (PMC) 移动到合作伙伴中心 – 管理与 Microsoft 的业务关系的单个目标。</span><span class="sxs-lookup"><span data-stu-id="34415-104">We are moving membership management from Partner Membership Center (PMC) to the partner center – the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="34415-105">我们希望您迁移到合作伙伴中心要为高效、 尽可能容易。</span><span class="sxs-lookup"><span data-stu-id="34415-105">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="34415-106">我们发现某些区域，其中合作伙伴中心不同于 PMC 中，我们认为你会想要了解并在进行迁移之前为其做准备。</span><span class="sxs-lookup"><span data-stu-id="34415-106">We’ve identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="34415-107">帐户和标识的安装程序</span><span class="sxs-lookup"><span data-stu-id="34415-107">Account and identity setup</span></span>

<span data-ttu-id="34415-108">**什么是 Azure Active Directory (Azure AD) 工作帐户？**</span><span class="sxs-lookup"><span data-stu-id="34415-108">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="34415-109">Azure 工作帐户是你的公司在 Azure 公共云中的专用独立虚拟表示形式，并且是在你订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时为你创建的。</span><span class="sxs-lookup"><span data-stu-id="34415-109">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="34415-110">你的工作帐户托管你的 Azure AD 用户和有关它们的其电子邮件、 密码、 配置文件数据、 权限和等等的信息。</span><span class="sxs-lookup"><span data-stu-id="34415-110">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="34415-111">工作帐户还包含组、 应用程序，以及与公司和其安全性相关的其他信息。</span><span class="sxs-lookup"><span data-stu-id="34415-111">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> <span data-ttu-id="34415-112">有关详细信息请参阅...</span><span class="sxs-lookup"><span data-stu-id="34415-112">For more information see …</span></span>

<span data-ttu-id="34415-113">在合作伙伴中心将使用工作电子邮件登录到你的帐户不是你个人的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="34415-113">In the Partner Center you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="34415-114">你的工作帐户： john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="34415-114">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="34415-115">您的个人帐户： John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="34415-115">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="34415-116">工作电子邮件是你的 Azure active directory 租户的一部分。</span><span class="sxs-lookup"><span data-stu-id="34415-116">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="34415-117">若要在合作伙伴中心有一个帐户，需要具有 AAD 租户。</span><span class="sxs-lookup"><span data-stu-id="34415-117">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="34415-118">Azure Active Directory 的详细信息，请阅读[在 Azure AD 中创建你的目录](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。</span><span class="sxs-lookup"><span data-stu-id="34415-118">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="34415-119">**移动时到合作伙伴中心从 PMC，哪些帐户应登录到合作伙伴中心如果您具有与 Microsoft （的示例中的 Office 365) 以及你的 AAD 租户还拥有的租户 CSP 业务？**</span><span class="sxs-lookup"><span data-stu-id="34415-119">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="34415-120">你可以使用 CSP 帐户或你的 MPN 工作电子邮件帐户登录到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="34415-120">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="34415-121">如果选择使用 CSP 工作电子邮件地址进行登录，在仪表板上的左侧导航栏将显示 MPN 和 CSP 程序信息。</span><span class="sxs-lookup"><span data-stu-id="34415-121">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="34415-122">如果你使用你的 MPN Azure AD 租户的工作电子邮件登录，将看到仅你的 MPN 计划信息。</span><span class="sxs-lookup"><span data-stu-id="34415-122">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="34415-123">用户角色 MPN 和 CSP 之间有所不同，因此如果于 MPN 和 CSP 的企业使用相同的帐户，请确保相应地分配用户角色。</span><span class="sxs-lookup"><span data-stu-id="34415-123">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="34415-124">用户角色的信息，请阅读[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="34415-124">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="34415-125">**AAD 全局管理员角色和 PMC MPN 全局管理员角色之间的区别是什么？**</span><span class="sxs-lookup"><span data-stu-id="34415-125">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="34415-126">这些是两个完全不同角色使用不同的权限。</span><span class="sxs-lookup"><span data-stu-id="34415-126">These are two completely different roles with different permissions.</span></span> <span data-ttu-id="34415-127">在合作伙伴中心中的 AAD 租户全局管理员管理租户-添加或删除用户、 提供和管理密码、 角色和权限，并在合作伙伴中心有权访问其公司的所有程序。</span><span class="sxs-lookup"><span data-stu-id="34415-127">The AAD tenant global admin in Partner Center administers the tenant – adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company’s programs in Partner Center.</span></span> 

<span data-ttu-id="34415-128">在 PMC 中的 MPN 全局管理员角色可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="34415-128">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="34415-129">查看和编辑与公司和所有公司的位置相关联的所有数据</span><span class="sxs-lookup"><span data-stu-id="34415-129">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="34415-130">在全局或本地级别添加管理员。</span><span class="sxs-lookup"><span data-stu-id="34415-130">Add administrators at the global or local level.</span></span>  <span data-ttu-id="34415-131">此外，全局管理员可以分配全局管理员访问权限，这意味着无论哪个位置与其相关的全局访问任何位置的任何人。</span><span class="sxs-lookup"><span data-stu-id="34415-131">Also, Global admins can assign any person at any location Global Administrator Access which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="34415-132">执行任何合作伙伴面向 UI 函数包括：</span><span class="sxs-lookup"><span data-stu-id="34415-132">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="34415-133">添加/删除用户</span><span class="sxs-lookup"><span data-stu-id="34415-133">Add/remove users</span></span>

 - <span data-ttu-id="34415-134">分配/删除角色</span><span class="sxs-lookup"><span data-stu-id="34415-134">Assign/remove roles</span></span> 

 - <span data-ttu-id="34415-135">添加/删除/更新位置</span><span class="sxs-lookup"><span data-stu-id="34415-135">Add/remove/update locations</span></span> 

 - <span data-ttu-id="34415-136">购买资格/映射</span><span class="sxs-lookup"><span data-stu-id="34415-136">Purchase competency/maps</span></span> 

-  <span data-ttu-id="34415-137">查看福利</span><span class="sxs-lookup"><span data-stu-id="34415-137">View benefits</span></span>

<span data-ttu-id="34415-138">当 MPN 全局管理员移动到合作伙伴中心角色被名为 MPN 合作伙伴管理员的具有不同的权限和任务比合作伙伴中心全局管理员。有关角色和合作伙伴中心中的权限的详细信息，请阅读[分配用户角色和权限](permissions-overview.md)</span><span class="sxs-lookup"><span data-stu-id="34415-138">When the MPN global admin moves to Partner Center the role is called the MPN partner admin which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md)</span></span>

<span data-ttu-id="34415-139">**合作伙伴中心中的用户角色**</span><span class="sxs-lookup"><span data-stu-id="34415-139">**User roles in Partner Center**</span></span>

<span data-ttu-id="34415-140">合作伙伴中心具有不同类型的角色根据工作需要完成的工作的类型。</span><span class="sxs-lookup"><span data-stu-id="34415-140">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="34415-141">有了 Azure AD 角色如全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="34415-141">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="34415-142">某些角色是特定的程序，例如云服务提供商计划或奖励，并且有特定于 MPN 的角色。</span><span class="sxs-lookup"><span data-stu-id="34415-142">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="34415-143">若要找出所有合作伙伴中心角色，请阅读[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="34415-143">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="34415-144">**会发生什么情况到我的用户角色时从 PMC 移到合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="34415-144">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="34415-145">除外的 MPN 全局管理员或主计划联系人，负责执行迁移，在 PMC 中的所有用户将都失去其管理员角色。</span><span class="sxs-lookup"><span data-stu-id="34415-145">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="34415-146">将需要在合作伙伴中心中分配角色的用户完成迁移。</span><span class="sxs-lookup"><span data-stu-id="34415-146">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="34415-147">合作伙伴中心中的角色不同于在 PMC 中。</span><span class="sxs-lookup"><span data-stu-id="34415-147">The roles in Partner Center differ from those in PMC.</span></span> <span data-ttu-id="34415-148">读取[分配用户角色和权限](permissions-overview)并[将从 PMC 移动到合作伙伴中心](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles)有关用户角色的详细信息在合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="34415-148">Read [Assign users roles and permissions](permissions-overview) and [Moving from PMC to Partner Center](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="34415-149">**我公司的个人资料和我的业务配置文件之间的区别是什么？**</span><span class="sxs-lookup"><span data-stu-id="34415-149">**What’s the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="34415-150">你公司的配置文件是你的公司，包括地址、 位置、 主要联系人、 银行和税务详细信息有关的信息。</span><span class="sxs-lookup"><span data-stu-id="34415-150">Your company profile is the information about your company that includes address, locations, primary contact, bank and tax details.</span></span>

<span data-ttu-id="34415-151">业务配置文件是如何向客户提供你自己，显示你的徽标，业务焦点、 你的专业知识等的详细信息的市场营销页。</span><span class="sxs-lookup"><span data-stu-id="34415-151">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="34415-152">**没有为我的帐户合并平均值的帐户？**</span><span class="sxs-lookup"><span data-stu-id="34415-152">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="34415-153">如果使用相同的 Azure AD 租户可以将多个 MPN 帐户迁移到合作伙伴中心，系统将自动识别，并询问您可以将合并你的帐户。</span><span class="sxs-lookup"><span data-stu-id="34415-153">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="34415-154">即使有多个域与同一个 Azure AD 租户相关联，这是如此。</span><span class="sxs-lookup"><span data-stu-id="34415-154">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="34415-155">您可以仍决定将迁移到合作伙伴中心使用单独的 AAD 租户，但请注意此结果在独立评估你的能力和额外购买成本。</span><span class="sxs-lookup"><span data-stu-id="34415-155">You could still decide to migrate to Partner Center using separate AAD tenants, but please note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="34415-156">**如果我有多个 AAD 租户和单个的 MPN 帐户，则可以将它们链接在合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="34415-156">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="34415-157">是的在合作伙伴中心可以指向单个合作伙伴中心帐户链接多个 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="34415-157">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="34415-158">此处了解详情。</span><span class="sxs-lookup"><span data-stu-id="34415-158">Learn more here.</span></span> 


## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="34415-159">Microsoft 合作伙伴网络 (MPN) 成员身份迁移</span><span class="sxs-lookup"><span data-stu-id="34415-159">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="34415-160">**谁可以执行移动到合作伙伴中心从 PMC？**</span><span class="sxs-lookup"><span data-stu-id="34415-160">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="34415-161">公司 MPN 全局系统管理员或主程序联系人 （通常由同一个人持有这两个角色） 可以启动并执行移动。</span><span class="sxs-lookup"><span data-stu-id="34415-161">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="34415-162">**完成迁移的人员将成为在合作伙伴中心中的公司法律配置文件的主要联系人？**</span><span class="sxs-lookup"><span data-stu-id="34415-162">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="34415-163">不一定，但是，主要联系人必须是具有签署协议的授权的人员。</span><span class="sxs-lookup"><span data-stu-id="34415-163">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="34415-164">**可以在 Microsoft 为我迁移我的 MPN 成员身份？**</span><span class="sxs-lookup"><span data-stu-id="34415-164">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="34415-165">否。</span><span class="sxs-lookup"><span data-stu-id="34415-165">No.</span></span> <span data-ttu-id="34415-166">Microsoft 无法帮助你将成员资格帐户移动到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="34415-166">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="34415-167">您需要通过登录到 PMC 使用工作帐户 （登录凭据） 若要开始迁移过程中移动你的帐户。</span><span class="sxs-lookup"><span data-stu-id="34415-167">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="34415-168">完成移动帐户的步骤后可以开始管理您的成员身份，并将用户角色和权限分配给你的团队，以便他们可以访问的权益并帮助管理的成员身份。</span><span class="sxs-lookup"><span data-stu-id="34415-168">After you’ve completed the steps to move your account you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="34415-169">当前的能力、 优点、 位置信息、 奖励和包括合作伙伴大学的访问权限的 MCP 关联银行/税务信息，Microsoft 会自动将迁移。</span><span class="sxs-lookup"><span data-stu-id="34415-169">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="34415-170">当前的能力、 优点、 位置信息、 奖励和包括合作伙伴大学的访问权限的 MCP 关联银行/税务信息，Microsoft 会自动将迁移。</span><span class="sxs-lookup"><span data-stu-id="34415-170">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="34415-171">**续订策略有何更改？**</span><span class="sxs-lookup"><span data-stu-id="34415-171">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="34415-172">在合作伙伴中心，在续订窗口是从你在以下的 30 天内通过的周年日。</span><span class="sxs-lookup"><span data-stu-id="34415-172">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="34415-173">**将我们的能力保持不变后我们将移到合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="34415-173">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="34415-174">是的称职情况不会受移动到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="34415-174">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="34415-175">如果您注意到差异，请联系[支持](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="34415-175">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="34415-176">**将我们移动后更改我的权益 （包括云优势、 技术支持、 软件权益，Visual Studio）？**</span><span class="sxs-lookup"><span data-stu-id="34415-176">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="34415-177">您有资格的权益不会更改。</span><span class="sxs-lookup"><span data-stu-id="34415-177">Your eligible benefits will not change.</span></span> <span data-ttu-id="34415-178">如果您注意到差异，请联系[支持](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="34415-178">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="34415-179">**将遵循我们提供 Visual Studio 权益分配的 Microsoft 帐户？**</span><span class="sxs-lookup"><span data-stu-id="34415-179">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>

 <span data-ttu-id="34415-180">是。</span><span class="sxs-lookup"><span data-stu-id="34415-180">Yes.</span></span> <span data-ttu-id="34415-181">将遵循 Wisual Studio 权益分配给采用的是 MSAs，并将其保留。</span><span class="sxs-lookup"><span data-stu-id="34415-181">Wisual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="34415-182">它们还将保留在合作伙伴中心续订后。</span><span class="sxs-lookup"><span data-stu-id="34415-182">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="34415-183">但是，如果您删除 MSA 分配一次迁移在合作伙伴中心，它不能添加回合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="34415-183">However, if you remove an MSA allocation once migrated in Partner Center, it can’t be added  back into Partner Center.</span></span>

<span data-ttu-id="34415-184">只有 MPN 管理员可以添加 Visual Studio 权益分配公司 Azure AD 租户中的工作帐户。</span><span class="sxs-lookup"><span data-stu-id="34415-184">Only the MPN admin can add Visual Studio benefit allocations to work accounts in the company Azure AD tenant.</span></span>

<span data-ttu-id="34415-185">关联到相同的合作伙伴中心帐户，所有租户时的多个 AAD 租户的全局管理员可以在所有这些租户添加用户到 Visual Studio 权益和 Azure 的基于使用情况的分配。</span><span class="sxs-lookup"><span data-stu-id="34415-185">The global admin for multiple AAD tenants when all tenants are associated to the same Partner Center account, can add users across all these tenants into Visual Studio benefits and Azure usage-based allocations.</span></span> 

 <span data-ttu-id="34415-186">**我们如何应管理我们 MCP 关联和我们合作伙伴大学访问？**</span><span class="sxs-lookup"><span data-stu-id="34415-186">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="34415-187">没有从 PMC 移动的 MCP 关联到的更改。</span><span class="sxs-lookup"><span data-stu-id="34415-187">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="34415-188">但是，任何新的新员工移动到合作伙伴中心后将需要在合作伙伴中心关联。</span><span class="sxs-lookup"><span data-stu-id="34415-188">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="34415-189">为现有用户的所有合作伙伴大学权限将都保留，但任何新员工应转到[培训 center](https://partner.microsoft.com/training)有关如何获取到合作伙伴大学的访问权限的信息。</span><span class="sxs-lookup"><span data-stu-id="34415-189">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="34415-190">**在合作伙伴中心中使用的客户引用？**</span><span class="sxs-lookup"><span data-stu-id="34415-190">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="34415-191">不，不需要客户引用，以满足在合作伙伴中心的资格要求。</span><span class="sxs-lookup"><span data-stu-id="34415-191">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="34415-192">**记录合作伙伴关联会将移动到合作伙伴中心？**</span><span class="sxs-lookup"><span data-stu-id="34415-192">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="34415-193">不是的对合作伙伴的记录进行任何更改。</span><span class="sxs-lookup"><span data-stu-id="34415-193">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="34415-194">详细了解如何[将你的合作伙伴 ID 链接到你的客户](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="34415-194">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="34415-195">**是否有激励的影响？**</span><span class="sxs-lookup"><span data-stu-id="34415-195">**Is there an impact to incentives?**</span></span>

<span data-ttu-id="34415-196">不存在不会影响到奖励。</span><span class="sxs-lookup"><span data-stu-id="34415-196">No there is no impact to incentives.</span></span> <span data-ttu-id="34415-197">此外，如果您的公司在 PMC 中有多个帐户，并且这些帐户移动到合作伙伴中心时都合并到全局帐户，不会对基于记录的奖励的合作伙伴没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="34415-197">Also, if your business has multiple accounts in PMC and, when you move to Partner Center those accounts are consolidated into a global account, there is no impact to the partner of record-based incentives.</span></span>

<span data-ttu-id="34415-198">**在合作伙伴中心的激励用户角色有哪些？**</span><span class="sxs-lookup"><span data-stu-id="34415-198">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="34415-199">在合作伙伴中心激励角色是基于位置的并包含奖励管理员和激励用户。</span><span class="sxs-lookup"><span data-stu-id="34415-199">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="34415-200">有关这些角色可以执行的操作的详细信息，请参阅[分配用户角色和权限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="34415-200">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="34415-201">**可以在全局和位置级别管理奖励**</span><span class="sxs-lookup"><span data-stu-id="34415-201">**Can incentives be managed at the global and location level?**</span></span>

 <span data-ttu-id="34415-202">是。</span><span class="sxs-lookup"><span data-stu-id="34415-202">Yes.</span></span> <span data-ttu-id="34415-203">可以分配奖励管理员，作为所有位置的奖励管理员或每个位置可以有其自己的激励管理员。</span><span class="sxs-lookup"><span data-stu-id="34415-203">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

<span data-ttu-id="34415-204">**有关引用，多少业务配置文件可以我们创建？**</span><span class="sxs-lookup"><span data-stu-id="34415-204">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="34415-205">因为你需要为许多业务配置文件完全代表公司的兴趣，可以创建你的公司。</span><span class="sxs-lookup"><span data-stu-id="34415-205">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="34415-206">在每个业务配置文件中，可以列出最多五个不同位置，每个国家/地区的一个位置。</span><span class="sxs-lookup"><span data-stu-id="34415-206">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="34415-207">每个业务配置文件可以接收有关每个其位置的引用。</span><span class="sxs-lookup"><span data-stu-id="34415-207">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="34415-208">**如何将引用分配，可以预期哪些更改？例如，如果我有其他市场中的一家全球性公司在一个市场和位置，如何将引用分配？**</span><span class="sxs-lookup"><span data-stu-id="34415-208">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="34415-209">基于客户定义的搜索参数分配引用。</span><span class="sxs-lookup"><span data-stu-id="34415-209">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="34415-210">因此无论是否有一个位置或许多人来说，如果客户指定所需的位置，并且你有那里的企业满足其他参数，则引用将转到该位置。</span><span class="sxs-lookup"><span data-stu-id="34415-210">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








