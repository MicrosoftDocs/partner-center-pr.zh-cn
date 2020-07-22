---
title: 从 PMC 迁移到合作伙伴中心
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 PMC 和合作伙伴中心在续订、帐户结构、登录、用户角色和资格等方面之间的差异。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: a6fc3fbfbc5ebf874460fbf2f0065150089db39d
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436806"
---
# <a name="moving-from-partner-membership-center-pmc-to-partner-center"></a>从 Partner Membership Center (PMC) 迁移到合作伙伴中心

**相应的角色**
-    全局管理员

为了让你能够轻松地与我们开展业务，我们建立了一个网站（合作伙伴中心），方便大家参与。 你会发现，在 Partner Membership Center (PMC) 中做的事情都能够在合作伙伴中心的仪表板中完成。 

你还可以执行更多操作，全都不需离开这个网站即可完成。 不过，部分术语和功能看起来可能有所不同。 为了消除一开始不知道相关内容所在位置和功能的疑虑，请务必在面板中浏览一下网站内容。

下表呈现了 PMC 与合作伙伴中心的一些差异。

## <a name="renewing-your-microsoft-partner-network--membership"></a>续订 Microsoft 合作伙伴网络成员身份

|**PMC**   |**合作伙伴中心**|
|----------------------|:-----------------------------|
|续订在周年日期之前的 90 天开始，必须在周年日期之前完成| 合作伙伴可以从周年日期之后的那一天开始续订，最多可以续订 30 天。|

## <a name="account-structure"></a>帐户结构

|**PMC**   |**合作伙伴中心**|
|----------------------|:-----------------------------|
|总部和位置 - 每一项都单独进行评估。 能力在本地评估|全球性公司、合作伙伴全局帐户 (PGA)，包括位置在内，都进行总体评估；绩效和技能数据在 PGA 级别聚合；包含多个配置文件视图，适用于合作伙伴配置文件和业务配置文件（用于引荐和营销）之类的程序。有关详细信息，请阅读[合作伙伴中心的帐户结构](account-structure.md)。|

## <a name="sign-in"></a>登录

|**PMC**   |**合作伙伴中心**|
|----------------------|:-----------------------------|
|可以使用 Microsoft 帐户 (MSA) 或个人帐户凭据 joe@outlook.com|你必须使用你的工作帐户凭据 (joe@joescompany.com)。 有关详细信息，请阅读[你的公司工作帐户与合作伙伴中心](azure-active-directory-tenants-and-partner-center.md)。|

## <a name="user-roles"></a>用户角色

|**PMC**   |**合作伙伴中心**|
|----------------------|:-----------------------------|
|PMC 中的许多角色不在合作伙伴中心使用|负责迁移到合作伙伴中心的管理员会被系统自动分配 MPN 管理员、帐户管理员和引荐管理员角色。 该管理员随后可以为其他用户分配用户角色。|
|用户在位置级别管理|用户在公司级别 (PGA) 而不是位置级别管理。 奖励计划管理员在位置级别工作，这是一个例外。|
|   |合作伙伴中心有两大组的角色：管理 Azure AD 租户的角色，以及管理公司业务的角色。 请按对公司有利的方式组织角色。 可以让一个人做所有事情，也可以将不同的角色和权限分配给许多人。 有关详细信息，请阅读[为用户分配角色和权限](permissions-overview.md)。 

## <a name="how-competencies-and-benefits-are-accounted-for"></a>能力和权益的具体说明

