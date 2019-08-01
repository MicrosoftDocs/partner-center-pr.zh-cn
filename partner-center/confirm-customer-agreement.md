---
title: 确认客户接受 Microsoft 客户协议 |合作伙伴中心
ms.topic: article
ms.date: 04/16/2019
Description: 作为合作伙伴, 你需要获取客户对 Microsoft 客户协议的接受, 然后才能对该客户的 Microsoft 产品和服务进行排序。 为了更好地帮助合作伙伴满足合规性要求, Microsoft 要求合作伙伴提供与接受协议的人员有关的特定详细信息, 以确认验收。
author: LauraBrenner
ms.author: labrenne
keywords: 客户, 客户, 同意, MCA, Microsoft 云协议, Microsoft 客户协议, 客户协议模板
ms.localizationpriority: medium
ms.openlocfilehash: 6ca8eb3acdee0114f01dbd5952e9c092859147a2
ms.sourcegitcommit: ee722dc2b9d82557d273738b64cec6d8cb435084
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "68681753"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>确认客户接受 Microsoft 客户协议 (预览版)

目前, 在 CSP 合作伙伴可以代表客户订购之前, 客户必须接受并签署适用的**Microsoft 云协议**。 然后, 合作伙伴必须通过向 Microsoft 提供有关签名者的信息来确认客户的接受。 如果客户未确认接受 Microsoft 云协议:
- 你将无法为此客户创建新订单。
- 你将无法为此客户更改基于席位的订阅的席位计数。

有关如何使用合作伙伴中心仪表板或 API 确认客户接受 Microsoft 云协议的详细信息, 请参阅[确认客户接受 Microsoft 云协议](confirm-consent.md)。

2019年10月1日, Microsoft 将向 CSP 计划提出**Microsoft 客户协议**来替换 Microsoft 云协议。 为了促进合作伙伴迁移到新协议, 在2019年1月31日之前, 将在 CSP 计划中支持当前 Microsoft 云协议。 有关时间线的详细信息, 请参阅下表:

| Date | 里程碑 | 详细信息 |
|------------|------------|--------------------------------|
|2019年8月01日|沙盒中提供 UX 预览|合作伙伴可以在 CSP 沙箱环境中使用合作伙伴中心仪表板确认客户对 Microsoft 客户协议的接受。 具有 CSP 沙箱环境访问权限的合作伙伴可以预览用户体验更改。 没有沙箱访问的合作伙伴可以了解本主题中的更改。|
|2019年9月2日|沙盒中提供了 API 预览。|合作伙伴可以在 CSP 沙箱环境中使用合作伙伴中心 API 确认客户接受 Microsoft 客户协议。 API 合作伙伴可以利用此机会预览 API 更改并开始处理 API 集成, 以支持新的协议。|
|2019年10月01日|生产中可用的 Microsoft 客户协议|Microsoft 向 CSP 计划推出了 Microsoft 客户协议来替换 Microsoft 云协议。 合作伙伴可以在生产中使用合作伙伴中心仪表板和 API 来确认客户接受 Microsoft 客户协议。 CSP 合作伙伴计划中仍支持 Microsoft 云协议。 但是, 建议合作伙伴开始迁移到 Microsoft 客户协议。 对于现有订阅, 新的购买和座位计数更改将要求合作伙伴确认 Microsoft 客户协议或 Microsoft 云协议。 某些新产品/服务 (例如, 新的 Azure 计划) 将需要确认 Microsoft 客户协议。|
|2019年1月31日|从生产中删除 Microsoft 云协议|CSP 合作伙伴计划中不再接受 Microsoft 云协议。 对于现有订阅, 新的购买和座位计数更改将要求合作伙伴提供 Microsoft 客户协议的确认。 此要求适用于以前可能已接受 Microsoft 云协议的新客户和现有客户。|


## <a name="confirm-customer-acceptance-for-new-customers"></a>确认客户对新客户的接受

在合作伙伴中心创建新客户租户时, 请使用以下步骤确认客户接受 Microsoft 客户协议。 若要执行这些步骤, 您必须是管理员代理或销售代理。

1. 选择**客户**，然后选择**新客户**。

2. 在 "**帐户信息**" 下, 为公司及其主要联系人输入信息。

3. 在 " **microsoft 协议**" 下, 选择 " **microsoft 客户协议**"。

4. 在**协议接受日期**下，输入相应的日期。 不能将此日期设置为未来日期。

5. 请确保显示的主要用户联系人信息正确。 如果不正确, 请选择 "**更新**" 并输入接受协议的人员的**名字**、**姓氏**、**电子邮件地址**和**电话号码**(可选)。

6. 选择**下一步**，继续执行创建客户租户的其余步骤。

![新客户](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>确认客户对现有客户的接受

您必须是管理员代理或销售代理才能执行此操作:

1. 选择 "**客户**"。 查找并选择 "客户"。

2. 选择 "**帐户信息**"。

3. 在 " **Microsoft 客户协议**" 下, 选择 "**更新**"。

4. 输入接受协议的人员的**名字**、**姓氏**、**电子邮件地址**和**电话号码**(可选)。 在**协议接受日期**下，输入相应的日期。 不能将此日期设置为未来日期。

5. 选择 "**保存**并继续"。

![现有客户](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>检索客户验收确认

您可以使用以下步骤检索现有客户已接受 Microsoft 客户协议的确认。 必须是管理员代理或销售代理，才能执行此操作。

1. 选择**客户**，然后查找并选择要查看的客户。

2. 选择 "**帐户信息**"。

3. 在 " **Microsoft 云协议**" 下, 查看此客户是否已提供确认。


