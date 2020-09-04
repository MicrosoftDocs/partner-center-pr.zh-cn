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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040763"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="8d312-103">为需要在合作伙伴中心工作的公司的用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="8d312-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="8d312-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="8d312-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8d312-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-105">Global admin</span></span>
- <span data-ttu-id="8d312-106">用户管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-106">User admin</span></span>
- <span data-ttu-id="8d312-107">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-107">MPN partner admin</span></span>

<span data-ttu-id="8d312-108">你已设置合作伙伴档案，包括法定名称和地址、支持详细信息、税务豁免、银行信息和公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="8d312-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="8d312-109">下一步：为用户设置密码和角色，使他们能够在合作伙伴中心开始与你合作。</span><span class="sxs-lookup"><span data-stu-id="8d312-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="8d312-110">进行设置，使员工能够在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="8d312-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="8d312-111">按分配的角色和权限确定用户对合作伙伴中心拥有访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="8d312-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="8d312-112">角色与企业参与的计划相关。</span><span class="sxs-lookup"><span data-stu-id="8d312-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="8d312-113">例如，如果你的企业是云解决方案提供商 (CSP)，则你只具有标准的 Azure AD 租户管理角色（例如全局管理员），但需要特定于 CSP 计划的角色。</span><span class="sxs-lookup"><span data-stu-id="8d312-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="8d312-114">每个计划都有自身特定的角色。</span><span class="sxs-lookup"><span data-stu-id="8d312-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="8d312-115">Azure Active Directory (AAD) 租户角色包括全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="8d312-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="8d312-116">非 AAD 角色是指不管理租户的角色，包括 MPN 管理员、企业档案管理员、引荐管理员、奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="8d312-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="8d312-117">在合作伙伴中心管理商业交易（Azure AD 和 CSP 角色）</span><span class="sxs-lookup"><span data-stu-id="8d312-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="8d312-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="8d312-118">**Role**</span></span>|<span data-ttu-id="8d312-119">**他们可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="8d312-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="8d312-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-120">Global admin</span></span>|<span data-ttu-id="8d312-121">\*    可以全权访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="8d312-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="8d312-122">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-123">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="8d312-124">\*    查看协议、价目表和套餐</span><span class="sxs-lookup"><span data-stu-id="8d312-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="8d312-125">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="8d312-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="8d312-126">查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="8d312-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="8d312-127">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-127">User management admin</span></span>   | <span data-ttu-id="8d312-128">\*    查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="8d312-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="8d312-129">\*    查看所有合作伙伴档案</span><span class="sxs-lookup"><span data-stu-id="8d312-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="8d312-130">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="8d312-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="8d312-131">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-132">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="8d312-133">计费管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-133">Billing admin</span></span> | <span data-ttu-id="8d312-134">- 查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="8d312-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="8d312-135">\*    查看定价</span><span class="sxs-lookup"><span data-stu-id="8d312-135">\*    View pricing</span></span>
||<span data-ttu-id="8d312-136">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-137">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="8d312-138">默认用户</span><span class="sxs-lookup"><span data-stu-id="8d312-138">Default user</span></span>|  <span data-ttu-id="8d312-139">查看“我的个人资料”</span><span class="sxs-lookup"><span data-stu-id="8d312-139">View My profile</span></span>   |
|<span data-ttu-id="8d312-140">管理员代理</span><span class="sxs-lookup"><span data-stu-id="8d312-140">Admin agent</span></span> | <span data-ttu-id="8d312-141">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="8d312-141">\*    Customer management</span></span>
||<span data-ttu-id="8d312-142">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8d312-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="8d312-143">\*    创建配置文件并将其应用到设备</span><span class="sxs-lookup"><span data-stu-id="8d312-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="8d312-144">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="8d312-144">\*    Subscription management</span></span>
||<span data-ttu-id="8d312-145">\*    客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="8d312-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="8d312-146">\*    请求委派管理员特权</span><span class="sxs-lookup"><span data-stu-id="8d312-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="8d312-147">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="8d312-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="8d312-148">\*    计费</span><span class="sxs-lookup"><span data-stu-id="8d312-148">\*    Billing</span></span>
||<span data-ttu-id="8d312-149">\*    代表客户的管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="8d312-150">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="8d312-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="8d312-151">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-152">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="8d312-153">销售代理</span><span class="sxs-lookup"><span data-stu-id="8d312-153">Sales agent</span></span> | <span data-ttu-id="8d312-154">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="8d312-154">\*    Customer management</span></span>
||<span data-ttu-id="8d312-155">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8d312-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="8d312-156">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="8d312-156">\*    Subscription management</span></span>
||<span data-ttu-id="8d312-157">\*    查看支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-157">\*    View support tickets</span></span>
||<span data-ttu-id="8d312-158">\*    请求与客户建立关系</span><span class="sxs-lookup"><span data-stu-id="8d312-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="8d312-159">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="8d312-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="8d312-160">\*    管理潜在顾客</span><span class="sxs-lookup"><span data-stu-id="8d312-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="8d312-161">\*    查看客户协议</span><span class="sxs-lookup"><span data-stu-id="8d312-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="8d312-162">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="8d312-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="8d312-163">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-164">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="8d312-165">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="8d312-165">Helpdesk agent</span></span>| <span data-ttu-id="8d312-166">\*    搜索和查看客户</span><span class="sxs-lookup"><span data-stu-id="8d312-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="8d312-167">\*    编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="8d312-167">\*    Edit customer details</span></span>
||<span data-ttu-id="8d312-168">\*    帮助解决计费或订阅管理方面的客户问题</span><span class="sxs-lookup"><span data-stu-id="8d312-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="8d312-169">\*    代表客户请求支持</span><span class="sxs-lookup"><span data-stu-id="8d312-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="8d312-170">\*    代表客户管理订阅和计费问题</span><span class="sxs-lookup"><span data-stu-id="8d312-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="8d312-171">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-172">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="8d312-173">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="8d312-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="8d312-174">（CSP 角色和非 AAD 角色）</span><span class="sxs-lookup"><span data-stu-id="8d312-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="8d312-175">CPVs 开发供云解决方案提供商 (CSP) 合作伙伴使用的应用，使其能够将自己的系统与合作伙伴中心 API 相集成。</span><span class="sxs-lookup"><span data-stu-id="8d312-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="8d312-176">**Role**</span><span class="sxs-lookup"><span data-stu-id="8d312-176">**Role**</span></span>   |<span data-ttu-id="8d312-177">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="8d312-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="8d312-178">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-178">Global admin</span></span>| <span data-ttu-id="8d312-179">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="8d312-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="8d312-180">查看和管理需要访问 CPV 功能的任何用户。</span><span class="sxs-lookup"><span data-stu-id="8d312-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="8d312-181">来宾用户（必须已添加到 AAD 租户）</span><span class="sxs-lookup"><span data-stu-id="8d312-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="8d312-182">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="8d312-182">**Guest user**</span></span>   | <span data-ttu-id="8d312-183">**角色**</span><span class="sxs-lookup"><span data-stu-id="8d312-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="8d312-184">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-184">MPN partner admin</span></span>|
||<span data-ttu-id="8d312-185">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-185">Accounts admin</span></span>|
||<span data-ttu-id="8d312-186">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-186">Incentives admin</span></span>|
||<span data-ttu-id="8d312-187">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-187">Business profile admin</span></span>|
||<span data-ttu-id="8d312-188">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="8d312-189">管理 MPN 成员身份和公司（非 AAD 角色：这些角色管理公司业务，而不是管理租户）</span><span class="sxs-lookup"><span data-stu-id="8d312-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="8d312-190">**Role**</span><span class="sxs-lookup"><span data-stu-id="8d312-190">**Role**</span></span> | <span data-ttu-id="8d312-191">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="8d312-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="8d312-192">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-192">MPN partner admin</span></span>|<span data-ttu-id="8d312-193">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="8d312-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="8d312-194">\*    查看法律、公司、业务和 MPN 档案</span><span class="sxs-lookup"><span data-stu-id="8d312-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="8d312-195">\*    查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="8d312-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="8d312-196">\*    查看资质</span><span class="sxs-lookup"><span data-stu-id="8d312-196">\*    View competencies</span></span>
||<span data-ttu-id="8d312-197">\*    查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="8d312-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="8d312-198">\*    查看和购买 MPN 套餐</span><span class="sxs-lookup"><span data-stu-id="8d312-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="8d312-199">\*    查看 MPN 套餐订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="8d312-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="8d312-200">\*    查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="8d312-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="8d312-201">\*    可以操作凭证验证工具</span><span class="sxs-lookup"><span data-stu-id="8d312-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="8d312-202">\*    查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="8d312-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="8d312-203">\*    查看公司内的其他用户角色，但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="8d312-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="8d312-204">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-205">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="8d312-206">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-206">Account admin</span></span>| <span data-ttu-id="8d312-207">添加位置</span><span class="sxs-lookup"><span data-stu-id="8d312-207">Add locations</span></span>
|| <span data-ttu-id="8d312-208">管理你是其管理员的帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="8d312-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="8d312-209">\*    将租户中用户的角色分配为非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="8d312-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="8d312-210">\*    将位置注册到计划</span><span class="sxs-lookup"><span data-stu-id="8d312-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="8d312-211">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-212">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="8d312-213">管理引荐</span><span class="sxs-lookup"><span data-stu-id="8d312-213">Manage referrals</span></span> 

