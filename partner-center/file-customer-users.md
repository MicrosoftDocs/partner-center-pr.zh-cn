---
title: 用于为客户帐户导入多个用户的 .csv 文件的字段
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要将多个用户添加到客户帐户，请使用相应的字段创建 ( .csv) 文件的逗号分隔值。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441415"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="23365-103">通过创建一个 .csv 文件，将多个用户添加到客户帐户</span><span class="sxs-lookup"><span data-stu-id="23365-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="23365-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="23365-104">**Appropriate roles**</span></span>

- <span data-ttu-id="23365-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="23365-105">Global admin</span></span>

<span data-ttu-id="23365-106">通过以逗号分隔的值文件)  ( 格式将数据文件上传到合作伙伴中心，将多个用户一次性添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="23365-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="23365-107">你可以从 "合作伙伴中心" 下载一个示例数据文件，然后编辑该文件以供使用，或者可以使用下面定义的数据模型创建新的数据文件。</span><span class="sxs-lookup"><span data-stu-id="23365-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="23365-108">数据文件要求</span><span class="sxs-lookup"><span data-stu-id="23365-108">Data file requirements</span></span>

<span data-ttu-id="23365-109">若要使用批量上传过程将多个用户添加到客户的帐户，需要满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="23365-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="23365-110">必须拥有客户帐户的全局管理员权限；</span><span class="sxs-lookup"><span data-stu-id="23365-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="23365-111">每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；</span><span class="sxs-lookup"><span data-stu-id="23365-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="23365-112">一次最多可上传 100 条记录。</span><span class="sxs-lookup"><span data-stu-id="23365-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="23365-113">如果需要添加超过 100 个用户，请创建并上传其他数据文件。</span><span class="sxs-lookup"><span data-stu-id="23365-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="23365-114">所有用户必须处在相同的地理 **位置**。</span><span class="sxs-lookup"><span data-stu-id="23365-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="23365-115">仅输入以下所述的数据。</span><span class="sxs-lookup"><span data-stu-id="23365-115">Enter only the data described below.</span></span> <span data-ttu-id="23365-116">无关的数据将导致上传失败。</span><span class="sxs-lookup"><span data-stu-id="23365-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="23365-117">在数据文件中输入以下数据：</span><span class="sxs-lookup"><span data-stu-id="23365-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="23365-118">**列名**</span><span class="sxs-lookup"><span data-stu-id="23365-118">**Column name**</span></span> | <span data-ttu-id="23365-119">**说明**</span><span class="sxs-lookup"><span data-stu-id="23365-119">**Description**</span></span>  | <span data-ttu-id="23365-120">**限制**</span><span class="sxs-lookup"><span data-stu-id="23365-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="23365-121">名字</span><span class="sxs-lookup"><span data-stu-id="23365-121">First name</span></span>  | <span data-ttu-id="23365-122">用户的名字 (可选字段) </span><span class="sxs-lookup"><span data-stu-id="23365-122">User's first name (optional field)</span></span>  | <span data-ttu-id="23365-123">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="23365-123">50-character limit</span></span>  |
| <span data-ttu-id="23365-124">姓氏</span><span class="sxs-lookup"><span data-stu-id="23365-124">Last name</span></span>  | <span data-ttu-id="23365-125">用户姓氏（可选字段）</span><span class="sxs-lookup"><span data-stu-id="23365-125">User's last name (optional field)</span></span>  | <span data-ttu-id="23365-126">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="23365-126">50-character limit</span></span>  |
| <span data-ttu-id="23365-127">显示名称</span><span class="sxs-lookup"><span data-stu-id="23365-127">Display name</span></span>    | <span data-ttu-id="23365-128">在 "合作伙伴中心" (必填字段中显示的名称) </span><span class="sxs-lookup"><span data-stu-id="23365-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="23365-129">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="23365-129">50-character limit</span></span>                         |
| <span data-ttu-id="23365-130">电子邮件</span><span class="sxs-lookup"><span data-stu-id="23365-130">Email</span></span>   | <span data-ttu-id="23365-131">客户公司的用户业务电子邮件地址 (必填字段) </span><span class="sxs-lookup"><span data-stu-id="23365-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="23365-132">每个用户的电子邮件地址必须唯一</span><span class="sxs-lookup"><span data-stu-id="23365-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="23365-133">状态更新</span><span class="sxs-lookup"><span data-stu-id="23365-133">Status update</span></span>   | <span data-ttu-id="23365-134">用于指示是否已成功创建新用户记录</span><span class="sxs-lookup"><span data-stu-id="23365-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="23365-135">\*\*留空\*\*</span><span class="sxs-lookup"><span data-stu-id="23365-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="23365-136">后续步骤</span><span class="sxs-lookup"><span data-stu-id="23365-136">Next steps</span></span>

- [<span data-ttu-id="23365-137">如何为客户添加多个用户</span><span class="sxs-lookup"><span data-stu-id="23365-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)