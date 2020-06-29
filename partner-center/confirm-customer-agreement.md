---
title: 确认客户接受 Microsoft 客户协议
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何确认客户接受 Microsoft 客户协议。 为客户订购 Microsoft 产品和服务时，云解决方案提供商需要这样做。
author: LauraBrenner
ms.author: labrenne
keywords: 客户, 许可, MCA, Microsoft 云协议, Microsoft 客户协议, 客户协议模板
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d89c625375c203fe77556c47b6061faa293e1b0
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679104"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>确认客户接受云解决方案提供商合作伙伴计划中的 Microsoft 客户协议

**适用于**

- 合作伙伴中心
- Microsoft 365 管理中心

**相应的角色**

- 管理员代理
- 销售代理

**适当的合作伙伴类型**

- 间接经销商、直接计费、间接提供商

2019 年 10 月 1 日，Microsoft 推出了针对云解决方案提供商计划的 **Microsoft 客户协议**，替代 Microsoft 云协议。 请阅读间接经销商的其他[指南](indirect-reseller-tasks-in-partner-center.md)。 为了方便合作伙伴迁移到新协议，在 2020 年 1 月 31 日之前，这两个协议在云解决方案提供商计划中共存。 从 2020 年 2 月 1 日开始，Microsoft 客户协议替代了 Microsoft 云协议。

客户有两个选项可用于接受 Microsoft 客户协议。 

**选项 1**：合作伙伴证明客户已接受 - 合作伙伴可以通过合作伙伴中心 API/SDK 或合作伙伴中心仪表板确认客户接受。

**选项 2**：客户直接接受 - 合作伙伴可以通过 URL 邀请客户在 Microsoft 365 管理中心查看并接受协议。

## <a name="access-microsoft-customer-agreement-template"></a>访问 Microsoft 客户协议模板

