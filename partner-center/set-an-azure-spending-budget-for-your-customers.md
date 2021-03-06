---
title: 为客户设置 Azure 支出预算
ms.topic: how-to
ms.date: 03/17/2021
description: 了解如何为客户设置或删除每月 Azure 支出预算，同时查看 Azure 支出数据并设置与预算相关的通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855346"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>为合作伙伴中心的客户设置、检查或删除每月 Azure 支出预算

**适当的角色**：管理代理

可以在合作伙伴中心 [为客户设置每月 Azure 支出预算](#set-azure-spending-budget) 。 这可以帮助客户管理其 Azure 支出。 此选项可让你将客户的 Azure 支出与当月的预算进行比较。 它还可帮助你的客户为其 Azure 支出预算，使每月帐单不会超过预期。

> [!NOTE]  
> 此功能在生产 (TIP) 帐户中不提供沙盒或测试。

[为客户 () 设置 Azure 支出预算](#set-azure-spending-budget)后，还可以通过以下方式查看客户使用情况。 这些选项可帮助你找出配置错误的服务或可能会导致欺诈的异常趋势。 然后，你可以与客户 () ，以确定根本原因并管理成本。 如果需要，还可以 [将客户的预算更改](#set-azure-spending-budget) 为较高的金额。

- [检查当前 Azure 支出](#check-current-azure-spending)

- [当客户的支出接近预算限制时，打开电子邮件通知](#notifications-for-budget-limits)

- [查看基于使用情况的订阅的按服务列出的费用](#itemized-costs-by-service)

你还可以随时删除客户 () 的 [Azure 支出预算](#remove-azure-spending-budget) 。

## <a name="azure-spending-data"></a>Azure 支出数据

Azure 支出数据是一个 *估计值* ， *实际计费金额可能会有所不同*。 此数据的值 *不会反映* 税金、信用额度、调整或可能适用的其他费用。

支出数据 *每天刷新一次*。 你的客户可以继续使用 (，并向) Azure 服务和资源收费，除非你在 Azure 门户中更改其帐户设置。

## <a name="set-azure-spending-budget"></a>设置 Azure 支出预算

可以为合作伙伴中心内的多个客户 *设置每月 Azure 支出预算* ：

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。

2. 在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。

3. 在 " **Azure 支出** " 页的 " **具有 Microsoft Azure 订阅的客户**" 下，选择要为其设置预算的客户 () 。

4. 为 " **月度预算**" 输入一个值。

5. 选择 " **应用** " 保存更改。

你还可以在其订阅设置中 *设置单个客户的预算* ：

1. 登录到合作伙伴中心面板。

2. 在 **CSP** 下的左侧菜单中，选择 " **客户**"。

3. 在 " **客户** " 页上，选择客户的 **公司名称**。

4. 在客户的 " **订阅** " 页的 " **基于使用情况的订阅**" 下，选择 " **更改预算**"。

5. 输入预算的值。

6. 选择 " **应用** " 保存更改。

## <a name="remove-azure-spending-budget"></a>删除 Azure 支出预算

可以在合作伙伴中心为客户 () *删除每月 Azure 支出预算* ：

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。

2. 在 " **CSP**" 下的左侧菜单中，选择 " **Azure 支出**"。

3. 在 " **Azure 支出** " 页的 " **具有 Microsoft Azure 订阅的客户**" 下，选择要删除其预算的客户 () 。

4. 选择 " **删除预算**"。

## <a name="check-current-azure-spending"></a>检查当前 Azure 支出

你可以随时 *跟踪客户的当前 Azure 支出和月度预算* ：

1. 登录到[合作伙伴中心面板](https://partner.microsoft.com/dashboard/)。

2. 在 CSP 下的左侧菜单中 **，选择****"Azure 支出"。**

3. 在 **"Azure 支出** " **页上** 的"Microsoft Azure订阅"下，可以看到客户每月预算、当前支出估算和已使用预算百分比的概述。

## <a name="notifications-for-budget-limits"></a>预算限制通知

当 *客户的每月支出接近其* 预算限制时，可以启用电子邮件通知。 启用此选项时，当客户使用其每月预算 80% 或更多时，你将收到通知。 此选项可帮助你关注 Azure 帐单。 配置电子邮件通知：

1. 登录到合作伙伴中心。

2. 转到“设置”  。

3. 选择 **"我的首选项"。**

4. 配置首选电子邮件地址（如果尚未配置）。

5. 配置通知的首选语言。

6. 选择 **"通知** 首选项 **"部分下的"CSP"** 选项卡。

7. 选中"Azure 支出通知"的"**电子邮件**"选项，并"**保存"。**


## <a name="itemized-costs-by-service"></a>按服务分项成本

可以查看 *基于使用情况的订阅 (按服务) 和估计的使用情况*：

1. 登录到合作伙伴中心。

2. 在 CSP 下的左侧菜单中 **，选择"** 客户 **"。**

3. 在" **客户** "页上，选择客户的公司 **名称**。

4. 在客户的"订阅 **"** 页上的"基于 **使用情况的订阅"下**，选择"订阅 **"的名称**。

5. 在订阅的页面上，你可以查看按服务分项成本，以及 **当前月份的估计** 使用量。


## <a name="next-steps"></a>后续步骤

- [CSP 中的新商务体验 - Azure 计费](azure-plan-billing.md)
