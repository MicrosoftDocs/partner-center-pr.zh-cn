---
title: 确认客户接受 Microsoft 客户协议 | 合作伙伴中心
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何确认客户接受 Microsoft 客户协议。 这可能需要为客户订购 Microsoft 产品和服务。
author: LauraBrenner
ms.author: labrenne
keywords: 客户, 许可, MCA, Microsoft 云协议, Microsoft 客户协议, 客户协议模板
ms.localizationpriority: medium
ms.openlocfilehash: 9d362f581d0d318b1a457ba6a75db54713fce6bb
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252224"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>确认客户接受 Microsoft 客户协议

目前，在 CSP 合作伙伴可以代表客户订购之前，客户必须接受并签署适用的**Microsoft 云协议**。 然后，合作伙伴必须向 Microsoft 提供签署人的相关信息，确认客户已接受协议。 如果未提供确认信息：
- 你将无法为此客户创建新订单。
- 你将无法更改此客户的现有基于座位的订阅的座位数。

若要详细了解如何使用合作伙伴中心面板或 API 来确认客户已接受 Microsoft 云协议，请参阅[确认客户接受 Microsoft 云协议](confirm-consent.md)。

2019 年 10 月 1 日，Microsoft 将推出针对云解决方案提供商计划的 **Microsoft 客户协议**，替代 Microsoft 云协议。 为了方便合作伙伴迁移到新协议，在 2020 年 1 月 31 日之前，云解决方案提供商计划仍会支持当前的 Microsoft 云协议。 如需更多的时间线详细信息，请查看下表：

| 日期 | 里程碑 | 详细信息 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|在沙盒中提供 UX 预览版|合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心面板确认客户接受 Microsoft 客户协议。 有权访问 CSP 沙盒环境的合作伙伴可以预览用户体验更改。 无权访问沙盒的合作伙伴可以在本主题中了解这些更改。|
|2019 年 9 月 3 日|在沙盒中提供 API 预览版。|合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心 API 确认客户接受 Microsoft 客户协议。 API 合作伙伴可以利用此机会预览 API 更改，并开始使用 API 集成为新协议提供支持。|
|2019年9月20日|在沙盒中提供 .NET SDK 预览版。|合作伙伴可以在云解决方案提供商沙盒环境中使用合作伙伴中心 .NET SDK 来确认客户接受 Microsoft 客户协议。 API 合作伙伴可以利用此机会预览 .NET SDK 更改，并开始使用 API 集成为新协议提供支持。|
|2019 年 10 月 1 日|在生产环境中提供 Microsoft 客户协议|Microsoft 推出针对云解决方案提供商计划的 Microsoft 客户协议，替代 Microsoft 云协议。 合作伙伴可以在生产环境中使用合作伙伴中心面板和 API 确认客户接受 Microsoft 客户协议。 Microsoft 云协议在云解决方案提供商合作伙伴计划中仍受支持。 不过，我们建议合作伙伴着手迁移到 Microsoft 客户协议。 进行新的购买以及对现有订阅进行席位计数更改时，都会要求合作伙伴确认 Microsoft 客户协议或 Microsoft 云协议。 某些新的套餐（例如，新的 Azure 计划）会要求确认 Microsoft 客户协议。|
|2020 年 1 月 31 日|已从生产环境中删除 Microsoft 云协议|云解决方案提供商合作伙伴计划不再接受 Microsoft 云协议。 进行新的购买以及对现有订阅进行席位计数更改时，都会要求合作伙伴确认 Microsoft 客户协议。 此要求适用于新客户以及可能在以前接受了 Microsoft 云协议的现有客户。|

## <a name="access-microsoft-customer-agreement-template"></a>访问 Microsoft 客户协议模板
合作伙伴可以从[此处](https://aka.ms/customeragreement)手动下载 Microsoft 客户协议模板的最新版本。 请注意，Microsoft 客户协议是国家/地区特定的。 请求 Microsoft 客户协议模板时，请确保根据客户的位置选择正确的国家/地区。 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>使用合作伙伴中心 API/SDK 确认客户接受
合作伙伴可以使用合作伙伴中心 API/SDK 确认客户接受 Microsoft 客户协议。 有关 API/SDK 的详细信息，请参阅：

- [获取 Microsoft 客户协议的协议元数据](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [确认客户接受 Microsoft 客户协议](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [获取客户接受 Microsoft 客户协议的确认](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [获取 Microsoft 客户协议模板的下载链接](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>在合作伙伴中心中确认客户已接受协议
合作伙伴可以在合作伙伴中心确认客户对新客户和现有客户的 Microsoft 客户协议的接受。

### <a name="confirm-customer-acceptance-for-new-customers"></a>确认新客户接受了协议

在合作伙伴中心创建新客户租户时，请按以下步骤确认客户接受了 Microsoft 客户协议。 必须是管理员代理或销售代理才能执行这些步骤。

1. 选择**客户**，然后选择**新客户**。

2. 在“帐户信息”下，输入公司及其主要联系人的信息。

3. 在“Microsoft 协议”下，选择“Microsoft 客户协议”。

4. 在“协议接受日期”下，输入相应的日期。 不能将此日期设置为未来日期。

5. 确保显示的主要用户联系人信息正确。 如果此信息不正确，请选择“更新”，然后输入已接受协议的人员的**名字**、**姓氏**、**电子邮件地址**和**电话号码**（可选）。

6. 选择“下一步”，继续执行创建客户租户的其余步骤。

![新客户](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>确认现有客户接受了协议

必须是管理员代理或销售代理才能执行此操作：

1. 选择“客户”。 找到并选择客户。

2. 选择“帐户信息”。

3. 在“Microsoft 客户协议”下选择“更新”。

4. 输入已接受协议的人员的**名字**、**姓氏**、**电子邮件地址**和**电话号码**（可选）。 在“协议接受日期”下，输入相应的日期。 不能将此日期设置为未来日期。

5. 选择“保存”，然后继续操作。

![现有客户](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>检索客户接受协议的确认信息

可以按下述步骤检索关于现有客户已接受 Microsoft 客户协议的确认信息。 必须是管理员代理或销售代理才能执行此操作。

1. 选择**客户**，然后查找并选择要查看的客户。

2. 选择“帐户信息”。

3. 在“Microsoft 客户协议”下，查看该客户是否提供过确认。