可以从[此处](https://aka.ms/customeragreement)手动下载最新版 Microsoft 客户协议模板。 Microsoft 客户协议特定于国家/地区。 在请求 Microsoft 客户协议模板时，请确保根据客户的位置选择正确的国家/地区。

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>选项 1：在合作伙伴中心中确认客户已接受协议

对于新客户和现有客户，合作伙伴可以在合作伙伴中心确认客户接受 Microsoft 客户协议。 经销商不能代表其客户进行证明，需通过其间接提供商来完成证明。

### <a name="confirm-customer-acceptance-for-new-customers"></a>确认新客户接受了协议

在合作伙伴中心创建新客户租户时，请按以下步骤确认客户接受了 Microsoft 客户协议。 必须是管理员代理或销售代理才能执行这些步骤。

1. 选择“客户”，然后选择“新客户”。

2. 在“帐户信息”下，输入公司及其主要联系人的信息。

3. 在“Microsoft 协议”下，选中相应的框来证明客户已接受 Microsoft 客户协议。

4. 在“协议接受日期”下，输入相应的日期。 不能将此日期设置为未来日期。

5. 确保显示的主要用户联系人信息正确。 如果不正确，请选择“更新”并输入接受该协议的人员的准确信息。

6. 选择“下一步”继续创建客户租户。

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客户":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>确认现有客户接受了协议

必须是管理员代理或销售代理才能执行此操作：

1. 选择“客户”。 找到并选择客户。

2. 选择“帐户信息”。

3. 在“Microsoft 客户协议”下选择“更新”。

4. 输入已接受协议的人员的**名字**、**姓氏**、**电子邮件地址**和**电话号码**（可选）。 在“协议接受日期”下，输入相应的日期。 不能将此日期设置为未来日期。

5. 选择“保存”，然后继续操作。

   :::image type="content" source="images/mcua2-update2.png" alt-text="现有客户":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>检索客户接受协议的确认信息

可以按下述步骤检索关于现有客户已接受 Microsoft 客户协议的确认信息。 必须是管理员代理或销售代理才能执行此操作。

1. 选择“客户”，然后找到并选择要查看的客户。

2. 选择“帐户信息”。

3. 在“Microsoft 客户协议”下，查看该客户是否提供过确认。

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>使用合作伙伴中心 API/SDK 确认客户接受协议

可以使用合作伙伴中心 API/SDK 确认客户接受 Microsoft 客户协议。 有关 API/SDK 的详细信息，请参阅：

- [获取 Microsoft 客户协议的协议元数据](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [确认客户接受 Microsoft 客户协议](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [获取客户接受 Microsoft 客户协议的确认](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [获取 Microsoft 客户协议模板的下载链接](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>选项 2：客户在 Microsoft 365 管理中心接受协议

合作伙伴可以通过 URL 邀请新客户和现有客户在 Microsoft 365 管理中心查看并接受协议。 接下来的几部分介绍如何执行以下操作：

- 创建一个新客户，并邀请该客户查看并接受协议。

- 邀请新客户查看并接受经销商关系和协议。

- 邀请现有客户查看并接受协议。

>[!NOTE]
> 可以使用[合作伙伴中心 API/SDK](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) 来获取客户直接接受 Microsoft 客户协议的状态。  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>创建一个新客户，并邀请该客户查看并接受协议

使用以下步骤在合作伙伴中心创建新客户，并邀请他们在 Microsoft 365 管理中心查看并接受 Microsoft 客户协议。

1. 从合作伙伴中心的“客户”选项卡中，选择“添加客户”。

2. 在“帐户信息”下的所有必填字段中输入新客户的信息，包括客户的公司名称和主要联系人。

3. 在“客户协议”下选择第一个选项，即“将要求客户在 Microsoft 365 管理中心接受 Microsoft 客户协议”。 完成页面上的所有其他必填字段。

4. 选择“下一步:查看”，然后继续执行创建客户租户的步骤。 

>[!NOTE] 
>新客户必须接受 Microsoft 客户协议才能进行新的购买。  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="创建新客户":::

5. 到达新客户工作流中的“确认”屏幕后，保存客户凭据。 稍后需将这些凭据分配给客户。

6. 在合作伙伴中心外部，创建并发送一封电子邮件，邀请客户在 Microsoft 365 管理中心接受 Microsoft 客户协议。 请确保电子邮件中包含以下项：

   - 此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的链接（需要登录）

   - 在步骤 5 中保存的客户凭据。

7. 然后，客户会收到来自合作伙伴的电子邮件邀请，并会选择 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。

8. 客户使用之前从合作伙伴处收到的客户凭据登录 Microsoft 365 管理中心。

9. 然后，客户选中用于接受 Microsoft 客户协议的复选框。

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>邀请新客户查看并接受经销商关系和 Microsoft 客户协议 

通过以下步骤邀请新客户查看并接受经销商关系和 Microsoft 客户协议。 

1. 从合作伙伴中心的“客户”选项卡中选择“请求建立经销商关系”链接。  

2. 系统会生成自动电子邮件模板，其中包括文本和参数化 URL，用于将客户定向到 Microsoft 365 管理中心。

3. 可以自定义自动生成的电子邮件模板，然后选择“复制到剪贴板”或“在电子邮件中打开”。 

4. 使用此电子邮件模板邀请客户接受**经销商关系**请求和 **Microsoft 客户协议**。 （注意：在电子邮件邀请中，请确保合作伙伴还包括自动提供的 URL 以及最近创建的客户凭据。）

   :::image type="content" source="images/mca/createrelationship.png" alt-text="创建关系":::

5. 客户通过电子邮件接收邀请，并单击参数化 URL。 

6. 客户使用电子邮件中合作伙伴提供的凭据登录 Microsoft 365 管理中心。

7. 客户选中用于接受**经销商关系**和 **Microsoft 客户协议**的复选框。 

8. 在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。 客户可以选择一个合作伙伴来查看详细信息。

   :::image type="content" source="images/mca/accept.jpg" alt-text="接受协议":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>邀请现有客户查看并接受协议

通过以下步骤邀请现有客户查看并接受 Microsoft 客户协议。 

1. 创建包含嵌入 URL 的客户电子邮件，邀请客户接受 Microsoft 客户协议。

2. 客户通过电子邮件接收邀请，并单击 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。 

3. 客户将其凭据输入 Microsoft 365 管理中心。

4. 客户选中用于接受 Microsoft 客户协议的复选框。 

5. 在同一 URL 中，客户可以查看与其协作的不同合作伙伴的合并列表。 客户可以选择一个合作伙伴来查看详细信息。

   :::image type="content" source="images/mca/customeraccept.png" alt-text="客户":::

>[!NOTE]
>在某些情况下，客户可能无法直接接受 Microsoft 客户协议。 若要详细了解这些情况，请参阅[需要代表客户证明的两种情况](attest-acceptance-customer-agreement.md)。

### <a name="historical-timeline-details"></a>历史时间线详细信息

| 日期 | 里程碑 | 详细信息 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|在沙盒中提供 UX 预览版|合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心面板确认客户接受 Microsoft 客户协议。 有权访问 CSP 沙盒环境的合作伙伴可以预览用户体验更改。 无权访问沙盒的合作伙伴可以在本主题中了解这些更改。|
|2019 年 9 月 3 日|在沙盒中提供 API 预览版。|合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心 API 确认客户接受 Microsoft 客户协议。 API 合作伙伴可以利用此机会预览 API 更改，并开始使用 API 集成为新协议提供支持。|
|2019 年 9 月 20 日|在沙盒中提供 .NET SDK 预览版。|合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心 .NET SDK 来确认客户接受 Microsoft 客户协议。 API 合作伙伴可以利用此机会预览 .NET SDK 更改，并开始使用 API 集成为新协议提供支持。|
|2019 年 10 月 1 日|在生产环境中提供 Microsoft 客户协议|Microsoft 推出针对云解决方案提供商计划的 Microsoft 客户协议，替代 Microsoft 云协议。 合作伙伴可以在生产环境中使用合作伙伴中心面板和 API 确认客户接受 Microsoft 客户协议。 Microsoft 云协议在云解决方案提供商合作伙伴计划中仍受支持。 不过，我们建议合作伙伴着手迁移到 Microsoft 客户协议。 进行新的购买以及对现有订阅进行席位计数更改时，都会要求合作伙伴确认 Microsoft 客户协议或 Microsoft 云协议。 某些新的套餐（例如，新的 Azure 计划）会要求确认 Microsoft 客户协议。|
|2020 年 1 月 31 日|已从生产环境中删除 Microsoft 云协议|云解决方案提供商合作伙伴计划不再接受 Microsoft 云协议。 进行新的购买以及对现有订阅进行席位计数更改时，都会要求合作伙伴确认 Microsoft 客户协议。 此要求适用于新客户以及可能在以前接受了 Microsoft 云协议的现有客户。|
|2020 年 2 月 3 日|合作伙伴现在可以使用相关选项，通过 URL 邀请客户在经身份验证的 Microsoft 365 管理中心查看并接受协议。 | 客户可以在 Microsoft 365 管理中心接受 Microsoft 客户协议。 客户在 Microsoft 365 管理中心直接接受协议即可确认对条款进行了批准。 
