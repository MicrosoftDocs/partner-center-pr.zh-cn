---
title: 在 Azure 计划下将 Azure 订阅转移到另一个 CSP 合作伙伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何在 Azure 计划下更改与客户的 Azure 订阅关联的云解决方案提供商计划合作伙伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e1b70f26dc146507ac3764ae223ca27915162f0c
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422544"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>将客户的 Azure 计划订阅转移到不同的合作伙伴

## <a name="applies-to"></a>适用于

- 云解决方案提供商 (CSP) 计划中的合作伙伴

本文介绍了客户如何在 Azure 计划下从一个云解决方案提供商 (CSP) 切换到另一个云解决方案。

若要从其他合作伙伴切换客户的 Azure 订阅，请执行以下步骤。 合作伙伴和客户都有完成的步骤。

>[!Note]  
>只有与 Microsoft 直接计费关系的合作伙伴可以访问转换工具。 间接经销商必须与其间接提供商合作，才能利用此转换工具。

在利用此工具之前，客户必须与双方 (当前和未来) 合作。 脱机对话需要避免混淆和改动。 此外，在启动过渡之前，合作伙伴和客户应了解以下注意事项和先决条件：

**关键注意事项：**

- Azure 保留将不会随订阅向未来合作伙伴移动
- 当前合作伙伴提供的 Azure 服务的 CSP 定价将不会转换  
- 客户的支持责任将转向未来的合作伙伴
- 计费和开具发票会在传输时移到未来合作伙伴
- Azure 基于角色的访问控制 (RBAC) 不受传输影响
- 默认情况下，将不会向未来伙伴授予 (AOBO) 的管理员
- 只要产品通过 Marketplace 资格检查，就会传输第三方 marketplace 产品。
    - 无特殊折扣或区域限制
    - 产品不是基于订阅的
    - 将来的合作伙伴应与发布者合作，以确保它们位于产品的允许列表中
    - 如果未满足所有这些条件，则应取消应用商店产品、已转让的 Azure 订阅，然后重新购买具有新合作伙伴的 Marketplace 产品

**先决条件：**

- 客户根据当前的 CSP 合作伙伴的转换意图
- 将来的 CSP 合作伙伴与客户合作，以确保可满足客户需求
- 未来的 CSP 合作伙伴在转换开始之前与客户建立关系  
- 客户必须向 Microsoft 客户协议签署未来的 CSP 合作伙伴
- 将来的 CSP 合作伙伴必须已签署 Microsoft 合作伙伴协议，才能使用此工具

## <a name="customer-tasks-to-be-completed"></a>要完成的客户任务

若要在 Azure 计划下传输 Azure 订阅，客户必须通过联系当前合作伙伴来启动该过程。 他们应收集当前合作伙伴的公司名称和域，以使其未来合作伙伴可以代表他们填写传输请求表单。

客户还必须确定他们希望从当前合作伙伴那里传输的订阅。 不能更改 Office 365、企业移动性套件或 Microsoft Dynamics CRM 订阅的合作伙伴。

>[!Note]  
>这是未来合作伙伴负责完成传输请求窗体的责任。 Microsoft 不能代表客户或当前合作伙伴进行干预。 客户应计划与未来和当前合作伙伴密切合作，使过渡顺利进行。

## <a name="future-partner-tasks-to-be-completed"></a>要完成的未来合作伙伴任务

未来的订阅合作伙伴需要从合作伙伴中心完成一个传输请求表单，请求订阅转让：

1.  从 "合作伙伴中心" 菜单中，选择 " **客户**"，然后选择要代表其完成传输请求表单的客户。
2.  从 "客户" 菜单中选择 " **订阅**"。
3.  选择 " **传输请求** " 部分。
4.  从 " **传输请求" 部分**中，选择 " **添加新请求**"。

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="传输部分":::

5.  完成 " **新建传输请求** " 窗体。

6.  选择**发送传输请求**  >  **发送**。

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="完成传输请求窗体":::

