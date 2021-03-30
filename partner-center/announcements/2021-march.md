---
title: 2021 年 3 月公告
description: Microsoft 合作伙伴中心 2021 年 3 月公告，包括新功能、促销、产品/服务、市场或对现有产品/服务的更改。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 03/22/2021
ms.openlocfilehash: a3172b78d41a966b52a824703a7f15f163467d63
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880729"
---
# <a name="march-2021-announcements"></a>2021 年 3 月公告

本页提供了 Microsoft 合作伙伴中心 2021 年 3 月公告。

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>更正了 2021 年 3 月 1 日永久性软件价目表

### <a name="categories"></a>类别

- 日期：2021-03-23
- 产品/市场

### <a name="impacted-audience"></a>影响受众

交易永久性软件的间接提供商和直接帐单合作伙伴在云解决方案提供商计划中 

### <a name="details"></a>详细信息

2021 年 3 月 1 日发布的永久性软件的价目表包含了不应包含的市场。 已于 2021 年 3 月 17 日更正永久性软件价目表。 这些更正仅适用于：

- 产品 ID：DF77X4D43RKT 
- 产品名称：Microsoft 365 商业版的 Windows 10 家庭版到专业版升级
- 已删除或不受支持的市场：AE、AF、AL、AM、AO、BA、BB、BD、BH、BM、BN、BO、BR、BS、BW、BY、BZ、CI、CL、CM、CO、CR、CW、DO、DZ、EC、EG、ET、FJ、FO、GE、GH、GT、HN、IL、IN、IQ、JM、JO、KE、KG、KN、KW、KY、KZ、LB、LK、LY、MA、MC、MD、ME、MN、MO、MU、NA、NG、NI、NP、OM、PA、PE、PH、PK、PR、PY、QA、RS、RU、RW、SG、SN、SV、TH、TJ、TM、TN、TT、TZ、UA、UG、UY、UZ、VE、VN、YE、ZM、ZW

这些更改仅适用于上述产品。 其他产品没有更正。 

### <a name="next-steps-and-resources"></a>后续步骤和资源

- 交易永久性软件的合作伙伴应下载最新的永久性软件价目表。
- 请参阅[国家/地区代码](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)，了解两个字母的缩写到国家/地区的易懂对应关系。
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13">.NET Standard 上的 SDK 版本 (v1.17.0)</a>

### <a name="categories"></a>类别

- 日期：2021-03-23

- 功能
 
### <a name="impacted-audience"></a>影响受众

使用合作伙伴中心 .NET SDK 且参与 CSP 计划的直接计费合作伙伴和间接提供商。

### <a name="details"></a>详细信息

