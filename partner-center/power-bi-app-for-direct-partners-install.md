---
title: 为 Power BI 安装合作伙伴中心分析
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 按照本文中的步骤，安装和预览合作伙伴中心分析应用，以便在 CSP) 中为直接伙伴 Power BI (。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302324"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="9f80f-103">安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用</span><span class="sxs-lookup"><span data-stu-id="9f80f-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="9f80f-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="9f80f-104">**Applies to**</span></span>

- <span data-ttu-id="9f80f-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="9f80f-105">Partner Center</span></span>

<span data-ttu-id="9f80f-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="9f80f-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="9f80f-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9f80f-107">Global admin</span></span>
-   <span data-ttu-id="9f80f-108">用户管理员</span><span class="sxs-lookup"><span data-stu-id="9f80f-108">User admin</span></span>
-   <span data-ttu-id="9f80f-109">销售代理</span><span class="sxs-lookup"><span data-stu-id="9f80f-109">Sales agent</span></span>
-   <span data-ttu-id="9f80f-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="9f80f-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="9f80f-111">开始之前</span><span class="sxs-lookup"><span data-stu-id="9f80f-111">Before you begin</span></span>

<span data-ttu-id="9f80f-112">从以下可用 Power BI 应用列表中选择与你的业务最相关的应用程序：</span><span class="sxs-lookup"><span data-stu-id="9f80f-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="9f80f-113">直接提供程序</span><span class="sxs-lookup"><span data-stu-id="9f80f-113">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="9f80f-114">间接提供程序</span><span class="sxs-lookup"><span data-stu-id="9f80f-114">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="9f80f-115">间接经销商</span><span class="sxs-lookup"><span data-stu-id="9f80f-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="9f80f-116">安装合作伙伴中心分析应用预览版本之前，请确保你满足以下要求。</span><span class="sxs-lookup"><span data-stu-id="9f80f-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="9f80f-117">你为你的业务选择正确的 Power BI 应用。</span><span class="sxs-lookup"><span data-stu-id="9f80f-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="9f80f-118">你有 Power BI pro 许可证。</span><span class="sxs-lookup"><span data-stu-id="9f80f-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="9f80f-119">你有权在你的租户上安装模板应用。</span><span class="sxs-lookup"><span data-stu-id="9f80f-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="9f80f-120">你可以登录 Power BI。</span><span class="sxs-lookup"><span data-stu-id="9f80f-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="9f80f-121">你可以使用 "全局管理员"、"管理员代理" 或 "计费管理员" 身份登录到[公司的 Azure Active Directory (Azure AD) 租户](azure-active-directory-tenants-and-partner-center.md)。</span><span class="sxs-lookup"><span data-stu-id="9f80f-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="9f80f-122">安装应用</span><span class="sxs-lookup"><span data-stu-id="9f80f-122">To install the app</span></span>

1. <span data-ttu-id="9f80f-123">单击上一节中提供的 (直接提供程序/间接提供商/间接经销商) 上提供的应用程序源链接。</span><span class="sxs-lookup"><span data-stu-id="9f80f-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="9f80f-124">单击 "**立即获取**"。</span><span class="sxs-lookup"><span data-stu-id="9f80f-124">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="9f80f-125">单击 "**继续**" 即表示同意条款和条件。</span><span class="sxs-lookup"><span data-stu-id="9f80f-125">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="9f80f-126">在已拥有帐户?下选择**登录**。</span><span class="sxs-lookup"><span data-stu-id="9f80f-126">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="9f80f-127">在下一页上，输入你的 Power BI 用户名和密码，然后选择登录。</span><span class="sxs-lookup"><span data-stu-id="9f80f-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="9f80f-128">通过提供工作区名称安装工作区。</span><span class="sxs-lookup"><span data-stu-id="9f80f-128">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="9f80f-129">可以在 "应用" 部分中找到安装的模板应用。</span><span class="sxs-lookup"><span data-stu-id="9f80f-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="9f80f-130">单击 "应用"，然后选择已安装的应用。</span><span class="sxs-lookup"><span data-stu-id="9f80f-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="9f80f-131">新应用屏幕入门会打开。</span><span class="sxs-lookup"><span data-stu-id="9f80f-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="9f80f-132">若要连接到数据，请单击 "**连接**"。</span><span class="sxs-lookup"><span data-stu-id="9f80f-132">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="9f80f-133">在 "**连接到合作伙伴中心分析**" 弹出窗口上，验证**身份验证方法**是否设置为 " **oAuth2** "，或者从列表中选择 " **oAuth2** " （如果不是）。</span><span class="sxs-lookup"><span data-stu-id="9f80f-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="9f80f-134">此窗口可能需要几分钟才会显示。</span><span class="sxs-lookup"><span data-stu-id="9f80f-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="9f80f-135">在 "**合作伙伴中心分析连接器**" 页面上，用你公司的 Azure AD 租户的 "全局管理员"、"管理代理" 或 "计费管理员凭据" 登录，然后选择 "**登录**"。</span><span class="sxs-lookup"><span data-stu-id="9f80f-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="9f80f-136">当提示你访问条款时，选择**接受**。</span><span class="sxs-lookup"><span data-stu-id="9f80f-136">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="9f80f-137">合作伙伴中心分析服务连接到 Power BI 之后，就会开始加载数据。</span><span class="sxs-lookup"><span data-stu-id="9f80f-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="9f80f-138">根据数据量，这一过程最多需要 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="9f80f-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="9f80f-139">数据完成加载后，即可开始在 Power BI 中使用合作伙伴中心分析应用仪表板和报告。</span><span class="sxs-lookup"><span data-stu-id="9f80f-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9f80f-140">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9f80f-140">Next steps</span></span>

[<span data-ttu-id="9f80f-141">使用适用于 Microsoft Power BI 的合作伙伴中心分析应用查看你的业务数据</span><span class="sxs-lookup"><span data-stu-id="9f80f-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
