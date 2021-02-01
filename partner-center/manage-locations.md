---
title: 管理合作伙伴帐户中的位置
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098884"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>管理 MPN 帐户位置并添加新位置


**相应的角色**

- 全局管理员
- 帐户管理员

位置 MPN ID 标识了公司的每一特定位置。 可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。 全局 MPN ID 用于非交易性活动，例如支持请求。

## <a name="the-following-is-a-typical-scenario"></a>下面是一个典型方案：

Contoso 的合作伙伴全局帐户 (PGA) 位于英国。 这是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。 Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。 在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。 PLA 用于交易性业务，例如 CSP 或奖励计划。 付款与特定位置相关。 

>[!NOTE]
>CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>为 CSP 业务添加新帐户的先决条件

若要添加新的 CSP 业务帐户，请先确保满足先决条件。

1. 必须在要开展 CSP 业务的国家/地区具有 MPN ID。 若要创建新的 MPN 位置，请阅读下面的“添加 MPN 位置”。
  
1. 若要创建新的 CSP Indirect Reseller 注册，请阅读[与间接提供商合作](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >请记得使用新凭据登录新的 CSP 帐户 。 不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。

2. 接受 Microsoft 合作伙伴协议并激活帐户。

## <a name="view-your-mpn-locations"></a>查看 MPN 位置

1. 使用 MPN 帐户凭据登录合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。 （MPN 凭据可能与 CSP 凭据不同） 
 
1. 从“设置”图标中，依次选择“帐户设置”、“组织资料”和“法务”   。 

1. 在“合作伙伴”选项卡中，验证确保没有横幅错误消息要求你修复从 PMC 迁移的位置。 如果有错误消息，请按照说明修复这些位置。 

3. 如果没有错误消息，请从“设置”中依次选择“帐户设置”、“组织资料”和“标识符”   。

4. 找到类型为“位置”且与此 CSP 帐户所在国家/地区匹配的 MPN ID，然后用它在下面进行搜索并完成关联。

5. 如果找不到与要使用的 CSP 帐户匹配的位置 MPN ID，可添加一个新位置，它将创建新的 MPN ID。 请查看下面的“添加 MPN 位置”。

## <a name="add-an-mpn-location"></a>添加 MPN 位置

1. 在合作伙伴中心使用 MPN 帐户进行登录。 （你的 MPN 凭据可能与 CSP 凭据不同）。 MPN 帐户应具有全局管理员或帐户管理员权限。 

1. 从设置图标中，选择“帐户设置”，然后选择“组织资料”  。

2. 选择“法务”，然后在“合作伙伴”选项卡上选择“业务位置”，然后单击“添加位置”   。

3. 提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和联系人。
 
1. 单击“添加位置”。 这将为新位置创建一个新的 MPN ID，你可用它来进行 CSP 交易和激励。

:::image type="content" source="images/legal-biz.png" alt-text="添加新的法定公司":::

> [!NOTE]
> 一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。 如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。

## <a name="change-country-of-partner-global-account"></a>更改合作伙伴全球帐户所在国家/地区 

1. 在合作伙伴中心使用 MPN 帐户进行登录。 （你的 MPN 凭据可能与 CSP 凭据不同）。 MPN 帐户应具有全局管理员或帐户管理员权限。 

2. 在“合作伙伴”选项卡上，转到“业务位置”，然后检查位置列表，确保已列出你想用作法律实体的位置 。 
 
1. 若要添加位置，请单击“添加位置”，然后在弹出窗口中，提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和主要联系人。 
 
1. 选择“国家/地区”下拉列表旁边的“更改国家/地区”，然后按照步骤操作 。 

:::image type="content" source="images/lbp.png" alt-text="法定公司资料数据弹出窗口":::

5. 单击“保存”。

6. MPN 全球帐户所在国家/地区将更改为新的法定国家/地区。
  
## <a name="next-steps"></a>后续步骤

- 了解[验证过程](verification-responses.md)。
