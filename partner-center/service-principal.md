---
title: Azure AD 服务主体
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将服务主体添加到 Azure AD 租户。 这样做意味着在合作伙伴中心添加 Azure AD 应用程序（服务主体）。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028462"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="fe6e5-104">在合作伙伴中心添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="fe6e5-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="fe6e5-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="fe6e5-105">**Appropriate roles**</span></span>

- <span data-ttu-id="fe6e5-106">全局管理员</span><span class="sxs-lookup"><span data-stu-id="fe6e5-106">Global admin</span></span>

<span data-ttu-id="fe6e5-107">在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="fe6e5-108">（你之前可以在云合作伙伴门户或 CPP 帐户中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="fe6e5-109">在你已迁移到合作伙伴中心后，CPP 帐户会是只读帐户。）</span><span class="sxs-lookup"><span data-stu-id="fe6e5-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="fe6e5-110">服务主体与 Azure AD 应用程序同义。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="fe6e5-111">添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="fe6e5-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="fe6e5-112">从合作伙伴中心面板中，选择“设置”，然后选择“开发人员设置”。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="fe6e5-113">选择“用户”，然后选择“添加 Azure AD 应用程序”。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="fe6e5-114">选择现有的 Azure AD 应用程序，或者新建一个。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="fe6e5-115">如果要新建 Azure AD 应用程序，请提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="fe6e5-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="fe6e5-116">**回复 URL**：用户为了使用 Azure AD 应用程序而可登录的 URL。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="fe6e5-117">**应用 ID URI**：Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="fe6e5-118">**安全角色**：角色“管理者”（与 CPP 中的“所有者”角色相同）和“开发人员”（与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="fe6e5-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="fe6e5-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fe6e5-119">Next steps</span></span>

- [<span data-ttu-id="fe6e5-120">合作伙伴中心内的商业市场概述</span><span class="sxs-lookup"><span data-stu-id="fe6e5-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)