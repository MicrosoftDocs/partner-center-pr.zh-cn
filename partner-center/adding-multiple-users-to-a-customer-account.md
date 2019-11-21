---
title: 为客户帐户创建多个用户 | 合作伙伴中心
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to Partner Center.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: 批量上传, 将多个用户添加到客户帐户, 添加客户的用户, 批量上传客户的用户, 客户帐户, 客户用户, 用户
ms.localizationpriority: medium
ms.openlocfilehash: 5c9de7ed78a0494790b447d1755d5eef70a89cca
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253182"
---
# <a name="add-multiple-users-to-a-customer-account"></a>将多个用户添加到客户帐户

**适用于**

-  合作伙伴中心

You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center. You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.

## <a href="" id="creatingtheimportcsvfile"></a>Data file requirements


To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:

-   必须拥有客户帐户的全局管理员权限；
-   每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；
-   一次最多可上传 100 条记录。 如果需要添加超过 100 个用户，请创建并上传其他数据文件。
-   所有用户必须处在相同的地理**位置**。
-   仅输入以下所述的数据。 无关的数据将导致上传失败。

在数据文件中输入以下数据：

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Column name** | **描述**                                                              | **Limitation**                             |
| 名字      | User's first name (optional field)                                           | 限 50 个字符                         |
| 姓氏       | 用户姓氏（可选字段）                                            | 限 50 个字符                         |
| 显示名称    | Name displayed in the Partner Center (required field)                            | 限 50 个字符                         |
| “电子邮件”           | User's business email address at customer company (required field)           | 每个用户必须拥有唯一的电子邮件地址 |
| 状态更新   | 用于指示是否成功创建了新用户记录 | \*\*Leave empty\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>To create multiple user accounts

<a href="" id="creatingtheaccounts"></a>
1.  使用上述数据创建逗号分隔值 (.csv) 数据文件。 保存文件，以供在后续步骤中浏览。
2.  From the **Partner Center** menu, select **Customers**, then choose a customer from the list.
3.  选择**上传用户**。
4.  在**上传用户信息**下，选择**浏览**。
5.  在文件选择器中，选择数据文件，然后选择**打开**。
6.  选择**验证**。

    **Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.

7.  After the Partner Center validates the file, select the geographic **Location** for the new users.
8.  选择**保存**。
9.  下载用户的临时密码信息。

**重要提示：** 确保现在就下载具有临时密码的文件，在后续步骤中将无法下载。 新用户必须使用新帐户的临时密码登录新帐户。

10. 系统会将**可使用许可证和服务**的权限自动分配给新用户。 

 

 



