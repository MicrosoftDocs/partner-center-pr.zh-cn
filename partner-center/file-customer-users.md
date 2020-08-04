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
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="06f94-103">通过创建一个 .csv 文件，将多个用户添加到客户帐户</span><span class="sxs-lookup"><span data-stu-id="06f94-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="06f94-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="06f94-104">**Applies to**</span></span>

- <span data-ttu-id="06f94-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="06f94-105">Partner Center</span></span>

<span data-ttu-id="06f94-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="06f94-106">**Appropriate roles**</span></span>

- <span data-ttu-id="06f94-107">全局管理员</span><span class="sxs-lookup"><span data-stu-id="06f94-107">Global admin</span></span>

<span data-ttu-id="06f94-108">通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，将多个用户一次性添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="06f94-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="06f94-109">你可以从 "合作伙伴中心" 下载一个示例数据文件，然后编辑该文件以供使用，或者可以使用下面定义的数据模型创建新的数据文件。</span><span class="sxs-lookup"><span data-stu-id="06f94-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="06f94-110">数据文件要求</span><span class="sxs-lookup"><span data-stu-id="06f94-110">Data file requirements</span></span>

<span data-ttu-id="06f94-111">若要使用批量上传过程将多个用户添加到客户的帐户，需要满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="06f94-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="06f94-112">必须拥有客户帐户的全局管理员权限；</span><span class="sxs-lookup"><span data-stu-id="06f94-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="06f94-113">每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；</span><span class="sxs-lookup"><span data-stu-id="06f94-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="06f94-114">一次最多可上传 100 条记录。</span><span class="sxs-lookup"><span data-stu-id="06f94-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="06f94-115">如果需要添加超过 100 个用户，请创建并上传其他数据文件。</span><span class="sxs-lookup"><span data-stu-id="06f94-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="06f94-116">所有用户必须处在相同的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="06f94-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="06f94-117">仅输入以下所述的数据。</span><span class="sxs-lookup"><span data-stu-id="06f94-117">Enter only the data described below.</span></span> <span data-ttu-id="06f94-118">无关的数据将导致上传失败。</span><span class="sxs-lookup"><span data-stu-id="06f94-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="06f94-119">在数据文件中输入以下数据：</span><span class="sxs-lookup"><span data-stu-id="06f94-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="06f94-120">**列名**</span><span class="sxs-lookup"><span data-stu-id="06f94-120">**Column name**</span></span> | <span data-ttu-id="06f94-121">**说明**</span><span class="sxs-lookup"><span data-stu-id="06f94-121">**Description**</span></span>  | <span data-ttu-id="06f94-122">**限制**</span><span class="sxs-lookup"><span data-stu-id="06f94-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="06f94-123">名字</span><span class="sxs-lookup"><span data-stu-id="06f94-123">First name</span></span>  | <span data-ttu-id="06f94-124">用户的名字（可选字段）</span><span class="sxs-lookup"><span data-stu-id="06f94-124">User's first name (optional field)</span></span>  | <span data-ttu-id="06f94-125">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="06f94-125">50-character limit</span></span>  |
| <span data-ttu-id="06f94-126">姓氏</span><span class="sxs-lookup"><span data-stu-id="06f94-126">Last name</span></span>  | <span data-ttu-id="06f94-127">用户姓氏（可选字段）</span><span class="sxs-lookup"><span data-stu-id="06f94-127">User's last name (optional field)</span></span>  | <span data-ttu-id="06f94-128">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="06f94-128">50-character limit</span></span>  |
| <span data-ttu-id="06f94-129">显示名称</span><span class="sxs-lookup"><span data-stu-id="06f94-129">Display name</span></span>    | <span data-ttu-id="06f94-130">"合作伙伴中心" 中显示的名称（必填字段）</span><span class="sxs-lookup"><span data-stu-id="06f94-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="06f94-131">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="06f94-131">50-character limit</span></span>                         |
| <span data-ttu-id="06f94-132">电子邮件</span><span class="sxs-lookup"><span data-stu-id="06f94-132">Email</span></span>   | <span data-ttu-id="06f94-133">客户公司的用户业务电子邮件地址（必填字段）</span><span class="sxs-lookup"><span data-stu-id="06f94-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="06f94-134">每个用户的电子邮件地址必须唯一</span><span class="sxs-lookup"><span data-stu-id="06f94-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="06f94-135">状态更新</span><span class="sxs-lookup"><span data-stu-id="06f94-135">Status update</span></span>   | <span data-ttu-id="06f94-136">用于指示是否成功创建了新用户记录</span><span class="sxs-lookup"><span data-stu-id="06f94-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="06f94-137">\*\*留空\*\*</span><span class="sxs-lookup"><span data-stu-id="06f94-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="06f94-138">后续步骤</span><span class="sxs-lookup"><span data-stu-id="06f94-138">Next steps</span></span>

- [<span data-ttu-id="06f94-139">如何为客户添加多个用户</span><span class="sxs-lookup"><span data-stu-id="06f94-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)