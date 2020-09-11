---
title: 注册云解决方案提供商计划
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解需要为美国政府注册云解决方案提供商 Microsoft 云计划的合作伙伴的 CSP 计划要求。
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.date: 06/30/2020
ms.openlocfilehash: 12ddd290f22fc672ca2fb0c911567ca7419d88b0
ms.sourcegitcommit: d3ff69f285a872fd0a214cc14ac3a6cf9cd124b3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2020
ms.locfileid: "90026275"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>注册美国政府 Microsoft 云的云解决方案提供商计划

**适用于**

- Microsoft Cloud for US Government 合作伙伴中心

**相应的角色**

- 全局管理员

现在，通过美国政府 Microsoft 云的云解决方案提供商计划 (CSP)，Microsoft 合作伙伴可向美国联邦、州、本地和族群实体销售 Microsoft 的云解决方案和服务。

美国政府 Microsoft 云提供了 Microsoft Azure 的私有、专用和单独实例，符合美国政府的数据安全、隐私和合规性方面的要求。 贵公司必须满足 Microsoft 的有关加入美国政府 Microsoft 云的 CSP 计划的资格要求。 有关详细信息，请参阅[美国政府 Microsoft 云合作伙伴中心](partner-center-for-microsoft-us-govt-cloud.md)。

## <a name="before-you-begin"></a>准备阶段

在你可以注册加入美国政府 Microsoft 云的 CSP 计划之前，我们需要验证贵公司是否满足向美国政府实体进行销售的要求。 开始注册过程之前，请填写 [Microsoft 政府云验证表单](https://azuregov.microsoft.com/csp)，以便我们验证贵公司的资格。 在验证了贵公司的资格后，我们将向你提供特定于美国政府 Microsoft 云的 Azure Active Directory (Azure AD) 租户。  

要创建合作伙伴中心帐户并注册美国政府 Microsoft 云的云解决方案提供商计划，你需要提供以下信息（你可能要在开始注册前收集此信息）：

- 贵组织的美国政府 Microsoft 云的新 Azure AD 租户的全局管理员凭据
- 贵组织的 Microsoft 合作伙伴网络 (MPN) ID
- 在美国的公司地址

> [!IMPORTANT]  
> 如果你在合作伙伴中心内已有帐户，并且要注册加入美国政府 Microsoft 云的 CSP，则必须专为美国政府市场单独创建新的帐户。

## <a name="how-to-enroll"></a>如何注册

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>第 1 步 - 为美国政府 Microsoft 云创建合作伙伴中心帐户

1. 在[此处](https://partnercenter.microsoft.com/register/resellerusgjoinnow)开始执行注册过程。

2. 使用贵组织的美国政府 Microsoft 云的 Azure AD 租户的全局管理员凭据进行登录。 如果贵组织没有此门户的帐户，则可以通过填写 [Microsoft 政府云验证表单](https://azuregov.microsoft.com/csp)申请一个帐户。

### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>第 2 步 - 申请加入美国政府 Microsoft 云的云解决方案提供商计划

1. 在注册表单中填写所有缺少的信息，包括你的 Microsoft 合作伙伴网络 ID 和你组织的客户支持详细信息。

2. 选择**接受并继续操作**。 我们审查你的申请可能需要几天时间。 完成审查后，我们将通过电子邮件通知你。

   > [!IMPORTANT]
   > 通过选择**接受并继续操作**，即表示你确认你已获得授权代表你的组织，且你同意允许 Microsoft 在审查你组织的云解决方案提供商申请前执行背景信用检查。

### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>第 3 步 - 签署美国政府 Microsoft 云经销商协议

1. 使用申请批准电子邮件中提供的链接登录到美国政府 Microsoft 云合作伙伴中心。

2. 在**协议**页上，阅读相关条款，如果你同意，请选择**接受并继续操作**，以数字方式签署[美国政府 Microsoft 云经销商协议](https://go.microsoft.com/fwlink/p/?linkid=843364)。 创建你的帐户可能需要几个小时。 从美国政府 Microsoft 云合作伙伴中心注销，稍后重新登录。

### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>第 4 步 - 将用户分配给 Microsoft Azure 美国政府 Microsoft 云管理门户中的管理员代理角色

美国政府 Microsoft 云提供一个满足政府合规、安全性和隐私标准的单独的 Microsoft Azure 实例。 若要允许管理员管理 Microsoft Azure 门户中的用户和许可证，你将需要手动将管理员代理角色分配给他们。

> [!NOTE]
> 将用户分配至“管理员代理”角色后，他们将能够访问**客户**页面上的客户列表，并[添加新客户](add-a-new-customer.md)。

1. 登录到 Microsoft Azure 管理门户，网址为 [https://portal.azure.us/](https://portal.azure.us/) 。

2. 将管理员代理角色分配给你组织中的适当用户。 若要执行此操作，你需要将这些用户添加到内置 **AdminAgent** 组。 请参阅[管理 Azure Active Directory 中的一组成员](https://docs.microsoft.com/azure/active-directory/active-directory-groups-members-azure-portal)，了解有关如何执行此操作的信息。

## <a name="connect-with-us"></a>与我们联系

- 是否有任何问题? 请发送电子邮件到 azgovcsp@microsoft.com 与我们联系

- 在 [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777) 上加入我们

## <a name="next-steps"></a>后续步骤

- [Microsoft Cloud for US Government 合作伙伴中心](partner-center-for-microsoft-us-govt-cloud.md)

- [Microsoft Cloud for US Government 合作伙伴中心中的用户和许可证管理](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)
