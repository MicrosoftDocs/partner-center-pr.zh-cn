---
title: "Azure Active Directory 租户和合作伙伴中心 | 合作伙伴中心"
description: "若要创建合作伙伴中心帐户，你的公司必须拥有 Azure Active Directory (Azure AD) 租户。 Azure AD 是 Microsoft 的基于云的目录和标识管理服务。"
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="d23c3-104">Azure Active Directory 租户和合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="d23c3-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="d23c3-105">适用于</span><span class="sxs-lookup"><span data-stu-id="d23c3-105">Applies to</span></span>**

-  <span data-ttu-id="d23c3-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="d23c3-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="d23c3-107">为什么需要 Azure AD 租户</span><span class="sxs-lookup"><span data-stu-id="d23c3-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="d23c3-108">我们需要将你的组织 Azure AD 租户链接到新的合作伙伴中心帐户，以便你的租户用户可以使用其 Azure AD（Microsoft 帐户）用户名和密码登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="d23c3-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="d23c3-109">如果你的公司已经拥有 Azure AD 租户，你可以将其链接到你的合作伙伴中心帐户。</span><span class="sxs-lookup"><span data-stu-id="d23c3-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="d23c3-110">注意</span><span class="sxs-lookup"><span data-stu-id="d23c3-110">Note</span></span>**<br> <span data-ttu-id="d23c3-111">在你决定使用现有的 Azure AD 租户之前，请考虑租户中将需要使用合作伙伴中心的用户数。</span><span class="sxs-lookup"><span data-stu-id="d23c3-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="d23c3-112">如果租户中有些用户不需要使用合作伙伴中心，请考虑只为将需要使用合作伙伴中心的那些用户创建一个新租户。</span><span class="sxs-lookup"><span data-stu-id="d23c3-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="d23c3-113">如果你的公司还没有 Azure AD 租户，则可以在注册过程中免费创建一个。</span><span class="sxs-lookup"><span data-stu-id="d23c3-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="d23c3-114">在**登录 Azure Active Directory** 页面上选择**创建新租户**。</span><span class="sxs-lookup"><span data-stu-id="d23c3-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="d23c3-115">不确定你的公司是否已经具有 Azure AD 租户？</span><span class="sxs-lookup"><span data-stu-id="d23c3-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="d23c3-116">如果你不确定你的公司是否具有 Azure AD 租户，请按照以下步骤进行检查。</span><span class="sxs-lookup"><span data-stu-id="d23c3-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="d23c3-117">请注意，如果你具有有效的 Microsoft Azure 或 Office 365 订阅，则你已经拥有了 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="d23c3-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="d23c3-118">登录到 Azure 管理门户，网址为 https://ms.portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="d23c3-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="d23c3-119">从菜单中选择“Azure Active Directory”，然后选择“域名”。</span><span class="sxs-lookup"><span data-stu-id="d23c3-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="d23c3-120">如果你已经有租户，则将列出你的域名。</span><span class="sxs-lookup"><span data-stu-id="d23c3-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="d23c3-121">使用现有租户？</span><span class="sxs-lookup"><span data-stu-id="d23c3-121">Using an existing tenant?</span></span>

<span data-ttu-id="d23c3-122">如果你想要使用现有的 Azure AD 租户，但在登录时遇到问题，请在下图中查找最符合你的情况的方案，然后按照推荐的步骤进行操作。</span><span class="sxs-lookup"><span data-stu-id="d23c3-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![是具有 Azure AD 租户还是需要创建一个租户？](images/onboardingAADFlow.png)

<span data-ttu-id="d23c3-124">有关在 Azure AD 中添加域的详细信息，请参阅[在 Azure AD 中添加或关联域](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="d23c3-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="d23c3-125">关于 Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d23c3-125">About Microsoft Azure</span></span>

<span data-ttu-id="d23c3-126">Microsoft Azure 是一个公共云平台，公司可以使用该平台在 Microsoft 管理的数据中心的全球网络中构建、部署和管理应用程序。</span><span class="sxs-lookup"><span data-stu-id="d23c3-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="d23c3-127">公司可以使用 Azure 构建一个具有虚拟功能或服务（而非物理计算机）的虚拟 IT 基础结构。</span><span class="sxs-lookup"><span data-stu-id="d23c3-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="d23c3-128">当你购买 Azure 订阅时，你实际上是在 Azure 公共云中租用了一个专用安全空间，这与在办公楼中租用楼层为公司的实体业务提供办公场所没有太大的不同。</span><span class="sxs-lookup"><span data-stu-id="d23c3-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="d23c3-129">对于办公大楼的业主而言，公司就是租户。</span><span class="sxs-lookup"><span data-stu-id="d23c3-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="d23c3-130">Azure AD 租户是 Azure 公共云中公司的专用独立虚拟表示形式，并且是在你订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时为你创建的。</span><span class="sxs-lookup"><span data-stu-id="d23c3-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="d23c3-131">你的租户托管 Azure AD 用户及其相关信息 - 其密码、配置文件数据、权限等。</span><span class="sxs-lookup"><span data-stu-id="d23c3-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="d23c3-132">租户还包含组、应用程序以及关于公司及其安全性的其他信息。</span><span class="sxs-lookup"><span data-stu-id="d23c3-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="d23c3-133">若要了解有关 Azure AD 的详细信息，请参阅 [Azure Active Directory 文档](https://docs.microsoft.com/ azure/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="d23c3-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 