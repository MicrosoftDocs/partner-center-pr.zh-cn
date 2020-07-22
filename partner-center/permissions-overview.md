---
title: 向用户分配角色和权限
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解哪些角色最适合你所在公司的用户，这些用户在合作伙伴中心管理商业交易、引荐、奖励或 MPN 成员资格。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434316"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="a3857-103">为需要在合作伙伴中心工作的公司的用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="a3857-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="a3857-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="a3857-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a3857-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-105">Global admin</span></span>
- <span data-ttu-id="a3857-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-106">User admin</span></span>
- <span data-ttu-id="a3857-107">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-107">MPN partner admin</span></span>

<span data-ttu-id="a3857-108">你已设置合作伙伴档案，包括法定名称和地址、支持详细信息、税务豁免、银行信息和公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="a3857-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="a3857-109">下一步：为用户设置密码和角色，使他们能够在合作伙伴中心开始与你合作。</span><span class="sxs-lookup"><span data-stu-id="a3857-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="a3857-110">进行设置，使员工能够在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="a3857-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="a3857-111">按分配的角色和权限确定用户对合作伙伴中心拥有访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="a3857-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="a3857-112">角色与企业参与的计划相关。</span><span class="sxs-lookup"><span data-stu-id="a3857-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="a3857-113">例如，如果你的企业是云解决方案提供商 (CSP)，则你只具有标准的 Azure AD 租户管理角色（例如全局管理员），但需要特定于 CSP 计划的角色。</span><span class="sxs-lookup"><span data-stu-id="a3857-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="a3857-114">每个计划都有自身特定的角色。</span><span class="sxs-lookup"><span data-stu-id="a3857-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="a3857-115">Azure Active Directory (AAD) 租户角色包括全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="a3857-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="a3857-116">非 AAD 角色是指不管理租户的角色，包括 MPN 管理员、企业档案管理员、引荐管理员、奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="a3857-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="a3857-117">在合作伙伴中心管理商业交易（Azure AD 和 CSP 角色）</span><span class="sxs-lookup"><span data-stu-id="a3857-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="a3857-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="a3857-118">**Role**</span></span>|<span data-ttu-id="a3857-119">**他们可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a3857-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="a3857-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-120">Global admin</span></span>|<span data-ttu-id="a3857-121">\*    可以全权访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="a3857-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="a3857-122">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="a3857-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a3857-123">\*    查看协议、价目表和套餐</span><span class="sxs-lookup"><span data-stu-id="a3857-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="a3857-124">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="a3857-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="a3857-125">查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="a3857-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="a3857-126">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-126">User management admin</span></span>   | <span data-ttu-id="a3857-127">\*    查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="a3857-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="a3857-128">\*    查看所有合作伙伴档案</span><span class="sxs-lookup"><span data-stu-id="a3857-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="a3857-129">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="a3857-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="a3857-130">计费管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-130">Billing admin</span></span> | <span data-ttu-id="a3857-131">- 查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="a3857-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="a3857-132">默认用户</span><span class="sxs-lookup"><span data-stu-id="a3857-132">Default user</span></span>|  <span data-ttu-id="a3857-133">查看“我的个人资料”</span><span class="sxs-lookup"><span data-stu-id="a3857-133">View My profile</span></span>   |
|<span data-ttu-id="a3857-134">管理员代理</span><span class="sxs-lookup"><span data-stu-id="a3857-134">Admin agent</span></span> | <span data-ttu-id="a3857-135">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="a3857-135">\*    Customer management</span></span>
||<span data-ttu-id="a3857-136">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="a3857-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a3857-137">\*    创建配置文件并将其应用到设备</span><span class="sxs-lookup"><span data-stu-id="a3857-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="a3857-138">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="a3857-138">\*    Subscription management</span></span>
||<span data-ttu-id="a3857-139">\*    客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="a3857-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="a3857-140">\*    请求委派管理员特权</span><span class="sxs-lookup"><span data-stu-id="a3857-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="a3857-141">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="a3857-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="a3857-142">\*    计费</span><span class="sxs-lookup"><span data-stu-id="a3857-142">\*    Billing</span></span>
||<span data-ttu-id="a3857-143">\*    代表客户的管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="a3857-144">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="a3857-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="a3857-145">销售代理</span><span class="sxs-lookup"><span data-stu-id="a3857-145">Sales agent</span></span> | <span data-ttu-id="a3857-146">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="a3857-146">\*    Customer management</span></span>
||<span data-ttu-id="a3857-147">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="a3857-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a3857-148">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="a3857-148">\*    Subscription management</span></span>
||<span data-ttu-id="a3857-149">\*    查看支持票证</span><span class="sxs-lookup"><span data-stu-id="a3857-149">\*    View support tickets</span></span>
||<span data-ttu-id="a3857-150">\*    请求与客户建立关系</span><span class="sxs-lookup"><span data-stu-id="a3857-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="a3857-151">\*    管理潜在顾客</span><span class="sxs-lookup"><span data-stu-id="a3857-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="a3857-152">\*    查看客户协议</span><span class="sxs-lookup"><span data-stu-id="a3857-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="a3857-153">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="a3857-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="a3857-154">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="a3857-154">Helpdesk agent</span></span>| <span data-ttu-id="a3857-155">\*    搜索和查看客户</span><span class="sxs-lookup"><span data-stu-id="a3857-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="a3857-156">\*    编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="a3857-156">\*    Edit customer details</span></span>
||<span data-ttu-id="a3857-157">\*    帮助解决计费或订阅管理方面的客户问题</span><span class="sxs-lookup"><span data-stu-id="a3857-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="a3857-158">\*    代表客户请求支持</span><span class="sxs-lookup"><span data-stu-id="a3857-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="a3857-159">\*    代表客户管理订阅和计费问题</span><span class="sxs-lookup"><span data-stu-id="a3857-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="a3857-160">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="a3857-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="a3857-161">（CSP 角色和非 AAD 角色）</span><span class="sxs-lookup"><span data-stu-id="a3857-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="a3857-162">CPVs 开发供云解决方案提供商 (CSP) 合作伙伴使用的应用，使其能够将自己的系统与合作伙伴中心 API 相集成。</span><span class="sxs-lookup"><span data-stu-id="a3857-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="a3857-163">**Role**</span><span class="sxs-lookup"><span data-stu-id="a3857-163">**Role**</span></span>   |<span data-ttu-id="a3857-164">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a3857-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="a3857-165">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-165">Global admin</span></span>| <span data-ttu-id="a3857-166">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="a3857-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="a3857-167">查看和管理需要访问 CPV 功能的任何用户。</span><span class="sxs-lookup"><span data-stu-id="a3857-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="a3857-168">来宾用户（必须已添加到 AAD 租户）</span><span class="sxs-lookup"><span data-stu-id="a3857-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="a3857-169">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="a3857-169">**Guest user**</span></span>   | <span data-ttu-id="a3857-170">**角色**</span><span class="sxs-lookup"><span data-stu-id="a3857-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="a3857-171">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-171">MPN partner admin</span></span>|
||<span data-ttu-id="a3857-172">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-172">Accounts admin</span></span>|
||<span data-ttu-id="a3857-173">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-173">Incentives admin</span></span>|
||<span data-ttu-id="a3857-174">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-174">Business profile admin</span></span>|
||<span data-ttu-id="a3857-175">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="a3857-176">管理 MPN 成员身份和公司（非 AAD 角色：这些角色管理公司业务，而不是管理租户）</span><span class="sxs-lookup"><span data-stu-id="a3857-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="a3857-177">**Role**</span><span class="sxs-lookup"><span data-stu-id="a3857-177">**Role**</span></span> | <span data-ttu-id="a3857-178">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a3857-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="a3857-179">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-179">MPN partner admin</span></span>|<span data-ttu-id="a3857-180">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="a3857-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="a3857-181">\*    查看法律、公司、业务和 MPN 档案</span><span class="sxs-lookup"><span data-stu-id="a3857-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="a3857-182">\*    查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="a3857-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="a3857-183">\*    查看资质</span><span class="sxs-lookup"><span data-stu-id="a3857-183">\*    View competencies</span></span>
||<span data-ttu-id="a3857-184">\*    查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="a3857-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="a3857-185">\*    查看和购买 MPN 套餐</span><span class="sxs-lookup"><span data-stu-id="a3857-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="a3857-186">\*    查看 MPN 套餐订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="a3857-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="a3857-187">\*    查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="a3857-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="a3857-188">\*    可以操作凭证验证工具</span><span class="sxs-lookup"><span data-stu-id="a3857-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="a3857-189">\*    查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="a3857-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="a3857-190">\*    查看公司内的其他用户角色，但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="a3857-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="a3857-191">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-191">Account admin</span></span>| <span data-ttu-id="a3857-192">添加位置</span><span class="sxs-lookup"><span data-stu-id="a3857-192">Add locations</span></span>
|| <span data-ttu-id="a3857-193">管理你是其管理员的帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="a3857-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="a3857-194">\*    将租户中用户的角色分配为非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="a3857-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="a3857-195">\*    将位置注册到计划</span><span class="sxs-lookup"><span data-stu-id="a3857-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="a3857-196">管理引荐</span><span class="sxs-lookup"><span data-stu-id="a3857-196">Manage referrals</span></span> 

