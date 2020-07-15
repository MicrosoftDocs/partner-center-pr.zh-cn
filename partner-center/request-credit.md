---
title: 从 Microsoft 请求 SLA 信用额度
ms.topic: article
ms.date: 04/28/2020
description: 如果你的客户遇到服务中断，请了解从 Microsoft 请求服务级别协议（SLA）信用额度的好处、限制和程序。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377751"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>如何以及何时向 Microsoft 请求服务级别协议（SLA）信用额度

如果你为客户提供的服务中断，你可以从 Microsoft 请求**服务级别协议（SLA）信用额度**。

## <a name="sla-credit-calculation"></a>SLA 信用计算

Microsoft 的 SLA 信用取决于受影响的服务。 例如，如果你的客户有 Office 365 套件但仅经历了 SharePoint 中断，则 SLA 信用仅针对 SharePoint 而不是客户的整个计划。

*信用额度基于受影响的服务和中断持续时间进行估价。* 若要查看符合 SLA 信用的方案类型，请参阅[联机服务合并 SLA 文档](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)。 此信息也适用于通过云解决方案提供商计划出售的服务。

## <a name="request-an-sla-credit"></a>请求 SLA 信用额度

*云解决方案提供商（CSP）合作伙伴必须在发生事件的月份后，按日历月结束时间提交声明和所有必需的信息。* 例如，如果事件在2月15日发生，则 Microsoft 必须在3月31日前收到声明和所有必需的信息。 最终客户和间接经销商无法提交 SLA 信用索赔;间接提供商或直接帐单合作伙伴必须代表他们提交声明。

### <a name="required-information"></a>必需的信息

向 Microsoft[提交 SLA 信用请求](#submit-sla-credit-request)之前，必须收集下列信息，以将其包括在支持票证中：

- 客户租户的 GUID
- [中断事件标识符](#outage-incident-identifier)？
- 受影响的订阅是否通过 CSP 购买？ （*是*或*否*）

#### <a name="outage-incident-identifier"></a>停机事件标识符

可以在 "**服务运行状况**" 页上的 "Microsoft 365 管理中心" 中找到中断事件的标识符。 "**中断事件 ID** " 前面有两个字母的缩写，它指示受影响的服务（例如，Exchange Online 中断的*EX25194* ）。 下面的表介绍了常见的服务缩写：

| 两字母缩写 | Microsoft 服务 |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online 保护 |
| SB | Skype for Business Online （以前称为 Lync Online） |
| OS | Office 订阅 |
| PB | Power BI for Office 365 |
| SP | SharePoint Online |
| 4EN-YA-P0U | Yammer 企业 |
| MO | 门户错误 |

### <a name="submit-sla-credit-request"></a>提交 SLA 信用请求

若要通过合作伙伴中心仪表板将 SLA 信用请求提交给 Microsoft，请执行以下操作：

1. 登录到合作伙伴中心面板。
2. 在左侧菜单中，选择 "**服务请求**"，然后选择 "**合作伙伴支持请求**"。
3. 在 "**合作伙伴请求**" 页上，选择 "**新建请求**"。
4. 在 "**启动请求**" 页上，找到 " **CSP-客户、订单和订阅**" 一节。 在此部分中，选择 "**选择问题类型**"，然后选择 "**客户服务信用请求**"。
5. 在 "**推荐的解决方案**" 页的 "**是否需要更多帮助？**" 下，选择 **"是"**。
6. 在 "**详细信息**" 页上，填写 "**问题详细信息**" 部分。 在 "**详细信息**" 文本框中，确保输入先前收集的[所需信息](#required-information)。
7. 选择 "**提交**" 以在 SLA 信用请求中发送。
