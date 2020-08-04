---
title: 为客户帐户添加多个用户
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要将多个用户添加到客户帐户，请使用逗号分隔值（.csv）文件格式将数据文件上传到合作伙伴中心。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535737"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>将用户的 .csv 文件上传到客户的帐户


**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员

通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，将多个用户一次性添加到客户的帐户。 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>创建客户用户的文件并上传到客户帐户

1. 使用上述数据创建逗号分隔值 (.csv) 数据文件。 保存文件，以供在后续步骤中浏览。 请参阅用于[.csv 文件的字段以导入客户帐户的多个用户](file-customer-users.md)。 

2. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

3. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。

4. 选择客户的 "**用户和许可证**" 选项卡，然后选择 "**上载用户**"。

5. 在 "**上载用户信息**" 下，选择 "**浏览**"。

6. 在文件选择器中，选择数据文件，然后选择 "**打开**"。

7. 选择“验证”。

    **注意**   大多数帐户创建错误都是由数据文件问题引起的，其中包括缺少的信息、格式不正确或重复的电子邮件地址，或者文件中的记录过多。

8. 合作伙伴中心验证该文件后，选择新用户的地理**位置**。
9. 选择“保存” 。
10. 下载用户的临时密码信息。

    >[!IMPORTANT]
    > 现在，请确保下载带有临时密码的文件，因为以后无法执行此操作。 新用户必须使用新帐户的临时密码登录新帐户。

11. 系统会将**可使用许可证和服务**的权限自动分配给新用户。 

## <a name="next-steps"></a>后续步骤

- [向客户授予合作伙伴中心的权限，以购买自己的产品或服务](give-customers-permission.md)
