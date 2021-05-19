---
title: 信用额度强制执行
ms.topic: how-to
ms.date: 05/11/2021
description: 了解信用限制及其计算方式。 包含常见问题解答。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148102"
---
# <a name="credit-limit-enforcement-cle"></a>信用限制实施 (CLE) 

**适当的角色**：计费管理员

## <a name="your-credit-limit-and-how-it-works"></a>信用限制及其工作原理

信用限制是指作为合作伙伴可以用来在合作伙伴中心购买产品或订阅的最大 (，以美元为) 。 如果超出了信用额度，则无法进行新的购买，直到进行了充足的付款。 现有订阅将继续不间断地继续。

信用限制适用于 Azure 计划、Azure 预订、软件、Marketplace、Azure 145 P、Office 和 Dynamics 产品中的产品/服务。 信用限制不适用于续订和持续消耗。

在载入期间，我们会在租户级别分配信用限制。 我们基于预测收入、购买技能和付款历史记录。 然后，使用以下公式来计算可用余额：

**[信用限制– (传入购买 + 未付的未付款发票 + 未开票费用–超额支付) ]**

## <a name="frequently-asked-questions"></a>常见问题

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>我的信用额度是否设置为租户或全局级别？

租户级别。 例如，假设您从美国、加拿大和日本进行操作。 如果加拿大租户达到其信用额度，则当租户尝试在合作伙伴中心购买时，会收到通知。 其他租户将不会受到影响。 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>如果我超过了信用限制，是否可以继续使用完全访问权限为现有客户和订阅提供服务？

是。 客户的现有订阅将继续进行，而不会中断。 但是，不能为客户购买新订阅。

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>直接计费合作伙伴和间接提供商是否同时应用了 CLE？

是的，这两者均适用。

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>提交付款以恢复帐户后，何时可以购买更多订阅？ 

假设 Microsoft 已收到继续进行信用检查过程的所有要求，你应该能够在付款后 24 小时内恢复购买。

### <a name="how-can-i-check-my-credit-limit"></a>如何检查信用额度？

请联系 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 查看信用额度限制，并获取有关最近购买的信息。

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>存在争议的发票是否计入信用额度限制？

是。 但是，可以通过 联系 Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 来解决此问题。

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>如果我向 写入了 ，多久就会听到回信 ucmwrcsp@microsoft.com ？

应在 24 小时内收到响应。 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Microsoft 使用什么条件来设置合作伙伴的信用额度限制？

我们根据预测的收入、购买能力以及付款历史记录来确定信用额度限制。

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>新商务体验当前是否强制实施了信用额度限制？

是。 信用额度适用于所有云解决方案提供商计划和合作伙伴中心。

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>我的组织即将达到其信用额度限制时，谁会收到通知？

组织的 Finance Account Should 联系人应收到通知。

## <a name="next-steps"></a>后续步骤

[计费基础知识](./billing-basics.md)
