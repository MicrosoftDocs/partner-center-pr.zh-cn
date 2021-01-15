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
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215843"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用


**相应的角色**
-   全局管理员
-   用户管理员
-   销售代理
-   管理员代理

## <a name="before-you-begin"></a>在开始之前

从以下可用 Power BI 应用列表中选择与你的业务最相关的应用程序：
- [直接提供程序](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [间接提供程序](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [间接经销商](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

安装合作伙伴中心分析应用预览版本之前，请确保你满足以下要求。

- 你为你的业务选择正确的 Power BI 应用。

- 你有 Power BI pro 许可证。

- 你有权在你的租户上安装模板应用。

- 你可以登录 Power BI。

- 你可以使用 "全局管理员"、"管理员代理" 或 "计费管理员" 身份登录到 [公司的 Azure Active Directory (Azure AD) 租户](azure-active-directory-tenants-and-partner-center.md)。

## <a name="to-install-the-app"></a>安装应用

1. 单击上一节中提供的 (直接提供程序/间接提供商/间接经销商) 上提供的应用程序源链接。

2. 单击 " **立即获取**"。 

3. 单击 " **继续**" 即表示同意条款和条件。

4. 在已拥有帐户?下选择 **登录**。

5. 在下一页上，输入你的 Power BI 用户名和密码，然后选择登录。

6. 通过提供工作区名称安装工作区。

7. 可以在 "应用" 部分中找到安装的模板应用。

8. 单击 "应用"，然后选择已安装的应用。

9. 新应用屏幕入门会打开。

10. 若要连接到数据，请单击 " **连接**"。

11. 在 " **连接到合作伙伴中心分析** " 弹出窗口上，验证 **身份验证方法** 是否设置为 " **oAuth2** "，或者从列表中选择 " **oAuth2** " （如果不是）。 

> [!NOTE]  
>  此窗口可能需要几分钟才会显示。

12. 在 " **合作伙伴中心分析连接器** " 页面上，用你公司的 Azure AD 租户的 "全局管理员"、"管理代理" 或 "计费管理员凭据" 登录，然后选择 " **登录**"。
 
13. 当提示你访问条款时，选择 **接受**。 

合作伙伴中心分析服务连接到 Power BI 之后，就会开始加载数据。 根据数据量，这一过程最多需要 10 分钟。 

数据完成加载后，即可开始在 Power BI 中使用合作伙伴中心分析应用仪表板和报告。

## <a name="next-steps"></a>后续步骤

[使用适用于 Microsoft Power BI 的合作伙伴中心分析应用查看你的业务数据](power-bi-app-for-direct-partners-use.md)
