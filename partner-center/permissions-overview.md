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
ms.openlocfilehash: b1ac34bbb92d600805465ca5f6d1b28af54cd5e1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855125"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="174e2-103">为需要在合作伙伴中心工作的公司的用户分配用户角色和权限</span><span class="sxs-lookup"><span data-stu-id="174e2-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="174e2-104">**相应的角色**：全局管理员 |“用户管理”管理员 | MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-104">**Appropriate roles**: Global admin | User management admin | MPN partner admin</span></span>

<span data-ttu-id="174e2-105">你已设置合作伙伴档案，包括法定名称和地址、支持详细信息、税务豁免、银行信息和公司的主要联系人。</span><span class="sxs-lookup"><span data-stu-id="174e2-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="174e2-106">下一步：为用户设置密码和角色，使他们能够在合作伙伴中心开始与你合作。</span><span class="sxs-lookup"><span data-stu-id="174e2-106">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="174e2-107">进行设置，使员工能够在合作伙伴中心工作</span><span class="sxs-lookup"><span data-stu-id="174e2-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="174e2-108">按分配的角色和权限确定用户对合作伙伴中心拥有访问权限类型。</span><span class="sxs-lookup"><span data-stu-id="174e2-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="174e2-109">角色与企业参与的计划相关。</span><span class="sxs-lookup"><span data-stu-id="174e2-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="174e2-110">例如，如果你的企业是云解决方案提供商 (CSP)，则你只具有标准的 Azure Active Directory 租户管理角色（例如全局管理员），但却需要 CSP 计划特定的角色。</span><span class="sxs-lookup"><span data-stu-id="174e2-110">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="174e2-111">每个计划都有自身特定的角色。</span><span class="sxs-lookup"><span data-stu-id="174e2-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="174e2-112">Azure Active Directory 租户角色包括全局管理员、用户管理员和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="174e2-112">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="174e2-113">非 Azure Active Directory 角色是指不管理租户的角色，包括 MPN 管理员、企业档案管理员、引荐管理员、奖励管理员和奖励用户。</span><span class="sxs-lookup"><span data-stu-id="174e2-113">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="174e2-114">在合作伙伴中心管理商业交易（Azure AD 和 CSP 角色）</span><span class="sxs-lookup"><span data-stu-id="174e2-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="174e2-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="174e2-115">**Role**</span></span>|<span data-ttu-id="174e2-116">**他们可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-116">**What they can do**</span></span>|<span data-ttu-id="174e2-117">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="174e2-117">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="174e2-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-118">Global admin</span></span>|<span data-ttu-id="174e2-119">\*    可以全权访问所有 Microsoft 帐户/服务</span><span class="sxs-lookup"><span data-stu-id="174e2-119">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="174e2-120">管理合作伙伴中心帐户</span><span class="sxs-lookup"><span data-stu-id="174e2-120">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="174e2-121">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-121">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-122">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-122">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="174e2-123">\*    查看协议、价目表和套餐</span><span class="sxs-lookup"><span data-stu-id="174e2-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="174e2-124">\*    查看、创建和管理合作伙伴用户</span><span class="sxs-lookup"><span data-stu-id="174e2-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="174e2-125">查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="174e2-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="174e2-126">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-126">User management admin</span></span>   | <span data-ttu-id="174e2-127">\*    查看、创建和管理用户</span><span class="sxs-lookup"><span data-stu-id="174e2-127">\*    View, create, and manage users</span></span>|[<span data-ttu-id="174e2-128">在合作伙伴中心管理 Microsoft 合作伙伴网络成员资格权益和优惠</span><span class="sxs-lookup"><span data-stu-id="174e2-128">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="174e2-129">\*    查看所有合作伙伴档案</span><span class="sxs-lookup"><span data-stu-id="174e2-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="174e2-130">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-130">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-131">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-131">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="174e2-132">计费管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-132">Billing admin</span></span> | <span data-ttu-id="174e2-133">- 查看、创建和管理帐单、发票与对帐文件</span><span class="sxs-lookup"><span data-stu-id="174e2-133">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="174e2-134">阅读账单</span><span class="sxs-lookup"><span data-stu-id="174e2-134">Read your bill</span></span>](billing.md)
||<span data-ttu-id="174e2-135">\*    查看定价</span><span class="sxs-lookup"><span data-stu-id="174e2-135">\*    View pricing</span></span>
||<span data-ttu-id="174e2-136">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-137">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="174e2-138">默认用户</span><span class="sxs-lookup"><span data-stu-id="174e2-138">Default user</span></span>|  <span data-ttu-id="174e2-139">查看“我的个人资料”</span><span class="sxs-lookup"><span data-stu-id="174e2-139">View My profile</span></span>   |[<span data-ttu-id="174e2-140">重置密码</span><span class="sxs-lookup"><span data-stu-id="174e2-140">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="174e2-141">管理员代理</span><span class="sxs-lookup"><span data-stu-id="174e2-141">Admin agent</span></span> | <span data-ttu-id="174e2-142">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="174e2-142">\*    Customer management</span></span>|[<span data-ttu-id="174e2-143">与客户联系</span><span class="sxs-lookup"><span data-stu-id="174e2-143">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="174e2-144">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="174e2-144">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="174e2-145">\*    创建配置文件并将其应用到设备</span><span class="sxs-lookup"><span data-stu-id="174e2-145">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="174e2-146">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="174e2-146">\*    Subscription management</span></span>
||<span data-ttu-id="174e2-147">\*    客户的服务运行状况和服务请求</span><span class="sxs-lookup"><span data-stu-id="174e2-147">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="174e2-148">\*    请求委派管理员特权</span><span class="sxs-lookup"><span data-stu-id="174e2-148">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="174e2-149">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="174e2-149">\*    View pricing and offers</span></span>
||<span data-ttu-id="174e2-150">\*    计费</span><span class="sxs-lookup"><span data-stu-id="174e2-150">\*    Billing</span></span>
||<span data-ttu-id="174e2-151">\*    代表客户的管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-151">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="174e2-152">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="174e2-152">\*    Register a value added reseller</span></span>
||<span data-ttu-id="174e2-153">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-153">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-154">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-154">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="174e2-155">销售代理</span><span class="sxs-lookup"><span data-stu-id="174e2-155">Sales agent</span></span> | <span data-ttu-id="174e2-156">\*    客户管理</span><span class="sxs-lookup"><span data-stu-id="174e2-156">\*    Customer management</span></span>|[<span data-ttu-id="174e2-157">为客户提供计费支持并帮助解答计费问题</span><span class="sxs-lookup"><span data-stu-id="174e2-157">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="174e2-158">\*    将设备列表添加到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="174e2-158">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="174e2-159">\*    订阅管理</span><span class="sxs-lookup"><span data-stu-id="174e2-159">\*    Subscription management</span></span>
||<span data-ttu-id="174e2-160">\*    查看支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-160">\*    View support tickets</span></span>
||<span data-ttu-id="174e2-161">\*    请求与客户建立关系</span><span class="sxs-lookup"><span data-stu-id="174e2-161">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="174e2-162">\*    查看定价和套餐</span><span class="sxs-lookup"><span data-stu-id="174e2-162">\*    View pricing and offers</span></span>
||<span data-ttu-id="174e2-163">\*    管理潜在顾客</span><span class="sxs-lookup"><span data-stu-id="174e2-163">\*    Manage customer leads</span></span>
||<span data-ttu-id="174e2-164">\*    查看客户协议</span><span class="sxs-lookup"><span data-stu-id="174e2-164">\*    View the customer agreement</span></span>
||<span data-ttu-id="174e2-165">\*    注册增值经销商</span><span class="sxs-lookup"><span data-stu-id="174e2-165">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="174e2-166">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-166">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-167">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-167">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="174e2-168">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="174e2-168">Helpdesk agent</span></span>| <span data-ttu-id="174e2-169">\*    搜索和查看客户</span><span class="sxs-lookup"><span data-stu-id="174e2-169">\*    Search for and view a customer</span></span>|[<span data-ttu-id="174e2-170">将问题报告给 Microsoft 并了解哪些问题更适合进行报告</span><span class="sxs-lookup"><span data-stu-id="174e2-170">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="174e2-171">\*    编辑客户详细信息</span><span class="sxs-lookup"><span data-stu-id="174e2-171">\*    Edit customer details</span></span>
||<span data-ttu-id="174e2-172">\*    帮助解决计费或订阅管理方面的客户问题</span><span class="sxs-lookup"><span data-stu-id="174e2-172">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="174e2-173">\*    代表客户请求支持</span><span class="sxs-lookup"><span data-stu-id="174e2-173">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="174e2-174">\*    代表客户管理订阅和计费问题</span><span class="sxs-lookup"><span data-stu-id="174e2-174">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="174e2-175">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-175">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-176">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-176">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="174e2-177">控制面板供应商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="174e2-177">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="174e2-178">（CSP 角色和非 Azure AD 角色）</span><span class="sxs-lookup"><span data-stu-id="174e2-178">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="174e2-179">CPVs 开发供云解决方案提供商 (CSP) 合作伙伴使用的应用，使其能够将自己的系统与合作伙伴中心 API 相集成。</span><span class="sxs-lookup"><span data-stu-id="174e2-179">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="174e2-180">**Role**</span><span class="sxs-lookup"><span data-stu-id="174e2-180">**Role**</span></span>   |<span data-ttu-id="174e2-181">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-181">**What you can do**</span></span>|<span data-ttu-id="174e2-182">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="174e2-182">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="174e2-183">全局管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-183">Global admin</span></span>| <span data-ttu-id="174e2-184">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="174e2-184">View and manage your CPV profile</span></span>|[<span data-ttu-id="174e2-185">注册为控制面板供应商来帮助将 CSP 合作伙伴系统和合作伙伴中心 API 进行集成</span><span class="sxs-lookup"><span data-stu-id="174e2-185">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="174e2-186">查看和管理需要访问 CPV 功能的任何用户。</span><span class="sxs-lookup"><span data-stu-id="174e2-186">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="174e2-187">来宾用户（必须添加到 Azure Active Directory 租户中）</span><span class="sxs-lookup"><span data-stu-id="174e2-187">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="174e2-188">**来宾用户**</span><span class="sxs-lookup"><span data-stu-id="174e2-188">**Guest user**</span></span>   | <span data-ttu-id="174e2-189">**角色**</span><span class="sxs-lookup"><span data-stu-id="174e2-189">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="174e2-190">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-190">MPN partner admin</span></span>|
||<span data-ttu-id="174e2-191">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-191">Business profile admin</span></span>|
||<span data-ttu-id="174e2-192">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-192">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="174e2-193">管理 MPN 成员资格和你的公司</span><span class="sxs-lookup"><span data-stu-id="174e2-193">Manage MPN membership and your company</span></span> 

