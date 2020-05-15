---
title: 准备从 Partner Membership Center 迁移到合作伙伴中心 | 合作伙伴中心
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在将业务从 PMC 迁移到合作伙伴中心之前，请先查看有用的信息和常见问题解答。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 127919c92bf6fffca846dd92cde4c787bfd16641
ms.sourcegitcommit: 87b13da77c16a304d2a7682bf24422f8b9288b51
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2020
ms.locfileid: "82859358"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>准备从 Partner Membership Center (PMC) 迁移到合作伙伴中心

**相应的角色**
-    全局管理员
-    用户管理员
-    销售代理
-    管理员代理

我们正在将成员资格管理从 Partner Membership Center (PMC) 迁移到合作伙伴中心- 管理与 Microsoft 的业务关系的单一目的地。 我们希望你迁移到合作伙伴中心后会尽可能实现轻松高效的管理。 我们确定了合作伙伴中心与 PMC 一些不同的部分，我们认为在你进行迁移之前需要了解这些部分并做好相应的准备。

## <a name="account-and-identity-setup"></a>帐户和标识设置

**什么是 Azure Active Directory (Azure AD) 工作帐户？**

Azure 工作帐户是公司在 Azure 公有云中的专用独立虚拟表示形式，它是在订阅 Microsoft 云服务（如 Azure、Microsoft Intune 或 Office 365）时创建的。

工作帐户托管 Azure AD 用户及其相关信息 - 他们的密码、个人资料数据和权限等。 工作帐户还包含组、应用程序以及有关公司及其安全性的其他信息。 