从 2021 年 3 月 23 日开始，合作伙伴便可下载最新版 [MicrosoftPartnerCenter.NETSDK（NuGet 库 | Microsoft.Store.PartnerCenter 1.17.0）](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)，还可下载更新的公共合作伙伴中心 SDK [GitHub 示例](https://github.com/Microsoft/Partner-Center-DotNet-Samples)。 此版本包括以下方法更新：

#### <a name="audit-updated-new-operation-types"></a>审核已更新：新操作类型

添加了新的[操作类型](https://docs.microsoft.com/partner-center/develop/auditing-resources)，以了解客户批准和终止 DAP 的时间。

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>审核已更新：新资源和操作类型

添加了新的[资源和操作类型](https://docs.microsoft.com/partner-center/develop/auditing-resources)以支持客户目录角色方案。

- 新资源类型“CustomerDirectoryRole”

- 操作类型“AddUserMember”和“RemoveUserMember”

#### <a name="sdk-updates-to-customer-accounts"></a>对客户帐户的 SDK 更新

- 对 GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus 的支持

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>其他更改

以下更改将作为“新商业”的一部分引入，当前仅适用于已加入 M365/D365 新商业体验技术预览版的合作伙伴。 未参与新商业技术预览版的合作伙伴应该不会注意到影响，并且应向后兼容。

- 目录更改：

  - GET /products/{product-id}/skus/{sku-id}

- 购买和管理：
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>后续步骤

- 下载最新版 [MicrosoftPartnerCenter.NETSDK（NuGet 库 | Microsoft.Store.PartnerCenter 1.17.0）](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- 下载并查看 [GitHub 示例](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP 商业市场产品/服务以及 2021 财年 CSP 奖励措施（针对符合条件的产品/服务）

### <a name="categories"></a>类别

- 日期：2021-03-18
- 功能

### <a name="impacted-audience"></a>影响受众

云解决方案提供商计划中的间接提供商和直接计费合作伙伴 

### <a name="details"></a>详细信息

云解决方案提供商计划中的间接提供商和直接帐单合作伙伴可以销售第三方产品/服务，并就合作伙伴中心或 Azure 门户中每个符合条件的第三方产品/服务获得退款奖励。 激励采取为符合资格的产品/服务的已计费销售进行退款的形式，有效期持续到 2021 年 6 月 30 日。  

在下方继续了解此云解决方案提供商商业市场产品/服务激励，并立即与客户联系，确定适当的产品/服务以便让他们能够实现持续成功和数字转换。

我们与独立软件供应商合作 (ISV) 合作，将最新的 IaaS 和 SaaS 解决方案推向市场以便 Microsoft 客户使用。 ISV 发布者可以选择允许通过 Microsoft 合作伙伴渠道销售其产品/服务。 有资格获得激励的产品/服务分为两类：

- 具有 Azure IP 共同销售激励状态的 SaaS 和 IaaS 第三方产品/服务。 

- 与 Teams 或至少两款 Microsoft 365 生产力应用程序（如 PowerPoint、Word、Excel、Outlook 或 SharePoint）集成的 SaaS 应用程序。

### <a name="next-steps-and-resources"></a>后续步骤和资源

- 了解如何通过销售符合资格的市场应用（有资格获得激励的应用）获得[合作伙伴奖励](https://partner.microsoft.com/membership/partner-incentives)。 每个月都会添加新产品/服务。  
- [云解决方案提供商直接计费合作伙伴激励资源](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [云解决方案提供商间接提供商激励资源](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- 查看此[演示文稿](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)，了解有关销售商业市场应用的详细信息。 可在[此处](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)查看更多资源。 
- 可在[合作伙伴中心](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover)或 [Azure 门户](https://ms.portal.azure.com/#home)中浏览商业市场目录
- 使用 [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) 将应用集成到公司的市场
- 与你想要与之开展业务的 ISV 联系
- 间接提供商需要使用 API 集成，并指导经销商应销售哪些应用

### <a name="questions"></a>是否有任何问题?  

请参阅[这篇文章](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)，了解合作伙伴中心商业市场的概述。

如需获得更多帮助，可以在合作伙伴中心创建支持请求。 更多信息请访问 [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1)。

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium 产品/服务命名和先决条件更新

### <a name="categories"></a>类别

- 日期：2021-03-18
- 功能

### <a name="summary"></a>摘要

2021 年 4 月 1 日的最终价目表将更新以明确 Power BI Premium Per User 产品/服务的命名和/或先决条件信息。

### <a name="impacted-audience"></a>影响受众

云解决方案提供商 (CSP) 直接和间接合作伙伴

### <a name="details"></a>详细信息

2021 年 4 月 1 日的最终价目表将更新以明确 Power BI Premium Per User 产品/服务的命名和/或先决条件信息。

在更新最终价目表之前，请使用此部分中的信息来确保订购适当的产品。

以下详细信息显示受影响的 SKU 和先决条件的详细信息。

| 3 月 1 日价目表预览中的的产品/服务显示名称 |  4 月 1 日最终价目表上更新的产品/服务显示名称| 产品/服务 ID |
| ------ | ----------- | ----------- |
| Power BI Premium Per User 加载项（非营利组织员工定价）  |  Power BI Premium Per User 加载项 (Office)（非营利组织员工定价）   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

客户需要满足以下任一先决条件才能购买此产品/服务：

| 产品/服务显示名称 | 产品/服务 ID |
| ------ | ----------- |
| Microsoft 365 E5（非营利组织员工定价）  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   不带音频会议的 Microsoft 365 E5（非营利组织员工定价）|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5（非营利组织员工定价）| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5（非营利组织员工定价）试用版|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   不带音频会议的 Office 365 E5（非营利组织员工定价）|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

需要满足先决条件才能购买以下 Power BI Premium 产品/服务：

| 产品/服务显示名称 | 产品/服务 ID |
| ------ | ----------- |
|   Power BI Premium Per User 加载项（非营利组织员工定价）|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

客户需要具有此先决条件才能购买此产品/服务：

| 产品/服务显示名称 | 产品/服务 ID |
| ------ |----------|
| Power BI Pro（非营利组织员工定价）  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>后续步骤

查看有关本主题的资源，并与组织内部的相关利益干系人共享此信息。  

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有任何疑问，请查看相关的 Yammer 社区。 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a>Microsoft 365 F3 的 3 月价格更新

### <a name="categories"></a>类别

- 日期：2021-03-16
- 产品/市场

### <a name="summary"></a>摘要

已更正 2021 年 3 月定价，以反映正确的 Microsoft 365 F3 英镑 (GBP) 和欧元 (EUR) 价格。

### <a name="impacted-audience"></a>影响受众

在 2021 年 3 月 1 日到 3月 17 日之间通过云解决方案提供商 (CSP) 程序以英镑或欧元购买 Microsoft 365 F3 的合作伙伴。

### <a name="details"></a>详细信息

Microsoft 已更正 Microsoft 365 F3 的错误定价。 只有英镑和欧元的价格不正确，并且只有 2021 年 3 月 1 日到 3 月 17 日之间购买的产品/服务受到影响。 下方列出了受影响的产品/服务和货币。 

| 产品名称 | 货币 | 产品/服务 ID | 材料 ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3（慈善） | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3（商业） | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
太平洋标准时间 3 月 16 日下午 5 点更新了 3 月和 4 月预览版基于许可证的价目表。

### <a name="next-steps"></a>后续步骤

- 合作伙伴应将重新下载当前基于许可证的价目表（3 月和 4 月预览版），其中包含相应的这些价格更正。  
- Microsoft 将在未来几周内通过电子邮件联系受影响的合作伙伴，告知他们与更正受影响的交易相关的后续步骤。

### <a name="questions"></a>是否有任何问题?

如果有任何进一步的问题，请访问相关的 CSP Yammer 社区。

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a>通过合作伙伴中心更新法定公司名称

### <a name="categories"></a>类别

- 日期：2021-03-16
- 促使提高效率和规模

### <a name="summary"></a>总结

从 2021 年 3 月起，Microsoft 合作伙伴网络 (MPN) 合作伙伴和云解决方案提供商 (CSP) 间接经销商可通过合作伙伴中心更新其法定公司名称。

### <a name="impacted-audience"></a>影响受众

MPN 合作伙伴和 CSP 间接经销商（不适用于 CSP 直接计费合作伙伴）

### <a name="details"></a>详细信息

从 2021 年 3 月起，MPN 合作伙伴和 CSP 间接经销商可在合作伙伴中心通过兼容的自助服务方式更新其法定公司名称。 借助这项新功能，合作伙伴将无需再提交合作伙伴中心支持票证来更新其公司名称。 这样可以在合作伙伴执行这些活动时节省大量时间。 

若要了解详细信息，请参阅[更新法定公司资料](../update-your-partner-profile.md#update-your-legal-business-profile)。

>[!NOTE]
>请确保法定公司资料中的公司名称没有拼写错误和缩写，并且与正式的公司商业注册记录完全一致。 若要详细了解如何更新组织资料，请查看[验证组织资料](../update-your-partner-profile.md#update-your-legal-business-profile)。

### <a name="next-steps"></a>后续步骤

在组织中分享此信息，以便相应团队可查看和更新其流程。

### <a name="questions"></a>是否有任何问题?

如果有任何进一步的问题，请访问相关的 CSP Yammer 社区。

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a>云解决方案提供商 (CSP) 计划演进和开放式许可计划变更更新

### <a name="categories"></a>类别

- 日期：2021-03-15
- 功能

### <a name="summary"></a>摘要

除了开放式许可计划出现变更，云解决方案提供商 (CSP) 也将增添新的商业和公共领域永久性软件产品。

### <a name="impacted-audience"></a>影响受众

通过开放式许可计划销售的商业分销商和托管经销商，以及交易永久性软件的所有 CSP 合作伙伴

### <a name="details"></a>详细信息

在 2020 年 9 月，Microsoft 就其数字转型之旅[宣布了](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)一系列的措施，目的是将机会扩大给已加入 CSP 计划的合作伙伴，这些机会包括合作伙伴本地软件的可用性。 借助这些变更，合作伙伴可利用 CSP 中的软件许可证发展自身业务并扩大触达范围，在如今以云为先的世界里摆正自己的定位来争取成功。 它们还帮助客户过渡到云中，并为合作伙伴提供客户混合云环境所需的灵活性。

在这次数字转型的延续中，我们宣布进行以下变更：

- 2021 年 7 月 1 日：不向开放式许可计划价目表添加任何新的 SKU、产品或促销。

- 2021 年 7 月 7 日：将向 CSP 永久性软件价目表添加两款商业产品/服务（Get Genuine Windows 和 Visual Studio Professional）和公共领域产品/服务（政府、教育和非营利性组织 - 具体查看[公告](./2020-december.md#9)）。  可在合作伙伴中心的[“销售”>“定价与产品”](https://partnercenter.microsoft.com/pcv/sales)的“软件”部分找到价目表，且该表格将在该日期重新发布。

有关 CSP 计划演进和开放式许可计划变更的完整详细信息，请查看下面的后续步骤。

### <a name="next-steps"></a>后续步骤：

- CSP 计划演进：请查看[云解决方案提供商计划中的永久性软件](https://partner.microsoft.com/resources/collection/software-in-csp#/)就绪性资料。 请使用此[就绪性地图](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)快速找到适合你的角色的信息。

- 开放式许可计划变更：请查看 [CSP 计划演进和开放式许可计划变更](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)就绪性资料。 请使用此[就绪性地图](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)快速找到适合你的角色的信息。

### <a name="questions"></a>问题

如果有任何进一步的问题，请访问相关的 CSP Yammer 社区。

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>对上一公告的更新：高级评估，合规性管理器加载项

### <a name="categories"></a>类别

- 日期：2021-03-15
- 拓展业务

### <a name="summary"></a>总结

不得在价目表中列出试用版产品/服务，这些内容将被删除。

### <a name="impacted-audience"></a>影响受众

通过云解决方案提供商交易的合作伙伴

### <a name="details"></a>详细信息

价目表中不得包含试用版产品/服务。 这些内容将从 2021 年 5 月 1 日的价目表中删除。

如需最初公告，请查看[此处](./2021-february.md#4)。

### <a name="additional-resources"></a>其他资源

- [Microsoft 365 E5 安全性和合规性](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [在 Microsoft 合规性管理器中生成和管理评估 - Microsoft 365 合规性](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>后续步骤

查看有关本主题的资源，并与组织内部的相关利益干系人共享此信息。

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有疑问，请查看相关的 Yammer 社区。

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a>将解决方案从 One Commercial Partner (OCP) 进入市场 (GTM) 迁移到 Microsoft 商业市场

### <a name="categories"></a>类别

- 日期：2021-03-12
- 功能

### <a name="summary"></a>摘要

从 2021 年 3 月 29 日开始，你将开始体验功能受限的 One Commercial Partner (OCP) 进入市场 (GTM) 功能。 建议你将解决方案迁移到合作伙伴中心的商业市场。

### <a name="impacted-audience"></a>影响受众

在 OCP GTM 中联合销售解决方案的组织

### <a name="details"></a>详细信息

在 2020 年 12 月，我们开始了从 Microsoft OCP GTM 工具迁移到合作伙伴中心的 Microsoft 商业市场的旅程。 这次过渡扩展了商业市场的能力，你可在这里向数百万名客户展示你的解决方案、与其他 Microsoft 和合作伙伴卖方相互分享销售机会，并联手销售创新的解决方案。

本次过渡的下一里程碑举措将在 2021 年 3 月 29 日实施。 届时，你将开始体验功能受限的 OCP GTM 功能，其中某些方面变为只供查看。 如果你当前正在 OCP GTM 中联合销售解决方案，建议你将解决方案迁移到商业市场来利用该市场中的功能并简化你的发布体验。 

移到商业市场后，合作伙伴中心就成为了获取联合销售发布体验的主要位置。 在这里，你可通过与我们对 Microsoft 产品使用的一样的通道和产品内体验将你的解决方案推广给我们共同的客户，从而继续发展你的业务。 [详细了解商业市场](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)。

### <a name="next-steps"></a>后续步骤

- 如果你尚未移动解决方案，请按照[过渡指南](/azure/marketplace/co-sell-solution-migration)中详述的说明或查看[视频分步教程](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)，来完成各项迁移活动并开始在商业市场发布你的解决方案。

- 如果对 OCP GTM 中的受限功能体验存有疑问，请查看[在 Microsoft 商业市场中发布内容的联合销售要求常见问题解答](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)。 （请查看“从 2021 年 3 月 29 日起推出 OCP GTM 受限功能”部分。）

### <a name="questions"></a>是否有任何问题?

如有任何疑问或需要更多信息，请联系[支持人员](https://partner.microsoft.com/support/?stage=1) 。

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>将 Azure 的云解决方案提供商 (CSP) 计划中新推出的商业体验扩展到俄罗斯

### <a name="categories"></a>类别

- 日期：2021-03-10
- 功能

### <a name="impacted-audience"></a>影响受众

参与云解决方案提供商 (CSP) 计划的所有俄罗斯的合作伙伴。

### <a name="details"></a>详细信息

我们很高兴宣布，从 2021 年 3 月 10 日起在俄罗斯的 CSP for Azure 中推出新的商业体验。 此体验将简化和改进客户购买及使用 Azure 服务的方式。 通过它，已加入 CSP 计划的合作伙伴可查看各销售活动中 Azure 定价的一致视图、获取美元定价（它可确保全球价格一致）、确保计费日期一致并访问 Azure 成本管理功能。

### <a name="next-steps"></a>后续步骤

提供了有多项资源，它们引入了新的 Azure 商业体验并提供其他信息。 有关最新的常见问题解答、宣传资料和视频等内容，可查看 [CSP 计划更新资源库](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).。

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>合作伙伴中心软件许可证密钥和下载履行

### <a name="categories"></a>类别

- 日期：2021-03-04
- 功能

### <a name="summary"></a>摘要

现已恢复合作伙伴中心软件下载和许可证密钥履行功能。

### <a name="impacted-audience"></a>影响受众

通过合作伙伴中心处理永久性和服务器订阅软件订单的所有云解决方案提供商 (CSP) 合作伙伴

### <a name="details"></a>详细信息

为了回应合作伙伴反馈，我们将恢复合作伙伴中心履行功能，你可为永久性和服务器订阅软件订单获取软件和许可证密钥。 此功能会还原到其之前的状态，然后在 2021 年 1 月 19 日被移除。 （请查看[公告](2020-september.md#17)。）

请注意，软件许可证密钥和下载链接是宝贵且受到热烈追捧的知识产权资产。 如果遭到泄露，其激活限制可能很快就被会耗尽，导致出现负面的客户和合作伙伴体验。

### <a name="next-steps"></a>后续步骤

请查看下列资源，了解有关软件密钥分发的使用说明和重要指导：

- [通过 CSP 计划出售本地软件](../csp-on-premise-software.md)
- [合作伙伴中心新版商业操作指南](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)（请查看“软件密钥分发指导”部分。）

### <a name="questions"></a>是否有任何问题?

如果对此通知还有其他疑问，请访问相关的 Yammer 社区。

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>将交易从 Partner Sales Connect (PSC) 迁移到合作伙伴中心

### <a name="categories"></a>类别

- 日期：2021-03-04
- 功能

### <a name="summary"></a>摘要

自 2021 年 3 月 31 日起，将只能以只读方式访问 Partner Sales Connect (PSC)，因此请开始将你在 PSC 中的交易迁移到合作伙伴中心。

### <a name="impacted-audience"></a>影响受众

在 PSC 中具有交易的合作伙伴

### <a name="details"></a>详细信息

作为我们共同的发展承诺的一部分，与 Microsoft 联合销售让你能够被发现、表现你的专业知识并扩大客户群体来获得积极的客户成果 。 在合作伙伴中心管理你的联合销售体验将使平均交易时间比平时快 3.5 倍，让你能够跨直接客户、合作伙伴和 Microsoft 卖家渠道进行销售，并在一个位置管理你的整个推荐管道。

自 2021 年 3 月 31 日起，将只能以只读方式访问 PSC，因此请开始迁移到合作伙伴中心，获取下列功能改进  ： 

- 根据你需要的协助类型，更准确地将你与 Microsoft 共享的交易引导给适当的卖家。
- 对符合激励计划的解决方案的前期交易资格验证，目的是满足 ISV Connect 计划标准，从而简化审批过程和最终的执行证明 (POE)。
- 无缝的用户体验，可在一个位置管理你的联合销售机会和销售合格潜在客户。

我们最近还在合作伙伴中心增添了新的功能来帮助你进行迁移：

- [针对联合销售机会的批量操作](../bulk-operations.md)
- [交易迁移功能](../psc-to-pc.md)（请查看“PSC 交易迁移”部分。）

借助合作伙伴中心的联合销售体验，你的销售团队将有更多时间专注于培养潜在客户、创造机会、达成交易和建立持久的客户关系。

### <a name="next-steps"></a>后续步骤

使用合作伙伴中心[过渡指南](../psc-to-pc.md)引导自己完成将交易从 PSC 迁移到合作伙伴中心的步骤。

### <a name="questions"></a>是否有任何问题?

如果还有其他疑问，请联系[支持部门](https://partner.microsoft.com/support/?stage=1)。

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>将于 2021 年 4 月 1 日推出的新增 Microsoft Dynamics 365 产品和服务

### <a name="categories"></a>类别

- 日期：2021-03-04
- 功能

### <a name="summary"></a>摘要

在 2021 年 4 月 1 日，Microsoft 将对云解决方案提供商 (CSP) 计划推出几项新的产品和服务。

### <a name="impacted-audience"></a>影响受众

参与云解决方案提供商 (CSP) 计划的所有合作伙伴

### <a name="details"></a>详细信息

在 2021 年 4 月 1 日，Microsoft 将推出下列新产品和服务：

- Power BI Premium Per User
- Customer Voice 和 Marketing USL 地域和细分市场拓展

**Power BI Premium Per User**

Microsoft 将引入首批 Power BI Premium 每用户产品/服务。 目前仅在容量构造中出售 Power BI Premium。 通过 Power BI Premium Per User，可访问企业商业智能 (BI) 和分析功能。 其灵活的个人席位许可很适合中小型企业。

若要详细了解此产品/服务，请查看 [Power BI 发布详细信息](/power-platform-release-plan/2020wave2/power-bi/planned-features)。


**产品/服务详细信息**

请注意，产品/服务名称与价目表预览中的略有不同。

| 产品名称 | 产品/服务 ID |
| ------ |----------- |
| Power BI Premium Per User | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Per User 教职员工版 | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Per User 学生版 | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Per User（非营利组织员工定价） | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Per User 加载项 | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Per User 加载项教职员工版 | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Per User 加载项学生版 | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Per User 加载项（非营利组织员工定价） | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Customer Voice 和 Marketing USL 地域和细分市场拓展**

作为 2020 年 12 月发布的后续，Dynamics 365 Customer Voice 和 Marketing USL 产品/服务进行了更改，现增添新的国家/地区和更多非营利及教育 SKU。

| 产品名称 | 产品/服务 ID |
| ------ |----------- |
| Dynamics 365 Customer Voice USL（非营利组织员工定价） | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL 教职员工版 | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

请访问以下页面，详细了解这些产品/服务：

- [Dynamics 365 Customer Service Voice 主页](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 Marketing 主页](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>后续步骤

请查看此主题的相关资源，与组织中的适当利益干系人分享此信息。  

### <a name="questions"></a>是否有任何问题?

如果对这些产品/服务有任何疑问，请查看相关的 Yammer 社区。 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a>现已在部分套件中提供 Microsoft 通用打印服务

### <a name="categories"></a>类别

- 日期：2021-03-33
- 功能

### <a name="summary"></a>摘要

从 2021 年 3 月 1 日起，可在特选 Microsoft 365 套件中或以独立加载项的形式办理 Microsoft 通用打印服务。

### <a name="impacted-audience"></a>影响受众

参与云解决方案提供商 (CSP) 计划的所有合作伙伴

### <a name="details"></a>详细信息

[通用打印](https://aka.ms/universalprint)是一项 Microsoft 365 打印服务，它让你不再需要本地打印服务器，还使 Windows 设备能够打印到注册了 Azure 的打印机。 自 2021 年 3 月 1 日起可办理此功能。

免用驱动程序的打印、基于位置轻松发现打印机，以及无需累积学习的直观打印体验，这些都使员工受益匪浅。 已加入 Azure Active Directory (Azure AD) 的设备使用现有的 Azure AD 凭据安全地进行打印。 管理员通过 Azure 门户管理打印，并可借助对通用打印的本机支持轻松连接打印机。 可使用通用打印连接器软件在不简单的打印机上部署通用打印服务。

在通用打印发布时，Windows E3、A3、E5 和 A5 以及 Microsoft 365 BP、F3、E3、A3、E5 和 A5 上将恢复该项服务。  

**产品/服务详细信息**

请注意，产品/服务名称与价目表预览中的略有不同。

| 产品名称 | 产品/服务 ID | 材料 ID |
| ------ |----------- |----------- |  
| 通用打印卷加载项（500 个作业）- Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| 通用打印卷加载项（500 个作业）教职员工版 - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| 通用打印卷加载项（500 个作业）- Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| 通用打印卷加载项（500 个作业）教职员工版 - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>后续步骤

熟悉价目表和[通用打印概述](/universal-print/fundamentals/universal-print-whatis)。 请与贵组织中的相应联系人共享这些信息。

### <a name="questions"></a>有疑问？

如果对这些产品/服务有任何疑问，请查看相关的 Yammer 社区。
