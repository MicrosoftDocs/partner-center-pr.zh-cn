---
title: 安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用 | 合作伙伴中心
ms.topic: article
ms.date: 10/29/2018
description: 请按照以下步骤预览适用于 Power BI（CSP 中的直接合作伙伴）的合作伙伴中心分析应用。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e4eaecc151f8cc4e5e45bbfa7d02236fb1444a24
ms.sourcegitcommit: 3eb069edf36bdb61518c0c7cc2ccaf2d8dde4adb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/07/2018
ms.locfileid: "6131696"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用

**适用于**

- 合作伙伴中心

## <a name="before-you-begin"></a>开始之前

选择的应用程序与业务最相关从以下列表中可用的 Power BI 应用：
- [直接合作伙伴](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [间接合作伙伴](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [间接经销商](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

安装合作伙伴中心分析应用预览版本之前，请确保你满足以下要求。

- 为你的企业选取正确的 Power BI 应用。

- 你具有 Microsoft Power BI 专业版或 Microsoft Power BI 高级版的活动订阅。

- 你可以登录 Power BI。

- 你可以以[贵公司的 Azure Active Directory (Azure AD) 租户](azure-active-directory-tenants-and-partner-center.md)的全局管理员、管理员代理或帐单管理员的身份登录。

## <a name="to-install-the-app"></a>安装应用

1. 开始执行[安装过程](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)。

2. 在**已拥有帐户?** 下选择**登录**。 

3.  在下一页上，输入你的 Power BI 用户名和密码，然后选择**登录**。 

4.  在**连接到合作伙伴中心分析**弹出窗口中，确认**身份验证方法**设置为 **oAuth2**，如果不是，请从列表中选择 **oAuth2**。 

    > [!NOTE]  
>  此窗口可能需要几分钟才会显示。

5.  在**合作伙伴中心分析连接器**页面上，使用贵公司的 Azure AD 租户的全局管理员、管理员代理或帐单管理员身份登录，然后选择**登录**。
 
6.  当提示你访问条款时，选择**接受**。 

合作伙伴中心分析服务连接到 Power BI 之后，就会开始加载数据。 根据数据量，这一过程最多需要 10 分钟。 

数据完成加载后，即可开始在 Power BI 中使用合作伙伴中心分析应用仪表板和报告。

## <a name="next-steps"></a>后续步骤

[使用适用于 Microsoft Power BI 的合作伙伴中心分析应用查看你的业务数据](power-bi-app-for-direct-partners-use.md)
