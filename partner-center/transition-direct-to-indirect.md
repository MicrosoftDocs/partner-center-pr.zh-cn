---
title: 将直接计费合作伙伴切换到间接经销商
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 计划合作伙伴如何使用 合作伙伴中心从直接计费合作伙伴过渡到间接经销商。
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57c4a5d0a02079e887b38fa9754d276062d20cc
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276410"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a>从云解决方案提供商 (CSP) 计划直接计费合作伙伴过渡到云解决方案提供商计划间接经销商

**相应的角色**：全局管理员

>[!Note]
>本文适用于决定过渡到间接经销商的直接计费合作伙伴。 但是，即使你尚未明确决定注册为间接经销商，当其直接计费功能受限时，Microsoft 也会通知不满足 CSP[](direct-partner-new-requirements.md)直接计费合作伙伴计划新要求的直接计费[合作伙伴。](restricted-direct-bill-capabilities.md)
<br>从 2021 年 1 月开始，将添加新的收入要求。 注册为直接计费合作伙伴的合作伙伴需要在过去 12 个月内在 云解决方案提供商 合作伙伴全局帐户级别交易至少 30 万美元的计划收入。

你将能够使用现有的直接计费租户注册间接经销商计划。

## <a name="get-started"></a>入门

1. 请确保你的合作伙伴配置文件合作伙伴中心 MPN ID 是最新的。

2. 以合作伙伴中心间接经销商的直接计费租户的全局管理员角色登录。

   :::image type="content" source="images/direct/direct1.png" alt-text="概述。":::

3. 查看注册表单上的合作伙伴详细信息。

   :::image type="content" source="images/direct/direct2a.png" alt-text="立即注册。":::

4. 选择“立即注册”。 间接经销商业务将使用用于直接业务的同一 AAD 租户。

    > [!NOTE]
    > 最初，这一新的转换功能适用于具有 9 月到 12 月周年日期的合作伙伴。 如果 9 月到 12 月之间没有周年日期，此时将看不到该功能。 为合作伙伴启用此功能后，2018 年 12 月之后具有周年日期的合作伙伴将收到通知。

5. 注册获得批准后，请再次合作伙伴中心注册。

    > [!NOTE]
    > 虽然审批通常是即时的，但最多可能需要五个工作日。 获得批准后，你将收到一条通知，告知你在注册窗体中的主要联系人下指定的电子邮件地址。 还可以在"设置帐户设置合作伙伴配置文件 **"和"** 计划信息"下>  >    >  状态。

6. 在" **概述** "页上，你将看到间接经销商协议。 选择 **接受并继续操作**。 此操作启用间接经销商功能。

接受间接经销商协议后，请注意，合作伙伴配置文件将你标识为直接计费和间接经销商。

:::image type="content" source="images/direct/direct3.png" alt-text="间接经销商协议。":::

> [!IMPORTANT]
> 使用新功能注册为间接经销商后，无法回退到直接计费租户。 在注册为间接经销商之前，请确保全面评估业务需求。

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a>从直接经销商过渡到间接经销商时

在此阶段，你将继续管理直接客户的订阅需求，包括计费过程。 还可以开始接受来自间接提供商的客户，并作为间接经销商运营。

:::image type="content" source="images/direct/direct4.png" alt-text="你是直接计费和间接经销商。":::

## <a name="find-an-indirect-provider"></a>查找间接提供商

注册后，左侧导航导航中会显示指向间接提供商的链接。 作为间接经销商，你将与间接提供商建立关系，该提供商随后可以处理计费、为客户购买产品和支持基础结构。

不同的间接提供商会提供不同的支持和服务，因此你应该评估所在地区的提供商，确定哪些提供商最能够满足你的需求。 通常，大多数提供商将：

- 为你提供技术培训和援助
- 帮助你推销产品和服务
- 管理额度和信用额度

