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
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811237"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="87d49-104">在合作伙伴中心添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="87d49-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="87d49-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="87d49-105">**Applies to**</span></span>

- <span data-ttu-id="87d49-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="87d49-106">Partner Center</span></span>

<span data-ttu-id="87d49-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="87d49-107">**Appropriate roles**</span></span>

- <span data-ttu-id="87d49-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="87d49-108">Global admin</span></span>

<span data-ttu-id="87d49-109">在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。</span><span class="sxs-lookup"><span data-stu-id="87d49-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="87d49-110">（你之前可以在云合作伙伴门户或 CPP 帐户中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="87d49-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="87d49-111">在你已迁移到合作伙伴中心后，CPP 帐户会是只读帐户。）</span><span class="sxs-lookup"><span data-stu-id="87d49-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="87d49-112">服务主体与 Azure AD 应用程序同义。</span><span class="sxs-lookup"><span data-stu-id="87d49-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="87d49-113">添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="87d49-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="87d49-114">从合作伙伴中心面板中，选择“设置”，然后选择“开发人员设置”。</span><span class="sxs-lookup"><span data-stu-id="87d49-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="87d49-115">选择“用户”，然后选择“添加 Azure AD 应用程序”。</span><span class="sxs-lookup"><span data-stu-id="87d49-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="87d49-116">选择现有的 Azure AD 应用程序，或者新建一个。</span><span class="sxs-lookup"><span data-stu-id="87d49-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="87d49-117">如果要新建 Azure AD 应用程序，请提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="87d49-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="87d49-118">**回复 URL**：用户为了使用 Azure AD 应用程序而可登录的 URL。</span><span class="sxs-lookup"><span data-stu-id="87d49-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="87d49-119">**应用 ID URI**：Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。</span><span class="sxs-lookup"><span data-stu-id="87d49-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="87d49-120">**安全角色**：角色“管理者”（与 CPP 中的“所有者”角色相同）和“开发人员”（与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="87d49-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="87d49-121">后续步骤</span><span class="sxs-lookup"><span data-stu-id="87d49-121">Next steps</span></span>

- [<span data-ttu-id="87d49-122">合作伙伴中心内的商业市场概述</span><span class="sxs-lookup"><span data-stu-id="87d49-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)