|**PMC**   |**合作伙伴中心**|
|----------------------|:-----------------------------|
|按位置获得，按位置管理|权益（包括权益管理）在整个公司分配，但是，你可以按最符合公司利益的方式管理这些权益。 |
|可以使用其他权益工具包 (ABTK)，直到其在 2018 年停用为止。|没有 ABTK；一个公司一个 MAPS；一个公司一个银牌能力；一个公司一个金牌能力|
||只要你还没有 MAPS，就可以购买它。 是否拥有 MAPS 与能力不挂钩。  
|在合作伙伴数字下载 (PDD) 位置访问权益 |所有权益都在合作伙伴中心访问|
|能力和权益分布在多个位置|所有位置的能力和权益在公司 (PGA) 级别合并，并保留到周年日期那一天。 到那时候，你需要在公司级别进行购买或续订。 性能和技能以及能力在全局进行聚合|
|软件保障凭证是通过凭证验证和兑换 (VVR) 工具索取的|现在可以在合作伙伴中心访问和管理软件保障培训凭证 (SATV) 和/或已部署规划服务 (DPS)。  旧版 VVR 工具将在 2019 年 10 月 1 日停用。  |

## <a name="associating-mcp-ids-to-partner-center"></a>将 MCP ID 关联到合作伙伴中心

|**PMC**   |**合作伙伴中心**   |
|-------------------------|:-------------------|
|可以将同一 MCP ID 关联到多家公司。| 只能将一个 MCP ID 关联到一个合作伙伴中心帐户。 关联操作必须手动执行。 在合作伙伴中心面板中，选择面板右上角的“我的帐户”图标，然后选择“我的个人资料” 。 在“我的 Learning”下方，可以关联你的 Microsoft Learning 帐户，还可以将你的 Microsoft 帐户连接到 Partner University。

## <a name="visual-studio-benefits-and-msa"></a>Visual Studio 权益和 MSA

|**PMC**   |**合作伙伴中心**   |
|-----------------|:-----------------|
|为 MSA 分配 Visual Studio 权益|分配给 MSA 的 Visual Studio 权益仍将有效，会继续保留。|
||在合作伙伴中心续订后，分配给 MSA 的 Visual Studio 权益会保留。|
||在合作伙伴中心，合作伙伴可以添加特定的工作帐户和来宾用户帐户，这些帐户是同一租户的 MSA，而这些租户中的合作伙伴在 Azure AD 租户中是 MPN 管理员。 如果合作伙伴在多个 Azure AD 租户中是全局管理员，并且所有这些租户都关联到同一个合作伙伴中心帐户，则该合作伙伴可以跨所有这些租户将用户添加到 Visual Studio 权益中以及基于 Azure 使用情况的分配计划中。 虽然来宾用户可以由 MPN 管理员或全局管理员分配基于使用情况的 Visual Studio 订阅，但来宾用户不能使用其 MSA 登录合作伙伴中心。 不过，来宾用户可以登录 Azure 和 Visual Studio，以便验证和使用分配给他们的权益。 |

## <a name="programs-now-located-and-managed-in-partner-center"></a>计划现在位于合作伙伴中心并在其中进行管理 

|**PMC**   |**合作伙伴中心**|
|----------------------|:-----------------------------|
|PDD  |优势|
|CHIP、ICP、PIE | 奖励|
||引荐|
|合作伙伴见解| 分析|
|凭证验证和兑换工具| 凭证验证和兑换工具|
|           |云解决方案提供商计划|

分配给 MSA 的 Visual Studio 权益仍将有效，会继续保留。 在合作伙伴中心续订后，仍会保留它们。 不过，如果你在迁移到合作伙伴中心以后删除了某个 MSA 分配，则不能将它重新添加到合作伙伴中心。

在合作伙伴中心，合作伙伴可以添加特定的工作帐户和来宾用户帐户，这些帐户是同一租户的 MSA，而这些租户中的合作伙伴在 Azure AD 租户中是 MPN 管理员。 如果合作伙伴在多个 Azure AD 租户中是全局管理员，并且所有这些租户都关联到同一个合作伙伴中心帐户，则该合作伙伴可以跨所有这些租户将用户添加到 Visual Studio 权益中以及基于 Azure 使用情况的分配计划中。

虽然来宾用户可以由 MPN 管理员或全局管理员分配基于使用情况的 Visual Studio 订阅，但来宾用户不能使用其 MSA 登录合作伙伴中心。 不过，来宾用户可以登录 Azure 和 Visual Studio，以便验证和使用分配给他们的权益。
