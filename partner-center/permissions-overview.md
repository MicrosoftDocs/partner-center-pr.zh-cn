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
ms.openlocfilehash: 80aeb62ba875d4ecd7c11063663f7c2d29912bdf
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492698"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="a848f-103">为需要在合作伙伴中心工作的公司的用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="a848f-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="a848f-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="a848f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a848f-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-105">Global admin</span></span>
- <span data-ttu-id="a848f-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-106">User admin</span></span>
- <span data-ttu-id="a848f-107">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-107">MPN partner admin</span></span>

<span data-ttu-id="a848f-108">你已设置合作伙伴档案，包括法定名称和地址、支持详细信息、税务豁免、银行信息和公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="a848f-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="a848f-109">下一步：为用户设置密码和角色，使他们能够在合作伙伴中心开始与你合作。</span><span class="sxs-lookup"><span data-stu-id="a848f-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="a848f-110">进行设置，使员工能够在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="a848f-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="a848f-111">按分配的角色和权限确定用户对合作伙伴中心拥有访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="a848f-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="a848f-112">角色与企业参与的计划相关。</span><span class="sxs-lookup"><span data-stu-id="a848f-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="a848f-113">例如，如果你的企业是云解决方案提供商 (CSP)，则你只具有标准的 Azure Active Directory 租户管理角色（例如全局管理员），但却需要 CSP 计划特定的角色。</span><span class="sxs-lookup"><span data-stu-id="a848f-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="a848f-114">每个计划都有自身特定的角色。</span><span class="sxs-lookup"><span data-stu-id="a848f-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="a848f-115">Azure Active Directory 租户角色包括全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="a848f-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="a848f-116">非 Azure Active Directory 角色是指不管理租户的角色，包括 MPN 管理员、企业档案管理员、引荐管理员、奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="a848f-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="a848f-117">在合作伙伴中心管理商业交易（Azure AD 和 CSP 角色）</span><span class="sxs-lookup"><span data-stu-id="a848f-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="a848f-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="a848f-118">**Role**</span></span>|<span data-ttu-id="a848f-119">**他们可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-119">**What they can do**</span></span>|<span data-ttu-id="a848f-120">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="a848f-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="a848f-121">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-121">Global admin</span></span>|<span data-ttu-id="a848f-122">\*    可以全权访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="a848f-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="a848f-123">管理合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="a848f-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="a848f-124">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-125">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="a848f-126">\*    查看协议、价目表和套餐</span><span class="sxs-lookup"><span data-stu-id="a848f-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="a848f-127">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="a848f-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="a848f-128">查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="a848f-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="a848f-129">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-129">User management admin</span></span>   | <span data-ttu-id="a848f-130">\*    查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="a848f-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="a848f-131">在合作伙伴中心管理 Microsoft 合作伙伴网络成员资格权益和优惠</span><span class="sxs-lookup"><span data-stu-id="a848f-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="a848f-132">\*    查看所有合作伙伴档案</span><span class="sxs-lookup"><span data-stu-id="a848f-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="a848f-133">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-134">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a848f-135">计费管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-135">Billing admin</span></span> | <span data-ttu-id="a848f-136">- 查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="a848f-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="a848f-137">阅读账单</span><span class="sxs-lookup"><span data-stu-id="a848f-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="a848f-138">\*    查看定价</span><span class="sxs-lookup"><span data-stu-id="a848f-138">\*    View pricing</span></span>
||<span data-ttu-id="a848f-139">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-140">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a848f-141">默认用户</span><span class="sxs-lookup"><span data-stu-id="a848f-141">Default user</span></span>|  <span data-ttu-id="a848f-142">查看“我的个人资料”</span><span class="sxs-lookup"><span data-stu-id="a848f-142">View My profile</span></span>   |[<span data-ttu-id="a848f-143">重置密码</span><span class="sxs-lookup"><span data-stu-id="a848f-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="a848f-144">管理员代理</span><span class="sxs-lookup"><span data-stu-id="a848f-144">Admin agent</span></span> | <span data-ttu-id="a848f-145">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="a848f-145">\*    Customer management</span></span>|[<span data-ttu-id="a848f-146">与客户联系</span><span class="sxs-lookup"><span data-stu-id="a848f-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="a848f-147">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="a848f-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a848f-148">\*    创建配置文件并将其应用到设备</span><span class="sxs-lookup"><span data-stu-id="a848f-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="a848f-149">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="a848f-149">\*    Subscription management</span></span>
||<span data-ttu-id="a848f-150">\*    客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="a848f-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="a848f-151">\*    请求委派管理员特权</span><span class="sxs-lookup"><span data-stu-id="a848f-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="a848f-152">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="a848f-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="a848f-153">\*    计费</span><span class="sxs-lookup"><span data-stu-id="a848f-153">\*    Billing</span></span>
||<span data-ttu-id="a848f-154">\*    代表客户的管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="a848f-155">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="a848f-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="a848f-156">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-157">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="a848f-158">销售代理</span><span class="sxs-lookup"><span data-stu-id="a848f-158">Sales agent</span></span> | <span data-ttu-id="a848f-159">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="a848f-159">\*    Customer management</span></span>|[<span data-ttu-id="a848f-160">为客户提供计费支持并帮助解答计费问题</span><span class="sxs-lookup"><span data-stu-id="a848f-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="a848f-161">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="a848f-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a848f-162">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="a848f-162">\*    Subscription management</span></span>
||<span data-ttu-id="a848f-163">\*    查看支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-163">\*    View support tickets</span></span>
||<span data-ttu-id="a848f-164">\*    请求与客户建立关系</span><span class="sxs-lookup"><span data-stu-id="a848f-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="a848f-165">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="a848f-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="a848f-166">\*    管理潜在顾客</span><span class="sxs-lookup"><span data-stu-id="a848f-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="a848f-167">\*    查看客户协议</span><span class="sxs-lookup"><span data-stu-id="a848f-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="a848f-168">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="a848f-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="a848f-169">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-170">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="a848f-171">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="a848f-171">Helpdesk agent</span></span>| <span data-ttu-id="a848f-172">\*    搜索和查看客户</span><span class="sxs-lookup"><span data-stu-id="a848f-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="a848f-173">将问题报告给 Microsoft 并了解哪些问题更适合进行报告</span><span class="sxs-lookup"><span data-stu-id="a848f-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="a848f-174">\*    编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="a848f-174">\*    Edit customer details</span></span>
||<span data-ttu-id="a848f-175">\*    帮助解决计费或订阅管理方面的客户问题</span><span class="sxs-lookup"><span data-stu-id="a848f-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="a848f-176">\*    代表客户请求支持</span><span class="sxs-lookup"><span data-stu-id="a848f-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="a848f-177">\*    代表客户管理订阅和计费问题</span><span class="sxs-lookup"><span data-stu-id="a848f-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="a848f-178">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-179">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="a848f-180">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="a848f-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="a848f-181">（CSP 角色和非 Azure AD 角色）</span><span class="sxs-lookup"><span data-stu-id="a848f-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="a848f-182">CPVs 开发供云解决方案提供商 (CSP) 合作伙伴使用的应用，使其能够将自己的系统与合作伙伴中心 API 相集成。</span><span class="sxs-lookup"><span data-stu-id="a848f-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="a848f-183">**Role**</span><span class="sxs-lookup"><span data-stu-id="a848f-183">**Role**</span></span>   |<span data-ttu-id="a848f-184">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-184">**What you can do**</span></span>|<span data-ttu-id="a848f-185">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="a848f-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="a848f-186">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-186">Global admin</span></span>| <span data-ttu-id="a848f-187">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="a848f-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="a848f-188">注册为控制面板供应商来帮助将 CSP 合作伙伴系统和合作伙伴中心 API 进行集成</span><span class="sxs-lookup"><span data-stu-id="a848f-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="a848f-189">查看和管理需要访问 CPV 功能的任何用户。</span><span class="sxs-lookup"><span data-stu-id="a848f-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="a848f-190">来宾用户（必须添加到 Azure Active Directory 租户中）</span><span class="sxs-lookup"><span data-stu-id="a848f-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="a848f-191">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="a848f-191">**Guest user**</span></span>   | <span data-ttu-id="a848f-192">**角色**</span><span class="sxs-lookup"><span data-stu-id="a848f-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="a848f-193">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-193">MPN partner admin</span></span>|
||<span data-ttu-id="a848f-194">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-194">Business profile admin</span></span>|
||<span data-ttu-id="a848f-195">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="a848f-196">管理 MPN 成员资格和你的公司</span><span class="sxs-lookup"><span data-stu-id="a848f-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="a848f-197">这些角色并非 Azure Active Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="a848f-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="a848f-198">这些角色负责管理公司业务，而不是租户。</span><span class="sxs-lookup"><span data-stu-id="a848f-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="a848f-199">**Role**</span><span class="sxs-lookup"><span data-stu-id="a848f-199">**Role**</span></span> | <span data-ttu-id="a848f-200">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-200">**What you can do**</span></span>|<span data-ttu-id="a848f-201">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="a848f-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="a848f-202">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-202">MPN partner admin</span></span>|<span data-ttu-id="a848f-203">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="a848f-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="a848f-204">购买或续订 Microsoft Action Pack 订阅或白银和黄金资格</span><span class="sxs-lookup"><span data-stu-id="a848f-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="a848f-205">\*    查看法律、公司、业务和 MPN 档案</span><span class="sxs-lookup"><span data-stu-id="a848f-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="a848f-206">\*    查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="a848f-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="a848f-207">\*    查看资质</span><span class="sxs-lookup"><span data-stu-id="a848f-207">\*    View competencies</span></span>
||<span data-ttu-id="a848f-208">\*    查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="a848f-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="a848f-209">\*    查看和购买 MPN 套餐</span><span class="sxs-lookup"><span data-stu-id="a848f-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="a848f-210">\*    查看 MPN 套餐订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="a848f-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="a848f-211">\*    查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="a848f-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="a848f-212">\*    可以操作凭证验证工具</span><span class="sxs-lookup"><span data-stu-id="a848f-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="a848f-213">\*    查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="a848f-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="a848f-214">\*    查看公司内的其他用户角色，但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="a848f-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="a848f-215">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-216">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a848f-217">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-217">Account admin</span></span>| <span data-ttu-id="a848f-218">添加位置</span><span class="sxs-lookup"><span data-stu-id="a848f-218">Add locations</span></span>|[<span data-ttu-id="a848f-219">管理位置</span><span class="sxs-lookup"><span data-stu-id="a848f-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="a848f-220">管理你是其管理员的帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="a848f-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="a848f-221">\*    将租户中用户的角色分配给非 Azure Active Directory 角色</span><span class="sxs-lookup"><span data-stu-id="a848f-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="a848f-222">\*    将位置注册到计划</span><span class="sxs-lookup"><span data-stu-id="a848f-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="a848f-223">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-224">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-224">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="a848f-225">管理引荐</span><span class="sxs-lookup"><span data-stu-id="a848f-225">Manage referrals</span></span>

> [!Note]
><span data-ttu-id="a848f-226">将自 2020 年 11 月 18 开始推出新的引荐用户角色。</span><span class="sxs-lookup"><span data-stu-id="a848f-226">The new Referrals user role will be available starting 18th November 2020.</span></span> <span data-ttu-id="a848f-227">现有的引荐管理员将保留其对整个公司有效的引荐管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a848f-227">Existing referral admins will retain their referral admin role scoped to the entire company.</span></span>

|<span data-ttu-id="a848f-228">**Role**</span><span class="sxs-lookup"><span data-stu-id="a848f-228">**Role**</span></span> | <span data-ttu-id="a848f-229">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-229">**What you can do**</span></span>|<span data-ttu-id="a848f-230">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="a848f-230">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="a848f-231">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-231">Referrals admin</span></span>|<span data-ttu-id="a848f-232">在合作伙伴中心的“引荐”选项卡下创建和管理所有内容</span><span class="sxs-lookup"><span data-stu-id="a848f-232">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="a848f-233">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="a848f-233">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="a848f-234">可查看和编辑所有联合销售机会和潜在客户</span><span class="sxs-lookup"><span data-stu-id="a848f-234">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="a848f-235">可为交易分配团队成员</span><span class="sxs-lookup"><span data-stu-id="a848f-235">Can assign team members for a deal</span></span>
||    <span data-ttu-id="a848f-236">可查看和编辑企业档案</span><span class="sxs-lookup"><span data-stu-id="a848f-236">Can view and edit business profiles</span></span>
||    <span data-ttu-id="a848f-237">可查看和登记标记为“已赢得”且有资格登记交易的机会的交易</span><span class="sxs-lookup"><span data-stu-id="a848f-237">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="a848f-238">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-238">Can create and view support tickets</span></span>
|<span data-ttu-id="a848f-239">引荐用户</span><span class="sxs-lookup"><span data-stu-id="a848f-239">Referrals user</span></span>|<span data-ttu-id="a848f-240">只有当联合销售机会属于团队时才可创建和管理它们</span><span class="sxs-lookup"><span data-stu-id="a848f-240">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="a848f-241">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="a848f-241">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="a848f-242">可为联合销售机会已分配有角色的位置创建这些机会。</span><span class="sxs-lookup"><span data-stu-id="a848f-242">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="a848f-243">可查看和登记标记为“已赢得”且有资格登记交易（如果属于团队）的机会的交易。</span><span class="sxs-lookup"><span data-stu-id="a848f-243">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="a848f-244">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-244">Can create and view support tickets</span></span>
|<span data-ttu-id="a848f-245">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-245">Business profile admin</span></span>|<span data-ttu-id="a848f-246">创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="a848f-246">Create and manage business profiles</span></span> | [<span data-ttu-id="a848f-247">管理企业档案</span><span class="sxs-lookup"><span data-stu-id="a848f-247">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="a848f-248">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-248">Can create and view support tickets</span></span>

<span data-ttu-id="a848f-249">除了新的引荐用户角色，我们还将为交易引入位置范围。</span><span class="sxs-lookup"><span data-stu-id="a848f-249">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="a848f-250">下表说明了基于位置的交易访问权限。</span><span class="sxs-lookup"><span data-stu-id="a848f-250">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="a848f-251">**范围**</span><span class="sxs-lookup"><span data-stu-id="a848f-251">**Scope**</span></span> | <span data-ttu-id="a848f-252">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-252">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="a848f-253">整个公司</span><span class="sxs-lookup"><span data-stu-id="a848f-253">Entire company</span></span> | <span data-ttu-id="a848f-254">管理员和用户都有权为其所在公司的任何位置创建交易</span><span class="sxs-lookup"><span data-stu-id="a848f-254">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="a848f-255">引荐管理员有权查看和编辑所有交易</span><span class="sxs-lookup"><span data-stu-id="a848f-255">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="a848f-256">只有当交易属于团队时，引荐用户才有权查看和编辑所有这些交易</span><span class="sxs-lookup"><span data-stu-id="a848f-256">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="a848f-257">一个或多个位置</span><span class="sxs-lookup"><span data-stu-id="a848f-257">One or more locations</span></span> | <span data-ttu-id="a848f-258">管理员和用户都有权为其所在公司中分配的位置创建交易</span><span class="sxs-lookup"><span data-stu-id="a848f-258">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="a848f-259">引荐管理员有权查看和编辑属于已分配的位置的所有交易</span><span class="sxs-lookup"><span data-stu-id="a848f-259">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="a848f-260">引荐用户有权查看和编辑属于已分配的位置且属于团队的所有交易</span><span class="sxs-lookup"><span data-stu-id="a848f-260">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="a848f-261">管理奖励</span><span class="sxs-lookup"><span data-stu-id="a848f-261">Manage incentives</span></span>

|<span data-ttu-id="a848f-262">**Role**</span><span class="sxs-lookup"><span data-stu-id="a848f-262">**Role**</span></span> | <span data-ttu-id="a848f-263">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-263">**What you can do**</span></span>|<span data-ttu-id="a848f-264">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="a848f-264">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="a848f-265">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="a848f-265">Incentives admin</span></span>|<span data-ttu-id="a848f-266">\*    发起和管理奖励</span><span class="sxs-lookup"><span data-stu-id="a848f-266">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="a848f-267">使用这些资源来帮助你立即体验激励</span><span class="sxs-lookup"><span data-stu-id="a848f-267">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="a848f-268">\*    可以查看和编辑奖励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="a848f-268">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="a848f-269">\*    可以查看和编辑银行与税务详细信息</span><span class="sxs-lookup"><span data-stu-id="a848f-269">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="a848f-270">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="a848f-270">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a848f-271">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="a848f-271">\*    Access support</span></span>
||<span data-ttu-id="a848f-272">\*    对奖励付款提起争议</span><span class="sxs-lookup"><span data-stu-id="a848f-272">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="a848f-273">奖励用户</span><span class="sxs-lookup"><span data-stu-id="a848f-273">Incentives user</span></span>|<span data-ttu-id="a848f-274">\*    可以查看奖励计划</span><span class="sxs-lookup"><span data-stu-id="a848f-274">\*    Can view incentives programs</span></span>
||<span data-ttu-id="a848f-275">\*    可以查看和发起奖励申请</span><span class="sxs-lookup"><span data-stu-id="a848f-275">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="a848f-276">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="a848f-276">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a848f-277">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-277">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a848f-278">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-278">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="a848f-279">查看合作伙伴中心见解数据</span><span class="sxs-lookup"><span data-stu-id="a848f-279">View Partner Center Insights data</span></span>

|<span data-ttu-id="a848f-280">**Role**</span><span class="sxs-lookup"><span data-stu-id="a848f-280">**Role**</span></span> | <span data-ttu-id="a848f-281">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a848f-281">**What you can do**</span></span>|<span data-ttu-id="a848f-282">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="a848f-282">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="a848f-283">主管人员报表查看器</span><span class="sxs-lookup"><span data-stu-id="a848f-283">Executive report viewer</span></span>|<span data-ttu-id="a848f-284">访问所有报告数据集，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-284">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="a848f-285">简要介绍合作伙伴中心见解内提供的仪表板报表</span><span class="sxs-lookup"><span data-stu-id="a848f-285">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="a848f-286">报表查看器</span><span class="sxs-lookup"><span data-stu-id="a848f-286">Report viewer</span></span>|<span data-ttu-id="a848f-287">访问不包括收入与客户和员工个人数据的数据报告，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="a848f-287">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="a848f-288">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a848f-288">Next steps</span></span>

- [<span data-ttu-id="a848f-289">创建用户帐户并分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="a848f-289">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="a848f-290">注册加入新的合作伙伴中心计划时验证你的帐户信息</span><span class="sxs-lookup"><span data-stu-id="a848f-290">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
