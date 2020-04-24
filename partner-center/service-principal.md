---
title: Azure AD 服务主体 | 合作伙伴中心
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 将服务主体添加到 Azure AD 租户
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure 计划, 服务主体, Azure AD 应用程序
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2020
ms.locfileid: "75716888"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="67de7-104">在合作伙伴中心添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="67de7-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="67de7-105">在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为合作伙伴中心帐户中的用户。</span><span class="sxs-lookup"><span data-stu-id="67de7-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="67de7-106">（之前可以在云合作伙伴门户 (CPP) 帐户中执行此操作，但现在你已迁移到合作伙伴中心，因此 CPP 帐户为只读帐户。）请注意，服务主体与 Azure AD 应用程序同义。</span><span class="sxs-lookup"><span data-stu-id="67de7-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="67de7-107">添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="67de7-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="67de7-108">从合作伙伴中心面板中，选择“设置”  ，然后选择“开发人员设置”  。</span><span class="sxs-lookup"><span data-stu-id="67de7-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="67de7-109">选择“用户”  ，然后选择“添加 Azure AD 应用程序”  。</span><span class="sxs-lookup"><span data-stu-id="67de7-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="67de7-110">选择现有的 Azure AD 应用程序，或者新建一个。</span><span class="sxs-lookup"><span data-stu-id="67de7-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="67de7-111">如果要新建 Azure AD 应用程序，请提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="67de7-111">If you create a new Azure AD Application, include the following information:</span></span>  

  


<span data-ttu-id="67de7-112">**回复 URL**：这是用户为了使用 Azure AD 应用程序而可登录的 URL。</span><span class="sxs-lookup"><span data-stu-id="67de7-112">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="67de7-113">**应用 ID URI**：这是 Azure AD 应用程序在向 Azure AD 发送单一登录请求时显示的该应用程序的逻辑标识符。</span><span class="sxs-lookup"><span data-stu-id="67de7-113">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="67de7-114">**安全角色**：角色“管理者”  （与 CPP 中的“所有者”角色相同）和“开发人员”  （与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="67de7-114">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

  
