---
title: 为客户帐户添加多个用户
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何一次将多个用户添加到客户的帐户。 使用逗号分隔值（.csv）文件格式将数据文件上传到合作伙伴中心。
author: LauraBrenner
ms.author: labrenne
keywords: 批量上传, 将多个用户添加到客户帐户, 添加客户的用户, 批量上传客户的用户, 客户帐户, 客户用户, 用户
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44e8da91a622fe640e9e41f8d8d464a61652ef30
ms.sourcegitcommit: f71963d6a7ced48ea73580fa57f559ae69f31940
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2020
ms.locfileid: "85104118"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a>向客户帐户添加多个用户-将数据文件上传到合作伙伴中心

**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员

可以通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，一次性将多个用户添加到客户的帐户。 你可以从 "合作伙伴中心" 下载一个示例数据文件，然后编辑该文件以供使用，或者可以使用下面定义的数据模型创建新的数据文件。

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>数据文件要求

若要使用批量上传过程将多个用户添加到客户的帐户，需要满足以下要求：

- 必须拥有客户帐户的全局管理员权限；
- 每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；
- 一次最多可上传 100 条记录。 如果需要添加超过 100 个用户，请创建并上传其他数据文件。
- 所有用户必须处在相同的地理**位置**。
- 仅输入以下所述的数据。 无关的数据将导致上传失败。

在数据文件中输入以下数据：

| **列名** | **说明**  | **限制**  |
|:-------- |:------  |:----- |
| 名字  | 用户的名字（可选字段）  | 50 个字符的限制  |
| 姓氏  | 用户姓氏（可选字段）  | 50 个字符的限制  |
| 显示名称    | "合作伙伴中心" 中显示的名称（必填字段）                            | 50 个字符的限制                         |
| 电子邮件   | 客户公司的用户业务电子邮件地址（必填字段）           | 每个用户的电子邮件地址必须唯一 |
| 状态更新   | 用于指示是否成功创建了新用户记录 | \*\*留空\*\*                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a>创建多个用户帐户

<a href="" id="creatingtheaccounts"></a>

1. 使用上述数据创建逗号分隔值 (.csv) 数据文件。 保存文件，以供在后续步骤中浏览。

2. 登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。

3. 在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。 

4. 选择客户的 "**用户和许可证**" 选项卡，然后选择 "**上载用户**"。

5. 在 "**上载用户信息**" 下，选择 "**浏览**"。

6. 在文件选择器中，选择数据文件，然后选择 "**打开**"。

7. 选择“验证”。

    **注意**   大多数帐户创建错误都是由数据文件问题引起的，其中包括缺少的信息、格式不正确或重复的电子邮件地址，或者文件中的记录过多。

8. 合作伙伴中心验证该文件后，选择新用户的地理**位置**。
9. 选择“保存”。
10. 下载用户的临时密码信息。

**重要提示：** 确保现在就下载具有临时密码的文件，在后续步骤中将无法下载。 新用户必须使用新帐户的临时密码登录新帐户。

10. 系统会将**可使用许可证和服务**的权限自动分配给新用户。 

 

 



