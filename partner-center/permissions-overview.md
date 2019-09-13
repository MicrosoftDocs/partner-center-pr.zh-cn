---
title: 分配用户角色和权限 | 合作伙伴中心
ms.topic: article
ms.date: 3/5/2019
description: 必须为需要在合作伙伴中心工作的每个员工分配一个角色。
author: LauraBrenner
ms.author: labrenne
keywords: 角色, 权限, 管理员, 代理
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708866"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="d93da-104">为用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="d93da-104">Assign users roles and permissions</span></span>


<span data-ttu-id="d93da-105">你已经设置了你的合作伙伴配置文件, 包括合法名称和地址、支持详细信息、文件税务豁免、银行信息以及公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="d93da-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="d93da-106">下一步: 使用密码和角色设置用户, 以便他们可以在合作伙伴中心开始使用。</span><span class="sxs-lookup"><span data-stu-id="d93da-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="d93da-107">将你的员工设置为在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="d93da-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="d93da-108">你确定你的用户对合作伙伴中心的访问类型, 以及你向他们授予的权限。</span><span class="sxs-lookup"><span data-stu-id="d93da-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="d93da-109">角色与您的业务所涉及的程序相关。</span><span class="sxs-lookup"><span data-stu-id="d93da-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="d93da-110">例如, 如果你的业务是云解决方案提供商 (CSP) 业务, 则你将只具有标准 Azure AD 租户管理角色 (如全局管理员), 但需要特定于 CSP 计划的角色。</span><span class="sxs-lookup"><span data-stu-id="d93da-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="d93da-111">每个程序都具有特定的角色。</span><span class="sxs-lookup"><span data-stu-id="d93da-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="d93da-112">Azure Active Directory (AAD) 租户角色包含全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="d93da-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="d93da-113">非 AAD 角色是指不管理租户的角色, 这些角色包括 MPN 管理员、业务配置文件管理员、引用管理员、激励管理员和激励用户。</span><span class="sxs-lookup"><span data-stu-id="d93da-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="d93da-114">管理合作伙伴中心的商业交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="d93da-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="d93da-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="d93da-115">**Role**</span></span>|<span data-ttu-id="d93da-116">**可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="d93da-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="d93da-117">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-117">Global admin</span></span>|<span data-ttu-id="d93da-118">•可使用完全权限访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="d93da-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="d93da-119">•为合作伙伴中心创建支持票证</span><span class="sxs-lookup"><span data-stu-id="d93da-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d93da-120">•查看协议、价格列表和产品/服务</span><span class="sxs-lookup"><span data-stu-id="d93da-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="d93da-121">•查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="d93da-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="d93da-122">查看、创建和管理计费、发票和侦测文件</span><span class="sxs-lookup"><span data-stu-id="d93da-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="d93da-123">用户管理管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-123">User management admin</span></span>   | <span data-ttu-id="d93da-124">•查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="d93da-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="d93da-125">•查看所有合作伙伴配置文件</span><span class="sxs-lookup"><span data-stu-id="d93da-125">• View all partner profiles</span></span>
||<span data-ttu-id="d93da-126">•查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="d93da-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="d93da-127">帐单管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-127">Billing admin</span></span> | <span data-ttu-id="d93da-128">-查看、创建和管理计费、发票和侦测文件</span><span class="sxs-lookup"><span data-stu-id="d93da-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="d93da-129">默认用户</span><span class="sxs-lookup"><span data-stu-id="d93da-129">Default user</span></span>|  <span data-ttu-id="d93da-130">查看我的个人资料</span><span class="sxs-lookup"><span data-stu-id="d93da-130">View My profile</span></span>   |
|<span data-ttu-id="d93da-131">管理员代理</span><span class="sxs-lookup"><span data-stu-id="d93da-131">Admin agent</span></span> | <span data-ttu-id="d93da-132">•客户管理</span><span class="sxs-lookup"><span data-stu-id="d93da-132">•    Customer management</span></span>
||<span data-ttu-id="d93da-133">•向合作伙伴中心添加设备列表</span><span class="sxs-lookup"><span data-stu-id="d93da-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="d93da-134">•创建配置文件并将其应用于设备</span><span class="sxs-lookup"><span data-stu-id="d93da-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="d93da-135">•订阅管理</span><span class="sxs-lookup"><span data-stu-id="d93da-135">• Subscription management</span></span>
||<span data-ttu-id="d93da-136">•客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="d93da-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="d93da-137">•请求委派的管理员权限</span><span class="sxs-lookup"><span data-stu-id="d93da-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="d93da-138">•查看定价和产品/服务</span><span class="sxs-lookup"><span data-stu-id="d93da-138">• View pricing and offers</span></span>
||<span data-ttu-id="d93da-139">•计费</span><span class="sxs-lookup"><span data-stu-id="d93da-139">• Billing</span></span>
||<span data-ttu-id="d93da-140">•代表客户管理</span><span class="sxs-lookup"><span data-stu-id="d93da-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="d93da-141">•注册增值分销商</span><span class="sxs-lookup"><span data-stu-id="d93da-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="d93da-142">销售代理</span><span class="sxs-lookup"><span data-stu-id="d93da-142">Sales agent</span></span> | <span data-ttu-id="d93da-143">•客户管理</span><span class="sxs-lookup"><span data-stu-id="d93da-143">•    Customer management</span></span>
||<span data-ttu-id="d93da-144">•向合作伙伴中心添加设备列表</span><span class="sxs-lookup"><span data-stu-id="d93da-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="d93da-145">•订阅管理</span><span class="sxs-lookup"><span data-stu-id="d93da-145">• Subscription management</span></span>
||<span data-ttu-id="d93da-146">•查看价格列表和产品/服务</span><span class="sxs-lookup"><span data-stu-id="d93da-146">• View price lists and offers</span></span>
||<span data-ttu-id="d93da-147">•查看支持票证</span><span class="sxs-lookup"><span data-stu-id="d93da-147">• View support tickets</span></span>
||<span data-ttu-id="d93da-148">•请求与客户之间的关系</span><span class="sxs-lookup"><span data-stu-id="d93da-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="d93da-149">•管理客户主管</span><span class="sxs-lookup"><span data-stu-id="d93da-149">• Manage customer leads</span></span>
||<span data-ttu-id="d93da-150">•查看客户协议</span><span class="sxs-lookup"><span data-stu-id="d93da-150">• View the customer agreement</span></span>
||<span data-ttu-id="d93da-151">•注册增值分销商</span><span class="sxs-lookup"><span data-stu-id="d93da-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="d93da-152">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="d93da-152">Helpdesk agent</span></span>| <span data-ttu-id="d93da-153">•搜索并查看客户</span><span class="sxs-lookup"><span data-stu-id="d93da-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="d93da-154">•编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="d93da-154">• Edit customer details</span></span>
||<span data-ttu-id="d93da-155">•帮助解决与计费或订阅管理有关的客户问题</span><span class="sxs-lookup"><span data-stu-id="d93da-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="d93da-156">•代表客户请求支持 (注意:你必须是管理员代理才能完成 Office 365 订阅的此任务)</span><span class="sxs-lookup"><span data-stu-id="d93da-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="d93da-157">•代表客户管理订阅和计费问题 (请注意:你必须是管理员代理才能完成 Office 365 订阅的此任务)</span><span class="sxs-lookup"><span data-stu-id="d93da-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="d93da-158">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="d93da-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="d93da-159">(CSP 角色和非 AAD 角色)</span><span class="sxs-lookup"><span data-stu-id="d93da-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="d93da-160">CPVs 开发云解决方案提供商 (CSP) 合作伙伴所使用的应用, 使其能够将其系统与合作伙伴中心 Api 集成。</span><span class="sxs-lookup"><span data-stu-id="d93da-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="d93da-161">**Role**</span><span class="sxs-lookup"><span data-stu-id="d93da-161">**Role**</span></span>   |<span data-ttu-id="d93da-162">**可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="d93da-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="d93da-163">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-163">Global admin</span></span>| <span data-ttu-id="d93da-164">查看并管理你的 CPV 配置文件</span><span class="sxs-lookup"><span data-stu-id="d93da-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="d93da-165">查看并管理任何需要访问 CPV 功能的用户</span><span class="sxs-lookup"><span data-stu-id="d93da-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="d93da-166">Guest 用户 (必须添加到 AAD 租户)</span><span class="sxs-lookup"><span data-stu-id="d93da-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="d93da-167">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="d93da-167">**Guest user**</span></span>   | <span data-ttu-id="d93da-168">**作用**</span><span class="sxs-lookup"><span data-stu-id="d93da-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="d93da-169">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-169">MPN partner admin</span></span>|
||<span data-ttu-id="d93da-170">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-170">Accounts admin</span></span>|
||<span data-ttu-id="d93da-171">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-171">Incentives admin</span></span>|
||<span data-ttu-id="d93da-172">业务档案管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-172">Business profile admin</span></span>|
||<span data-ttu-id="d93da-173">引用管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="d93da-174">管理 MPN 成员身份和公司 (非 AAD 角色: 这些角色管理公司企业, 而不是租户)</span><span class="sxs-lookup"><span data-stu-id="d93da-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="d93da-175">**Role**</span><span class="sxs-lookup"><span data-stu-id="d93da-175">**Role**</span></span> | <span data-ttu-id="d93da-176">**可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="d93da-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="d93da-177">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-177">MPN partner admin</span></span>|<span data-ttu-id="d93da-178">•查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="d93da-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="d93da-179">•查看法律、公司、商业和 MPN 的配置文件</span><span class="sxs-lookup"><span data-stu-id="d93da-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="d93da-180">•查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="d93da-180">• View user details and their skills data</span></span>
||<span data-ttu-id="d93da-181">•查看称职情况</span><span class="sxs-lookup"><span data-stu-id="d93da-181">• View competencies</span></span>
||<span data-ttu-id="d93da-182">•查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="d93da-182">• View and manage benefits</span></span>
||<span data-ttu-id="d93da-183">•查看和购买 MPN 产品</span><span class="sxs-lookup"><span data-stu-id="d93da-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="d93da-184">•查看 MPN 产品/服务订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="d93da-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="d93da-185">•查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="d93da-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="d93da-186">•可以在凭证验证工具中工作</span><span class="sxs-lookup"><span data-stu-id="d93da-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="d93da-187">-查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="d93da-187">- View customer data analytics</span></span>
|| <span data-ttu-id="d93da-188">查看公司内的其他用户角色, 但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="d93da-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="d93da-189">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-189">Account admin</span></span>| <span data-ttu-id="d93da-190">添加位置</span><span class="sxs-lookup"><span data-stu-id="d93da-190">Add locations</span></span>
|| <span data-ttu-id="d93da-191">管理与你的管理员帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="d93da-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="d93da-192">•为租户中的用户分配角色到非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="d93da-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="d93da-193">•将位置注册到程序中</span><span class="sxs-lookup"><span data-stu-id="d93da-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="d93da-194">管理引用</span><span class="sxs-lookup"><span data-stu-id="d93da-194">Manage referrals</span></span> 