搜索官方 Microsoft 间接 [提供商的列表](https://partnercenter.microsoft.com/partner/find-a-provider)。

有关详细信息，请阅读  [与间接提供商合作](indirect-reseller-tasks-in-partner-center.md)

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a>接受来自间接提供商的合作关系邀请

当你找到要与间接提供商合作时，请与云中的间接提供商合作伙伴中心。

你选择的间接提供商将通过电子邮件将合作伙伴邀请链接发送给你，该链接将让你在 合作伙伴中心。 请确保全局管理员登录 合作伙伴中心并遵循邀请链接。 接受邀请时，提供商的名称将显示在间接提供商列表中。

## <a name="acquire-new-customers-as-indirect-reseller"></a>获取作为间接经销商的新客户

你和间接提供商都需要与客户建立经销商关系。 通过这些经销商关系，你可以代表客户管理客户的订阅和服务。 若要获取具有现有租户的Azure AD客户，可以邀请客户同时与你和提供商建立经销商关系。

创建间接经销商邀请：

1. 从 **左侧导航导航** 合作伙伴中心间接提供商"。

2. 选择“邀请新客户”以邀请客户同时与你和间接提供商建立经销商关系。 提供商需要与客户建立经销商关系，以便客户想要购买新订阅或将新许可证添加到现有订阅时，可以代表客户提交订单。

3. 在下一页上，查看草稿电子邮件。 可以在电子邮件中打开草稿消息，也可以将邮件复制到剪贴板并将其粘贴到电子邮件中。

4. 编辑电子邮件中的文本，以说明所需的内容，但请务必包含该链接，因为它已个性化，可将客户直接连接到帐户和提供商的帐户。 然后选择“完成”。

5. 客户准许你和你的提供商成为其备案经销商后，你将拥有管理员权限，可以代表他们管理其订阅、许可证和用户，并且你的间接提供商将能够代表他们提交订单。
6. 若要管理客户的帐户、服务、用户和许可证，请选择客户名称旁边的向下箭头，展开客户的记录。

与直接计费合作伙伴不同，间接经销商无法为Azure AD中的新客户创建合作伙伴中心。 提供商将创建租户，并指定你作为此客户的间接经销商。 这可确保客户将显示在客户列表中的合作伙伴中心。

>[!Note]
>你将无法使用直接计费功能为作为间接经销商获取的客户创建购买。

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a>管理直接计费客户和间接经销商客户

你以不同方式管理直接计费客户和间接经销商客户。

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a>直接计费 (不作为间接经销商客户执行) 

- 为产品创建订单
- 管理 Azure 预留项
- 管理其订单历史记录
- 购买软件
- 直接为客户计费

### <a name="indirect-reseller-customers"></a>间接经销商客户

- 间接提供商为客户订购产品
- 管理客户的许可证和用户
- 处理订阅续订

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a>确定作为直接计费合作伙伴获取的客户

1. 选择“客户”。

2. 选择客户以查看其详细信息。

3. 如果此客户是作为直接计费合作伙伴获取的客户，你将看到添加或查看产品的选项，并且会看到其订阅。

4. 如果客户与你有间接经销商关系，则这些选项将不可用。

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a>将直接计费客户移到间接提供商

在间接提供商与现有直接计费客户建立经销商关系之前，他们无法提交订单或现有订阅转移。 若要在间接提供商和现有的直接计费客户之间建立经销商关系，可以使用以下方法之一：

- [经销商关系扩展](#reseller-relationship-extension)

- [向客户发送间接经销商邀请](#send-an-indirect-reseller-invitation-to-the-customer)

可以在直接到间接转换文档中找到分步 [过程的详细概述](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)

### <a name="reseller-relationship-extension"></a>经销商关系扩展

可以使用经销商关系扩展功能，通过仪表板在现有的直接计费客户和间接提供商合作伙伴中心关系。 使用该功能之前，请注意以下事项：

- 此功能仅适用于正在过渡到间接经销商的直接计费合作伙伴，这些合作伙伴已完成间接 [经销商注册](#get-started)。

- 只能将此功能应用于现有的直接计费客户。 它不适用于间接 [经销商客户](#acquire-new-customers-as-indirect-reseller)。

- 只能选择已接受来自间接提供商 的合作伙伴 [邀请的间接提供商](#accept-a-partnership-invitation-from-your-indirect-provider)。

- 你为此客户提供的计费对象信息副本将提供给间接提供商。 可以通过在仪表板中访问此客户的"帐户"页来访问合作伙伴中心信息。

    > [!NOTE]
    > 使用分销商关系扩展功能，即表示你同意使用间接提供商共享此客户的帐单信息。

- 你的间接提供程序将不会提供给客户租户的 [委派管理权限](customers-revoke-admin-privileges.md) 。 如果间接提供商需要委派的管理权限，则必须改为向客户发送间接经销商邀请。

- 建立分销商关系后，在 [Microsoft 365 管理中心](https://admin.microsoft.com/AdminPortal/Home#/partners) 和 [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business)的 "合作伙伴关系" 页下，间接提供商将显示为客户的 CSP 合作伙伴。

    > [!IMPORTANT]
    > 若要避免混淆和误解，你的合作伙伴协议会合同形式不必，以便在使用关系扩展功能建立现有直销客户和间接提供商之间的分销商关系之前通知并获得直接帐单客户的同意。

在现有客户租户上使用此功能：

1. 以 **管理代理** 的身份登录到合作伙伴中心。

2. 在 " **客户" 页** 上，选择现有客户，并单击其 " **快速链接** " 图标以展开客户的 "摘要" 视图。

3. 在 **间接提供程序 (s)** 下，单击 " **在间接提供程序上传输客户**"。

    :::image type="content" source="images/direct/direct5-1.png" alt-text="将客户转移到间接提供商。":::

4. 在弹出对话框中，选择要与客户建立分销商关系的 **间接提供商** 。

5. 单击“保存并继续”。

6. 验证所选的间接提供程序是否以 **间接提供程序 (s)** 显示。

    :::image type="content" source="images/direct/direct5-2.png" alt-text="间接提供程序已列出。":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a>向客户发送间接经销商邀请

如果你的间接提供商与客户的销售商关系，你的间接提供商将无法提交订单。 若要在现有客户和间接提供商之间建立经销商关系，请使用间接经销商邀请邀请客户。

1. 从合作伙伴中心左侧导航栏中选择 " **间接提供程序** "。

2. 选择“邀请新客户”以邀请客户同时与你和间接提供商建立经销商关系。 提供商需要与客户建立分销商关系，因此，当客户想要购买新订阅或向现有订阅添加新许可证时，他们可以代表客户提交订单。

    :::image type="content" source="images/direct/direct6.png" alt-text="邀请新客户。":::

3. 在下一页上，查看草稿电子邮件。 可以通过电子邮件打开草稿邮件，也可以将邮件复制到剪贴板，然后将其粘贴到电子邮件中。

4. 编辑电子邮件中的文本以说明所需内容，但请确保在个性化的同时将该链接连接到帐户和提供商的帐户。 然后选择“完成”。

5. 客户准许你和你的提供商成为其备案经销商后，你将拥有管理员权限，可以代表他们管理其订阅、许可证和用户，并且你的间接提供商将能够代表他们提交订单。

6. 若要管理客户的帐户、服务、用户和许可证，请选择客户名称旁边的向下箭头，展开客户的记录。

### <a name="microsoft-customer-agreement-acceptance"></a>Microsoft 客户协议接受

Microsoft 云协议在2020年1月31日之前有效。 在此日期之后，所有客户（现有和新）都必须签署新的 [Microsoft 客户协议](confirm-customer-agreement.md)。 对于过渡客户，如果：

- **客户尚未接受 Microsoft 客户协议**

   请与间接提供商合作，让客户 [接受 Microsoft 客户协议](confirm-customer-agreement.md)。

- **客户已通过 Microsoft 365 管理中心接受 Microsoft 客户协议**

   一旦与间接提供商建立了分销商关系，就会保留接受。 无需执行任何操作。

- **客户已通过合作伙伴证明接受了 Microsoft 客户协议**

   不会保留接受。 请与间接提供商合作，以 [更新客户在合作伙伴中心的接受](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)情况。

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a>将现有的直接帐单订阅转移到间接提供程序

在 "CSP 间接模型" 下，间接经销商与 Microsoft 没有计费关系。 相反，间接经销商通过其间接提供商获取其客户的订阅。 从直销伙伴过渡到间接经销商时，需要将你的现有订阅作为直接帐单合作伙伴传送到间接提供商。 你可以使用合作伙伴中心仪表板中提供的自助订阅转移功能来执行此操作。

### <a name="prerequisites"></a>先决条件

- 此功能仅适用于使用现有直销合作伙伴租户完成间接经销商注册的合作伙伴。

- 在传输与给定客户关联的订阅之前，过渡合作伙伴必须将客户转移到间接提供商。

- 客户必须已 [通过间接提供商接受了 Microsoft 客户协议](#microsoft-customer-agreement-acceptance)。

### <a name="how-to-transition-to-indirect-reseller-status"></a>如何过渡到间接经销商状态

此功能是一个4步骤过程，其中：

- 过渡伙伴会创建订阅传输请求。 请求中包含一个或多个与同一客户关联的现有订阅，并将其发送到间接提供程序。

- 间接提供程序查看并接受 (或拒绝) 传输请求。

- 间接提供程序验证传输请求是否已完成。

- 过渡伙伴将验证传输请求是否已完成。

### <a name="transitioning-partner"></a>过渡合作伙伴

> [!NOTE]
> 你还可以使用 [合作伙伴中心 API/SDK](/partner-center/develop/manage-customers) 将现有订阅传输到间接提供程序。
>
> - [获取客户的订阅转让资格](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [创建客户的转让](/partner-center/develop/create-a-transfer)
> - [撤消客户的转让](/partner-center/develop/withdraw-a-transfer)
> - [接受客户的转让](/partner-center/develop/accept-a-transfer)
> - [拒绝客户的转移](/partner-center/develop/reject-a-transfer)
> - [获取客户的转让](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [按 id 获取传输详细信息](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a>正在转换合作伙伴-创建传输请求

创建传输请求作为过渡伙伴：

1. 以 **管理代理** 的身份登录到合作伙伴中心。

2. 在 " **客户** " 页上，选择目标客户，并单击 "快速链接" 图标以展开客户的 "摘要" 视图。

3. 在 " **间接提供程序 (s)**" 下，确认列出了预期的间接提供程序。

4. 单击 " **查看订阅**"。

5. 在 " **订阅** " 页中，查找 **订阅传输**。

6. 在 " **订阅传输**" 下，单击 " **请求订阅传输**"。

    :::image type="content" source="images/direct/direct8.png" alt-text="请求订阅传输。":::

7. 在 "传输请求" 对话框中，选择要传输的一个或多个订阅。

    :::image type="content" source="images/direct/direct9.png" alt-text="创建传输请求。":::

8. 单击“创建”。

9. " **订阅传输**" 下将显示一个有效的订阅传输请求。

    :::image type="content" source="images/direct/direct10.png" alt-text="传输请求列表。":::

10. 向间接提供商通知你已创建了订阅传输请求。

### <a name="indirect-provider---accept-transfer-request"></a>间接提供程序-接受传输请求

查看并接受作为间接提供程序的传输请求：

1. 以 **管理** 代理或 **销售代理** 的身份登录到合作伙伴中心。

2. 在 " **客户** " 页上，选择目标客户，并单击其 "快速链接" 图标以展开客户的 "摘要" 视图。

3. 在 " **间接经销商 (s)** 下，确认已列出过渡伙伴。

4. 单击 " **查看订阅**"。

5. 在 " **订阅** " 页中，查找 **订阅传输**。

    :::image type="content" source="images/direct/direct11.png" alt-text="查看传输请求。":::

6. 在 " **订阅传输**" 下，单击要查看的传输请求。

7. 根据需要单击 " **接受** (或 **拒绝**) 。

    :::image type="content" source="images/direct/direct12.png" alt-text="接受传输请求。":::

8. 等待传输请求完成。

### <a name="indirect-provider---verify-transfer-request-is-complete"></a>间接提供程序-确认传输请求已完成

1. 成功完成传输请求后，验证是否可以看到订阅显示在 " **订阅**" 下。

2. 通知转换合作伙伴。

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a>过渡伙伴-验证传输请求已完成

过渡伙伴应执行以下操作：

1. 以 **管理代理** 或 **销售代理** 的身份登录到合作伙伴中心。

2. 在 " **客户** " 页上，选择目标客户，并单击 " **快速链接** " 图标以展开客户的 "摘要" 视图。

3. 单击 " **查看订阅**"。

4. 在 " **订阅** " 页中，查找 **订阅传输**。

5. 验证传输请求是否已标记为已 **完成**。

6. 验证 **"订阅" 页中** () 的订阅不再显示为活动状态：

   1. 如果这是 Azure 订阅 (0145P) ，它将不再列出。

   2. 如果这是基于许可证的订阅 (Office 365，Dynamics，Intune) ，它将以 "已 **挂起**" 状态列出。

   :::image type="content" source="images/direct/direct13.png" alt-text="订阅已挂起。":::

### <a name="considerations"></a>注意事项

- **传输后，订阅 ID 将不同。** 如果它是 Azure 订阅 (BC-OP-NT-AZR-0145P) ，另外，它将具有 Azure 订阅 ID，该 ID 将从以前的所有者保留，并将显示在 Azure 管理门户中。

- **多个传输请求无法引用同一订阅。** 创建了包含现有订阅的传输请求后，在取消第一个传输请求之前，你无法创建包含同一订阅的其他传输请求。

- **基于许可证的订阅的外接程序必须与其基本订阅一起传输。** 创建传输请求时，如果使用一个或多个加载项选择现有订阅，则该加载项将自动包含在传输请求中。

- **现有传输请求中不会反映对订阅的许可证计数更改。** 创建包含现有订阅的传输请求后，应避免更新订阅 (或关联的加载项) 的许可证数量。 如果这样做，新数量将不会在传输请求中反映出来。 在间接提供程序接受传输请求后，生成的订阅将具有旧的数量。 如果希望将新数量转移到间接提供程序，必须取消现有的传输请求并重新创建一个新的请求。

- **并非所有购买都可以使用自助服务订阅传输来传输。** 目前，只能使用此功能)  (BC-OP-NT-AZR-0145P 传输 O365 订阅和 Azure PAYG 订阅。 不支持其他购买内容，包括 Azure 计划、Azure 保留实例、基于字词的订阅和 Azure Marketplace 的 SaaS 订阅。 你将在提交传输请求页中看到无法传输订阅的原因。 若要传输这些订阅，你将需要 [取消现有订阅](create-a-new-subscription.md#suspend-or-cancel-a-subscription) ，并通过间接提供程序为客户购买新的产品/服务。

- **不能使用沙盒环境进行测试。**

## <a name="enroll-for-indirect-reseller-incentives"></a>注册间接经销商奖励

在现有直销合作伙伴租户上成功注册为间接经销商后，你将收到一封邀请，邀请你在30天内注册间接经销商奖励。 邀请基于当前与你的 CSP 合作伙伴租户关联的合作伙伴 MPN 帐户。 邀请将发送到与合作伙伴 MPN 帐户关联的电子邮件地址。

你也有资格向同一合作伙伴租户注册直接帐单激励计划。 您必须单独管理这些程序。

## <a name="next-steps"></a>后续步骤

- [成为间接经销商的其他信息](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [云解决方案提供商计划直接合作伙伴新要求](direct-partner-new-requirements.md)
- [受限的直接计费功能](restricted-direct-bill-capabilities.md)
