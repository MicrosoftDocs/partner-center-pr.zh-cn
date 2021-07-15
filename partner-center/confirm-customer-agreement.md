---
title: 如何确认客户已接受 CSP 计划的 Microsoft 客户协议
description: 云解决方案提供商 (CSP) 合作伙伴在为客户订购 Microsoft 服务之前，需要确认客户接受 Microsoft 客户协议。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277005"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>如何确认客户已接受 CSP 计划的 Microsoft 客户协议

相应的角色：管理员代理 | 销售代理


关于是否接受 Microsoft 客户协议，客户有两种选择。

**选项 1**：合作伙伴证明客户已接受 - 合作伙伴可以通过合作伙伴中心 API/SDK 或合作伙伴中心仪表板确认客户接受。

**选项 2**：客户直接接受 - 合作伙伴可以通过 URL 邀请客户在 Microsoft 365 管理中心查看并接受协议。

## <a name="access-microsoft-customer-agreement-template"></a>访问 Microsoft 客户协议模板

可以从[此处](https://aka.ms/customeragreement)手动下载最新版 Microsoft 客户协议模板。 Microsoft 客户协议特定于国家/地区。 在请求 Microsoft 客户协议模板时，请确保根据客户的位置选择正确的国家/地区。

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>选项 1：在合作伙伴中心中确认客户已接受协议

对于新客户和现有客户，直接计费合作伙伴可以在合作伙伴中心确认客户接受 Microsoft 客户协议。 间接经销商不能代表其客户进行证明，需通过其间接提供商来完成证明。

### <a name="confirm-customer-acceptance-for-new-customers"></a>确认新客户接受了协议

在合作伙伴中心创建新客户租户时，请按以下步骤确认客户接受了 Microsoft 客户协议。 必须是管理员代理或销售代理才能执行这些步骤。

1. 选择“客户”，然后选择“新客户”。

2. 在“帐户信息”下，输入公司及其主要联系人的信息。

3. 在“Microsoft 协议”下，选中相应的框来证明客户已接受 Microsoft 客户协议。

4. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。

5. 确保显示的主要用户联系人信息正确。 如果不正确，请选择“更新”并输入接受该协议的人员的准确信息。

6. 选择“下一步”继续创建客户租户。

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客户。":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>确认现有客户接受了协议

必须是管理员代理或销售代理才能执行此操作：

1. 选择“客户”。 找到并选择客户。

2. 选择“帐户信息”。 

3. 在“Microsoft 客户协议”下选择“更新”。

4. 输入已接受协议的人员的 **名字**、**姓氏**、**电子邮件地址** 和 **电话号码**（可选）。 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。

5. 选择“保存”，然后继续操作。

   :::image type="content" source="images/mcua2-update2.png" alt-text="现有客户。":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>检索客户接受协议的确认信息

若要检索关于现有客户已接受 Microsoft 客户协议的确认信息，请使用下述步骤。 必须是管理员代理或销售代理才能执行此操作。

1. 选择“客户”，然后找到并选择要查看的客户。

2. 选择“帐户信息”。 

3. 在“Microsoft 客户协议”下，查看该客户是否提供过确认。

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>使用合作伙伴中心 API/SDK 确认客户接受协议

可以使用合作伙伴中心 API/SDK 确认客户接受 Microsoft 客户协议。 有关 API/SDK 的详细信息，请参阅：

- [获取 Microsoft 客户协议的协议元数据](/partner-center/develop/get-customer-agreement-metadata)

- [确认客户接受 Microsoft 客户协议](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [获取客户接受 Microsoft 客户协议的确认](/partner-center/develop/get-confirmation-of-customer-agreement)

- [获取 Microsoft 客户协议模板的下载链接](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>选项 2：客户在 Microsoft 365 管理中心接受协议

合作伙伴可以通过 URL 邀请新客户和现有客户在 Microsoft 365 管理中心查看并接受协议。 接下来的几部分介绍如何执行以下操作：

- 创建一个新客户，并邀请该客户查看并接受协议。

- 邀请新客户查看并接受经销商关系和协议。

- 邀请现有客户查看并接受协议。

>[!NOTE]
> 可以使用[合作伙伴中心 API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) 来获取客户直接接受 Microsoft 客户协议的状态。  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>创建一个新客户，并邀请该客户查看并接受协议

使用以下步骤在合作伙伴中心创建新客户，并邀请他们在 Microsoft 365 管理中心查看并接受 Microsoft 客户协议。

1. 从合作伙伴中心的“客户”选项卡中，选择“添加客户”。

2. 在“帐户信息”下的所有必填字段中输入新客户的信息，包括客户的公司名称和主要联系人。

3. 在“客户协议”下选择“将要求客户在 Microsoft 365 管理中心接受 Microsoft 客户协议”。 完成页面上的所有其他必填字段。

4. 选择“下一步:查看”，然后继续执行创建客户租户的步骤。 

>[!NOTE] 
>新客户必须接受 Microsoft 客户协议才能进行购买。  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="创建新客户。":::

5. 到达新客户工作流中的“确认”屏幕后，保存客户凭据。 稍后需将这些凭据分配给客户。

6. 在合作伙伴中心外部，创建并发送一封电子邮件，邀请客户在 Microsoft 365 管理中心接受 Microsoft 客户协议。 请确保电子邮件中包含以下项：

   - 此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的链接（需要登录）

   - 在步骤 5 中保存的客户凭据。

7. 然后，客户会收到来自合作伙伴的电子邮件邀请，并会选择 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。

8. 客户使用你提供的客户凭据登录 Microsoft 365 管理中心。

9. 客户选中用于接受 Microsoft 客户协议的复选框。

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>邀请新客户查看并接受经销商关系和 Microsoft 客户协议 

通过以下步骤邀请新客户查看并接受经销商关系和 Microsoft 客户协议。 

1. 从合作伙伴中心的“客户”选项卡中选择“请求建立经销商关系”链接。 

2. 系统会生成自动电子邮件模板，其中包括文本和参数化 URL，用于将客户定向到 Microsoft 365 管理中心。

3. 可以自定义自动生成的电子邮件模板，然后选择“复制到剪贴板”或“在电子邮件中打开”。

4. 使用此电子邮件模板邀请客户接受 **经销商关系** 请求和 **Microsoft 客户协议**。 （注意：在电子邮件邀请中，请确保合作伙伴还包括自动提供的 URL 以及最近创建的客户凭据。）

   :::image type="content" source="images/mca/createrelationship.png" alt-text="创建关系。":::

5. 客户通过电子邮件接收邀请，并单击参数化 URL。 

6. 客户使用你在电子邮件中提供的凭据登录 Microsoft 365 管理中心。

7. 客户选中用于接受 **经销商关系** 和 **Microsoft 客户协议** 的复选框。 

8. 在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。 客户可以选择一个合作伙伴来查看详细信息。

   :::image type="content" source="images/mca/accept.jpg" alt-text="接受协议。":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>邀请现有客户查看并接受协议

通过以下步骤邀请现有客户查看并接受 Microsoft 客户协议。 

1. 创建包含嵌入 URL 的客户电子邮件，邀请客户接受 Microsoft 客户协议。

2. 客户通过电子邮件接收邀请，并单击 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。 

3. 客户将其凭据输入 Microsoft 365 管理中心。

4. 客户选中用于接受 Microsoft 客户协议的复选框。 

5. 在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。 客户可以选择一个合作伙伴来查看详细信息。

   :::image type="content" source="images/mca/customeraccept.png" alt-text="客户。":::

>[!NOTE]
>在某些情况下，客户可能无法直接接受 Microsoft 客户协议。 若要详细了解这些情况，请参阅下面的“需要代表客户证明的两种情况”。

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>需要代表客户证明的两种情况

在两种情况下，客户可能无法在 Microsoft 365 管理中心直接接受 Microsoft 客户协议。

**情况 1**：现有客户已通过现有合作伙伴关系购买以下任何一项：产品/服务、软件或软件订阅、预留实例或 Azure 计划。 客户现在正在尝试进行新的购买（不包括自动续订）。 该客户在单击 URL 时会收到消息：“请联系你的合作伙伴，确认你接受 Microsoft 客户协议。”  

**解决方法**：必须代表客户进行证明。

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Microsoft 365 管理中心页的屏幕截图，其中要求你与合作伙伴联系以确认接受 Microsoft 客户协议。":::

**情况 2**：现有客户已购买以下任何一项：产品/服务、软件和软件订阅、预留实例和 Azure 计划。 客户现在正在尝试通过新的合作伙伴进行新的购买。

在单击 Microsoft 365 管理中心的 URL 以接受新的合作伙伴关系和协议时，该客户会收到消息：“请联系你的合作伙伴，确认你接受 Microsoft 客户协议。”  

**解决方法**：必须代表客户进行证明。  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>确认客户已接受该协议

如果为之前未确认过是否接受了协议的现有客户创建新订单，你将收到完成确认的提示。 请使用下面的过程执行此操作。

1. 输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    

2. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。

3. 选择“保存并继续”。  

## <a name="next-steps"></a>后续步骤

- [验证或更新你的公司资料信息](update-your-partner-profile.md)
- [Microsoft 客户协议（按区域和语言排列）](Agreements.md)