|<span data-ttu-id="d93da-195">**Role**</span><span class="sxs-lookup"><span data-stu-id="d93da-195">**Role**</span></span>|<span data-ttu-id="d93da-196">**可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="d93da-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="d93da-197">引用管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-197">Referrals admin</span></span>       |<span data-ttu-id="d93da-198">•查看、创建和管理业务配置文件</span><span class="sxs-lookup"><span data-stu-id="d93da-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="d93da-199">•接收和管理引用</span><span class="sxs-lookup"><span data-stu-id="d93da-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="d93da-200">•查看、创建和管理共同销售的引用</span><span class="sxs-lookup"><span data-stu-id="d93da-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="d93da-201">•查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="d93da-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="d93da-202">业务档案管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-202">Business profile admin</span></span>   |<span data-ttu-id="d93da-203">•查看、创建和管理业务配置文件</span><span class="sxs-lookup"><span data-stu-id="d93da-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="d93da-204">•查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="d93da-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="d93da-205">管理激励</span><span class="sxs-lookup"><span data-stu-id="d93da-205">Manage incentives</span></span> 

|<span data-ttu-id="d93da-206">**Role**</span><span class="sxs-lookup"><span data-stu-id="d93da-206">**Role**</span></span> | <span data-ttu-id="d93da-207">**可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="d93da-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="d93da-208">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="d93da-208">Incentives admin</span></span>|<span data-ttu-id="d93da-209">•启动和管理激励</span><span class="sxs-lookup"><span data-stu-id="d93da-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="d93da-210">•可以查看和编辑激励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="d93da-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="d93da-211">•可以查看和编辑银行和税务详细信息</span><span class="sxs-lookup"><span data-stu-id="d93da-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="d93da-212">•查看折扣和合作收入</span><span class="sxs-lookup"><span data-stu-id="d93da-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="d93da-213">•访问支持</span><span class="sxs-lookup"><span data-stu-id="d93da-213">• Access support</span></span>
||<span data-ttu-id="d93da-214">•争议奖励付款</span><span class="sxs-lookup"><span data-stu-id="d93da-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="d93da-215">奖励用户</span><span class="sxs-lookup"><span data-stu-id="d93da-215">Incentives user</span></span>|<span data-ttu-id="d93da-216">•可以查看激励计划</span><span class="sxs-lookup"><span data-stu-id="d93da-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="d93da-217">•可以查看并启动激励声明</span><span class="sxs-lookup"><span data-stu-id="d93da-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="d93da-218">•查看折扣和合作收入</span><span class="sxs-lookup"><span data-stu-id="d93da-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="d93da-219">•访问支持</span><span class="sxs-lookup"><span data-stu-id="d93da-219">• Access support</span></span>












