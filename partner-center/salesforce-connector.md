---
title: Salesforce CRM 合作伙伴中心的共同销售连接器
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Salesforce CRM 连接器，从 Microsoft 获取推荐
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825694"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM 的共同销售连接器-概述

### <a name="appropriate-roles"></a>相应的角色

- 引荐管理员
- CRM 上的系统管理员或系统定制员

合作伙伴中心共同销售连接器可让你的卖方与 Microsoft 在 CRM 系统中共同销售。 他们无需定型即可使用合作伙伴中心来管理共同销售交易。 使用共同销售连接器，你将能够创建新的共同销售引用来与 Microsoft 卖方联系，从 Microsoft 卖方接收引用、接受/拒绝引用、修改交易数据（如交易价值、结算日期等），以及从 Microsoft 卖方接收有关这些共同销售交易的任何更新。 您可以在所选的 CRM 内而不是在合作伙伴中心内完成所有这些工作。 

此解决方案基于 Microsoft Power 自动化解决方案，并使用 Microsoft 合作伙伴中心 Api。


## <a name="before-you-install---pre-requisites"></a>安装之前-必备组件

|**主题**   |**详细信息**   |**链接**   |
|--------------|--------------------|------|
|Microsoft 合作伙伴网络 ID |需要一个有效的 MPN ID|加入[MPN](https://partner.microsoft.com/)|
|合作销售就绪|你的 IP/服务解决方案必须共同销售。|[与 Microsoft 一起销售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作伙伴中心帐户|与合作伙伴中心租户关联的 MPN ID 必须与共同销售解决方案关联的 MPN ID 相同。 在部署连接器之前，请确认你可以在合作伙伴中心门户中看到共同销售的引用。|[管理帐户](create-user-accounts-and-set-permissions.md)|
|合作伙伴中心用户角色|将安装和使用连接器的员工必须是推荐管理员|[为用户分配角色和权限](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 用户角色是系统管理员或系统定制员|[在 Dynamics 365 中分配角色](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power 自动化 Flow 帐户|CRM 系统管理员或系统定制员的有效[电源自动完成](https://flow.microsoft.com)帐户。 在安装之前，该用户至少应登录到一次[电源](https://flow.microsoft.com)。|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>为 Salesforce CRM 安装合作伙伴中心引用同步

1. 请继续[执行 "电源自动](https://flow.microsoft.com)"，并选择右上角的 "**环境**"。 这会显示可用的 CRM 实例。

2. 从右上角的下拉菜单中选择相应的 CRM 实例。 

3. 选择左侧导航栏上的 "**解决方案**"。

4. 单击顶部菜单上的 "**打开 AppSource** " 链接。

![打开 AppSource](images/cosellconnectors/openappsource.png)

5. 在弹出屏幕中搜索 Salesforce 的 "**合作伙伴中心引用连接器**"。  

6. 单击 "**立即获取**" 按钮，然后**继续**。 

7. 这将打开一个页面，可以在其中选择要安装应用程序的 CRM （Dynamics 365）环境。  同意条款和条件。 

8. 然后，你将转到 "**管理你的解决方案**" 页。  通过使用页面底部的箭头按钮，导航到 "合作伙伴中心引用"。 **计划的安装**应显示在合作伙伴中心引用解决方案旁边。 安装将需要10-15 分钟。 

9. 安装完成后，导航回 "[自动启动](https://flow.microsoft.com)"，并从左侧导航区域中选择 "**解决方案**"。 请注意，"解决方案" 列表中提供了**Salesforce 的合作伙伴中心引用同步**。

10. 选择**Dynamics 365 的伙伴中心引用同步**。 可以使用以下功能自动执行流和实体：

![可用 CRM](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在上线之前进行测试

在生产环境中安装、配置和自定义电源自动解决方案之前，请确保在过渡 CRM 实例上测试解决方案。

- 在过渡环境/CRM 实例上安装 Microsoft Power 自动解决方案解决方案。
- 制作解决方案的副本，并在过渡环境中执行配置和自动自动流自定义功能。
- 在过渡/CRM 实例上测试解决方案。 
- 成功后，将作为托管解决方案导入到生产实例。 

## <a name="configure-the-solution"></a>配置解决方案

1. 在 CRM 实例中安装解决方案后，请导航回 "[电源自动](https://flow.microsoft.com/)"。

2. 在右上角的 "**环境**" 下拉位置，选择安装了 Power 自动解决方案的 CRM 实例。

3. 你将需要创建关联三个用户帐户的连接： 

- 具有引用管理员凭据的合作伙伴中心用户 
- 合作伙伴中心事件
- CRM 管理员，并在解决方案中自动执行流处理。 

    a. 从左侧导航栏中选择 "**连接**"，然后从列表中选择 "合作伙伴中心引用" 解决方案。
    b. 通过单击 "**创建连接**" 创建连接。 

    ![创建连接](images/cosellconnectors/createconnection.png)

    c. 在右上角的搜索栏中搜索 "**合作伙伴中心引用（预览版）** "。
    d. 使用 "引用管理员" 凭据角色为合作伙伴中心用户创建连接。电邮. 接下来，使用 "引用管理员" 的凭据为合作伙伴中心用户创建合作伙伴中心事件连接。果. 为 CRM 管理员用户 Common Data Service （当前环境）创建连接。

4. 若要将电源自动流与连接进行关联，请编辑每个电源自动流，以连接到 Common Data Service 和合作伙伴中心引用。 保存更改。

5. **打开**"自动执行流" 功能。

## <a name="next-steps"></a>后续步骤

- [使用 Webhook 获取资源更改事件](referral-connector-webhooks.md)

- [有关 Microsoft Power 自动化平台的详细信息？](https://docs.microsoft.com/power-automate/)

- [管理潜在客户](manage-leads.md)

- [管理联合销售机会](manage-co-sell-opportunities.md)
