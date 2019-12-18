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
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010378"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="b64b0-104">在合作伙伴中心添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="b64b0-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="b64b0-105">在合作伙伴中心的“商业市场”计划中，现在可以将 Azure AD 应用程序（服务主体）添加为 Azure AD 租户中的用户。</span><span class="sxs-lookup"><span data-stu-id="b64b0-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Azure AD tenant.</span></span> <span data-ttu-id="b64b0-106">（之前可以在云合作伙伴门户 (CPP) 帐户中执行此操作，但现在你已迁移到合作伙伴中心，因此 CPP 帐户为只读帐户。）请注意，服务主体与 Azure AD 应用程序同义。</span><span class="sxs-lookup"><span data-stu-id="b64b0-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="b64b0-107">添加 Azure AD 应用程序（服务主体）</span><span class="sxs-lookup"><span data-stu-id="b64b0-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="b64b0-108">从合作伙伴中心面板中，选择“设置”  ，然后选择“开发人员设置”  。</span><span class="sxs-lookup"><span data-stu-id="b64b0-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="b64b0-109">选择“用户”  ，然后选择“添加 Azure AD 应用程序”  。</span><span class="sxs-lookup"><span data-stu-id="b64b0-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="b64b0-110">选择现有的 Azure AD 应用程序，或者新建一个。</span><span class="sxs-lookup"><span data-stu-id="b64b0-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="b64b0-111">如果要新建 Azure AD 应用程序，请提供以下信息：</span><span class="sxs-lookup"><span data-stu-id="b64b0-111">If you create a new Azure AD Application, include the following information:</span></span>  
<span data-ttu-id="b64b0-112">  
**名称\*\*：这类似于 CPP 门户中的“易记名称”字段。</span><span class="sxs-lookup"><span data-stu-id="b64b0-112">  
\*\*Name\*\*: This is similar to the ‘friendly name’ field in the CPP portal.</span></span>

<span data-ttu-id="b64b0-113">**回复 URL**：这是用户为了使用 Azure AD 应用程序而可登录的 URL。</span><span class="sxs-lookup"><span data-stu-id="b64b0-113">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="b64b0-114">**应用 ID URI**：这是 Azure AD 应用程序在向 Azure AD 发送单一登录请求时所显示的逻辑标识符。</span><span class="sxs-lookup"><span data-stu-id="b64b0-114">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="b64b0-115">**安全角色**：角色“管理者”  （与 CPP 中的“所有者”角色相同）和“开发人员”  （与 CPP 中的“参与者”角色相同）适用于合作伙伴中心的“商业市场”计划，并且可与此 Azure AD 应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="b64b0-115">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

<span data-ttu-id="b64b0-116">选择“保存”  以在合作伙伴中心创建此应用程序时，该信息也会同步回 CPP 系统。</span><span class="sxs-lookup"><span data-stu-id="b64b0-116">When you select **Save**,  to create this in Partner Center, the information is also synced back to the CPP system.</span></span>  
