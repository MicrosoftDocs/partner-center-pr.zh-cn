---
title: 代表客户报告问题
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解何时将客户服务问题上报给 Microsoft，以及如何为不同类型的客户提交支持Microsoft 服务。
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ba25d0bfc4796ca43d36bb34bf6d9e82889881c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855703"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>代表客户报告服务问题 - 包括何时以及如何这样做

**适用于 ：** 合作伙伴中心 |合作伙伴中心Microsoft Cloud for US Government

**适当角色**：全局管理员

如果客户遇到无法解决的服务问题，并且符合将问题上报 [给 Microsoft](escalate-problems-to-microsoft.md)中所述的条件，则间接提供商可以提交支持票证。 此过程也可用于反映计费问题或争议以及欺诈担忧。

## <a name="submit-a-service-request-for-a-customer"></a>提交客户服务请求

1. 在 CSP 下的合作伙伴中心菜单中，选择" **客户"**

2. 在"客户"页上，选择或搜索想要的客户
    
3. 从客户菜单中，选择 **"服务请求"**

4. 从“新建请求”下拉菜单中，选择“Azure”或“Office 365、Dynamics 365、企业移动性套件”。 你将被重定向到 Microsoft Azure 门户 Office 365 管理中心。

>[!NOTE]
>在 CSP 中交易 Dynamics 365 的支持运营合作伙伴需要维护对 ASfP 合作伙伴计划或 (高级支持) 协议。 代表 CSP 客户提交 Dynamics 365 事件需要此支持协议。 [详细了解](https://partner.microsoft.com/support/partnersupport) 支持协议选项。

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> 如果需要在 Azure 中为客户创建服务请求，请注意：
>
>- 为了使你作为间接经销商在 Azure 中为客户创建服务请求，间接提供商必须授予你访问客户的 Azure 帐户的权限。 这不同于代表 Office 365 客户进行管理。
>
>- 合作伙伴中心的支持管理员不能在 Azure 服务门户中创建服务请求，而只能在 Azure 服务门户中创建支持组，为该组提供记录支持请求的权限。

1. 选择“新建支持请求”。

2. 使用相应信息填写支持请求，然后选择“创建”：

   - 在支持请求的“基本信息”部分，确保在“支持计划”字段中选择“云解决方案提供商”。

   - 在支持请求的 **联系人** 信息部分中，输入你的信息，而不是你的客户的信息。

3. 以后若要在 Microsoft Azure 门户中查看客户的服务请求，则选择“管理支持请求”即可。

没有客户的管理员权限时，可能需要为客户创建支持请求。 这可能出现在下面的两种情况中：

- 首次建立关系时，未请求管理员权限。
- 仅管理客户的 Azure 订阅，因此没有管理权限。
 
不管什么情况，均可通过以下过程创建支持请求。 

1. 从客户的帐户页复制客户的域名，合作伙伴中心。

2. 访问 https://portal.azure.com/[customerdomainname]。 

3. 选择需要支持的 Azure 订阅。

4. 选择“新建支持请求”，然后按提示创建请求。 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365、Microsoft Dynamics CRM Online、企业移动性套件

1. 在" **创建服务请求"** 部分中，选择适当的支持类别。 可能需要选择"更多 **..."** 来查看其他文章。

2. 完成服务请求表单，然后选择“提交”。

   > [!TIP]
   > 请确保其中包含的是你的联系人信息，而不是客户的。

3. 稍后，转到 Office 365 管理中心，然后选择 " **查看所有支持票证**"，查看客户的服务请求。

### <a name="support-for-commercial-marketplace-products"></a>对商业市场产品的支持

Microsoft 不为商业 marketplace 产品提供产品支持。 你需要与发布产品的独立软件供应商 (ISV) 联系以获取支持。

若要查找 ISV 的联系人信息，请执行以下操作：

1.  在“市场”页上，选择需要获取相关帮助的产品。

2.  在产品的页面上，你将找到支持联系人信息。 这可能是以下一个或多个选项：

    - 指向 ISV 的网站上的支持入口点的链接
    - 支持部门的电子邮件
    - 支持部门的联系电话号码

## <a name="faq"></a>FAQ

请参阅以下常见问题，其中介绍了你可能代表客户提交的服务请求。 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>哪些内容作为支持权利的一部分包含在内？

应通过合作伙伴中心来归档服务请求。 它们适用于 Azure、Microsoft Office 365、Microsoft Dynamics CRM Online 和企业移动性套件。 作为参与云解决方案提供商计划的合作伙伴，你的主要问题会得到优先响应。

CSP 支持权益不包括对你自己的合作伙伴租户的支持。 但是，Office 365、Microsoft Dynamics CRM Online 和企业移动性套件不对合作伙伴或客户收取单独的支持订阅费用。 Azure 会向你收取费用，但如果你有权签名云支持或其他 Microsoft 合作伙伴网络 (MPN) 权益，你可以使用这些权益来支付费用。

此权益适用于所有参与云解决方案提供商计划（不管是付费计划还是免费试用计划）的合作伙伴。 帐单和订阅管理支持也作为此程序包的免费组件包含在内。

### <a name="how-quickly-will-i-get-an-initial-response"></a>我多快才能获得初始响应？

我们的初始响应时间取决于已提交事件的严重性。 提交服务请求时，问题的严重性将由业务影响指示确定。

**技术中断修复事件** 的初始响应时间：

- 严重影响 (严重性 A) ：两小时， (严重丢失或服务降级。 生产服务关闭。）
- 中等影响 (严重性 B) ：四个小时， (服务的适中丢失或降级。 生产服务受到部分影响。 ) 
- 最小影响 (严重性 C) ：8小时， (服务的最小丢失或下降。 服务仍处于可用或非生产服务。 ) 

初始响应时间仅适用于英语语言支持。 在营业时间提供本地语言支持。
对于落在支持权利边界内的事件，但不视为中断修复事件，初始响应时间可能会长达一天。

### <a name="can-i-submit-a-service-request-by-phone"></a>是否可以通过电话提交服务请求？

不，此程序不提供电话支持。

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>如果我登录 Azure 门户但绕过合作伙伴中心，会发生什么？

如果直接登录到 Microsoft Azure 门户，则可以在自己的上下文中查看中心，而不是客户的上下文。 因此，在创建自己的订阅的服务请求时，Microsoft Azure 门户直接登录到订阅。

CSP 计划支持权利不提供对你自己的合作伙伴订阅的支持。 因此，创建与自己的合作伙伴订阅有关的服务请求时，需要提供有效的支持计划权利。 示例包括 MPN 合同 ID、顶级或 Azure 支持计划。 有关详细信息，请参阅常见问题 [Azure 支持常见问题解答](https://go.microsoft.com/fwlink/?LinkId=717532)。

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>如果我登录到 Office 365 管理中心门户并绕过登录，会发生什么合作伙伴中心？

如果直接登录到 Office 365 管理中心，你将在你自己的上下文中查看中心，而不是客户的上下文。 因此，在创建自己的订阅的服务请求时，只应直接登录到 Office 365 管理中心。

### <a name="how-do-i-get-additional-dynamics-365-support"></a>如何获取更多 Dynamics 365 支持？

如果遇到与 Dynamics 365 计划订阅、许可、计费、财务 & 运营、Dynamics 365 产品许可证相关的问题，或者需要进一步技术支持：
 
请联系 [Dynamics 支持人员](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>后续步骤

- [向你的客户提供支持](customer-support.md)
- [检查服务运行状况](check-service-health.md)
