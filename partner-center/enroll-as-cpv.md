---
title: 注册为控制面板供应商
description: 了解如何在合作伙伴中心注册为控制面板供应商 (CPV) 以便可以更好地将 CSP 合作伙伴系统与合作伙伴中心 Api 集成。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560504"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="0051f-103">注册为控制面板供应商来帮助将 CSP 合作伙伴系统和合作伙伴中心 API 进行集成</span><span class="sxs-lookup"><span data-stu-id="0051f-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="0051f-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="0051f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0051f-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0051f-105">Global admin</span></span>

<span data-ttu-id="0051f-106">控制面板供应商 (CPV) 是一家独立软件供应商，可开发云解决方案提供商 (CSP) 合作伙伴所使用的应用程序，使其能够将其系统与合作伙伴中心 Api 集成。</span><span class="sxs-lookup"><span data-stu-id="0051f-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="0051f-107">控制面板供应商不是可直接访问合作伙伴中心仪表板或合作伙伴中心 Api 的 CSP 合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="0051f-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="0051f-108">无论你是 (CPV) 的新控制面板供应商，还是想要与 Microsoft 合作伙伴合作的新 CPV，Microsoft 现在都要求你注册合作伙伴中心，以便注册应用程序并支持云解决方案提供商合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="0051f-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="0051f-109">若要创建帐户，CPV 合作伙伴可以使用现有的 CSP 合作伙伴租户或现有的 CPV 租户，也可以在载入过程中创建新租户。</span><span class="sxs-lookup"><span data-stu-id="0051f-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="0051f-110">如果 CPV 合作伙伴选择使用现有的 CSP 租户，则他们将需要创建单独的多租户应用程序，并将其注册到合作伙伴中心进行 CPV 活动。</span><span class="sxs-lookup"><span data-stu-id="0051f-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="0051f-111">无法将应用程序注册为 CSP 和 CPV 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0051f-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="0051f-112">在合作伙伴中心注册并注册应用程序后，你将有权访问合作伙伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="0051f-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="0051f-113">如果需要沙盒帐户，请通过 Microsoft 支持部门请求与 Microsoft 联系。</span><span class="sxs-lookup"><span data-stu-id="0051f-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="0051f-114">如果已有沙盒帐户，请继续使用它。</span><span class="sxs-lookup"><span data-stu-id="0051f-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="0051f-115">不需要新的沙箱</span><span class="sxs-lookup"><span data-stu-id="0051f-115">You won't need a new sandbox</span></span>

<span data-ttu-id="0051f-116">查看 [Microsoft 控制面板供应商协议](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="0051f-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="0051f-117">在合作伙伴中心内工作</span><span class="sxs-lookup"><span data-stu-id="0051f-117">Working in Partner Center</span></span>

<span data-ttu-id="0051f-118">注册到合作伙伴中心 CPV 经验并接受 CPV 协议后，可以：</span><span class="sxs-lookup"><span data-stu-id="0051f-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="0051f-119">管理多租户应用程序 (将应用程序添加到合作伙伴中心) 中 Azure 门户、注册和注销应用程序。</span><span class="sxs-lookup"><span data-stu-id="0051f-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="0051f-120">CPVs 必须在合作伙伴中心注册其应用程序，才能获得合作伙伴中心 Api 的授权。</span><span class="sxs-lookup"><span data-stu-id="0051f-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="0051f-121">只是将应用程序添加到 Azure 门户并不会为 CPV 应用程序授予使用合作伙伴中心 API 的权限。</span><span class="sxs-lookup"><span data-stu-id="0051f-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="0051f-122">查看和管理 CPV 档案。</span><span class="sxs-lookup"><span data-stu-id="0051f-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="0051f-123">查看和管理需访问 CPV 功能的用户。</span><span class="sxs-lookup"><span data-stu-id="0051f-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="0051f-124">全局管理员是 CPV 可以拥有的唯一角色。</span><span class="sxs-lookup"><span data-stu-id="0051f-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0051f-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0051f-125">Next steps</span></span>

<span data-ttu-id="0051f-126">-[向合作伙伴中心帐户添加其他租户](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="0051f-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>