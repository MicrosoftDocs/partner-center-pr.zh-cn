---
title: 为客户帐户添加多个用户
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何一次将多个用户添加到客户的帐户。 使用逗号分隔值（.csv）文件格式将数据文件上传到合作伙伴中心。
author: LauraBrenner
ms.author: labrenne
keywords: 批量上传, 将多个用户添加到客户帐户, 添加客户的用户, 批量上传客户的用户, 客户帐户, 客户用户, 用户
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 09bb83b82cf1db78a54af9bab98a5cbdaa00c0d9
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991076"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="1123f-105">向客户帐户添加多个用户-将数据文件上传到合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1123f-105">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="1123f-106">**适用于**</span><span class="sxs-lookup"><span data-stu-id="1123f-106">**Applies to**</span></span>

- <span data-ttu-id="1123f-107">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="1123f-107">Partner Center</span></span>

<span data-ttu-id="1123f-108">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="1123f-108">**Appropriate roles**</span></span>

- <span data-ttu-id="1123f-109">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1123f-109">Global admin</span></span>

<span data-ttu-id="1123f-110">可以通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，一次性将多个用户添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="1123f-110">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="1123f-111">你可以从 "合作伙伴中心" 下载一个示例数据文件，然后编辑该文件以供使用，或者可以使用下面定义的数据模型创建新的数据文件。</span><span class="sxs-lookup"><span data-stu-id="1123f-111">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="1123f-112">数据文件要求</span><span class="sxs-lookup"><span data-stu-id="1123f-112">Data file requirements</span></span>

