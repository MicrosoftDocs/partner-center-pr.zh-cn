---
title: 用于为客户帐户导入多个用户的 .csv 文件的字段
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要将多个用户添加到客户帐户，请创建包含相应字段的逗号分隔值（.csv）文件。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528175"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>通过创建一个 .csv 文件，将多个用户添加到客户帐户

**适用于**

- 合作伙伴中心

**相应的角色**

- 全局管理员

通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，将多个用户一次性添加到客户的帐户。 你可以从 "合作伙伴中心" 下载一个示例数据文件，然后编辑该文件以供使用，或者可以使用下面定义的数据模型创建新的数据文件。

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

## <a name="next-steps"></a>后续步骤

- [如何为客户添加多个用户](adding-multiple-users-to-a-customer-account.md)