你的工作电子邮件属于你 Azure Active Directory 租户的一部分。 若要在合作伙伴中心中拥有帐户，你需要拥有 AAD 租户。 有关 Azure Active Directory 的详细信息，请参阅[在 Azure AD 中创建目录](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。

在合作伙伴中心，你将使用工作电子邮件来登录你的帐户，而不是使用个人电子邮件。
- 你的工作帐户：john@contoso.com
- 你的个人帐户：John@outlook.com

**如果你有一个 Microsoft （例如 Office 365）的 AAD 租户并且还有适用于你的 CSP 业务的租户，你应该使用哪个帐户登录到合作伙伴中心？**

可以使用 CSP 帐户或 MPN 工作电子邮件帐户登录到合作伙伴中心。 如果选择使用 CSP 工作电子邮件登录，面板上的左侧导航则将显示 MPN 和 CSP 计划信息。 如果使用 MPN Azure AD 租户工作电子邮件登录，则只会看到 MPN 计划信息。 

**如果不想将现有的 Office 365 Azure AD 租户用于合作伙伴中心，则可以在从 PMC 迁移之前创建新租户。**

可能有很多原因导致你不想使用现有的 Azure AD 租户来设置合作伙伴中心帐户。 在开始迁移到合作伙伴中心之前，请先转至 [Azure 门户](https://ms.portal.azure.com/#home)以创建新的 Azure AD 租户。 按照[在 Azure Active Directory 中创建新租户](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)中的指南进行操作。 使用新的 AAD 租户设置合作伙伴中心帐户。 只有全局管理员才能创建租户。 


**用户角色，包括合作伙伴中心中的来宾用户角色**

合作伙伴中心具有不同类型的角色，具体取决于需要完成的工作类型。 有属于 Azure AD 角色的全局管理员等角色。 某些角色特定于云服务提供商计划或奖励等计划，并且有特定于 MPN 的角色。 若要了解所有的合作伙伴中心角色，请参阅[为用户分配角色和权限](permissions-overview.md)。

**当我用户的角色从 PMC 迁移到合作伙伴中心时会发生什么情况？**

除了 MPN 全局管理员或执行迁移的主要计划联系人外，PMC 中的所有用户将失去他们的管理员角色。 完成迁移的个人需要在合作伙伴中心中分配角色。 合作伙伴中心中的角色不同于 PMC 中的角色。 若要详细了解合作伙伴中心中的用户角色，请参阅 [为用户分配角色和权限](permissions-overview.md 以及[从 PMC 迁移到合作伙伴中心](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)。


**我的公司配置文件和我的业务配置文件之间有什么区别？**

公司配置文件是公司的相关信息，包括地址、位置、主要联系人、银行和税务详细信息。

你的业务配置文件是你像客户展示自己的方式，并且是显示你的徽标、业务重心的详细信息，以及你的专长等信息的一个营销页面。

**帐户合并对我的帐户而言有什么意义？**

如果你使用相同的 Azure AD 租户将多个 MPN 帐户迁移到合作伙伴中心，系统将自动识别出来并要求你合并帐户。 这也适用于你有多个关联到同一 Azure AD 租户的域。 

你仍然可以决定使用单独的 ADD 租户迁移到合作伙伴中心，但请注意，这会导致对你的资格进行单独评估并且会产生额外的购买成本。 有关帐户合并的详细信息，请参阅[合并公司帐户](consolidate-accounts.md)

**如果我有多个 ADD 租户和一个 MPN 帐户，是否可以在合作伙伴中心中链接它们？**

是的，可以在合作伙伴中心中将多个 Azure AD 租户链接到一个合作伙伴中心帐户。
有关帐户合并的详细信息，请参阅[合并公司帐户](consolidate-accounts.md)

**将多个 Azure AD 租户添加到一个合作伙伴中心帐户有什么限制吗？**

如果 Azure AD 租户已与一个现有的合作伙伴中心帐户相关联，则不能使用多租户功能将它关联到新的合作伙伴中心帐户。 另一种思考方向是，一个 Azure AD 租户只能关联到一个合作伙伴中心帐户，但一个合作伙伴中心帐户可以有多个与之关联的租户。

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft 合作伙伴网络 (MPN) 成员资格迁移 

**谁可以执行从 PMC 到合作伙伴中心的迁移？**

公司 MPN 全局管理员或主要计划联系人（这两个角色通常由同一人持有）可以发起和执行迁移。

**完成迁移的人员是否会成为合作伙伴中心中公司法定配置文件上的主要联系人？**

不一定，然而，主要联系人需要是有权签署协议的人员。

**Microsoft 能否为我迁移我的 MPN 成员资格？**

不能。 Microsoft 无法帮助你将成员资格帐户移到合作伙伴中心。 你需要使用你的工作帐户（登录凭据）登录 PMC 来迁移你的帐户，以便开始进行迁移。 完成迁移帐户的步骤后，可以开始管理你的成员资格并向你的团队分配用户角色和权限，使他们可以访问权益并帮助管理成员资格。 Microsoft 将自动迁移当前的资格、权益、位置信息、用于奖励的银行/税务信息，以及 MCP 关联，包括 Partner University 访问权限。

Microsoft 将自动迁移当前的资格、权益、位置信息、用于奖励的银行/税务信息，以及 MCP 关联，包括 Partner University 访问权限。

**续订策略会如何变化？**

 在合作伙伴中心，续订时段自你的周年日期起到接下来的 30 天内。

**在迁移到合作伙伴中心后，我们的资格是否保持不变？**

是的，资格不会受迁移到合作伙伴中心的影响。 如果出现不相符的情况，请联系[支持部门](https://partner.microsoft.com/support)。


 **我的权益（包括云权益、技术支持、软件权益、Visual Studio）是否会在迁移后更改？**

 你符合使用资格的权益将不会更改。 如果出现不相符的情况，请联系[支持部门](https://partner.microsoft.com/support)。

 **我们的 Microsoft 帐户是否会享有已有的 Visual Studio 权益分配？**


 是的。 分配给 MSA 的 Visual Studio 权益仍将有效，会继续保留。 在合作伙伴中心续订后，仍会保留它们。 不过，如果你在迁移到合作伙伴中心以后删除了某个 MSA 分配，则不能将它重新添加到合作伙伴中心。

在合作伙伴中心，合作伙伴可以添加特定的工作帐户和来宾用户帐户，这些帐户是同一租户的 MSA，而这些租户中的合作伙伴在 Azure AD 租户中是 MPN 管理员。 如果合作伙伴在多个 Azure AD 租户中是全局管理员，并且所有这些租户都关联到同一个合作伙伴中心帐户，则该合作伙伴可以跨所有这些租户将用户添加到 Visual Studio 权益中以及基于 Azure 使用情况的分配计划中。

虽然来宾用户可以由 MPN 管理员或全局管理员分配基于使用情况的 Visual Studio 订阅，但来宾用户不能使用其 MSA 登录合作伙伴中心。 不过，来宾用户可以登录 Azure 和 Visual Studio，以便验证和使用分配给他们的权益。


 **我们应如何管理 MCP 关联和 Partner University 访问权限？**

 从 PMC 迁移的 MCP 关联不会有什么更改。 然而，需要在合作伙伴中心将迁移到合作伙伴中心后的任何新员工进行关联。 你所有针对现有用户的 Partner University 权限将保留，不过，任何新员工都应该访问[培训中心](https://partner.microsoft.com/training)获取有关如何获取对 Partner University 的访问权限的信息。

 **迁移到合作伙伴中心后如何查看 MCP 信息？**

在面板的左侧导航栏中选择“资格”。  在“资格”页面中，你可以下载技能报告。  技能报告将列出合作伙伴中心中已获得了与资格相关的技能以及计划的用户。 如果你的用户获得了技能，但这些技能与你所围绕展开工作的资格无关，这些用户则不会在报告中列出。


 **合作伙伴中心中是否使用了客户证明？**

 否，无需客户证明即可满足合作伙伴中心的资格要求。

 **记录合作伙伴关联是否将迁移到合作伙伴中心？**

 是的，记录合作伙伴不会有任何更改。 了解[将合作伙伴 ID 链接到客户](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)的详细信息。

**奖励计划是否会因迁移到合作伙伴中心而受到影响？**

不会，如果你迁移了帐户但没有合并位置，奖励计划则不会受到任何影响。 如果你的企业在 PMC 中有多个帐户，但你迁移到合作伙伴中心并决定合并到一个全局帐户时，不会对奖励造成任何损失，不过可能会稻城奖励付款出现延迟的情况。 如果不迁移所有涉及到奖励计划的 PMC 帐户，你可能会停止获得与这些帐户相绑定的奖励。


**合作伙伴中心中的奖励角色是什么？** 

合作伙伴中心中的奖励用户是基于位置的角色，并且包含奖励管理员和奖励用户。 有关这些角色可以执行的操作的详细信息，请参阅[为用户分配角色和权限](permissions-overview.md)。

**是否可以在全局和位置级别分配奖励管理员？**

 是的。 你可以将奖励管理员分配为所有位置的奖励管理员，或者每一位置可以有自己的奖励管理员。

 **奖励是否可以在全局或本地级别支付？**

 奖励仅在位置级别支付。

**就引荐而言，我们可以创建多少个业务配置文件？**

你的公司可以按需创建任意数量的业务配置文件，以完全代表你公司的兴趣。 在每一业务配置文件中，你可以列出多达五个位置，每国家/地区一个位置。 每一业务配置文件都可以接收每一相关位置的引荐。

**引荐将如何分配，会出现什么更改？例如，如果我在某一市场中有一个全球公司并且在其他市场中有多个位置，引荐将如何分配？**

引荐是根据客户定义的搜索参数分配的。 无论你有一个还是多个位置，如果客户定义了一个所需位置并且你在此位置有满足其他参数的业务，那么引荐则将转至此位置。








