---
title: 2021 年 4 月公告
description: Microsoft 合作伙伴中心 2021 年 4 月公告，包括新功能、促销、产品/服务、市场或对现有产品/服务的更改。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702818"
---
# <a name="april-2021-announcements"></a>2021 年 4 月公告

本页提供了 Microsoft 合作伙伴中心 2021 年 4 月公告。

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>就绪情况：更新的 CSP 客户地址验证 API 将于 6 月上线；测试功能现已可用

### <a name="categories"></a>类别

- 日期：2021-04-30
- 就绪

### <a name="summary"></a>总结

为帮助合作伙伴和客户在相互信任的基础上开展其业务，我们将邀请世界各地的合作伙伴测试对验证地址 API 的更改。

### <a name="impacted-audience"></a>影响受众

新建客户地址详细信息或更新现有客户地址详细信息的 CSP 直接计费合作伙伴和间接提供商

### <a name="details"></a>详细信息

Microsoft 值得信赖。 我们致力于在 CSP 计划中为交易客户订阅提供合规、安全且可靠的客户地址验证方法。 从 2021 年 3 月 31 日起，我们已向验证地址 API 中引入更改。 我们邀请合作伙伴在上线之前（2021 年 6 月底）测试该 API。 

请注意，这些更改仅影响验证地址 API。 创建客户和更新计费配置文件 API 不受影响。 尽管建议的地址目前不需要与创建客户 API 结合使用，但强烈建议这样做。

响应将返回以下某个状态消息：

| 状态     | 说明 |    返回的建议地址数 |
|-------|---------------|-------------------|
|Verified shippable | 地址已经过验证且可送达。 | Single |
|已验证 | 已验证地址。 | Single |
|Interaction required | 建议的地址发生了重大更改，需要用户确认。 | Single |
|Street partial | 地址中给出的街道信息不完整，需要更多信息。 | 多个 - 最多 3 个 |
|Premises partial | 给出的场所信息（楼栋号、房号等）不完整，需要更多信息。 | 多个 - 最多 3 个 |
|多个 | 地址中有多个字段不完整（也可能包括 street partial 和 premises partial）。 | 多个 - 最多 3 个 |
|无 | 地址错误。 | 无 |
|未验证 | 无法通过验证过程发送地址。 | 无 |

美国邮政编码将返回额外 4 个数字 + 连字符，例如 12345-6789。

### <a name="next-steps"></a>后续步骤

- 有关更详细的指南，请查看[专门的合作伙伴集锦](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)中的技术文档和常见问题。
- 准备使用合作伙伴中心 API 和 Web 用户体验来整合更改。 
- 与行业专家 Ali Khaki 分享你的沙盒租户 ID，以加入外部测试，这样你便可以开始准备更新。 
- 如果正在使用控制面板供应商 (CPV) 解决方案，请咨询 CPV。

### <a name="questions"></a>是否有任何问题?

