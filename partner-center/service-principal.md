---
title: Azure AD 服务主体
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将服务主体添加到 Azure AD 租户。 这样做意味着在合作伙伴中心添加 Azure AD 应用程序（服务主体）。
author: dhirajgandhi
ms.author: dhgandhi
Keywords: Azure, Azure 计划, 服务主体, Azure AD 应用程序
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: bd2880f57d1ccb3c3675fef4fae7499f7ac02f4b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949624"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="96f2e-105">在合作伙伴中心添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="96f2e-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="96f2e-106">在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。</span><span class="sxs-lookup"><span data-stu-id="96f2e-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="96f2e-107">（你之前可以在云合作伙伴门户或 CPP 帐户中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="96f2e-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="96f2e-108">在你已迁移到合作伙伴中心后，CPP 帐户会是只读帐户。）</span><span class="sxs-lookup"><span data-stu-id="96f2e-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="96f2e-109">服务主体与 Azure AD 应用程序同义。</span><span class="sxs-lookup"><span data-stu-id="96f2e-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="96f2e-110">添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="96f2e-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="96f2e-111">从合作伙伴中心面板中，选择“设置”，然后选择“开发人员设置”。</span><span class="sxs-lookup"><span data-stu-id="96f2e-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="96f2e-112">选择“用户”，然后选择“添加 Azure AD 应用程序”。</span><span class="sxs-lookup"><span data-stu-id="96f2e-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="96f2e-113">选择现有的 Azure AD 应用程序，或者新建一个。</span><span class="sxs-lookup"><span data-stu-id="96f2e-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="96f2e-114">如果要新建 Azure AD 应用程序，请提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="96f2e-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="96f2e-115">**回复 URL**：用户为了使用 Azure AD 应用程序而可登录的 URL。</span><span class="sxs-lookup"><span data-stu-id="96f2e-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="96f2e-116">**应用 ID URI**：Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。</span><span class="sxs-lookup"><span data-stu-id="96f2e-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="96f2e-117">**安全角色**：角色“管理者”（与 CPP 中的“所有者”角色相同）和“开发人员”（与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="96f2e-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
