---
title: 用于导入客户帐户的多个用户的 .csv 文件的字段
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要将多个用户添加到客户帐户，请创建一个逗号分隔值 (.csv) 文件，并包含相应的字段。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150975"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="08733-103">通过创建 .csv 文件将多个用户添加到客户帐户</span><span class="sxs-lookup"><span data-stu-id="08733-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="08733-104">**相应的角色**：全局管理员</span><span class="sxs-lookup"><span data-stu-id="08733-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="08733-105">将逗号分隔值文件格式为 (.csv 的数据文件上传到客户帐户) 一次合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="08733-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="08733-106">可以从应用程序下载示例数据文件合作伙伴中心编辑它供你使用，或者可以使用下面定义的数据模型创建新的数据文件。</span><span class="sxs-lookup"><span data-stu-id="08733-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="08733-107">数据文件要求</span><span class="sxs-lookup"><span data-stu-id="08733-107">Data file requirements</span></span>

<span data-ttu-id="08733-108">若要使用批量上传过程将多个用户添加到客户的帐户，需要满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="08733-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="08733-109">必须拥有客户帐户的全局管理员权限；</span><span class="sxs-lookup"><span data-stu-id="08733-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="08733-110">每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；</span><span class="sxs-lookup"><span data-stu-id="08733-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="08733-111">一次最多可上传 100 条记录。</span><span class="sxs-lookup"><span data-stu-id="08733-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="08733-112">如果需要添加超过 100 个用户，请创建并上传其他数据文件。</span><span class="sxs-lookup"><span data-stu-id="08733-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="08733-113">所有用户必须处在相同的地理 **位置**。</span><span class="sxs-lookup"><span data-stu-id="08733-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="08733-114">仅输入以下所述的数据。</span><span class="sxs-lookup"><span data-stu-id="08733-114">Enter only the data described below.</span></span> <span data-ttu-id="08733-115">无关的数据将导致上传失败。</span><span class="sxs-lookup"><span data-stu-id="08733-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="08733-116">在数据文件中输入以下数据：</span><span class="sxs-lookup"><span data-stu-id="08733-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="08733-117">**列名**</span><span class="sxs-lookup"><span data-stu-id="08733-117">**Column name**</span></span> | <span data-ttu-id="08733-118">**说明**</span><span class="sxs-lookup"><span data-stu-id="08733-118">**Description**</span></span>  | <span data-ttu-id="08733-119">**限制**</span><span class="sxs-lookup"><span data-stu-id="08733-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="08733-120">名字</span><span class="sxs-lookup"><span data-stu-id="08733-120">First name</span></span>  | <span data-ttu-id="08733-121">用户的名字 (可选字段) </span><span class="sxs-lookup"><span data-stu-id="08733-121">User's first name (optional field)</span></span>  | <span data-ttu-id="08733-122">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="08733-122">50-character limit</span></span>  |
| <span data-ttu-id="08733-123">姓氏</span><span class="sxs-lookup"><span data-stu-id="08733-123">Last name</span></span>  | <span data-ttu-id="08733-124">用户姓氏（可选字段）</span><span class="sxs-lookup"><span data-stu-id="08733-124">User's last name (optional field)</span></span>  | <span data-ttu-id="08733-125">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="08733-125">50-character limit</span></span>  |
| <span data-ttu-id="08733-126">显示名称</span><span class="sxs-lookup"><span data-stu-id="08733-126">Display name</span></span>    | <span data-ttu-id="08733-127">必填字段合作伙伴中心 (显示的名称) </span><span class="sxs-lookup"><span data-stu-id="08733-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="08733-128">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="08733-128">50-character limit</span></span>                         |
| <span data-ttu-id="08733-129">电子邮件</span><span class="sxs-lookup"><span data-stu-id="08733-129">Email</span></span>   | <span data-ttu-id="08733-130">客户公司用户的业务电子邮件地址 (必填字段) </span><span class="sxs-lookup"><span data-stu-id="08733-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="08733-131">每个用户的电子邮件地址必须唯一</span><span class="sxs-lookup"><span data-stu-id="08733-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="08733-132">状态更新</span><span class="sxs-lookup"><span data-stu-id="08733-132">Status update</span></span>   | <span data-ttu-id="08733-133">用于指示是否已成功创建新用户记录</span><span class="sxs-lookup"><span data-stu-id="08733-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="08733-134">\*\*留空\*\*</span><span class="sxs-lookup"><span data-stu-id="08733-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="08733-135">后续步骤</span><span class="sxs-lookup"><span data-stu-id="08733-135">Next steps</span></span>

- [<span data-ttu-id="08733-136">如何为客户添加多个用户</span><span class="sxs-lookup"><span data-stu-id="08733-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)