|<span data-ttu-id="8d312-214">**Role**</span><span class="sxs-lookup"><span data-stu-id="8d312-214">**Role**</span></span>|<span data-ttu-id="8d312-215">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="8d312-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="8d312-216">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-216">Referrals admin</span></span>       |<span data-ttu-id="8d312-217">\*    查看、创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="8d312-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="8d312-218">\*    接收和管理引荐</span><span class="sxs-lookup"><span data-stu-id="8d312-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="8d312-219">\* 查看、创建和管理共同销售引荐</span><span class="sxs-lookup"><span data-stu-id="8d312-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="8d312-220">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="8d312-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="8d312-221">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-221">Business profile admin</span></span>   |<span data-ttu-id="8d312-222">\* 查看、创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="8d312-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="8d312-223">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="8d312-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="8d312-224">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-225">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="8d312-226">管理奖励</span><span class="sxs-lookup"><span data-stu-id="8d312-226">Manage incentives</span></span> 

|<span data-ttu-id="8d312-227">**Role**</span><span class="sxs-lookup"><span data-stu-id="8d312-227">**Role**</span></span> | <span data-ttu-id="8d312-228">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="8d312-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8d312-229">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="8d312-229">Incentives admin</span></span>|<span data-ttu-id="8d312-230">\*    发起和管理奖励</span><span class="sxs-lookup"><span data-stu-id="8d312-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="8d312-231">\*    可以查看和编辑奖励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="8d312-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="8d312-232">\*    可以查看和编辑银行与税务详细信息</span><span class="sxs-lookup"><span data-stu-id="8d312-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="8d312-233">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="8d312-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="8d312-234">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="8d312-234">\*    Access support</span></span>
||<span data-ttu-id="8d312-235">\*    对奖励付款提起争议</span><span class="sxs-lookup"><span data-stu-id="8d312-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="8d312-236">奖励用户</span><span class="sxs-lookup"><span data-stu-id="8d312-236">Incentives user</span></span>|<span data-ttu-id="8d312-237">\*    可以查看奖励计划</span><span class="sxs-lookup"><span data-stu-id="8d312-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="8d312-238">\*    可以查看和发起奖励申请</span><span class="sxs-lookup"><span data-stu-id="8d312-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="8d312-239">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="8d312-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="8d312-240">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8d312-241">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="8d312-242">查看合作伙伴中心见解数据</span><span class="sxs-lookup"><span data-stu-id="8d312-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="8d312-243">**Role**</span><span class="sxs-lookup"><span data-stu-id="8d312-243">**Role**</span></span> | <span data-ttu-id="8d312-244">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="8d312-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8d312-245">主管人员报表查看器</span><span class="sxs-lookup"><span data-stu-id="8d312-245">Executive report viewer</span></span>|<span data-ttu-id="8d312-246">访问所有报告数据集，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="8d312-247">报表查看器</span><span class="sxs-lookup"><span data-stu-id="8d312-247">Report viewer</span></span>|<span data-ttu-id="8d312-248">访问不包括收入与客户和员工个人数据的数据报告，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="8d312-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
