---
title: 管理合作伙伴帐户中的位置
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何添加新位置，以及位置 MPN ID 如何用于奖励计划、CSP 业务、订阅和其他交易。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276818"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>管理 MPN 帐户位置并添加（删除）位置


**相应的角色**：全局管理员 | 帐户管理员

位置 MPN ID 标识了公司的每一特定位置。 可以使用位置 MPN ID 注册奖励计划、进行云解决方案提供商 (CSP) 业务交易以及其他业务交易。 全局 MPN ID 用于非交易性活动，例如支持请求。

## <a name="the-following-scenario-is-typical"></a>以下为典型场景：

Contoso 的合作伙伴全局帐户 (PGA) 位于英国。 PGA 是其注册的合法业务，它具有一个用于管理所有非交易性业务的全局 MPN ID。 Contoso 在英国、法国和美国的其他位置也具有相当于子公司或部门的合作伙伴位置帐户 (PLA)。 在 MPN 帐户结构中，这些 PLA 表示为唯一位置 MPN ID。 PLA 用于交易性业务，例如 CSP 或奖励计划。 付款与特定位置相关。 

>[!NOTE]
>CSP 租户与 MPN 位置 ID 之间存在 1 对 1 关系。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的结构。":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>为 CSP 业务添加新帐户的先决条件

若要添加新的 CSP 业务帐户，请先确保满足先决条件。

1. 必须在要开展 CSP 业务的国家/地区具有 MPN ID。 若要创建新的 MPN 位置，请阅读下面的“添加 MPN 位置”。
  
1. 若要创建新的 CSP Indirect Reseller 注册，请阅读[与间接提供商合作](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >请记得使用新凭据登录新的 CSP 帐户 。 不要使用现有凭据，因为合作伙伴中心会将你识别为已经拥有帐户。

2. 接受 Microsoft 合作伙伴协议并激活帐户。

1. 如果要注册为直接计费合作伙伴，请阅读[直接计费合作伙伴要求](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>查看和更新 MPN 位置

1. 使用 MPN 帐户凭据登录合作伙伴中心[仪表板](https://partner.microsoft.com/dashboard/home)。 （MPN 凭据可能与 CSP 凭据不同） 
 
1. 从“设置”图标中，依次选择“帐户设置”、“组织资料”和“法务”   。 

1. 在“合作伙伴”选项卡中，验证确保没有横幅错误消息要求你修复从 PMC 迁移的位置。  如果位置未在 PMC 中正确设置，并且尚未转换为 PC，则需要更新这些位置。

:::image type="content" source="images/locations/location-two.png" alt-text="截图演示如何更新位置。":::
 
4.  在“查看 PMC 位置”屏幕上，选择“更新” 。
更新以下字段：

- “名称”字段：确保公司位置的名称正确。 如果显示重复错误，请尝试进行更改，例如将“Contoso”更改为“Contoso, Inc”。

- “法律实体”字段：确保已选择该位置所绑定到的法律实体

- “地址行 1”和“地址行 2”字段：确保地址正确

- “城市和省/直辖市/自治区”字段：确保城市和省/市/自治区之间的组合是正确的。 在某些国家/地区可以应用用于选择省/直辖市/自治区的下拉菜单，在其他国家/地区则需要手动插入该字段。

- “邮政编码”字段：确保“邮政编码”字段与指定的国家/地区、区域、城市或地址匹配。

- “主要联系人信息”字段：确保已填写“名字”和“姓氏”字段，并且所指示的电子邮件地址是工作电子邮件地址，而不是个人电子邮件地址（例如，@outlook.com、@live.com 等）

- “电话号码”字段：确保电话号码不包含特殊字符、空格或国家/地区代码。 “电话号码”字段中输入的值将始终包含最多 10 个字符。

5. 如果没有错误消息，请从“设置”中依次选择“帐户设置”、“组织资料”和“标识符”   。

6. 找到类型为“位置”且与此 CSP 帐户所在国家/地区匹配的 MPN ID，然后用它完成关联。

7. 如果找不到与要使用的 CSP 帐户匹配的位置 MPN ID，可添加一个新位置，它将创建新的 MPN ID。 请查看下面的“添加 MPN 位置”。

## <a name="add-an-mpn-location"></a>添加 MPN 位置

1. 在合作伙伴中心使用 MPN 帐户进行登录。 （MPN 凭据可能与 CSP 凭据不同。）MPN 帐户应具有全局管理员或帐户管理员权限。 

1. 从设置图标中，选择“帐户设置”，然后选择“组织资料”  。

2. 选择“法务”，然后在“合作伙伴”选项卡上选择“业务位置”，然后选择“添加位置”   。

3. 提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和联系人。
 
1. 选择“添加位置”。 这将为新位置创建一个新的 MPN ID，你可用它来进行 CSP 交易和激励。

:::image type="content" source="images/legal-biz.png" alt-text="添加新的法人。":::

> [!NOTE]
> 一旦将某一位置添加到合作伙伴中心后，就不能再删除它了。 如果已使用正确的 MPN ID 登录，则会在合作伙伴中心的左侧菜单中看到 MPN。

## <a name="add-the-registration-number-id"></a>添加注册号 ID

如果你是间接提供商、直接计费合作伙伴或间接经销商，并且与以下国家/地区的新客户和现有客户开展业务，则需要为你的企业提供注册 ID 号。 如果你开展业务的国家/地区未在下面列出，则不必提供注册 ID。

- 亚美尼亚 
- 阿塞拜疆 
- 白俄罗斯 
- 巴西 
- 匈牙利 
- 印度 
- 伊拉克 
- 哈萨克斯坦 
- 吉尔吉斯斯坦 
- 摩尔多瓦 
- 缅甸 
- 波兰 
- 俄罗斯 
- 沙特阿拉伯 
- 南非 
- 南苏丹  
- 塔吉克斯坦 
- 泰国
- 土耳其 
- 乌克兰 
- 阿拉伯联合酋长国 
- 乌兹别克斯坦 
- 委内瑞拉
- 越南 


有关详细信息，请参阅[注册 ID 号信息](reg-number-id.md)

## <a name="delete-a-location"></a>删除位置

若要从帐户中删除某个位置，需要联系[合作伙伴支持人员](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)。 请确保了解此操作的影响。 无法检索已删除的位置，并且将不再为你的公司识别或激活任何绑定到该特定 MPN ID 的内容。

## <a name="change-country-of-partner-global-account"></a>更改合作伙伴全球帐户所在国家/地区 

1. 在合作伙伴中心使用 MPN 帐户进行登录。 （MPN 凭据可能与 CSP 凭据不同。）MPN 帐户应具有全局管理员或帐户管理员权限。 

2. 在“合作伙伴”选项卡上，转到“业务位置”，然后检查位置列表，确保已列出你想用作法律实体的位置 。 
 
1. 若要添加位置，请单击“添加位置”，然后在弹出窗口中，提供必需的详细信息，包括你想要添加到你的公司的位置的业务名称、地址和主要联系人。 
 
1. 选择“国家/地区”下拉列表旁边的“更改国家/地区”，然后按照步骤操作 。 

:::image type="content" source="images/lbp.png" alt-text="法人资料数据弹出窗口。":::

5. 选择“保存”。

6. MPN 全球帐户所在国家/地区将更改为新的法定国家/地区。
  
## <a name="next-steps"></a>后续步骤

- 了解[验证过程](verification-responses.md)。
