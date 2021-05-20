---
title: 从 Microsoft 请求 SLA 信用额度
ms.topic: article
ms.date: 03/31/2021
description: 了解在客户遇到服务中断时从 Microsoft 请求服务级别协议 (SLA) 和信用额度的好处、限制和过程。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 100a3d2988c19d57f7426c7212b7464d8e96dc94
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152947"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>如何以及何时向 Microsoft 请求服务级别协议 (SLA) 额度

**适当的角色**：管理员代理|全局管理员

如果为客户提供 **的服务发生服务中断 (，)** Microsoft 提供 SLA 和信用额度。

## <a name="sla-credit-calculation"></a>SLA 信用计算

Microsoft 的 SLA 信用额度是根据哪个服务 (服务) 影响的。 例如，如果客户有 Office 365 套件，但仅遇到 SharePoint 服务中断，则仅批准 SharePoint 的 SLA 额度，而不是客户的整个计划。

*额度根据受影响的服务以及中断持续时间按比例计算。* 若要了解符合 SLA 额度的方案类型，请参阅 [联机服务合并 SLA 文档](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)。 此信息也适用于通过计划销售云解决方案提供商服务。


## <a name="request-an-sla-credit"></a>请求 SLA 信用额度

*云云解决方案提供商 (CSP) 合作伙伴必须在事件发生的月份之后日历月结束时提交声明以及所有必需信息。* 例如，如果事件发生在 2 月 15 日，Microsoft 必须在 3 月 31 日前收到声明以及所有必需信息。 最终客户和间接经销商无法提交 SLA 信用申请;间接提供商或直接计费合作伙伴必须代表他们提交索赔。

>[!NOTE]
>咨询事件 ([如何检查Microsoft 365运行状况](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)) 不符合 SLA 额度条件。

### <a name="required-information"></a>必需的信息

客户名称、租户标识符、合作伙伴票证#和票证创建日期/时间戳不足以处理声明。

在向 Microsoft[提交 SLA 信用额度](#submit-sla-credit-request)请求之前，必须收集以下信息以包括在支持票证中：

- 客户租户的 GUID
- [中断事件标识符](#outage-incident-identifier)？
- 证明客户受到中断的影响，并请求 SLA 信用。
- 受影响的订阅是否通过 CSP 购买？  (*"是" 或 "* *否* ") 

#### <a name="evidence-that-proves-customer-impact"></a>证明客户影响的证据

- 有关停机时间和持续时间的信息
- 受影响的用户的 () 数量和位置 (（如果适用）) 
- 尝试在发生事件时解决事件
- 受影响客户请求支持并随后信用的电子邮件
- 有关解决服务影响的客户联系人的支持票证编号和详细信息


#### <a name="outage-incident-identifier"></a>停机事件标识符

可以在 " **服务运行状况** " 页上的 "Microsoft 365 管理中心" 中找到中断事件的标识符。 " **中断事件 ID** " 前面有两个字母的缩写，它指示受影响的服务 (例如， *EX25194* 用于 Exchange Online 中断) 。 下面的表介绍了常见的服务缩写：

| 两字母缩写 | Microsoft 服务 |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online 保护 |
| SB | Skype for Business Online (以前称为 Lync Online)  |
| (OS) | Office 订阅 |
| PB | Power BI for Office 365 |
| SP | SharePoint Online |
| 4EN-YA-P0U | Yammer 企业 |
| MO | 门户错误 |

### <a name="submit-sla-credit-request"></a>提交 SLA 信用额度请求

若要通过仪表板向 Microsoft 提交 SLA 信用合作伙伴中心请求：

1. 登录到合作伙伴中心面板。
2. 在左侧菜单中，选择"**服务请求"，** 然后选择"**合作伙伴支持请求"。**
3. 在"**合作伙伴请求"** 页上，选择"**新建请求"。**
4. 在" **启动请求"页上** ，找到 **"CSP - 客户、订单和订阅"部分**。 在本部分，选择 **"选择问题类型"，** 然后选择"**客户服务信用额度请求"。**
5. 在"**建议的解决方案"** 页上的"**是否需要更多帮助？"下**，选择"**是"。**
6. 在" **详细信息"** 页上，填写" **问题详细信息"** 部分。 在 **"详细信息** "文本框中，请务必 [输入之前](#required-information) 收集的所需信息。
7. 选择 **"提交** "以在 SLA 额度请求中发送。

## <a name="next-steps"></a>后续步骤

- [代表客户报告问题](report-problems-on-behalf-of-a-customer.md)
