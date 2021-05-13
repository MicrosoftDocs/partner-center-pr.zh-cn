---
title: 安装 合作伙伴中心 Analytics for Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 按照本文中的步骤安装和预览 CSP 适用于 Power BI 的合作伙伴中心分析应用 (中的直接合作伙伴) 。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854479"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>安装并预览适用于 Microsoft Power BI 的合作伙伴中心分析应用


**适当的角色**：全局管理员|用户管理管理员|销售代理|管理员代理

## <a name="before-you-begin"></a>开始之前

从以下可用应用列表中选择与业务Power BI应用程序：

- [直接提供程序](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [间接提供商](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [间接经销商](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

安装合作伙伴中心分析应用预览版本之前，请确保你满足以下要求。

- 为业务选择正确的Power BI应用。

- 你有一个Power BI Pro 许可证。

- 你有权在租户中安装模板应用。

- 你可以登录 Power BI。

- 你可以以全局管理员、管理员代理或计费管理员角色登录到公司的租户 [Azure Active Directory (Azure AD) 租户](azure-active-directory-tenants-and-partner-center.md)。

## <a name="to-install-the-app"></a>安装应用

1. 选择在上一部分中 (提供商/间接提供商/间接经销商) 应用源链接。

2. 选择“立即获取”  。 

3. 通过选择"继续"来同意 **条款和条件**。

4. 在已拥有帐户?下选择 **登录**。

5. 在下一页上，输入你的 Power BI 用户名和密码，然后选择 **登录**。

6. 通过提供工作区名称安装工作区。

7. 可以在"应用"部分下找到安装的模板应用。

8. 选择 **"** 应用"，然后选择已安装的应用。

9. "开始使用新应用"屏幕随即打开。

10. 若要连接到数据，请选择"连接 **"。**

11. 在 **"连接到 合作伙伴中心 Analytics"** 弹出窗口中，验证身份验证方法是否设置为 **oAuth2，或者从列表中选择"oAuth2"（** 如果不是）。  

> [!NOTE]  
>  此窗口可能需要几分钟才会显示。

12. 在 **"合作伙伴中心 Analytics 连接器**"页上，使用公司的 Azure AD 租户的全局管理员、管理员代理或计费管理员凭据登录，然后选择"**登录"。**
 
13. 当提示你访问条款时，选择 **接受**。 

合作伙伴中心分析服务连接到 Power BI 之后，就会开始加载数据。 根据数据量，这一过程最多需要 10 分钟。 

数据完成加载后，即可开始在 Power BI 中使用合作伙伴中心分析应用仪表板和报告。

## <a name="next-steps"></a>后续步骤

[使用适用于 Microsoft Power BI 的合作伙伴中心分析应用查看你的业务数据](power-bi-app-for-direct-partners-use.md)
