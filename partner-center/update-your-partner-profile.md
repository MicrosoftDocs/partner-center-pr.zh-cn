---
title: 验证公司配置文件
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何验证公司详细信息，例如主要联系人、地址和计划信息。 还可以更新法律和帐单地址。
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 04/12/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q4
ms.openlocfilehash: 9f9a055ce3bfbff568287267b74b04e8f9d03ad1
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080616"
---
# <a name="verify-or-update-your-company-profile-information"></a>验证或更新你的公司资料信息 

**相应的角色**：全局管理员 | MPN 帐户管理员

在首次以全局管理员身份登录到合作伙伴中心时，应确认你所有的公司详细信息是否正确。 包括主要联系人、法定公司名称和地址，以及计划信息。 如果公司有多个位置，请查看位置数据以确保其准确性。 作为全局管理员、帐务管理员或管理员代理，你也可以查看并更新帐务和税务信息。

> [!NOTE]
> 只有全局管理员才能更新帐单邮寄地址。

合作伙伴配置文件包含法定公司信息、主要联系人名称和电子邮件、公司参与的计划，以及现在合并到法定公司名下的其他公司（如果适用）。 请确保法人资料中的公司名称和地址没有拼写错误和缩写，并且与正式的公司商业注册记录完全一致。 如果以个体经营者的身份运营，则需要将公司名称用作法人名称。


## <a name="locate-the-legal-business-profile"></a>找到公司法定资料

1. 在“合作伙伴中心”中，选择“设置”图标，然后选择“帐户设置”。 
 
1. 选择“组织资料”。 

2. 查看“法人资料”、“主要联系人信息”和“计划信息”的值。  

如果已将其他公司合并到法定公司名下，则也可查看其信息。 

## <a name="update-your-legal-business-profile"></a>更新法定公司配置文件 

在合作伙伴中心更新你的法定公司名称或地址。

>[!Important]
>- 对于 Microsoft 合作伙伴网络 (MPN) 帐户，全局管理员和帐户管理员都可以更新法定公司名称。
>- 对于云解决方案提供商 (CSP) 间接经销商帐户，只有全局管理员才可更新法定公司名称。 
>- 如果帐户验证状态为“已授权”，则直接计费合作伙伴和间接提供商不能更改其公司的法定名称。 如需更改名称，必须创建[支持票证](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772)。



1. 在“合作伙伴中心”中，依次选择“设置”、“帐户设置”和“组织资料”。

2. 选择“法人”，然后选择要更新的法人资料（合作伙伴或经销商）。

1. 选择公司名称/地址旁边的“更新”，然后更改详细信息。
 
1. 选择“提交”后，系统将重新评估你的法定标识。 我们只重新评估更改的内容。

1. 如果验证失败，请了解如何[解决问题](verification-responses.md)。

>[!Important]
>如果你是云解决方案提供商合作伙伴，则无法更改与你的法定地址关联的国家/地区。 法定地址所在的国家/地区已绑定到你租户和服务，还已绑定到你开展业务时所使用的货币。 若要了解 MPN 国家/地区更新，请阅读 [MPN 国家/地区更新](manage-locations.md#change-country-of-partner-global-account)。


### <a name="who-can-update-legal-business-name-and-when"></a>谁在何时可更新法定公司名称

|Program|**谁可更新公司名称**|**当状态为 (status) 时，可更新该名称**|**允许**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|全局管理员；帐户管理员|已授权；待定；已拒绝| 然后用户才能访问|
|CSP：间接经销商|全局管理员|已授权；待定；已拒绝| 然后用户才能访问|


## <a name="update-your-mpn-global-business-account"></a>更新 MPN 全球企业帐户

在从 Partner Membership Center 迁移到合作伙伴中心的过程中，如果系统将错误的公司帐户确定为法人帐户，你可以将其更改为正确的法人帐户。

要进行这些更新，你需要是全局管理员或帐户管理员。了解如何[管理 MPN 全球位置帐户](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>更新与 CSP 帐户关联的 MPN ID

若要更新与 CSP 帐户关联的 MPN ID：

1. 使用 CSP 帐户凭据以全局管理员身份登录到合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)，然后选择“设置”。 （MPN 凭据可能与 CSP 凭据不同。）
 
1. 从“帐户设置”中选择“标识符” 。

1. 在 CSP 部分下，使用“更新”链接更新与 CSP 帐户关联的 MPN ID 。 


## <a name="update-your-csp-legal-billing-address"></a>更新 CSP 合法帐单邮寄地址

如果你是全局管理员，则可以在“付款和税务资料”中更改发票上显示的地址。 但是，你无法更改发票上的公司名称，因为发票系统存在限制。

:::image type="content" source="images/billing-profile.png" alt-text="添加了账单信息的区域的屏幕截图。":::

|字段  |**说明**|  
|---------------------|:------------------|
|收票公司名称|CSP 发票上“账单寄往地址”信息中显示的公司名称。  此信息在合作伙伴中心内不可编辑。  若要更新，请创建支持工单。|
|账单寄往地址|CSP 发票上显示的账单寄往地址。 可以从[计费对象信息](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)中更新。|
|收票联系人|CSP 帐户的账单联系人详细信息（名字、姓氏、主要号码）。  可以从[计费对象信息](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)中更新。|
|PO 编号|合作伙伴发票上显示的采购订单编号。 可以从[计费对象信息](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)中更新。|
|公司税号|某些国家/地区的公司可以提供其[增值税 (VAT) 号或本地等效税号](./organization-tax-info.md)。 若要更新你的税号/增值税号，你必须是全局管理员、帐单管理员或管理员代理。|
|计费货币|CSP 帐户的计费货币由 CSP 帐户的法定国家/地区决定。  创建云解决方案提供商帐户后，便不能更改此信息。|

## <a name="next-steps"></a>后续步骤

- [检查验证状态](verification-responses.md)

- [管理 MPN 位置](manage-locations.md)