<span data-ttu-id="1123f-113">若要使用批量上传过程将多个用户添加到客户的帐户，需要满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="1123f-113">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="1123f-114">必须拥有客户帐户的全局管理员权限；</span><span class="sxs-lookup"><span data-stu-id="1123f-114">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="1123f-115">每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；</span><span class="sxs-lookup"><span data-stu-id="1123f-115">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="1123f-116">一次最多可上传 100 条记录。</span><span class="sxs-lookup"><span data-stu-id="1123f-116">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="1123f-117">如果需要添加超过 100 个用户，请创建并上传其他数据文件。</span><span class="sxs-lookup"><span data-stu-id="1123f-117">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="1123f-118">所有用户必须处在相同的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="1123f-118">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="1123f-119">仅输入以下所述的数据。</span><span class="sxs-lookup"><span data-stu-id="1123f-119">Enter only the data described below.</span></span> <span data-ttu-id="1123f-120">无关的数据将导致上传失败。</span><span class="sxs-lookup"><span data-stu-id="1123f-120">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="1123f-121">在数据文件中输入以下数据：</span><span class="sxs-lookup"><span data-stu-id="1123f-121">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="1123f-122">**列名**</span><span class="sxs-lookup"><span data-stu-id="1123f-122">**Column name**</span></span> | <span data-ttu-id="1123f-123">**说明**</span><span class="sxs-lookup"><span data-stu-id="1123f-123">**Description**</span></span>                                                              | <span data-ttu-id="1123f-124">**限制**</span><span class="sxs-lookup"><span data-stu-id="1123f-124">**Limitation**</span></span>                             |
| <span data-ttu-id="1123f-125">名字</span><span class="sxs-lookup"><span data-stu-id="1123f-125">First name</span></span>      | <span data-ttu-id="1123f-126">用户的名字（可选字段）</span><span class="sxs-lookup"><span data-stu-id="1123f-126">User's first name (optional field)</span></span>                                           | <span data-ttu-id="1123f-127">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="1123f-127">50-character limit</span></span>                         |
| <span data-ttu-id="1123f-128">姓氏</span><span class="sxs-lookup"><span data-stu-id="1123f-128">Last name</span></span>       | <span data-ttu-id="1123f-129">用户姓氏（可选字段）</span><span class="sxs-lookup"><span data-stu-id="1123f-129">User's last name (optional field)</span></span>                                            | <span data-ttu-id="1123f-130">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="1123f-130">50-character limit</span></span>                         |
| <span data-ttu-id="1123f-131">显示名称</span><span class="sxs-lookup"><span data-stu-id="1123f-131">Display name</span></span>    | <span data-ttu-id="1123f-132">"合作伙伴中心" 中显示的名称（必填字段）</span><span class="sxs-lookup"><span data-stu-id="1123f-132">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="1123f-133">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="1123f-133">50-character limit</span></span>                         |
| <span data-ttu-id="1123f-134">电子邮件</span><span class="sxs-lookup"><span data-stu-id="1123f-134">Email</span></span>           | <span data-ttu-id="1123f-135">客户公司的用户业务电子邮件地址（必填字段）</span><span class="sxs-lookup"><span data-stu-id="1123f-135">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="1123f-136">每个用户的电子邮件地址必须唯一</span><span class="sxs-lookup"><span data-stu-id="1123f-136">Each user must have a unique email address</span></span> |
| <span data-ttu-id="1123f-137">状态更新</span><span class="sxs-lookup"><span data-stu-id="1123f-137">Status update</span></span>   | <span data-ttu-id="1123f-138">用于指示是否成功创建了新用户记录</span><span class="sxs-lookup"><span data-stu-id="1123f-138">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="1123f-139">\*\*留空\*\*</span><span class="sxs-lookup"><span data-stu-id="1123f-139">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="1123f-140">创建多个用户帐户</span><span class="sxs-lookup"><span data-stu-id="1123f-140">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="1123f-141">使用上述数据创建逗号分隔值 (.csv) 数据文件。</span><span class="sxs-lookup"><span data-stu-id="1123f-141">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="1123f-142">保存文件，以供在后续步骤中浏览。</span><span class="sxs-lookup"><span data-stu-id="1123f-142">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="1123f-143">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="1123f-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="1123f-144">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。 </span><span class="sxs-lookup"><span data-stu-id="1123f-144">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="1123f-145">选择客户的 "**用户和许可证**" 选项卡，然后选择 "**上载用户**"。</span><span class="sxs-lookup"><span data-stu-id="1123f-145">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="1123f-146">在 "**上载用户信息**" 下，选择 "**浏览**"。</span><span class="sxs-lookup"><span data-stu-id="1123f-146">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="1123f-147">在文件选择器中，选择数据文件，然后选择 "**打开**"。</span><span class="sxs-lookup"><span data-stu-id="1123f-147">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="1123f-148">选择“验证”。</span><span class="sxs-lookup"><span data-stu-id="1123f-148">Select **Validate**.</span></span>

    <span data-ttu-id="1123f-149">**注意**   大多数帐户创建错误都是由数据文件问题引起的，其中包括缺少的信息、格式不正确或重复的电子邮件地址，或者文件中的记录过多。</span><span class="sxs-lookup"><span data-stu-id="1123f-149">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="1123f-150">合作伙伴中心验证该文件后，选择新用户的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="1123f-150">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="1123f-151">选择“保存”。</span><span class="sxs-lookup"><span data-stu-id="1123f-151">Select **Save**.</span></span>
10. <span data-ttu-id="1123f-152">下载用户的临时密码信息。</span><span class="sxs-lookup"><span data-stu-id="1123f-152">Download the temporary password information for the users.</span></span>

<span data-ttu-id="1123f-153">**重要提示：** 确保现在就下载具有临时密码的文件，在后续步骤中将无法下载。</span><span class="sxs-lookup"><span data-stu-id="1123f-153">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="1123f-154">新用户必须使用新帐户的临时密码登录新帐户。</span><span class="sxs-lookup"><span data-stu-id="1123f-154">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="1123f-155">系统会将**可使用许可证和服务**的权限自动分配给新用户。</span><span class="sxs-lookup"><span data-stu-id="1123f-155">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