|<span data-ttu-id="a3857-197">**Role**</span><span class="sxs-lookup"><span data-stu-id="a3857-197">**Role**</span></span>|<span data-ttu-id="a3857-198">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a3857-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="a3857-199">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-199">Referrals admin</span></span>       |<span data-ttu-id="a3857-200">\*    查看、创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="a3857-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="a3857-201">\*    接收和管理引荐</span><span class="sxs-lookup"><span data-stu-id="a3857-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="a3857-202">\* 查看、创建和管理共同销售引荐</span><span class="sxs-lookup"><span data-stu-id="a3857-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="a3857-203">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="a3857-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="a3857-204">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-204">Business profile admin</span></span>   |<span data-ttu-id="a3857-205">\* 查看、创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="a3857-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="a3857-206">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="a3857-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="a3857-207">管理奖励</span><span class="sxs-lookup"><span data-stu-id="a3857-207">Manage incentives</span></span> 

|<span data-ttu-id="a3857-208">**Role**</span><span class="sxs-lookup"><span data-stu-id="a3857-208">**Role**</span></span> | <span data-ttu-id="a3857-209">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a3857-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="a3857-210">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="a3857-210">Incentives admin</span></span>|<span data-ttu-id="a3857-211">\*    发起和管理奖励</span><span class="sxs-lookup"><span data-stu-id="a3857-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="a3857-212">\*    可以查看和编辑奖励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="a3857-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="a3857-213">\*    可以查看和编辑银行与税务详细信息</span><span class="sxs-lookup"><span data-stu-id="a3857-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="a3857-214">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="a3857-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a3857-215">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="a3857-215">\*    Access support</span></span>
||<span data-ttu-id="a3857-216">\*    对奖励付款提起争议</span><span class="sxs-lookup"><span data-stu-id="a3857-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="a3857-217">奖励用户</span><span class="sxs-lookup"><span data-stu-id="a3857-217">Incentives user</span></span>|<span data-ttu-id="a3857-218">\*    可以查看奖励计划</span><span class="sxs-lookup"><span data-stu-id="a3857-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="a3857-219">\*    可以查看和发起奖励申请</span><span class="sxs-lookup"><span data-stu-id="a3857-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="a3857-220">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="a3857-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a3857-221">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="a3857-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="a3857-222">查看合作伙伴中心见解数据</span><span class="sxs-lookup"><span data-stu-id="a3857-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="a3857-223">**Role**</span><span class="sxs-lookup"><span data-stu-id="a3857-223">**Role**</span></span> | <span data-ttu-id="a3857-224">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="a3857-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="a3857-225">主管人员报表查看器</span><span class="sxs-lookup"><span data-stu-id="a3857-225">Executive report viewer</span></span>|<span data-ttu-id="a3857-226">访问所有报告数据集</span><span class="sxs-lookup"><span data-stu-id="a3857-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="a3857-227">报表查看器</span><span class="sxs-lookup"><span data-stu-id="a3857-227">Report viewer</span></span>|<span data-ttu-id="a3857-228">访问不包括收入与客户和员工个人数据的数据报告</span><span class="sxs-lookup"><span data-stu-id="a3857-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    