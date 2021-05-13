---
title: 信用限制实施
ms.topic: how-to
ms.date: 05/11/2021
description: 了解信用限制及其计算方式。 包含常见问题解答。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819203"
---
# <a name="credit-limit-enforcement-cle"></a>信用限制实施 (CLE) 

**相应的角色**

- 计费管理员

## <a name="your-credit-limit-and-how-it-works"></a>信用限制及其工作原理

信用限制是指作为合作伙伴可以用来在合作伙伴中心购买产品或订阅的最大 (，以美元为) 。 如果超出了信用额度，则无法进行新的购买，直到进行了充足的付款。 现有订阅将继续不间断地继续。

信用限制适用于 Azure 计划、Azure 预订、软件、Marketplace、Azure 145 P、Office 和 Dynamics 产品中的产品/服务。 信用限制不适用于续订和持续消耗。

在载入期间，我们会在租户级别分配信用限制。 我们基于预测收入、购买技能和付款历史记录。 然后，使用以下公式来计算可用余额：

**[信用限制– (传入购买 + 未付的未付款发票 + 未开票费用–超额支付) ]**

## <a name="frequently-asked-questions"></a>常见问题

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>我的信用额度是否设置为租户或全局级别？

租户级别。 例如，假设您从美国、加拿大和日本进行操作。 如果加拿大租户达到其信用额度，则当租户尝试在合作伙伴中心购买时，会收到通知。 其他租户将不会受到影响。 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>如果我超过了信用限制，是否可以继续使用完全访问权限为现有客户和订阅提供服务？

是的。 你的客户的现有订阅将继续进行而不中断。 但是，你不能为客户购买新的订阅。

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>CLE 是否适用于直属客户和间接提供商？

是的，它适用于这两种情况。

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>提交我的付款以恢复我的帐户后，我可以在何时购买更多订阅？ 

你应能够在你的付款24小时内恢复购买，假设 Microsoft 已收到继续信用检查过程的所有要求。

### <a name="how-can-i-check-my-credit-limit"></a>如何检查信用额度？

联系 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 以查看信用限制并获取有关最近购买的信息。

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>是否有针对信用额度的争议计数的发票？

是的。 不过，您可以在上与 Microsoft 联系 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 以解决此问题。

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>如果我要写入，会多久再收到 ucmwrcsp@microsoft.com ？

你的响应应在24小时内。 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Microsoft 用于设置合作伙伴信用限制的条件是什么？

我们根据预测收入、购买技能和付款历史记录来确定信用限制。

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>当前是否在新的商业体验上强制实施信用限制？

是的。 信用限制适用于合作伙伴中心的所有 CSP 计划和产品。

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>如果组织接近信用限制，谁会收到通知？

组织的财务帐户应付帐款联系人应收到通知。

## <a name="next-steps"></a>后续步骤

[计费基础知识](./billing-basics.md)
