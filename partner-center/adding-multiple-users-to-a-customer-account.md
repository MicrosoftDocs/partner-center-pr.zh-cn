---
title: 为客户帐户创建多个用户 | 合作伙伴中心
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，了解如何一次性将多个用户添加到客户的帐户。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 批量上传, 将多个用户添加到客户帐户, 添加客户的用户, 批量上传客户的用户, 客户帐户, 客户用户, 用户
ms.localizationpriority: medium
ms.openlocfilehash: 36130f268c9d33217ef3473136ec511f374fb583
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798625"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="8e1c0-104">将多个用户添加到客户帐户</span><span class="sxs-lookup"><span data-stu-id="8e1c0-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="8e1c0-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="8e1c0-105">**Applies to**</span></span>

- <span data-ttu-id="8e1c0-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="8e1c0-106">Partner Center</span></span>

<span data-ttu-id="8e1c0-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="8e1c0-107">**Appropriate roles**</span></span>

- <span data-ttu-id="8e1c0-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8e1c0-108">Global admin</span></span>

<span data-ttu-id="8e1c0-109">可以通过将逗号分隔值文件格式（.csv）中的数据文件上传到合作伙伴中心，一次性将多个用户添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="8e1c0-110">你可以从 "合作伙伴中心" 下载一个示例数据文件，然后编辑该文件以供使用，或者可以使用下面定义的数据模型创建新的数据文件。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="8e1c0-111">数据文件要求</span><span class="sxs-lookup"><span data-stu-id="8e1c0-111">Data file requirements</span></span>

<span data-ttu-id="8e1c0-112">若要使用批量上传过程将多个用户添加到客户的帐户，需要满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="8e1c0-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="8e1c0-113">必须拥有客户帐户的全局管理员权限；</span><span class="sxs-lookup"><span data-stu-id="8e1c0-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="8e1c0-114">每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；</span><span class="sxs-lookup"><span data-stu-id="8e1c0-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="8e1c0-115">一次最多可上传 100 条记录。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="8e1c0-116">如果需要添加超过 100 个用户，请创建并上传其他数据文件。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="8e1c0-117">所有用户必须处在相同的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="8e1c0-118">仅输入以下所述的数据。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-118">Enter only the data described below.</span></span> <span data-ttu-id="8e1c0-119">无关的数据将导致上传失败。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="8e1c0-120">在数据文件中输入以下数据：</span><span class="sxs-lookup"><span data-stu-id="8e1c0-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="8e1c0-121">**列名称**</span><span class="sxs-lookup"><span data-stu-id="8e1c0-121">**Column name**</span></span> | <span data-ttu-id="8e1c0-122">**说明**</span><span class="sxs-lookup"><span data-stu-id="8e1c0-122">**Description**</span></span>                                                              | <span data-ttu-id="8e1c0-123">**限制**</span><span class="sxs-lookup"><span data-stu-id="8e1c0-123">**Limitation**</span></span>                             |
| <span data-ttu-id="8e1c0-124">名字</span><span class="sxs-lookup"><span data-stu-id="8e1c0-124">First name</span></span>      | <span data-ttu-id="8e1c0-125">用户的名字（可选字段）</span><span class="sxs-lookup"><span data-stu-id="8e1c0-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="8e1c0-126">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="8e1c0-126">50-character limit</span></span>                         |
| <span data-ttu-id="8e1c0-127">姓氏</span><span class="sxs-lookup"><span data-stu-id="8e1c0-127">Last name</span></span>       | <span data-ttu-id="8e1c0-128">用户姓氏（可选字段）</span><span class="sxs-lookup"><span data-stu-id="8e1c0-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="8e1c0-129">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="8e1c0-129">50-character limit</span></span>                         |
| <span data-ttu-id="8e1c0-130">显示名称</span><span class="sxs-lookup"><span data-stu-id="8e1c0-130">Display name</span></span>    | <span data-ttu-id="8e1c0-131">"合作伙伴中心" 中显示的名称（必填字段）</span><span class="sxs-lookup"><span data-stu-id="8e1c0-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="8e1c0-132">50 个字符的限制</span><span class="sxs-lookup"><span data-stu-id="8e1c0-132">50-character limit</span></span>                         |
| <span data-ttu-id="8e1c0-133">电子邮件
</span><span class="sxs-lookup"><span data-stu-id="8e1c0-133">Email</span></span>           | <span data-ttu-id="8e1c0-134">客户公司的用户业务电子邮件地址（必填字段）</span><span class="sxs-lookup"><span data-stu-id="8e1c0-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="8e1c0-135">每个用户的电子邮件地址必须唯一</span><span class="sxs-lookup"><span data-stu-id="8e1c0-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="8e1c0-136">状态更新</span><span class="sxs-lookup"><span data-stu-id="8e1c0-136">Status update</span></span>   | <span data-ttu-id="8e1c0-137">用于指示是否成功创建了新用户记录</span><span class="sxs-lookup"><span data-stu-id="8e1c0-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="8e1c0-138">\*\*留空\*\*</span><span class="sxs-lookup"><span data-stu-id="8e1c0-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="8e1c0-139">创建多个用户帐户</span><span class="sxs-lookup"><span data-stu-id="8e1c0-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="8e1c0-140">使用上述数据创建逗号分隔值 (.csv) 数据文件。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="8e1c0-141">保存文件，以供在后续步骤中浏览。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="8e1c0-142">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="8e1c0-143">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。 </span><span class="sxs-lookup"><span data-stu-id="8e1c0-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="8e1c0-144">选择客户的 "**用户和许可证**" 选项卡，然后选择 "**上载用户**"。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="8e1c0-145">在 "**上载用户信息**" 下，选择 "**浏览**"。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="8e1c0-146">在文件选择器中，选择数据文件，然后选择 "**打开**"。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="8e1c0-147">选择“验证”。 </span><span class="sxs-lookup"><span data-stu-id="8e1c0-147">Select **Validate**.</span></span>

    <span data-ttu-id="8e1c0-148">**请注意**  ，大多数帐户创建错误是由数据文件问题引起的，其中包括缺少的信息、格式不正确的或重复的电子邮件地址，或者文件中的记录过多。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="8e1c0-149">合作伙伴中心验证该文件后，选择新用户的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="8e1c0-150">选择“保存”  。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-150">Select **Save**.</span></span>
10. <span data-ttu-id="8e1c0-151">下载用户的临时密码信息。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="8e1c0-152">**重要提示：** 确保现在就下载具有临时密码的文件，在后续步骤中将无法下载。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="8e1c0-153">新用户必须使用新帐户的临时密码登录新帐户。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="8e1c0-154">系统会将**可使用许可证和服务**的权限自动分配给新用户。</span><span class="sxs-lookup"><span data-stu-id="8e1c0-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



