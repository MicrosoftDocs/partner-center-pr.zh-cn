---
title: 从 PMC 迁移到合作伙伴中心的指南 | 合作伙伴中心
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何将你的公司从 Partner Membership Center (PMC) 迁移到合作伙伴中心。
author: LauraBrenner
ms.author: labrenne
keywords: PMC, 迁移, 移到合作伙伴中心
ms.localizationpriority: high
ms.openlocfilehash: f9ce53adddd2faecf22ef795e8ffe97189c57353
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252204"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>从 PMC 迁移到合作伙伴中心的指南

Microsoft 合作伙伴网站 partner.microsoft.com 是面向合作伙伴的统一数字体验。 通过合作伙伴网站，可以发掘商机并参与引导式体验，帮助公司在 Microsoft 的配合下构建和销售应用与服务。 Microsoft 合作伙伴网络的会员可以使用整个合作伙伴网站上提供的“仪表板”链接登录到合作伙伴中心，在其中可以管理与 Microsoft 之间的关系、注册计划和注册套餐。 

Partner Membership Center (PMC) 即将停用。 我们已邀请贵公司将 Microsoft 合作伙伴网络会员管理过渡到合作伙伴中心。 本指南将描述在从 PMC 迁移到合作伙伴中心时期望会出现的情况，以此帮助你做好迁移准备。

>[!Note]
>即使公司有多个帐户或在多个位置运营，迁移到合作伙伴中心的过程一开始也只会将一个帐户（你的第一个帐户）移到合作伙伴中心。

## <a name="get-started"></a>立即开始行动

迁移从 PMC 开始。 全局管理员将会收到开始迁移的邀请。 

**在 PMC 中做好准备**
- 验证公司详细信息 
- 验证计划的主要联系人 
- 验证企业位置
- 更新已批准的用户

**准备就绪时**

在邀请信件中选择“开始”。  随后会转到合作伙伴中心登录页。

![立即开始行动](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>从工作电子邮件开始

如果公司没有工作电子邮件和 AAD 租户，在合作伙伴中心登录过程中，我们可以帮助你设置一个。 如果尝试使用不属于工作电子邮件的电子邮件帐户（例如个人帐户）登录，网站会指示你提供有关公司的信息，以便我们可以设置 AAD 租户和工作电子邮件。
这些公司详细信息用于在合作伙伴中心完成帐户设置，因此请确保信息准确无误。

>[!Note]
>如果你是位于中国的合作伙伴并已同时注册 Microsoft 合作伙伴网络和云解决方案提供商 (CSP) 计划，则每个帐户都有一个单独的租户。 注册了云解决方案提供商计划的帐户将在国家云中进行管理，而 Microsoft 合作伙伴网络帐户将在全球云中进行管理。 无法链接这两个帐户。

![将公司信息告诉我们](images/migration/newtellusabout.png)

验证或更新信息后，选择“接受并继续”。 
此页上的条款和条件与公司已在 PMC 中签署的协议**完全相同**。  
然后，将开始创建 Azure AD 租户并提供工作帐户。

选择“接受并继续”还会执行以下操作： 

•   将帐户连同其所有位置一起迁移到合作伙伴中心

•   迁移你可能在 PMC 中购买的任何资质或 MAP

•   迁移你在 PMC 中享有的任何权益（MAP、银级、金级）

## <a name="invite-employees-to-join-you"></a>邀请员工加入

创建新的 Azure AD 租户后，可以邀请员工登录到合作伙伴中心。

![邀请员工](images/migration/invite.png)


如果你已使用现有的 AAD 租户登录，则员工的信息和权益也已同你一起迁移。 在这种情况下，请分配员工角色，以确定他们可在合作伙伴中心执行哪些操作。 注意：合作伙伴中心内的角色不同于 PMC 中的角色。 有关详细信息，请参阅[从 PMC 迁移到合作伙伴中心](move-pmc-pc-map.md)。

## <a name="verify-your-domain-and-become-a-global-admin"></a>验证域并成为全局管理员  

如果 AAD 租户是新的，则暂时还没有为任何人分配全局管理员角色。若要成为全局管理员，需要验证域所有权。 可能需要求助域管理员来完成此操作。 请注意，尽管可以使用已购买的套餐，但在完成获取全局管理员角色的步骤之前，无法购买任何新套餐。 

![获取控制权](images/migration/takecontrol.png)

选择“开始”后，将看到以下屏幕：

![验证域所有权](images/migration/verifytxt.png)

网站中已填充域注册机构。 只有域所有者可以更新 DNS 文件，我们可以通过将该文本文件复制并添加到 DNS 记录，来验证你是否为所有者。 完成更新需要几分钟时间。 需要从合作伙伴中心注销，然后重新登录。 你的角色将更改为全局管理员。 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>熟悉仪表板和合作伙伴中心

全面浏览一下仪表板。 在仪表板中可以管理会员资格、添加企业档案供我们引荐、注册云解决方案提供商计划，并随时可以通过选择“仪表板”来查看与自己的业务相关的通知和套餐。  还可以管理奖励、在市场中购买套餐、注册市场投放服务，等等。  

![全面浏览](images/migration/fre.png)

## <a name="next-steps"></a>后续步骤

- [创建用户帐户](create-user-accounts-and-set-permissions.md)
- [为用户分配角色和权限](permissions-overview.md)
- [管理成员身份计划](renew-mpn-offers.md)
- [创建公司的业务配置文件](create-a-marketing-profile.md)
- [通过引荐与客户联系](responding-to-referrals.md)

## <a name="see-also"></a>另请参阅

- [将多个公司从 PMC 迁移到合作伙伴中心的指南](move-multiple-companies.md)
