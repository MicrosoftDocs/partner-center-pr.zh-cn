---
title: 向用户分配角色和权限
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解哪些角色最适合你所在公司的用户，这些用户在合作伙伴中心管理商业交易、引荐、奖励或 MPN 成员资格。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 964c0e6be3003c2b3c9da8828d6e896e2fff82f9
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756462"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="c683c-103">为需要在合作伙伴中心工作的公司的用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="c683c-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="c683c-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="c683c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c683c-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-105">Global admin</span></span>
- <span data-ttu-id="c683c-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-106">User admin</span></span>
- <span data-ttu-id="c683c-107">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-107">MPN partner admin</span></span>

<span data-ttu-id="c683c-108">你已设置合作伙伴档案，包括法定名称和地址、支持详细信息、税务豁免、银行信息和公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="c683c-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c683c-109">下一步：为用户设置密码和角色，使他们能够在合作伙伴中心开始与你合作。</span><span class="sxs-lookup"><span data-stu-id="c683c-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c683c-110">进行设置，使员工能够在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="c683c-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c683c-111">按分配的角色和权限确定用户对合作伙伴中心拥有访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="c683c-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c683c-112">角色与企业参与的计划相关。</span><span class="sxs-lookup"><span data-stu-id="c683c-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c683c-113">例如，如果你的企业是云解决方案提供商 (CSP)，则你只具有标准的 Azure Active Directory 租户管理角色（例如全局管理员），但却需要 CSP 计划特定的角色。</span><span class="sxs-lookup"><span data-stu-id="c683c-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c683c-114">每个计划都有自身特定的角色。</span><span class="sxs-lookup"><span data-stu-id="c683c-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c683c-115">Azure Active Directory 租户角色包括全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="c683c-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c683c-116">非 Azure Active Directory 角色是指不管理租户的角色，包括 MPN 管理员、企业档案管理员、引荐管理员、奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="c683c-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c683c-117">在合作伙伴中心管理商业交易（Azure AD 和 CSP 角色）</span><span class="sxs-lookup"><span data-stu-id="c683c-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c683c-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="c683c-118">**Role**</span></span>|<span data-ttu-id="c683c-119">**他们可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-119">**What they can do**</span></span>|<span data-ttu-id="c683c-120">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="c683c-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="c683c-121">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-121">Global admin</span></span>|<span data-ttu-id="c683c-122">\*    可以全权访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="c683c-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="c683c-123">管理合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="c683c-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="c683c-124">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-125">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="c683c-126">\*    查看协议、价目表和套餐</span><span class="sxs-lookup"><span data-stu-id="c683c-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c683c-127">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="c683c-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="c683c-128">查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="c683c-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="c683c-129">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-129">User management admin</span></span>   | <span data-ttu-id="c683c-130">\*    查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="c683c-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="c683c-131">在合作伙伴中心管理 Microsoft 合作伙伴网络成员资格权益和优惠</span><span class="sxs-lookup"><span data-stu-id="c683c-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="c683c-132">\*    查看所有合作伙伴档案</span><span class="sxs-lookup"><span data-stu-id="c683c-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="c683c-133">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-134">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="c683c-135">计费管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-135">Billing admin</span></span> | <span data-ttu-id="c683c-136">- 查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="c683c-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="c683c-137">阅读账单</span><span class="sxs-lookup"><span data-stu-id="c683c-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="c683c-138">\*    查看定价</span><span class="sxs-lookup"><span data-stu-id="c683c-138">\*    View pricing</span></span>
||<span data-ttu-id="c683c-139">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-140">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="c683c-141">默认用户</span><span class="sxs-lookup"><span data-stu-id="c683c-141">Default user</span></span>|  <span data-ttu-id="c683c-142">查看“我的个人资料”</span><span class="sxs-lookup"><span data-stu-id="c683c-142">View My profile</span></span>   |[<span data-ttu-id="c683c-143">重置密码</span><span class="sxs-lookup"><span data-stu-id="c683c-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="c683c-144">管理员代理</span><span class="sxs-lookup"><span data-stu-id="c683c-144">Admin agent</span></span> | <span data-ttu-id="c683c-145">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="c683c-145">\*    Customer management</span></span>|[<span data-ttu-id="c683c-146">与客户联系</span><span class="sxs-lookup"><span data-stu-id="c683c-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="c683c-147">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="c683c-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="c683c-148">\*    创建配置文件并将其应用到设备</span><span class="sxs-lookup"><span data-stu-id="c683c-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="c683c-149">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="c683c-149">\*    Subscription management</span></span>
||<span data-ttu-id="c683c-150">\*    客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="c683c-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="c683c-151">\*    请求委派管理员特权</span><span class="sxs-lookup"><span data-stu-id="c683c-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="c683c-152">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="c683c-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="c683c-153">\*    计费</span><span class="sxs-lookup"><span data-stu-id="c683c-153">\*    Billing</span></span>
||<span data-ttu-id="c683c-154">\*    代表客户的管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="c683c-155">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="c683c-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="c683c-156">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-157">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="c683c-158">销售代理</span><span class="sxs-lookup"><span data-stu-id="c683c-158">Sales agent</span></span> | <span data-ttu-id="c683c-159">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="c683c-159">\*    Customer management</span></span>|[<span data-ttu-id="c683c-160">为客户提供计费支持并帮助解答计费问题</span><span class="sxs-lookup"><span data-stu-id="c683c-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="c683c-161">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="c683c-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="c683c-162">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="c683c-162">\*    Subscription management</span></span>
||<span data-ttu-id="c683c-163">\*    查看支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-163">\*    View support tickets</span></span>
||<span data-ttu-id="c683c-164">\*    请求与客户建立关系</span><span class="sxs-lookup"><span data-stu-id="c683c-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="c683c-165">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="c683c-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="c683c-166">\*    管理潜在顾客</span><span class="sxs-lookup"><span data-stu-id="c683c-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="c683c-167">\*    查看客户协议</span><span class="sxs-lookup"><span data-stu-id="c683c-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="c683c-168">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="c683c-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="c683c-169">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-170">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="c683c-171">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="c683c-171">Helpdesk agent</span></span>| <span data-ttu-id="c683c-172">\*    搜索和查看客户</span><span class="sxs-lookup"><span data-stu-id="c683c-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="c683c-173">将问题报告给 Microsoft 并了解哪些问题更适合进行报告</span><span class="sxs-lookup"><span data-stu-id="c683c-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="c683c-174">\*    编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="c683c-174">\*    Edit customer details</span></span>
||<span data-ttu-id="c683c-175">\*    帮助解决计费或订阅管理方面的客户问题</span><span class="sxs-lookup"><span data-stu-id="c683c-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c683c-176">\*    代表客户请求支持</span><span class="sxs-lookup"><span data-stu-id="c683c-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="c683c-177">\*    代表客户管理订阅和计费问题</span><span class="sxs-lookup"><span data-stu-id="c683c-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="c683c-178">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-179">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="c683c-180">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="c683c-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c683c-181">（CSP 角色和非 Azure AD 角色）</span><span class="sxs-lookup"><span data-stu-id="c683c-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="c683c-182">CPVs 开发供云解决方案提供商 (CSP) 合作伙伴使用的应用，使其能够将自己的系统与合作伙伴中心 API 相集成。</span><span class="sxs-lookup"><span data-stu-id="c683c-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c683c-183">**Role**</span><span class="sxs-lookup"><span data-stu-id="c683c-183">**Role**</span></span>   |<span data-ttu-id="c683c-184">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-184">**What you can do**</span></span>|<span data-ttu-id="c683c-185">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="c683c-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="c683c-186">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-186">Global admin</span></span>| <span data-ttu-id="c683c-187">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="c683c-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="c683c-188">注册为控制面板供应商来帮助将 CSP 合作伙伴系统和合作伙伴中心 API 进行集成</span><span class="sxs-lookup"><span data-stu-id="c683c-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="c683c-189">查看和管理需要访问 CPV 功能的任何用户。</span><span class="sxs-lookup"><span data-stu-id="c683c-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="c683c-190">来宾用户（必须添加到 Azure Active Directory 租户中）</span><span class="sxs-lookup"><span data-stu-id="c683c-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="c683c-191">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="c683c-191">**Guest user**</span></span>   | <span data-ttu-id="c683c-192">**角色**</span><span class="sxs-lookup"><span data-stu-id="c683c-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="c683c-193">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-193">MPN partner admin</span></span>|
||<span data-ttu-id="c683c-194">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-194">Business profile admin</span></span>|
||<span data-ttu-id="c683c-195">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="c683c-196">管理 MPN 成员资格和你的公司</span><span class="sxs-lookup"><span data-stu-id="c683c-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="c683c-197">这些角色并非 Azure Active Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="c683c-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="c683c-198">这些角色负责管理公司业务，而不是租户。</span><span class="sxs-lookup"><span data-stu-id="c683c-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="c683c-199">**Role**</span><span class="sxs-lookup"><span data-stu-id="c683c-199">**Role**</span></span> | <span data-ttu-id="c683c-200">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-200">**What you can do**</span></span>|<span data-ttu-id="c683c-201">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="c683c-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="c683c-202">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-202">MPN partner admin</span></span>|<span data-ttu-id="c683c-203">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="c683c-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="c683c-204">购买或续订 Microsoft Action Pack 订阅或白银和黄金资格</span><span class="sxs-lookup"><span data-stu-id="c683c-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="c683c-205">\*    查看法律、公司、业务和 MPN 档案</span><span class="sxs-lookup"><span data-stu-id="c683c-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="c683c-206">\*    查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="c683c-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="c683c-207">\*    查看资质</span><span class="sxs-lookup"><span data-stu-id="c683c-207">\*    View competencies</span></span>
||<span data-ttu-id="c683c-208">\*    查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="c683c-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="c683c-209">\*    查看和购买 MPN 套餐</span><span class="sxs-lookup"><span data-stu-id="c683c-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="c683c-210">\*    查看 MPN 套餐订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="c683c-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c683c-211">\*    查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="c683c-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="c683c-212">\*    可以操作凭证验证工具</span><span class="sxs-lookup"><span data-stu-id="c683c-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c683c-213">\*    查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="c683c-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="c683c-214">\*    查看公司内的其他用户角色，但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="c683c-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="c683c-215">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-216">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="c683c-217">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-217">Account admin</span></span>| <span data-ttu-id="c683c-218">添加位置</span><span class="sxs-lookup"><span data-stu-id="c683c-218">Add locations</span></span>|[<span data-ttu-id="c683c-219">管理位置</span><span class="sxs-lookup"><span data-stu-id="c683c-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="c683c-220">管理你是其管理员的帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="c683c-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c683c-221">\*    将租户中用户的角色分配给非 Azure Active Directory 角色</span><span class="sxs-lookup"><span data-stu-id="c683c-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="c683c-222">\*    将位置注册到计划</span><span class="sxs-lookup"><span data-stu-id="c683c-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="c683c-223">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-224">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-224">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="c683c-225">管理引荐</span><span class="sxs-lookup"><span data-stu-id="c683c-225">Manage referrals</span></span>

|<span data-ttu-id="c683c-226">**Role**</span><span class="sxs-lookup"><span data-stu-id="c683c-226">**Role**</span></span> | <span data-ttu-id="c683c-227">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-227">**What you can do**</span></span>|<span data-ttu-id="c683c-228">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="c683c-228">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="c683c-229">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-229">Referrals admin</span></span>|<span data-ttu-id="c683c-230">在合作伙伴中心的“引荐”选项卡下创建和管理所有内容</span><span class="sxs-lookup"><span data-stu-id="c683c-230">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="c683c-231">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="c683c-231">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="c683c-232">可查看和编辑所有联合销售机会和潜在客户</span><span class="sxs-lookup"><span data-stu-id="c683c-232">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="c683c-233">可为交易分配团队成员</span><span class="sxs-lookup"><span data-stu-id="c683c-233">Can assign team members for a deal</span></span>
||    <span data-ttu-id="c683c-234">可查看和编辑企业档案</span><span class="sxs-lookup"><span data-stu-id="c683c-234">Can view and edit business profiles</span></span>
||    <span data-ttu-id="c683c-235">可查看和登记标记为“已赢得”且有资格登记交易的机会的交易</span><span class="sxs-lookup"><span data-stu-id="c683c-235">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="c683c-236">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-236">Can create and view support tickets</span></span>
|<span data-ttu-id="c683c-237">引荐用户</span><span class="sxs-lookup"><span data-stu-id="c683c-237">Referrals user</span></span>|<span data-ttu-id="c683c-238">只有当联合销售机会属于团队时才可创建和管理它们</span><span class="sxs-lookup"><span data-stu-id="c683c-238">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="c683c-239">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="c683c-239">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="c683c-240">可为联合销售机会已分配有角色的位置创建这些机会。</span><span class="sxs-lookup"><span data-stu-id="c683c-240">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="c683c-241">可查看和登记标记为“已赢得”且有资格登记交易（如果属于团队）的机会的交易。</span><span class="sxs-lookup"><span data-stu-id="c683c-241">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="c683c-242">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-242">Can create and view support tickets</span></span>
|<span data-ttu-id="c683c-243">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-243">Business profile admin</span></span>|<span data-ttu-id="c683c-244">创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="c683c-244">Create and manage business profiles</span></span> | [<span data-ttu-id="c683c-245">管理企业档案</span><span class="sxs-lookup"><span data-stu-id="c683c-245">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="c683c-246">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-246">Can create and view support tickets</span></span>

<span data-ttu-id="c683c-247">除了新的引荐用户角色，我们还将为交易引入位置范围。</span><span class="sxs-lookup"><span data-stu-id="c683c-247">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="c683c-248">下表说明了基于位置的交易访问权限。</span><span class="sxs-lookup"><span data-stu-id="c683c-248">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="c683c-249">**范围**</span><span class="sxs-lookup"><span data-stu-id="c683c-249">**Scope**</span></span> | <span data-ttu-id="c683c-250">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-250">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="c683c-251">整个公司</span><span class="sxs-lookup"><span data-stu-id="c683c-251">Entire company</span></span> | <span data-ttu-id="c683c-252">管理员和用户都有权为其所在公司的任何位置创建交易</span><span class="sxs-lookup"><span data-stu-id="c683c-252">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="c683c-253">引荐管理员有权查看和编辑所有交易</span><span class="sxs-lookup"><span data-stu-id="c683c-253">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="c683c-254">只有当交易属于团队时，引荐用户才有权查看和编辑所有这些交易</span><span class="sxs-lookup"><span data-stu-id="c683c-254">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="c683c-255">一个或多个位置</span><span class="sxs-lookup"><span data-stu-id="c683c-255">One or more locations</span></span> | <span data-ttu-id="c683c-256">管理员和用户都有权为其所在公司中分配的位置创建交易</span><span class="sxs-lookup"><span data-stu-id="c683c-256">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="c683c-257">引荐管理员有权查看和编辑属于已分配的位置的所有交易</span><span class="sxs-lookup"><span data-stu-id="c683c-257">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="c683c-258">引荐用户有权查看和编辑属于已分配的位置且属于团队的所有交易</span><span class="sxs-lookup"><span data-stu-id="c683c-258">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="c683c-259">管理奖励</span><span class="sxs-lookup"><span data-stu-id="c683c-259">Manage incentives</span></span>

|<span data-ttu-id="c683c-260">**Role**</span><span class="sxs-lookup"><span data-stu-id="c683c-260">**Role**</span></span> | <span data-ttu-id="c683c-261">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-261">**What you can do**</span></span>|<span data-ttu-id="c683c-262">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="c683c-262">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="c683c-263">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="c683c-263">Incentives admin</span></span>|<span data-ttu-id="c683c-264">\*    发起和管理奖励</span><span class="sxs-lookup"><span data-stu-id="c683c-264">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="c683c-265">使用这些资源来帮助你立即体验激励</span><span class="sxs-lookup"><span data-stu-id="c683c-265">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="c683c-266">\*    可以查看和编辑奖励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="c683c-266">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c683c-267">\*    可以查看和编辑银行与税务详细信息</span><span class="sxs-lookup"><span data-stu-id="c683c-267">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c683c-268">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="c683c-268">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="c683c-269">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="c683c-269">\*    Access support</span></span>
||<span data-ttu-id="c683c-270">\*    对奖励付款提起争议</span><span class="sxs-lookup"><span data-stu-id="c683c-270">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="c683c-271">奖励用户</span><span class="sxs-lookup"><span data-stu-id="c683c-271">Incentives user</span></span>|<span data-ttu-id="c683c-272">\*    可以查看奖励计划</span><span class="sxs-lookup"><span data-stu-id="c683c-272">\*    Can view incentives programs</span></span>
||<span data-ttu-id="c683c-273">\*    可以查看和发起奖励申请</span><span class="sxs-lookup"><span data-stu-id="c683c-273">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c683c-274">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="c683c-274">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="c683c-275">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-275">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c683c-276">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-276">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="c683c-277">查看合作伙伴中心见解数据</span><span class="sxs-lookup"><span data-stu-id="c683c-277">View Partner Center Insights data</span></span>

|<span data-ttu-id="c683c-278">**Role**</span><span class="sxs-lookup"><span data-stu-id="c683c-278">**Role**</span></span> | <span data-ttu-id="c683c-279">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="c683c-279">**What you can do**</span></span>|<span data-ttu-id="c683c-280">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="c683c-280">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="c683c-281">主管人员报表查看器</span><span class="sxs-lookup"><span data-stu-id="c683c-281">Executive report viewer</span></span>|<span data-ttu-id="c683c-282">访问所有报告数据集，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-282">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="c683c-283">简要介绍合作伙伴中心见解内提供的仪表板报表</span><span class="sxs-lookup"><span data-stu-id="c683c-283">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="c683c-284">报表查看器</span><span class="sxs-lookup"><span data-stu-id="c683c-284">Report viewer</span></span>|<span data-ttu-id="c683c-285">访问不包括收入与客户和员工个人数据的数据报告，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="c683c-285">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="c683c-286">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c683c-286">Next steps</span></span>

- [<span data-ttu-id="c683c-287">创建用户帐户并分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="c683c-287">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="c683c-288">注册加入新的合作伙伴中心计划时验证你的帐户信息</span><span class="sxs-lookup"><span data-stu-id="c683c-288">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