7.  查看传输请求确认

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="查看挂起的传输":::

    >[!Note]
    >只有在传输请求状态为 "挂起" 时，才能通过选择右上角的 " **取消请求** " 来取消传输请求。 传输请求状态为 "正在进行" 或 "完成" 后，将无法取消取消。

## <a name="current-partner-tasks-to-be-completed"></a>当前要完成的合作伙伴任务

客户的当前合作伙伴的管理员代理将收到一封电子邮件，指出其客户正在请求传输其订阅：

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="审阅":::

查看并接受合作伙伴中心的传输请求窗体，以完成订阅转移。

>[!Note]  
>如果当前合作伙伴在30天内没有执行任何操作，则该请求将过期，将来的合作伙伴将拥有来创建新的传输请求。

1.  选择电子邮件中的 " **查看传输请求** " 或
1.  从 "合作伙伴中心" 菜单中，选择 " **客户**"，然后选择代表其提交了传输请求的客户。
2.  从 "客户" 菜单中选择 " **订阅**"。
3.  选择 " **传输请求** " 部分。
4.  通过选择 "**接收的请求**" 下的所选**传输请求 ID**展开传输信息。

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="源审阅传输请求":::

5.  查看传输请求。 选择要传输的请求的 Azure 订阅。

>[!Note]  
> 请注意，在继续操作之前，你将无法再访问所选订阅。
> 不会向你开具发票以便进一步使用。
> Azure 预订不会与订阅一起传输。

6.  然后选择 " **接受并传输** " 完成传输过程。

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="选择要在 Azure 计划下传输的订阅":::

7.  查看传输接受确认。

   此时，将通过电子邮件向未来合作伙伴、客户和当前合作伙伴发送接受的传输请求通知。

   在此之后，转换已被接受：传输状态可能在系统更新时保持挂起状态最多15分钟。 如果需要更长时间，系统将继续尝试3天。 如果传输状态仍处于挂起状态，则合作伙伴应提交服务请求。

   传输完成后，请求中包含的订阅将显示在未来合作伙伴的 Azure 计划中，不再与你一起列出。

>[!Note]  
>对于间接提供程序：请通知间接经销商已接受传输请求。

### <a name="managing-your-transferred-customer-subscriptions"></a>管理已传输的客户订阅
- 在转换期间，使用 Azure 基于角色的访问控制 (RBAC) 为现有用户、组或服务主体分配的访问权限不受影响。 Azure [ RBAC) ](/azure/role-based-access-control/overview) 的基于角色的访问控制 (可帮助你的客户管理有权访问 Azure 资源的人员、他们可以使用这些资源执行哪些操作，以及他们有权访问哪些区域。 作为新合作伙伴，你不会在订阅转让后向你的客户的资源提供任何 RBAC 访问权限。 你的客户的上一个合作伙伴将保留其 RBAC 访问权限。 与客户合作，了解谁有权了解他们的订阅以及如何进行任何所需的更改。

- 因此，重要的是，您的客户必须删除其以前合作伙伴的 Azure RBAC 访问权限，并为新合作伙伴添加访问权限。 有关提供新访问权限的客户的详细信息，请参阅 [什么是 AZURE RBAC)  (azure 基于角色的访问控制？](/azure/role-based-access-control/overview) 若要详细了解你的客户如何删除以前合作伙伴的 RBAC 访问权限，请参阅 [删除角色分配](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。

- 此外，不会 [代表 (AOBO) ](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 访问订阅来自动获取管理员。 若要使合作伙伴自行管理客户的 Azure 订阅，AOBO 是必需的。 有关 Azure 特权的详细信息，请参阅 [获取管理客户服务或订阅的权限。](/partner-center/customers-revoke-admin-privileges)

## <a name="next-steps"></a>后续步骤：

- [ (Azure RBAC) ](/azure/role-based-access-control/overview)
- [获取管理客户服务或订阅的权限。](/partner-center/customers-revoke-admin-privileges)