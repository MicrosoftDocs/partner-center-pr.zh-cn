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
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854921"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="23022-104">在合作伙伴中心添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="23022-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="23022-105">**相应的角色**：全局管理员</span><span class="sxs-lookup"><span data-stu-id="23022-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="23022-106">在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。</span><span class="sxs-lookup"><span data-stu-id="23022-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="23022-107">（你之前可以在云合作伙伴门户或 CPP 帐户中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="23022-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="23022-108">在你已迁移到合作伙伴中心后，CPP 帐户会是只读帐户。）</span><span class="sxs-lookup"><span data-stu-id="23022-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="23022-109">服务主体与 Azure AD 应用程序同义。</span><span class="sxs-lookup"><span data-stu-id="23022-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="23022-110">添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="23022-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="23022-111">从合作伙伴中心面板中，选择“设置”，然后选择“开发人员设置”。</span><span class="sxs-lookup"><span data-stu-id="23022-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="23022-112">选择“用户”，然后选择“添加 Azure AD 应用程序”。</span><span class="sxs-lookup"><span data-stu-id="23022-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="23022-113">选择现有的 Azure AD 应用程序，或者新建一个。</span><span class="sxs-lookup"><span data-stu-id="23022-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="23022-114">如果要新建 Azure AD 应用程序，请提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="23022-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="23022-115">**回复 URL**：用户为了使用 Azure AD 应用程序而可登录的 URL。</span><span class="sxs-lookup"><span data-stu-id="23022-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="23022-116">**应用 ID URI**：Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。</span><span class="sxs-lookup"><span data-stu-id="23022-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="23022-117">**安全角色**：角色“管理者”（与 CPP 中的“所有者”角色相同）和“开发人员”（与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="23022-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="23022-118">后续步骤</span><span class="sxs-lookup"><span data-stu-id="23022-118">Next steps</span></span>

- [<span data-ttu-id="23022-119">合作伙伴中心内的商业市场概述</span><span class="sxs-lookup"><span data-stu-id="23022-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)