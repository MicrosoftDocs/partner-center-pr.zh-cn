---
title: 安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用 | 合作伙伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 按照以下步骤安装和预览合作伙伴中心分析应用，以便 Power BI （对于 CSP 中的直接合作伙伴）。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: cd328ce8afed02af377a94b40fcf75125b008d1f
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004966"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用

**适用于**

- 合作伙伴中心

**相应的角色**
-   全局管理员
-   用户管理员
-   销售代理
-   管理员代理

## <a name="before-you-begin"></a>开始之前

从以下可用 Power BI 应用列表中选择与你的业务最相关的应用程序：
- [直接合作伙伴](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [间接合作伙伴](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [间接经销商](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

安装合作伙伴中心分析应用预览版本之前，请确保你满足以下要求。

- 你为你的业务选择正确的 Power BI 应用。

- 你具有 Microsoft Power BI 专业版或 Microsoft Power BI 高级版的活动订阅。

- 你可以登录 Power BI。

- 你可以使用 "全局管理员"、"管理代理" 或 "计费管理员" 身份登录到[你公司的 Azure Active Directory （Azure AD）租户](azure-active-directory-tenants-and-partner-center.md)。

## <a name="to-install-the-app"></a>安装应用

1. 开始执行[安装过程](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)。

2. 在**已拥有帐户?** 下选择**登录**。 

3. 在下一页上，输入你的 Power BI 用户名和密码，然后选择**登录**。 

4. 在 "**连接到合作伙伴中心分析**" 弹出窗口上，验证**身份验证方法**是否设置为 " **oAuth2** "，或者从列表中选择 " **oAuth2** " （如果不是）。 

> [!NOTE]  
>  此窗口可能需要几分钟才会显示。

5. 在 "**合作伙伴中心分析连接器**" 页面上，用你公司的 Azure AD 租户的 "全局管理员"、"管理代理" 或 "计费管理员凭据" 登录，然后选择 "**登录**"。
 
6. 当提示你访问条款时，选择**接受**。 

合作伙伴中心分析服务连接到 Power BI 之后，就会开始加载数据。 根据数据量，这一过程最多需要 10 分钟。 

数据完成加载后，即可开始在 Power BI 中使用合作伙伴中心分析应用仪表板和报告。

## <a name="next-steps"></a>后续步骤

[查看适用于 Microsoft Power BI 的合作伙伴中心分析应用的业务数据](power-bi-app-for-direct-partners-use.md)
