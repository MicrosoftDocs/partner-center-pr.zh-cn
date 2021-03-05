---
title: 验证公司配置文件
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何验证公司详细信息，例如主要联系人、地址和计划信息。 还可以更新法律和帐单地址。
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 03/03/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q3
ms.openlocfilehash: 2527e57ea0c95c5d91728dd6198490365b264c6f
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124765"
---
# <a name="verify-your-company-profile-information-in-partner-center"></a>在合作伙伴中心验证公司配置文件信息

**相应的角色**

- 全局管理员
- MPN 帐户管理员

在首次以全局管理员身份登录到合作伙伴中心时，应确认你所有的公司详细信息是否正确。 包括主要联系人、法定公司名称和地址，以及计划信息。 如果公司有多个位置，请查看位置数据以确保其准确性。 作为全局管理员、帐务管理员或管理员代理，你也可以查看并更新帐务和税务信息。

合作伙伴配置文件包含法定公司信息、主要联系人名称和电子邮件、公司参与的计划，以及现在合并到法定公司名下的其他公司（如果适用）。 请确保法人资料中的公司名称和地址没有拼写错误和缩写，并且与正式的公司商业注册记录完全一致。 如果以个体经营者的身份运营，则需要将公司名称用作法人名称。



## <a name="locate-the-legal-business-profile"></a>找到公司法定资料

1. 转到“设置”图标，然后选择“帐户设置” 。
 
1. 选择“组织资料”。 

2. 查看“法定公司配置文件”、“主要联系人信息”和“计划信息”。

如果已将其他公司合并到法定公司名下，则也可查看其信息。 

## <a name="update-your-legal-business-profile"></a>更新法定公司配置文件

在合作伙伴中心更新法定地址。

>[!Important]
>- 对于 MPN 帐户，全局管理员和帐户管理员都可以更新公司法定名称。
>- 对于 CSP 间接经销商帐户，只有全局管理员才可更新公司法定名称。 

1. 转到“设置”，然后选择“组织资料” 。

2. 选择“法人”，然后选择要使用的法定公司资料。
 
1. 选择“提交”后，我们会对你的法定身份重新进行评估。你将收到另一封电子邮件，并且需要接受它。

>[!Important]
>如果你是云解决方案提供商 (CSP) 合作伙伴，那么你不能更改与法定地址相关联的国家/地区。法定地址所在的国家/地区已绑定到租户和服务以及你开展业务时所使用的货币。 如果未加入到云解决方案提供商计划，则可以更改与法定地址相关联的国家/地区。 如果验证状态为“已授权”，则直接计费合作伙伴和间接提供商不能更改公司法定名称。 如果需要更改名称，则需要[创建支持工单](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772)。



## <a name="update-your-mpn-global-business-account"></a>更新 MPN 全球企业帐户

如果在从 Partner Membership Center 迁移到合作伙伴中心的过程中，系统将错误的企业帐户确定为法定企业帐户，你可以将其更改为正确的法定企业帐户。

要进行这些更新，你需要是全局管理员或帐户管理员。了解如何[管理 MPN 全球位置帐户](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>更新与 CSP 帐户关联的 MPN ID

若要更新与 CSP 帐户关联的 MPN ID：

1. 使用 CSP 帐户凭据以全局管理员身份登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)，然后选择“设置”。 （MPN 凭据可能与 CSP 凭据不同。）
 
1. 从“帐户设置”中选择“标识符” 。

1. 在 CSP 部分下，使用“更新”链接更新与 CSP 帐户关联的 MPN ID 。 


## <a name="update-your-csp-legal-billing-address"></a>更新 CSP 合法帐单邮寄地址

如果你是全局管理员、计费管理员或管理员代理，则可以更改发票上“付款和税务资料”中显示的地址。 但是，不能更改发票上的公司名称，因为发票系统存在限制。



## <a name="next-steps"></a>后续步骤

- [检查验证状态](verification-responses.md)

- [管理 MPN 位置](manage-locations.md)
