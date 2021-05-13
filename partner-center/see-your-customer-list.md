---
title: 管理客户列表
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 客户记录是最重要的信息资产之一。 了解如何查看、搜索、更新&客户列表上的合作伙伴中心信息。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854496"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>管理客户列表 - 在客户列表中搜索、更新或导出合作伙伴中心

**适用于 ：** 合作伙伴中心 |合作伙伴中心Microsoft Cloud for US Government

**适当的角色**：管理员代理|全局管理员

客户记录是合作伙伴中心中最重要的信息资源。 可搜索客户帐户的数据库，将整个客户数据库或子集导出为 Excel 兼容的逗号分隔值文件格式 (.csv)。 还可将客户订阅信息导出为 .csv 文件。

活动日志也为客户提供有关交易和管理操作的可导出数据。 有关详细信息，请参阅[查看客户活动日志](activity-logs.md)。

## <a name="search-for-a-customer"></a>搜索客户

1. 从 **"合作伙伴中心** 菜单中，选择"客户 **"。**
2. 若要搜索某个客户，请在搜索框中输入客户名称或域名。
3. 选择 **客户行** 末尾的向下箭头，查看其 Microsoft ID 及其关联的订阅和服务快速链接。

## <a name="update-a-customers-company-name"></a>更新客户的公司名称

从 **"合作伙伴中心** 菜单中，选择"客户 **"。**
2. 若要搜索某个客户，请在搜索框中输入客户名称或域名。
3. 选择 **客户行** 末尾的向下箭头，查看其 Microsoft ID 及其关联的订阅和服务快速链接。
4. 在客户的 **帐单邮寄地址** 信息下面，更新公司名称。 当你保存新值后，它将会反映在客户列表中。 此操作只会更改帐单邮寄地址中的公司名称和客户列表值。 其他位置均不会反映此项更改。

## <a name="export-your-customer-list"></a>导出客户列表

1. 从 **"合作伙伴中心** 菜单中，选择"客户 **"。**
2. 选择"**导出客户"。**

   合作伙伴中心将完整的客户列表转换为 .csv 文件，并将其上传到计算机上的默认下载文件夹。 还可导出客户数据的子集。 数据列包含以下内容：

   - **Microsoft ID**;
   - **公司名称**;
   - **主域名**;
   - **关系** - 合作伙伴与每个列出的客户的业务关系。

    默认情况下，合作伙伴中心将导出整个客户列表，无需考虑长度。 还可按公司名称或域来搜索客户列表，并导出数据子集。

3. 如果是间接提供商，可按间接经销商筛选客户列表。 选择列表中的 **按间接经销商筛选**，然后选择经销商。


## <a name="export-customer-subscription-information"></a>导出客户订阅信息

1. 从 **"合作伙伴中心** 菜单中，选择"客户 **"。**

2. 选择 **任何客户的** 公司名称。 将打开 **客户的"订阅** "页，其中显示了其完整的产品订阅列表。

3. 选择 **"导出订阅"。** 合作伙伴中心在计算机上将客户订阅数据转换为 .csv 文件，并将其上传到默认下载文件夹。 数据列包含以下内容：
   - **订阅 ID;**
   - **订阅** - 订阅的产品名称；
   - **数量** - 购买的许可证数；
   - **状态**;
   - **经销商** - 拥有并管理订阅的经销商的 ID。

> [!NOTE]  
> 有关订阅管理的详细信息，请参阅[客户订阅](customer-subscriptions.md)。
