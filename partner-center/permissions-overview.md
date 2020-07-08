---
title: 向用户分配角色和权限
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解哪些角色最适合你所在公司的用户，这些用户在合作伙伴中心管理商业交易、引荐、奖励或 MPN 成员资格。
author: hemas
ms.author: hemas
keywords: 角色, 权限, 管理员, 代理
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4f4ec3a1a14e6845f7b6079e286876d9bb1f3dd5
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948593"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="67f76-104">为需要在合作伙伴中心工作的公司的用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="67f76-104">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="67f76-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="67f76-105">**Appropriate roles**</span></span>

- <span data-ttu-id="67f76-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-106">Global admin</span></span>
- <span data-ttu-id="67f76-107">用户管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-107">User admin</span></span>
- <span data-ttu-id="67f76-108">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-108">MPN partner admin</span></span>

<span data-ttu-id="67f76-109">你已设置合作伙伴档案，包括法定名称和地址、支持详细信息、税务豁免、银行信息和公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="67f76-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="67f76-110">下一步：为用户设置密码和角色，使他们能够在合作伙伴中心开始与你合作。</span><span class="sxs-lookup"><span data-stu-id="67f76-110">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="67f76-111">进行设置，使员工能够在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="67f76-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="67f76-112">按分配的角色和权限确定用户对合作伙伴中心拥有访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="67f76-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="67f76-113">角色与企业参与的计划相关。</span><span class="sxs-lookup"><span data-stu-id="67f76-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="67f76-114">例如，如果你的企业是云解决方案提供商 (CSP)，则你只具有标准的 Azure AD 租户管理角色（例如全局管理员），但需要特定于 CSP 计划的角色。</span><span class="sxs-lookup"><span data-stu-id="67f76-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="67f76-115">每个计划都有自身特定的角色。</span><span class="sxs-lookup"><span data-stu-id="67f76-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="67f76-116">Azure Active Directory (AAD) 租户角色包括全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="67f76-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="67f76-117">非 AAD 角色是指不管理租户的角色，包括 MPN 管理员、企业档案管理员、引荐管理员、奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="67f76-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="67f76-118">在合作伙伴中心管理商业交易（Azure AD 和 CSP 角色）</span><span class="sxs-lookup"><span data-stu-id="67f76-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="67f76-119">**Role**</span><span class="sxs-lookup"><span data-stu-id="67f76-119">**Role**</span></span>|<span data-ttu-id="67f76-120">**他们可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="67f76-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="67f76-121">全局管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-121">Global admin</span></span>|<span data-ttu-id="67f76-122">\*    可以全权访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="67f76-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="67f76-123">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="67f76-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="67f76-124">\*    查看协议、价目表和套餐</span><span class="sxs-lookup"><span data-stu-id="67f76-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="67f76-125">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="67f76-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="67f76-126">查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="67f76-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="67f76-127">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-127">User management admin</span></span>   | <span data-ttu-id="67f76-128">\*    查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="67f76-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="67f76-129">\*    查看所有合作伙伴档案</span><span class="sxs-lookup"><span data-stu-id="67f76-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="67f76-130">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="67f76-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="67f76-131">计费管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-131">Billing admin</span></span> | <span data-ttu-id="67f76-132">- 查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="67f76-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="67f76-133">默认用户</span><span class="sxs-lookup"><span data-stu-id="67f76-133">Default user</span></span>|  <span data-ttu-id="67f76-134">查看“我的个人资料”</span><span class="sxs-lookup"><span data-stu-id="67f76-134">View My profile</span></span>   |
|<span data-ttu-id="67f76-135">管理员代理</span><span class="sxs-lookup"><span data-stu-id="67f76-135">Admin agent</span></span> | <span data-ttu-id="67f76-136">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="67f76-136">\*    Customer management</span></span>
||<span data-ttu-id="67f76-137">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="67f76-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="67f76-138">\*    创建配置文件并将其应用到设备</span><span class="sxs-lookup"><span data-stu-id="67f76-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="67f76-139">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="67f76-139">\*    Subscription management</span></span>
||<span data-ttu-id="67f76-140">\*    客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="67f76-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="67f76-141">\*    请求委派管理员特权</span><span class="sxs-lookup"><span data-stu-id="67f76-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="67f76-142">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="67f76-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="67f76-143">\*    计费</span><span class="sxs-lookup"><span data-stu-id="67f76-143">\*    Billing</span></span>
||<span data-ttu-id="67f76-144">\*    代表客户的管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="67f76-145">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="67f76-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="67f76-146">销售代理</span><span class="sxs-lookup"><span data-stu-id="67f76-146">Sales agent</span></span> | <span data-ttu-id="67f76-147">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="67f76-147">\*    Customer management</span></span>
||<span data-ttu-id="67f76-148">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="67f76-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="67f76-149">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="67f76-149">\*    Subscription management</span></span>
||<span data-ttu-id="67f76-150">\*    查看支持票证</span><span class="sxs-lookup"><span data-stu-id="67f76-150">\*    View support tickets</span></span>
||<span data-ttu-id="67f76-151">\*    请求与客户建立关系</span><span class="sxs-lookup"><span data-stu-id="67f76-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="67f76-152">\*    管理潜在顾客</span><span class="sxs-lookup"><span data-stu-id="67f76-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="67f76-153">\*    查看客户协议</span><span class="sxs-lookup"><span data-stu-id="67f76-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="67f76-154">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="67f76-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="67f76-155">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="67f76-155">Helpdesk agent</span></span>| <span data-ttu-id="67f76-156">\*    搜索和查看客户</span><span class="sxs-lookup"><span data-stu-id="67f76-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="67f76-157">\*    编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="67f76-157">\*    Edit customer details</span></span>
||<span data-ttu-id="67f76-158">\*    帮助解决计费或订阅管理方面的客户问题</span><span class="sxs-lookup"><span data-stu-id="67f76-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="67f76-159">\*    代表客户请求支持</span><span class="sxs-lookup"><span data-stu-id="67f76-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="67f76-160">\*    代表客户管理订阅和计费问题</span><span class="sxs-lookup"><span data-stu-id="67f76-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="67f76-161">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="67f76-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="67f76-162">（CSP 角色和非 AAD 角色）</span><span class="sxs-lookup"><span data-stu-id="67f76-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="67f76-163">CPVs 开发供云解决方案提供商 (CSP) 合作伙伴使用的应用，使其能够将自己的系统与合作伙伴中心 API 相集成。</span><span class="sxs-lookup"><span data-stu-id="67f76-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="67f76-164">**Role**</span><span class="sxs-lookup"><span data-stu-id="67f76-164">**Role**</span></span>   |<span data-ttu-id="67f76-165">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="67f76-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="67f76-166">全局管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-166">Global admin</span></span>| <span data-ttu-id="67f76-167">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="67f76-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="67f76-168">查看和管理需要访问 CPV 功能的任何用户。</span><span class="sxs-lookup"><span data-stu-id="67f76-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="67f76-169">来宾用户（必须已添加到 AAD 租户）</span><span class="sxs-lookup"><span data-stu-id="67f76-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="67f76-170">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="67f76-170">**Guest user**</span></span>   | <span data-ttu-id="67f76-171">**角色**</span><span class="sxs-lookup"><span data-stu-id="67f76-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="67f76-172">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-172">MPN partner admin</span></span>|
||<span data-ttu-id="67f76-173">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-173">Accounts admin</span></span>|
||<span data-ttu-id="67f76-174">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-174">Incentives admin</span></span>|
||<span data-ttu-id="67f76-175">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-175">Business profile admin</span></span>|
||<span data-ttu-id="67f76-176">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="67f76-177">管理 MPN 成员身份和公司（非 AAD 角色：这些角色管理公司业务，而不是管理租户）</span><span class="sxs-lookup"><span data-stu-id="67f76-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="67f76-178">**Role**</span><span class="sxs-lookup"><span data-stu-id="67f76-178">**Role**</span></span> | <span data-ttu-id="67f76-179">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="67f76-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="67f76-180">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-180">MPN partner admin</span></span>|<span data-ttu-id="67f76-181">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="67f76-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="67f76-182">\*    查看法律、公司、业务和 MPN 档案</span><span class="sxs-lookup"><span data-stu-id="67f76-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="67f76-183">\*    查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="67f76-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="67f76-184">\*    查看资质</span><span class="sxs-lookup"><span data-stu-id="67f76-184">\*    View competencies</span></span>
||<span data-ttu-id="67f76-185">\*    查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="67f76-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="67f76-186">\*    查看和购买 MPN 套餐</span><span class="sxs-lookup"><span data-stu-id="67f76-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="67f76-187">\*    查看 MPN 套餐订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="67f76-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="67f76-188">\*    查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="67f76-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="67f76-189">\*    可以操作凭证验证工具</span><span class="sxs-lookup"><span data-stu-id="67f76-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="67f76-190">\*    查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="67f76-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="67f76-191">\*    查看公司内的其他用户角色，但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="67f76-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="67f76-192">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-192">Account admin</span></span>| <span data-ttu-id="67f76-193">添加位置</span><span class="sxs-lookup"><span data-stu-id="67f76-193">Add locations</span></span>
|| <span data-ttu-id="67f76-194">管理你是其管理员的帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="67f76-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="67f76-195">\*    将租户中用户的角色分配为非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="67f76-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="67f76-196">\*    将位置注册到计划</span><span class="sxs-lookup"><span data-stu-id="67f76-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="67f76-197">管理引荐</span><span class="sxs-lookup"><span data-stu-id="67f76-197">Manage referrals</span></span> 

