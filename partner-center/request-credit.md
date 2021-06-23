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
ms.openlocfilehash: 4a8e785de051aa6f722a1bfddc4ad83d6502bbb3
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551650"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>如何以及何时向 Microsoft 请求服务级别协议 (SLA) 额度

**适当的角色**：管理员代理|全局管理员

如果为客户提供 **的服务发生服务中断 (，)** Microsoft 提供 SLA 和信用额度。

## <a name="sla-credit-calculation"></a>SLA 信用计算

Microsoft 的 SLA 信用额度是根据哪个服务 (服务) 影响的。 例如，如果客户有 Office 365 套件，但仅遇到 SharePoint 服务中断，则仅批准 SharePoint 的 SLA 额度，而不是客户的整个计划。

*额度根据受影响的服务以及中断持续时间按比例计算。* 若要了解符合 SLA 额度的方案类型，请参阅 [联机服务合并 SLA 文档](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)。 此信息也适用于通过云解决方案提供商云解决方案提供商 (计划) 的服务。


## <a name="request-an-sla-credit"></a>请求 SLA 信用额度

*CSP 合作伙伴必须在事件发生的月份之后日历月结束时提交声明以及所有必需信息。* 例如，如果事件发生在 2 月 15 日，Microsoft 必须在 3 月 31 日前收到声明以及所有必需信息。 最终客户和间接经销商无法提交 SLA 信用申请;间接提供商或直接计费合作伙伴必须代表他们提交索赔。

>[!NOTE]
>咨询事件 ([如何检查Microsoft 365运行状况](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)) 不符合 SLA 额度条件。

### <a name="required-information"></a>必需的信息

客户名称、租户标识符、合作伙伴票证#和票证创建日期/时间戳不足以处理声明。

在向 Microsoft[提交 SLA 信用额度](#submit-sla-credit-request)请求之前，必须收集以下信息以包括在支持票证中：

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
| (OS) | Office 订阅 |
| PB | Power BI for Office 365 |
| SP | SharePoint Online |
| 你 | Yammer Enterprise |
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