如果在 Microsoft 运营方面需要支持，请联系你的合作伙伴 Yammer 支持组或创建[服务请求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>合作伙伴中心 API Swagger 文档的新位置

### <a name="categories"></a>类别

- 日期：2021-04-26
- 功能

### <a name="summary"></a>摘要

合作伙伴中心 API Swagger 文档已从[以前的 Swagger 文档网站](https://apidocs.microsoft.com/services/partnercenter)迁移到[新 Swagger 文档网站](https://docs.microsoft.com/rest/api/partner-center-rest/)。

### <a name="impacted-audience"></a>影响受众

使用合作伙伴中心 API 且参与云解决方案提供商 (CSP) 计划的直接计费合作伙伴和间接提供商

### <a name="details"></a>详细信息

从 2021 年 4 月 26 日起，合作伙伴中心 API Swagger 文档（包括 Rest API 内容）在[新站点](https://docs.microsoft.com/rest/api/partner-center-rest/)提供。 几周后，旧站点将无法访问。

### <a name="benefits"></a>好处

合作伙伴中心 API Swagger 文档将提供“试看”功能。 使用此功能需要拥有持有者令牌，可以按照[合作伙伴中心身份验证](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)中列出的步骤生成该令牌。

### <a name="next-steps"></a>后续步骤

在组织中分享此信息，以便相应团队可查看和更新其流程。

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有疑问，请查看相关的 Yammer 社区。

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>云解决方案提供商 (CSP) 软件退货期政策和下载链接有效期通知

### <a name="categories"></a>类别

- 日期：2021-04-21
- 功能

### <a name="summary"></a>摘要

CSP 软件退货期政策和下载链接有效期发生了更改。

### <a name="impacted-audience"></a>影响受众

在 CSP 中购买永久性软件或软件订阅产品/服务的合作伙伴

### <a name="details"></a>详细信息

请注意以下关于通过合作伙伴中心购买永久性软件和软件订阅的重要通知：

#### <a name="software-return-period-policy"></a>软件退货期政策

按照 Microsoft 合作伙伴协议 (MPA) 的规定，从 2021 年 6 月 1 日起，CSP 中的软件产品/服务的退货期将从下单日期后的 60 天更改下单日期后的 30 天。

在提交软件产品/服务的订单后，合作伙伴将有 30 天的时间来提交对该订单的任何修改：

- 任何在 30 天退货期内退回的永久性软件许可证将获得已付购买价格的全额退款。

- 任何在 30 天退货期内退回的软件订购产品将获得已付购买价格的相应比例的退款。

为了跟进我们在 2020 年 12 月和 2021 年 4 月向所有 CSP 合作伙伴发出的关于退货期和其他 MPA 更新的电子邮件，我们发布了此消息。 请参考这些通知，全面详细地了解有关影响 MPA 的更改。

#### <a name="software-download-link-expiry"></a>软件下载链接有效期

从 2021 年 6 月 3 日起，通过合作伙伴中心购买的永久性软件和软件订阅产品的软件下载链接将有一个有效期，从首次下载后的 5 天内有效。 在 2021 年 6 月 3 日之前购买，以及在 2021 年 6 月 3 日当天或以后购买均可适用此有效期。

### <a name="next-steps"></a>后续步骤

查看 [CSP 退货期和下载链接有效期常见问题解答](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)，并向组织中的所有相应团队通知这些更改：

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有疑问，请查看相关的 Yammer 社区。

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>开放许可计划：将经销商转换到云解决方案提供商 (CSP) 计划

### <a name="categories"></a>类别

- 日期：2021-04-19
- 发展你的业务

### <a name="summary"></a>总结

此通知详细说明了如何准备好应对开放许可计划即将出现的变更。

### <a name="impacted-audience"></a>影响受众

CSP 和开放许可合作伙伴

### <a name="details"></a>详细信息

2020 年，Microsoft [宣布](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/)将通过云解决方案提供商 (CSP) 计划向合作伙伴和客户广泛提供永久性软件许可证。 第一个里程碑已在 2021 年 1 月达成，当时提供了商用永久性软件产品/服务。 下一个关键的里程碑将在 2021 年 7 月发生，当时将提供[公共部门](https://aka.ms/openlicensepublicsector)产品/服务。 我们还[宣布](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)自 2022 年 1 月 1 日起，不可通过开放许可计划针对软件保障或联机服务进行新的软件许可证购买或续订。

在新的商业体验中将永久性软件过渡到 CSP 计划将帮助合作伙伴拓展机遇来提供多种解决方案和托管服务。 这也将加速客户过渡到云端的速度。  为了帮助确保合作伙伴和客户顺利过渡，我们作出了这些调整和资料来加速这一数字转型：

#### <a name="april-2021"></a>2021 年 4 月

[现已推出](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)：面向经销商的“开放许可到 CSP 过渡”资料

#### <a name="july-2021"></a>2021 年 7 月

##### <a name="csp"></a>CSP

- 7 月 1 日：向公共部门客户提供永久性软件许可证

- 7 月 7 日：向所有细分领域提供 Visual Studio Pro 和 Get Genuine Windows Agreement 永久性软件许可证

##### <a name="open-value"></a>开发价值

- 7 月1 日：在开发价值计划中向教育领域和非营利领域提供额外的 SKU，从而向开放许可计划提供类似的产品/服务

##### <a name="open-license"></a>开放许可

- 7 月 1 日：Microsoft 将不再在开放许可计划中发布新的产品/服务。

#### <a name="january-2022"></a>2022 年 1 月

- 1 月 1 日：不可通过开放许可计划进行新的购买或续订

### <a name="next-steps"></a>后续步骤

#### <a name="csp-indirect-providers"></a>CSP 间接提供商

在未来几个月中，参加合作伙伴社区活动并采用面向经销商的“开放许可到 CSP 过渡”资料，帮助开放许可经销商适应 CSP 计划：

- [面向经销商的“开放许可到 CSP 过渡”资料](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/) - 可自定义的概述演示文稿、电子邮件模板、CSP 间接经销商培训指南等等，可帮助你推动经销商大规模采用。

- 由 Microsoft 业务运营部主持的 [CSP 合作伙伴社区活动](https://globalpbocomm.eventbuilder.com/GlobalCSP)。  加入各种研讨会来学习 CSP 基础（CSP 基本知识）或跟进最新动向，还可就 CSP 中的软件提问求解（问答研讨会）。

- （即将推出）Microsoft 业务运营部主持的聚焦 CSP 间接经销商的培训研讨会。

#### <a name="open-license-resellers"></a>开放许可经销商

- 如果你的组织目前未注册加入 CSP 计划，请联系分销商了解如何开始操作。 请在[此处](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)与间接提供商联系。

- 如果你的组织已注册加入 CSP 计划，请在[此处](https://partner.microsoft.com/resources/collection/software-in-csp)详细了解永久性软件。

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有进一步的问题，请访问相关的 Yammer 社区。

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>现已推出：全球促销就绪指南

### <a name="categories"></a>类别

- 日期：2021-04-16
- 功能

### <a name="summary"></a>摘要

发布准备部已针对运营就绪性资源库发布了新的[全球促销就绪指南](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)。 本指南综合显示了所有现行[全球促销](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)。

### <a name="impacted-audience"></a>影响受众

所有批量许可 (VL)、动态价目表 (DPL) 和云解决方案提供商 (CSP) 合作伙伴

### <a name="details"></a>详细信息

Microsoft 合作伙伴和我们有同一个需求，那就是提供各项全球促销的综合视图并附上辅助详细信息。 你希望此综合指南可帮助你运用促销，确信所有可用信息都将在一个集中便利的位置随时可供访问。

从 2021 年 4 月开始，Microsoft 将每月更新一次本指南，它将在运营就绪性资源库中的专用“全球促销就绪指南”集合中提供。

本指南的链接还将包含在下列集合中：

- [发布日历集合](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)，它将集中显示即将发生的变更和发布。

- [社区集合](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)它包含我们每月合作伙伴通话的辅助资料，重点突出即将发生的变更和及时的热门运营主题。

- [合作伙伴新闻稿](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)，例如 CSP 每月更新

在每月提醒中，我们还将发布合作伙伴中心公告，其中包含全球促销就绪指南的每项新问题。

### <a name="next-steps"></a>后续步骤

在每月初，你将在[运营就绪性资源库](https://partner.microsoft.com/resources)中找到最新的[全球促销就绪指南](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)。

请与组织中适当的联系人分享此信息，并通过每页底部的“此页面有帮助吗？”按钮告诉我们指南 在多大程度上有所帮助。

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>4 月云解决方案提供商 (CSP) 社区更新和提醒

### <a name="categories"></a>类别

- 日期：2021-04-16
- 社区 | 邀请和提醒

### <a name="summary"></a>总结

CSP 社区资源按需提供且每月更新，便于你保持知情且准备好应对 CSP 计划中的变更。

### <a name="impacted-audience"></a>影响受众

CSP 直接计费合作伙伴和间接提供商

### <a name="details"></a>详细信息

在本月，资源将纳入下列重要主题：

- [关于 CSP 计划演进和开放许可计划变更的新信息](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [对某些区域的 CSP 客户加入要求的变更](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [对 CSP 计划中新的商务 PDF 发票使用新格式](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

在 [CSP 社区集合](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)中，你将找到：

- 可下载的 [CSP 每月更新新闻稿](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)，它在易于阅读的文档中汇总了最新的 CSP 公告、更新、活动和提醒。

- [CSP 公告日历](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)，它就即将发生的会影响计划的变更提供时间线视图。

- 新的[产品发布日历](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)，你可在此查看即将进行的产品发布和套餐。

- [CSP 发布更新资源](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/)，它包含关于关键运营变更的易用内容。

- [新资讯和提醒](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf)，介绍人们感兴趣和询问的关键 CSP 主题。

#### <a name="csp-community-call-qas"></a>CSP 社区通话问答

提供了社区通话问答来帮助你解答有关即将发生的变更的问题。 请立即注册参加 4 月、5 月和 6 月举行的 CSP 社区通话问答活动。 这些活动将聚焦于最新的发布、重要新资讯和提醒。

[在此处注册](https://globalpbocomm.eventbuilder.com/GlobalCSP)。

### <a name="next-steps"></a>后续步骤

查看社区资源并注册参加社区通话问答活动。

为了确保你从社区通话问答活动中获得最大收益，请查看按需社区内容，并在通话前 48 小时内提交你的问题。

### <a name="questions"></a>是否有任何问题?

如有关于 CSP 计划变更的问题，最适合提问的地方就是每月的 CSP 社区通话问答活动。 在每月，请查看资料并提前提交问题，以便我们可在研讨会上聚焦对你来说最重要的主题。

有关详细信息，请联系[支持人员](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)。

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>最后提醒：于 2021 年 5 月 6 日弃用 GET 资格

### <a name="categories"></a>类别

- 日期：2021-05-04

- 功能

### <a name="impacted-audience"></a>影响受众

使用合作伙伴中心 API，通过云解决方案提供商计划销售学术、非盈利和政府社区云 (GCC) 产品/服务的合作伙伴

### <a name="details"></a>详细信息

本公告是对 [12 月发布的合作伙伴中心增强功能](https://docs.microsoft.com/partner-center/announcements/2020-december#1)的跟进。 此版本部署了新的 GET 和 POST 资格 API，因此现有 GET 资格将于 2021 年 5 月 6 日停用。 届时，你需要已经过渡到使用新的 POST 合作伙伴中心 API。 可使用新的 POST API 购买教育版产品/服务，同时将可使用新的 GET API 购买预获资格的非营利组织’和 GCC 产品/服务。

### <a name="next-steps"></a>后续步骤

- 请更新到新的 API，以便及时成功转换。

- 请访问运营准备资源 - [合作伙伴中心教育客户验证过程增强](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)，查看新的合作伙伴中心 API 更改和指南。

- 请与经销商和组织中的相应团队分享此信息，帮助他们为这些更改做好准备。

### <a name="questions"></a>是否有任何问题?

若有与此通知相关的任何问题，请联系[合作伙伴中心支持部门](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)。

### <a name="change-log"></a>更改日志

- 2021 年 4 月 4 日：最后提醒即将弃用 GET 资格

- 2021 年 4 月 9 日：提醒即将弃用 GET 资格 

- 二月：更新了停用 GET 和 PUT 资格的时间线

- 一月：提醒即将开始弃用 GET 和 PUT 资格

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>对 CSP 中新的商务 PDF 发票使用新格式

### <a name="categories"></a>类别

- 日期：2021-04-05
- 功能

### <a name="summary"></a>摘要

Microsoft 在云解决方案提供商 (CSP) 计划中为新的商务 PDF 发票引入一种新格式，以按产品详细信息而不是按 SKU 说明显示账单详细信息。

### <a name="impacted-audience"></a>影响受众

通过 CSP 计划进行交易的合作伙伴

### <a name="details"></a>详细信息

Microsoft 将从 2021 年 5 月起在 CSP 计划中为新的商务 PDF 发票引入一种新格式，即按产品详细信息（而不是 SKU 说明）显示账单详细信息。 通过此更新，我们将按产品类型聚合行项，同时在单独的行上显示每个产品。

合作伙伴请注意，此更改将在 5 月的发票中（计费周期为 2021 年 4 月 1 日到 2021 年 4 月 30 日）开始生效。 受影响的产品/服务包括 Microsoft Azure 预留实例、Azure 订阅（Azure 计划）和市场。

发票格式更新后提出的任何额度重计请求都会采用新格式。

#### <a name="partner-benefits"></a>合作伙伴权益

此更新在合作伙伴开票体验方面提供以下改进：

- 减小了发票大小，同时保留了关键数据

- 使格式与行业标准保持一致，以生成精简且便于用户使用的发票 

以下元素不会受到影响：

- 发票 PDF 中的“账单摘要”页

- 现有开票 API

- 对帐文件（对帐文件可用于检索精细数据。） 

- 基于使用量和许可证的费用发票

### <a name="next-steps"></a>后续步骤

在 Microsoft 合作伙伴网站上的[运营准备资源库](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)中查看有关此主题的信息。 有关计费和税务主题（包括计费资源、发票、CSP 计费和税务）的详细信息，请访问合作伙伴中心的[计费部分](https://docs.microsoft.com/partner-center/billing)。

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>对云解决方案提供商 (CSP) 客户加入要求的更改

### <a name="categories"></a>Categories

- 日期：2021-04-02
- 产品/市场

### <a name="summary"></a>摘要

我们承诺帮助合作伙伴和客户在相互信任的基础上开展其业务，在此过程中，我们将请求其他客户信息，从 2021 年 3 月 25 日生效。

### <a name="impacted-audience"></a>影响受众

CSP 商直接计费合作伙伴和间接提供商，他们在下一节中列出的国家/地区具有新客户或现有客户

### <a name="details"></a>详细信息

Microsoft 值得信赖。 我们致力于在 CSP 计划中为交易客户订阅提供合规、安全且可靠的客户验证方法。 在 2021 年 5 月 25 日，我们将引入合作伙伴中心 API 和用户界面 (UI) 增强功能，它们将影响同时满足以下两个条件的合作伙伴：

- 合作伙伴与 Microsoft 有直接计费关系（这意味着合作伙伴是直接计费合作伙伴或间接提供商）。

- 合作伙伴与以下国家/地区的新客户或现有客户开展业务：

    - 泰国
    - 越南
    - 土耳其
    - 波兰
    - 南非
    - 印度
    - 巴西
    - 伊拉克
    - 缅甸
    - 南苏丹
    - 沙特阿拉伯
    - 阿拉伯联合酋长国
    - 委内瑞拉

满足条件的合作伙伴必须在其下一次更新或为客户创建订阅时提交该客户的公司注册 ID（也称为客户的组织 INN）和电话号码。 这些合作伙伴还可以为客户输入可选的中间名。

请注意，在添加公司注册 ID 时，应使用企业纳税人标识号，而不是客户的个人 ID。

与以下国家/地区的新客户和现有客户合作的合作伙伴已加入 2020 年 11 月的以前版本中。

- 亚美尼亚
- 阿塞拜疆
- 白俄罗斯
- 匈牙利
- 哈萨克斯坦
- 吉尔吉斯斯坦
- 摩尔多瓦
- 俄罗斯
- 塔吉克斯坦
- 乌克兰
- 乌兹别克斯坦

与世界上其他国家/地区的客户合作的合作伙伴可以在 2021 年 3 月底输入客户的公司注册 ID、电话号码和中间名（可选）详细信息。

### <a name="next-steps"></a>后续步骤

- 有关更详细的指南，请查看专门的[合作伙伴集锦](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)中的技术文档和常见问题。
- 准备使用合作伙伴中心 API 和 Web 用户体验来整合更改。 API/SDK 将可用于测试。
- 请确保在加入新客户或修改现有客户详细信息时提交其他数据。
- 如果正在使用控制面板供应商 (CPV) 解决方案，请咨询 CPV。

### <a name="questions"></a>是否有任何问题?

如果你有任何与公司注册 ID（也称为 INN 或 TIN）相关的问题，请与你的税务顾问或当地税务局联系。 Microsoft 无法提供有关税务事宜的指导。

如果需要 Microsoft 运营方面的支持，请创建[服务请求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>查看本月的产品发布以及产品/服务

### <a name="categories"></a>类别

- 日期：2021-04-01
- 功能
 
### <a name="summary"></a>摘要

2021 年 4 月的产品发布日历现已发布。

### <a name="impacted-audience"></a>影响受众

参与云解决方案提供商 (CSP) 计划的所有合作伙伴

### <a name="details"></a>详细信息

现已在运营准备资源库中提供 2021 年 4 月的[产品发布日历](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)。 在此处查看即将进行的产品发布和将推出的产品/服务。

### <a name="next-steps"></a>后续步骤

请查看[产品发布日历](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)，与组织中的相应利益干系人分享此信息。  

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有任何进一步的问题，请访问相关的 Yammer 社区。
