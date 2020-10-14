---
title: 管理合作伙伴帐户中的位置
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c4435227cdd5d777d11c79bf4adc63471ad925e9
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006858"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>管理 MPN 帐户位置并添加新位置

**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员
- 帐户管理员

位置 MPN ID 标识了公司的每一特定位置。 可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。 全局 MPN ID 用于非交易性活动，例如支持请求。

## <a name="the-following-is-a-typical-scenario"></a>下面是一个典型方案：

Contoso 的合作伙伴全局帐户 (PGA) 位于英国。 这是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。 Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。 在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。 PLA 用于交易性业务，例如 CSP 或奖励计划。 付款与特定位置相关。 

>[!NOTE]
>CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>为 CSP 业务添加新位置的先决条件

若要添加新的 CSP 业务位置，需要满足以下先决条件：

1. 必须在要开展业务的国家/地区具有 MPN ID。

1. 你需要在尚未注册 CSP 的[业务区域](regional-authorization-overview.md)中具有一个新的 Azure AD 租户。 在注册 CSP 时创建此租户。
 
3. 使用新的 AAD 租户注册在该区域注册 CSP 计划。
提供法定的公司详细信息，包括合法的公司名称、地址、主要联系人详细信息。 此帐户将经过验证，因此请确保添加有效的信息。

>[!NOTE] 
 >请记住，使用新的凭据登录新的 Azure AD 租户 。 不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。

4. 接受 Microsoft 合作伙伴协议并激活帐户。

## <a name="add-a-location"></a>添加位置

1. 使用合作伙伴中心的 MPN 帐户登录。 MPN 帐户应具有全局管理员或帐户管理员权限。 

1. 从“设置”图标中选择“合作伙伴设置”。 

2. 选择“位置”。

3. 选择“添加位置”，然后插入要添加到公司的位置的地址详细信息以及该位置的主要联系人。

> [!NOTE]
> 一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。 如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。

## <a name="change-global-partner-account-location"></a>更改全局合作伙伴帐户位置

1. 在“[位置](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)”页面上，检查位置列表，确保其中已列出你希望作为法人实体的位置。 否则，请添加该位置。

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN 位置的结构":::

2. 选择“合作伙伴配置文件”，然后选择“更新法定公司配置文件” 

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN 位置的结构":::

3. 选择区域和法人，并“提交”。

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN 位置的结构":::

## <a name="next-steps"></a>后续步骤

- 了解[验证过程](verification-responses.md)。