|<span data-ttu-id="67f76-198">**Role**</span><span class="sxs-lookup"><span data-stu-id="67f76-198">**Role**</span></span>|<span data-ttu-id="67f76-199">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="67f76-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="67f76-200">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-200">Referrals admin</span></span>       |<span data-ttu-id="67f76-201">\*    查看、创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="67f76-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="67f76-202">\*    接收和管理引荐</span><span class="sxs-lookup"><span data-stu-id="67f76-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="67f76-203">\* 查看、创建和管理共同销售引荐</span><span class="sxs-lookup"><span data-stu-id="67f76-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="67f76-204">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="67f76-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="67f76-205">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-205">Business profile admin</span></span>   |<span data-ttu-id="67f76-206">\* 查看、创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="67f76-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="67f76-207">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="67f76-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="67f76-208">管理奖励</span><span class="sxs-lookup"><span data-stu-id="67f76-208">Manage incentives</span></span> 

|<span data-ttu-id="67f76-209">**Role**</span><span class="sxs-lookup"><span data-stu-id="67f76-209">**Role**</span></span> | <span data-ttu-id="67f76-210">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="67f76-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="67f76-211">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="67f76-211">Incentives admin</span></span>|<span data-ttu-id="67f76-212">\*    发起和管理奖励</span><span class="sxs-lookup"><span data-stu-id="67f76-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="67f76-213">\*    可以查看和编辑奖励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="67f76-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="67f76-214">\*    可以查看和编辑银行与税务详细信息</span><span class="sxs-lookup"><span data-stu-id="67f76-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="67f76-215">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="67f76-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="67f76-216">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="67f76-216">\*    Access support</span></span>
||<span data-ttu-id="67f76-217">\*    对奖励付款提起争议</span><span class="sxs-lookup"><span data-stu-id="67f76-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="67f76-218">奖励用户</span><span class="sxs-lookup"><span data-stu-id="67f76-218">Incentives user</span></span>|<span data-ttu-id="67f76-219">\*    可以查看奖励计划</span><span class="sxs-lookup"><span data-stu-id="67f76-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="67f76-220">\*    可以查看和发起奖励申请</span><span class="sxs-lookup"><span data-stu-id="67f76-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="67f76-221">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="67f76-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="67f76-222">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="67f76-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="67f76-223">查看合作伙伴中心见解数据</span><span class="sxs-lookup"><span data-stu-id="67f76-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="67f76-224">**Role**</span><span class="sxs-lookup"><span data-stu-id="67f76-224">**Role**</span></span> | <span data-ttu-id="67f76-225">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="67f76-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="67f76-226">主管人员报表查看器</span><span class="sxs-lookup"><span data-stu-id="67f76-226">Executive report viewer</span></span>|<span data-ttu-id="67f76-227">访问所有报告数据集</span><span class="sxs-lookup"><span data-stu-id="67f76-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="67f76-228">报表查看器</span><span class="sxs-lookup"><span data-stu-id="67f76-228">Report viewer</span></span>|<span data-ttu-id="67f76-229">访问不包括收入与客户和员工个人数据的数据报告</span><span class="sxs-lookup"><span data-stu-id="67f76-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    