---
title: 无法登录到合作伙伴中心
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 排查可能的原因，并了解无法登录合作伙伴中心的解决方案 - 详细了解重置密码、检查角色和检查凭据。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818790"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="1a441-103">排查登录问题合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1a441-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="1a441-104">**适当的角色**：对角色感兴趣的所有合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1a441-104">**Appropriate roles**: All partners interested in Partner Center</span></span>

<span data-ttu-id="1a441-105">本文包含适用于用户登录的常见登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="1a441-105">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="1a441-106">你忘记了密码合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1a441-106">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="1a441-107">如果忘记了密码，并且无法登录到合作伙伴中心，请联系支持人员。</span><span class="sxs-lookup"><span data-stu-id="1a441-107">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="1a441-108">在"业务产品支持 ["中查找相应的联系人](/microsoft-365/admin/contact-support-for-business-products)。</span><span class="sxs-lookup"><span data-stu-id="1a441-108">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="1a441-109">如果你是 MPN 合作伙伴，请让全局管理员创建一个新密码。</span><span class="sxs-lookup"><span data-stu-id="1a441-109">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="1a441-110">如果你是 CSP 间接经销商，请要求间接提供商在 Azure AD 租户上创建新的全局管理员，或者使用其委派的管理员权限创建新的密码。</span><span class="sxs-lookup"><span data-stu-id="1a441-110">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="1a441-111">若要详细了解如何重置密码并重新获得对工作帐户的访问权限，请阅读使用安全信息重置工作或 [学校密码](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)。</span><span class="sxs-lookup"><span data-stu-id="1a441-111">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="1a441-112">无法查看或管理中预期的页面或合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1a441-112">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="1a441-113">对 合作伙伴中心 页的访问权限由你分配的角色控制。</span><span class="sxs-lookup"><span data-stu-id="1a441-113">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="1a441-114">若要检查已分配的角色，请在"设置"合作伙伴中心选择"设置"图标，选择"帐户设置"，然后在"帐户设置"中选择"用户 **管理"。**</span><span class="sxs-lookup"><span data-stu-id="1a441-114">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="1a441-115">在"搜索"中，键入你的姓名，然后查看结果。</span><span class="sxs-lookup"><span data-stu-id="1a441-115">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="1a441-116">如果无法查看或管理你期望的能力、客户、奖励或用户，请尝试以下解决方案：</span><span class="sxs-lookup"><span data-stu-id="1a441-116">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="1a441-117">若要访问 MPN、CSP 和引荐的功能，请联系全局管理员或帐户管理员。若要详细了解角色及其在 合作伙伴中心 中启用的任务，请参阅将& [角色分配给用户](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="1a441-117">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="1a441-118">若要访问商业市场和 Windows & Xbox、Office 应用商店、Microsoft Edge 和硬件开发人员计划的功能，请与组织中的 "所有者" 或 "经理" 角色联系。</span><span class="sxs-lookup"><span data-stu-id="1a441-118">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="1a441-119">若要了解有关角色和权限的详细信息，请参阅 [如何在 Microsoft 合作伙伴中心管理商业 marketplace 帐户](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)。</span><span class="sxs-lookup"><span data-stu-id="1a441-119">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="1a441-120">你无法在合作伙伴中心看到你的产品/服务或权益</span><span class="sxs-lookup"><span data-stu-id="1a441-120">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="1a441-121">确认使用正确的凭据进行登录。</span><span class="sxs-lookup"><span data-stu-id="1a441-121">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="1a441-122">例如，您的工作帐户和个人帐户可能看起来像是相同的 (abc@contoso.com ，如) ，而另一个帐户可能是您创建的个人帐户，而另一个帐户可能是代表您设置的企业帐户。</span><span class="sxs-lookup"><span data-stu-id="1a441-122">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="1a441-123">在这种情况下，如果你已登录，但无法查看与 MPN、CSP 和商用 Marketplace 相关的预期功能，请尝试选择你的工作帐户。</span><span class="sxs-lookup"><span data-stu-id="1a441-123">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a441-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="1a441-124">Next steps</span></span>

- [<span data-ttu-id="1a441-125">验证帐户信息</span><span class="sxs-lookup"><span data-stu-id="1a441-125">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="1a441-126">重置我的密码</span><span class="sxs-lookup"><span data-stu-id="1a441-126">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="1a441-127">重置用户密码</span><span class="sxs-lookup"><span data-stu-id="1a441-127">Reset a user password</span></span>](reset-a-user-password.md)