<span data-ttu-id="174e2-194">这些角色并非 Azure Active Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="174e2-194">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="174e2-195">这些角色负责管理公司业务，而不是租户。</span><span class="sxs-lookup"><span data-stu-id="174e2-195">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="174e2-196">**Role**</span><span class="sxs-lookup"><span data-stu-id="174e2-196">**Role**</span></span> | <span data-ttu-id="174e2-197">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-197">**What you can do**</span></span>|<span data-ttu-id="174e2-198">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="174e2-198">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="174e2-199">MPN 合作伙伴管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-199">MPN partner admin</span></span>|<span data-ttu-id="174e2-200">\*    查看、创建和管理合作伙伴服务请求</span><span class="sxs-lookup"><span data-stu-id="174e2-200">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="174e2-201">购买或续订 Microsoft Action Pack 订阅或白银和黄金资格</span><span class="sxs-lookup"><span data-stu-id="174e2-201">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="174e2-202">\*    查看法律、公司、业务和 MPN 档案</span><span class="sxs-lookup"><span data-stu-id="174e2-202">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="174e2-203">\*    查看用户详细信息及其技能数据</span><span class="sxs-lookup"><span data-stu-id="174e2-203">\*    View user details and their skills data</span></span>
||<span data-ttu-id="174e2-204">\*    查看资质</span><span class="sxs-lookup"><span data-stu-id="174e2-204">\*    View competencies</span></span>
||<span data-ttu-id="174e2-205">\*    查看和管理权益</span><span class="sxs-lookup"><span data-stu-id="174e2-205">\*    View and manage benefits</span></span>
||<span data-ttu-id="174e2-206">\*    查看和购买 MPN 套餐</span><span class="sxs-lookup"><span data-stu-id="174e2-206">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="174e2-207">\*    查看 MPN 套餐订单历史记录和发票</span><span class="sxs-lookup"><span data-stu-id="174e2-207">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="174e2-208">\*    查看合作伙伴贡献指标数据</span><span class="sxs-lookup"><span data-stu-id="174e2-208">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="174e2-209">\*    可以操作凭证验证工具</span><span class="sxs-lookup"><span data-stu-id="174e2-209">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="174e2-210">\*    查看客户数据分析</span><span class="sxs-lookup"><span data-stu-id="174e2-210">\*    View customer data analytics</span></span>
||<span data-ttu-id="174e2-211">\*    查看公司内的其他用户角色，但不能分配角色</span><span class="sxs-lookup"><span data-stu-id="174e2-211">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="174e2-212">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-212">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-213">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-213">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="174e2-214">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-214">Account admin</span></span>| <span data-ttu-id="174e2-215">添加位置</span><span class="sxs-lookup"><span data-stu-id="174e2-215">Add locations</span></span>|[<span data-ttu-id="174e2-216">管理位置</span><span class="sxs-lookup"><span data-stu-id="174e2-216">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="174e2-217">管理你是其管理员的帐户相关的配置文件</span><span class="sxs-lookup"><span data-stu-id="174e2-217">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="174e2-218">\*    将租户中用户的角色分配给非 Azure Active Directory 角色</span><span class="sxs-lookup"><span data-stu-id="174e2-218">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="174e2-219">\*    将位置注册到计划</span><span class="sxs-lookup"><span data-stu-id="174e2-219">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="174e2-220">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-220">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-221">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-221">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="174e2-222">管理引荐</span><span class="sxs-lookup"><span data-stu-id="174e2-222">Manage referrals</span></span>

|<span data-ttu-id="174e2-223">**Role**</span><span class="sxs-lookup"><span data-stu-id="174e2-223">**Role**</span></span> | <span data-ttu-id="174e2-224">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-224">**What you can do**</span></span>|<span data-ttu-id="174e2-225">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="174e2-225">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="174e2-226">引荐管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-226">Referrals admin</span></span>|<span data-ttu-id="174e2-227">在合作伙伴中心的“引荐”选项卡下创建和管理所有内容</span><span class="sxs-lookup"><span data-stu-id="174e2-227">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="174e2-228">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="174e2-228">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="174e2-229">可查看和编辑所有联合销售机会和潜在客户</span><span class="sxs-lookup"><span data-stu-id="174e2-229">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="174e2-230">可为交易分配团队成员</span><span class="sxs-lookup"><span data-stu-id="174e2-230">Can assign team members for a deal</span></span>
||    <span data-ttu-id="174e2-231">可查看和编辑企业档案</span><span class="sxs-lookup"><span data-stu-id="174e2-231">Can view and edit business profiles</span></span>
||    <span data-ttu-id="174e2-232">可查看和登记标记为“已赢得”且有资格登记交易的机会的交易</span><span class="sxs-lookup"><span data-stu-id="174e2-232">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="174e2-233">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-233">Can create and view support tickets</span></span>
|<span data-ttu-id="174e2-234">引荐用户</span><span class="sxs-lookup"><span data-stu-id="174e2-234">Referrals user</span></span>|<span data-ttu-id="174e2-235">只有当联合销售机会属于团队时才可创建和管理它们</span><span class="sxs-lookup"><span data-stu-id="174e2-235">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="174e2-236">管理联合销售机会</span><span class="sxs-lookup"><span data-stu-id="174e2-236">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="174e2-237">可为联合销售机会已分配有角色的位置创建这些机会。</span><span class="sxs-lookup"><span data-stu-id="174e2-237">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="174e2-238">可查看和登记标记为“已赢得”且有资格登记交易（如果属于团队）的机会的交易。</span><span class="sxs-lookup"><span data-stu-id="174e2-238">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="174e2-239">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-239">Can create and view support tickets</span></span>
|<span data-ttu-id="174e2-240">企业档案管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-240">Business profile admin</span></span>|<span data-ttu-id="174e2-241">创建和管理企业档案</span><span class="sxs-lookup"><span data-stu-id="174e2-241">Create and manage business profiles</span></span> | [<span data-ttu-id="174e2-242">管理企业档案</span><span class="sxs-lookup"><span data-stu-id="174e2-242">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="174e2-243">可创建和查看支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-243">Can create and view support tickets</span></span>

<span data-ttu-id="174e2-244">除了新的引荐用户角色，我们还将为交易引入位置范围。</span><span class="sxs-lookup"><span data-stu-id="174e2-244">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="174e2-245">下表说明了基于位置的交易访问权限。</span><span class="sxs-lookup"><span data-stu-id="174e2-245">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="174e2-246">**范围**</span><span class="sxs-lookup"><span data-stu-id="174e2-246">**Scope**</span></span> | <span data-ttu-id="174e2-247">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-247">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="174e2-248">整个公司</span><span class="sxs-lookup"><span data-stu-id="174e2-248">Entire company</span></span> | <span data-ttu-id="174e2-249">管理员和用户都有权为其所在公司的任何位置创建交易</span><span class="sxs-lookup"><span data-stu-id="174e2-249">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="174e2-250">引荐管理员有权查看和编辑所有交易</span><span class="sxs-lookup"><span data-stu-id="174e2-250">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="174e2-251">只有当交易属于团队时，引荐用户才有权查看和编辑所有这些交易</span><span class="sxs-lookup"><span data-stu-id="174e2-251">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="174e2-252">一个或多个位置</span><span class="sxs-lookup"><span data-stu-id="174e2-252">One or more locations</span></span> | <span data-ttu-id="174e2-253">管理员和用户都有权为其所在公司中分配的位置创建交易</span><span class="sxs-lookup"><span data-stu-id="174e2-253">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="174e2-254">引荐管理员有权查看和编辑属于已分配的位置的所有交易</span><span class="sxs-lookup"><span data-stu-id="174e2-254">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="174e2-255">引荐用户有权查看和编辑属于已分配的位置且属于团队的所有交易</span><span class="sxs-lookup"><span data-stu-id="174e2-255">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="174e2-256">管理奖励</span><span class="sxs-lookup"><span data-stu-id="174e2-256">Manage incentives</span></span>

|<span data-ttu-id="174e2-257">**Role**</span><span class="sxs-lookup"><span data-stu-id="174e2-257">**Role**</span></span> | <span data-ttu-id="174e2-258">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-258">**What you can do**</span></span>|<span data-ttu-id="174e2-259">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="174e2-259">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="174e2-260">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="174e2-260">Incentives admin</span></span>|<span data-ttu-id="174e2-261">\*    发起和管理奖励</span><span class="sxs-lookup"><span data-stu-id="174e2-261">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="174e2-262">使用这些资源来帮助你立即体验激励</span><span class="sxs-lookup"><span data-stu-id="174e2-262">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="174e2-263">\*    可以查看和编辑奖励计划的所有方面</span><span class="sxs-lookup"><span data-stu-id="174e2-263">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="174e2-264">\*    可以查看和编辑银行与税务详细信息</span><span class="sxs-lookup"><span data-stu-id="174e2-264">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="174e2-265">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="174e2-265">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="174e2-266">\*    访问支持</span><span class="sxs-lookup"><span data-stu-id="174e2-266">\*    Access support</span></span>
||<span data-ttu-id="174e2-267">\*    对奖励付款提起争议</span><span class="sxs-lookup"><span data-stu-id="174e2-267">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="174e2-268">奖励用户</span><span class="sxs-lookup"><span data-stu-id="174e2-268">Incentives user</span></span>|<span data-ttu-id="174e2-269">\*    可以查看奖励计划</span><span class="sxs-lookup"><span data-stu-id="174e2-269">\*    Can view incentives programs</span></span>
||<span data-ttu-id="174e2-270">\*    可以查看和发起奖励申请</span><span class="sxs-lookup"><span data-stu-id="174e2-270">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="174e2-271">\*    查看回扣与合作收益</span><span class="sxs-lookup"><span data-stu-id="174e2-271">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="174e2-272">\*    创建合作伙伴中心的支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-272">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="174e2-273">\*    查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-273">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="174e2-274">查看合作伙伴中心见解数据</span><span class="sxs-lookup"><span data-stu-id="174e2-274">View Partner Center Insights data</span></span>

|<span data-ttu-id="174e2-275">**Role**</span><span class="sxs-lookup"><span data-stu-id="174e2-275">**Role**</span></span> | <span data-ttu-id="174e2-276">**你可以执行的操作**</span><span class="sxs-lookup"><span data-stu-id="174e2-276">**What you can do**</span></span>|<span data-ttu-id="174e2-277">**了解详细信息**</span><span class="sxs-lookup"><span data-stu-id="174e2-277">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="174e2-278">主管人员报表查看器</span><span class="sxs-lookup"><span data-stu-id="174e2-278">Executive report viewer</span></span>|<span data-ttu-id="174e2-279">访问所有报告数据集，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-279">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="174e2-280">简要介绍合作伙伴中心见解内提供的仪表板报表</span><span class="sxs-lookup"><span data-stu-id="174e2-280">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="174e2-281">报表查看器</span><span class="sxs-lookup"><span data-stu-id="174e2-281">Report viewer</span></span>|<span data-ttu-id="174e2-282">访问不包括收入与客户和员工个人数据的数据报告，创建合作伙伴支持票证，查看你创建的合作伙伴支持票证</span><span class="sxs-lookup"><span data-stu-id="174e2-282">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="174e2-283">后续步骤</span><span class="sxs-lookup"><span data-stu-id="174e2-283">Next steps</span></span>

- [<span data-ttu-id="174e2-284">创建用户帐户并分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="174e2-284">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="174e2-285">注册加入新的合作伙伴中心计划时验证你的帐户信息</span><span class="sxs-lookup"><span data-stu-id="174e2-285">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
