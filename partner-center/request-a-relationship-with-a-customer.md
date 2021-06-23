---
title: 请求经销商与客户的关系
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 请求与多合作伙伴、多渠道方案的客户建立关系，或者，如果需要还原客户的委派管理员权限，
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 83f615e69a9285365e68305fa909104e0da52992
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551633"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>如何在合作伙伴中心向客户请求经销商关系

**适当的角色**：管理员代理|全局管理员

如果要代表客户管理客户的服务或订阅，客户必须授予该服务或订阅的管理员权限，并签署Microsoft 客户协议。

如果要与客户建立经销商关系并仅管理预配的 Azure 订阅，则无需获取管理员权限。

>[!NOTE] 
>不请求权限的选项不适用于在 Microsoft Cloud for US Government Microsoft Cloud Germany 中运行的合作伙伴。 若要了解有关详细信息，请参阅 [客户将管理权限委托给合作伙伴](customers-revoke-admin-privileges.md)。

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>邀请客户与你建立经销商关系

可以从你的国家/地区或同一区域请求与客户建立经销商关系。

1. 从“合作伙伴中心”菜单中选择“客户”，然后选择“请求经销商关系”。

2. 若要从此客户请求管理员权限，请选择"包括 Azure Active Directory **Office 365 的委派管理权限"。** 如果要建立关系但不请求管理员权限，请清除此选项。

3. 在下一页上，查看电子邮件草稿。 可以在默认的电子邮件应用程序中打开邮件草稿，也可以将其复制到剪贴板，然后将其粘贴到电子邮件中。

   你可以编辑电子邮件中的文本，但请务必包括链接，因为它进行了个性化设置，可以将客户直接链接到你的帐户。 完成此步骤后选择“完成”。

4. 将电子邮件发送到客户。

5. 客户接受邀请后，他们将出现在"客户"页上，并可以从该页为客户预配和管理服务。

   > [!NOTE]
   > 如果客户尚未接受你的Microsoft 客户协议，则当他们接受你的邀请时，系统会提示他们这样做。 客户需要全局管理员才能接受邀请。

6. 若要管理客户的帐户、服务、用户和许可证，请选择客户名称旁边的向下箭头，展开客户的记录。

> [!IMPORTANT]  
> 客户可以在服务的管理门户中重新分配或删除管理员权限。 但是，除非你与客户重新协商协议，否则你将继续负责提供客户支持并遵守 Microsoft 合作伙伴协议 条款，即使在客户重新分配或删除管理员权限之后。 在这种情况下，如果客户需要帮助，你可以致电 Microsoft 支持以代表客户打开服务请求。

## <a name="changes-to-the-customer-invitation-experience"></a>客户邀请体验的更改

从云解决方案提供商提供商合作伙伴云解决方案提供商 (经销商关系邀请) 由不同的面向客户的门户托管。 门户位置取决于客户是位于 Microsoft 公有云还是国家云中：

|云客户类型  | 客户在何处接受经销商关系邀请？ |
|---------|---------
| 公有云中的客户 | Microsoft 365 管理中心 |
| 德国合作伙伴中心 Microsoft 云的客户 | Microsoft Office管理门户 |
| 客户合作伙伴中心Microsoft Cloud for US Government | Microsoft Office管理门户 |
|

## <a name="next-steps"></a>后续步骤

- [分配支持联系人](assign-support-contacts.md)

- [删除与客户的关系](remove-a-relationship.md)
