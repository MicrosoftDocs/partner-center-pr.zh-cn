---
title: 将 Azure 计划下的 Azure 订阅转移到其他 CSP 合作伙伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何更改与云解决方案提供商 Azure 计划下客户的 Azure 订阅关联的计划合作伙伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856043"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>将客户的 Azure 计划订阅转移到其他合作伙伴

**适当角色**：帐户管理员|销售代理|计费代理

本文介绍客户如何在 Azure 计划下将 Azure 订阅从一个云解决方案提供商云解决方案提供商 (切换到另) 云解决方案提供商。

若要从其他合作伙伴切换客户的 Azure 订阅，请执行以下步骤。 合作伙伴和客户都有完成的步骤。

>[!Note]  
>只有与 Microsoft 有直接计费关系的合作伙伴才能访问转换工具。 间接经销商必须与间接提供商合作，以利用此转换工具。

在利用此工具之前，客户 (与) 合作伙伴对话。 需要使脱机对话避免混淆和改动。 此外，合作伙伴和客户应在启动转换之前了解这些注意事项和先决条件：

**主要注意事项：**

- Azure 预留不会随订阅转移到未来的合作伙伴
- 当前合作伙伴下 Azure 服务的 CSP 定价不会转换  
- 客户的支持责任将转移到未来的合作伙伴
- 转移时，计费和开票将转移到未来的合作伙伴
- Azure Role-Based 访问控制 (RBAC) 不受传输影响
- 默认情况下， (AOBO) 不会向未来合作伙伴授予管理员权限
- 只要产品通过市场资格检查，第三方市场产品就会转移。
    - 没有特殊折扣或区域限制
    - 产品不是基于订阅的
    - 将来的合作伙伴应与发布者合作，以确保它们位于产品部署的允许列表中
    - 如果未满足所有这些条件，则应取消应用商店产品、已转让的 Azure 订阅，然后重新购买具有新合作伙伴的 Marketplace 产品

**先决条件：**

- 客户根据当前的 CSP 合作伙伴的转换意图
- 将来的 CSP 合作伙伴与客户合作，以确保可满足客户需求
- 将来的 CSP 合作伙伴与客户建立关系，并在转换开始之前购买 Azure 计划  
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
3.  选择" **转移请求"** 部分。
4.  在"**传输请求"部分中**，选择 **"添加新请求"。**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="传输部分":::

5.  填写" **新建转移请求"** 表单。

6.  选择 **"发送传输请求发送**  >  **"。**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="完整的转移请求表单":::

7.  查看传输请求确认

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="查看挂起的传输":::

    >[!Note]
    >只有当转移请求状态为"挂起"时，未来的合作伙伴才能通过在右上角选择"取消请求"来取消转移请求。 传输请求状态为"正在进行"或"已完成"后，将不能取消。

## <a name="current-partner-tasks-to-be-completed"></a>当前要完成的合作伙伴任务

客户的当前合作伙伴的管理员代理将收到一封电子邮件，其中客户正在请求转移其订阅：

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="检讨":::

查看并接受来自 合作伙伴中心的转移请求表单，以完成订阅转移。

>[!Note]  
>如果当前合作伙伴在 30 天内未采取任何操作，则请求将过期，并且未来合作伙伴将拥有创建新的转移请求的 。

1.  从 **电子邮件中选择"查看** 转移请求"或
1.  在"合作伙伴中心"菜单中，选择"客户"，然后选择已代表提交转移请求的客户。
2.  在"客户"菜单中，选择"**订阅"。**
3.  选择" **转移请求"** 部分。
4.  通过在"已接收请求"下选择 **所选的"传输请求 ID"****来展开传输信息**

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

- 因此，客户必须删除其上一合作伙伴的 Azure RBAC 访问权限，并添加新合作伙伴的访问权限。 有关客户提供新访问权限的信息，请参阅什么是[Azure RBAC](/azure/role-based-access-control/overview) (Azure 基于角色的) ？ 有关客户删除以前合作伙伴的 RBAC 访问权限详细信息，请参阅 [删除角色分配](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。

- 此外，你不会自动代表管理员访问 ([AOBO ](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)) 订阅。 合作伙伴的 需要 AOBO 来代表他们管理客户的 Azure 订阅。 有关 Azure 特权的信息，请参阅 [获取管理客户的服务或订阅的权限。](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>后续步骤：

- [ (Azure RBAC) ](/azure/role-based-access-control/overview)
- [获取管理客户的服务或订阅的权限。](./customers-revoke-admin-privileges.md)
