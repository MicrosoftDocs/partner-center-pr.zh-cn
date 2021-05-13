---
title: 从 Microsoft 请求 SLA 信用额度
ms.topic: article
ms.date: 03/31/2021
description: 如果客户遇到服务中断，请了解 (SLA 请求服务级别协议所带来的好处、限制和过程) 的信用额度。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 74dd5c2c9457961f07dd0dd8d5a6ead9047c5579
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855550"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>如何以及何时向 Microsoft (SLA 请求服务级别协议) 信用额度

**适当的角色**：管理代理 |全局管理员

如果提供给客户的服务发生服务中断，则可以 **(SLA 请求服务级别协议) 信用额度** 。

## <a name="sla-credit-calculation"></a>SLA 信用计算

Microsoft 的 SLA 信用取决于) 受影响的服务 (。 例如，如果你的客户有 Office 365 套件但仅经历了 SharePoint 中断，则 SLA 信用仅针对 SharePoint 而不是客户的整个计划。

*信用额度基于受影响的服务和中断持续时间进行估价。* 若要查看符合 SLA 信用的方案类型，请参阅 [联机服务合并 SLA 文档](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)。 此信息也适用于通过云解决方案提供商计划出售的服务。


## <a name="request-an-sla-credit"></a>请求 SLA 信用额度

*云解决方案提供商 (CSP) 合作伙伴必须在发生事件的月份后，按日历月的结束时间提交声明和所有必需的信息。* 例如，如果事件在2月15日发生，则 Microsoft 必须在3月31日前收到声明和所有必需的信息。 最终客户和间接经销商无法提交 SLA 信用索赔;间接提供商或直接帐单合作伙伴必须代表他们提交声明。

>[!NOTE]
>咨询事件 ([如何检查 Microsoft 365 服务运行状况](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) 是否有资格获得 SLA 信用。

### <a name="required-information"></a>必需的信息

客户名称、租户标识符、合作伙伴票证号和票证创建日期/时间戳不足以处理声明。

向 Microsoft [提交 SLA 信用请求](#submit-sla-credit-request) 之前，必须收集以下 **所有** 信息，包括在支持票证中：

- 客户租户的 GUID
- 中断[事件标识符？](#outage-incident-identifier)
- 客户受中断影响并请求 SLA 额度的证据。
- 通过 CSP 购买的受影响的订阅吗？  (*是* 或 *没有)*

#### <a name="evidence-that-proves-customer-impact"></a>证明客户影响的证据

- 有关停机时间时间和持续时间的信息
- 受影响用户 (的数量) 位置 (（如果适用) 
- 发生事件时尝试解决事件的说明
- 来自受到影响的客户的电子邮件，请求支持和后续额度
- 有关解决服务影响的支持票证编号和客户联系人的详细信息


#### <a name="outage-incident-identifier"></a>中断事件标识符

可以在服务运行状况页的"服务运行状况"页上找到中断事件的Microsoft 365 管理中心。 **中断事件 ID** 是前面带有两个字母缩写的一个数字，指示受影响的服务 (例如，Exchange Online 服务中断的 *EX25194*) 。 下表描述了常见服务缩写：

| 双字母缩写 | Microsoft 服务 |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype for Business Online (之前为 Lync Online)  |
| OS | Office 订阅 |
| PB | Power BI for Office 365 |
| SP | SharePoint Online |
| 你 | Yammer Enterprise |
| MO | 门户错误 |

### <a name="submit-sla-credit-request"></a>提交 SLA 信用请求

若要通过合作伙伴中心仪表板将 SLA 信用请求提交给 Microsoft，请执行以下操作：

1. 登录到合作伙伴中心面板。
2. 在左侧菜单中，选择 " **服务请求**"，然后选择 " **合作伙伴支持请求**"。
3. 在 " **合作伙伴请求** " 页上，选择 " **新建请求**"。
4. 在 " **启动请求** " 页上，找到 " **CSP-客户、订单和订阅**" 一节。 在此部分中，选择 " **选择问题类型**"，然后选择 " **客户服务信用请求**"。
5. 在 " **推荐的解决方案** " 页的 " **是否需要更多帮助？**" 下，选择 **"是"**。
6. 在 " **详细信息** " 页上，填写 " **问题详细信息** " 部分。 在 " **详细信息** " 文本框中，确保输入先前收集的 [所需信息](#required-information) 。
7. 选择 " **提交** " 以在 SLA 信用请求中发送。

## <a name="next-steps"></a>后续步骤

- [代表你的客户报告问题](report-problems-on-behalf-of-a-customer.md)
