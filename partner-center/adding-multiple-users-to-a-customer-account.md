---
title: 为客户帐户创建多个用户 | 合作伙伴中心
description: 通过将逗号分隔值文件格式 (.csv) 的数据文件上传到合作伙伴中心，可同时将多个用户添加至客户帐户。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: 批量上传, 将多个用户添加到客户帐户, 添加客户的用户, 批量上传客户的用户, 客户帐户, 客户用户, 用户
ms.localizationpriority: medium
ms.openlocfilehash: e7a5e7f9c0cebf81373c500dd3a552710fcf845a
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876967"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="9806d-104">将多个用户添加到客户帐户</span><span class="sxs-lookup"><span data-stu-id="9806d-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="9806d-105">适用于</span><span class="sxs-lookup"><span data-stu-id="9806d-105">Applies to</span></span>**

-  <span data-ttu-id="9806d-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="9806d-106">Partner Center</span></span>

<span data-ttu-id="9806d-107">通过将逗号分隔值文件格式 (.csv) 的数据文件上传到合作伙伴仪表板，可同时将多个用户添加至客户帐户。</span><span class="sxs-lookup"><span data-stu-id="9806d-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Dashboard.</span></span> <span data-ttu-id="9806d-108">可从合作伙伴仪表板下载示例数据文件，然后对其进行编辑以供使用，或者使用下面定义的数据模型新建数据文件。</span><span class="sxs-lookup"><span data-stu-id="9806d-108">You can download a sample data file from the Partner Dashboard and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="9806d-109">数据文件要求</span><span class="sxs-lookup"><span data-stu-id="9806d-109">Data file requirements</span></span>


<span data-ttu-id="9806d-110">若要使用批量上传进程向客户帐户添加多个用户，你需要满足以下要求：</span><span class="sxs-lookup"><span data-stu-id="9806d-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="9806d-111">必须拥有客户帐户的全局管理员权限；</span><span class="sxs-lookup"><span data-stu-id="9806d-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="9806d-112">每个用户必须拥有附加到客户电子邮件域的唯一电子邮件地址；</span><span class="sxs-lookup"><span data-stu-id="9806d-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="9806d-113">一次最多可上传 100 条记录。</span><span class="sxs-lookup"><span data-stu-id="9806d-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="9806d-114">如果需要添加超过 100 个用户，请创建并上传其他数据文件。</span><span class="sxs-lookup"><span data-stu-id="9806d-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="9806d-115">所有用户必须处在相同的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="9806d-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="9806d-116">仅输入以下所述的数据。</span><span class="sxs-lookup"><span data-stu-id="9806d-116">Enter only the data described below.</span></span> <span data-ttu-id="9806d-117">无关的数据将导致上传失败。</span><span class="sxs-lookup"><span data-stu-id="9806d-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="9806d-118">在数据文件中输入以下数据：</span><span class="sxs-lookup"><span data-stu-id="9806d-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="9806d-119">列名称</span><span class="sxs-lookup"><span data-stu-id="9806d-119">Column name</span></span>** | **<span data-ttu-id="9806d-120">说明</span><span class="sxs-lookup"><span data-stu-id="9806d-120">Description</span></span>**                                                              | **<span data-ttu-id="9806d-121">限制</span><span class="sxs-lookup"><span data-stu-id="9806d-121">Limitation</span></span>**                             |
| <span data-ttu-id="9806d-122">名字</span><span class="sxs-lookup"><span data-stu-id="9806d-122">First name</span></span>      | <span data-ttu-id="9806d-123">用户名字（可选字段）</span><span class="sxs-lookup"><span data-stu-id="9806d-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="9806d-124">限 50 个字符</span><span class="sxs-lookup"><span data-stu-id="9806d-124">50-character limit</span></span>                         |
| <span data-ttu-id="9806d-125">姓氏</span><span class="sxs-lookup"><span data-stu-id="9806d-125">Last name</span></span>       | <span data-ttu-id="9806d-126">用户姓氏（可选字段）</span><span class="sxs-lookup"><span data-stu-id="9806d-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="9806d-127">限 50 个字符</span><span class="sxs-lookup"><span data-stu-id="9806d-127">50-character limit</span></span>                         |
| <span data-ttu-id="9806d-128">显示名称</span><span class="sxs-lookup"><span data-stu-id="9806d-128">Display name</span></span>    | <span data-ttu-id="9806d-129">显示在合作伙伴仪表板中的名称（必填字段）</span><span class="sxs-lookup"><span data-stu-id="9806d-129">Name displayed in the Partner Dashboard (required field)</span></span>                            | <span data-ttu-id="9806d-130">限 50 个字符</span><span class="sxs-lookup"><span data-stu-id="9806d-130">50-character limit</span></span>                         |
| <span data-ttu-id="9806d-131">电子邮件</span><span class="sxs-lookup"><span data-stu-id="9806d-131">Email</span></span>           | <span data-ttu-id="9806d-132">客户公司中的用户业务电子邮件地址（必填字段）</span><span class="sxs-lookup"><span data-stu-id="9806d-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="9806d-133">每个用户必须拥有唯一的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="9806d-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="9806d-134">状态更新</span><span class="sxs-lookup"><span data-stu-id="9806d-134">Status update</span></span>   | <span data-ttu-id="9806d-135">用于指示是否成功创建了新用户记录</span><span class="sxs-lookup"><span data-stu-id="9806d-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="9806d-136">\*\*保留为空\*\*</span><span class="sxs-lookup"><span data-stu-id="9806d-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="9806d-137">创建多个用户帐户</span><span class="sxs-lookup"><span data-stu-id="9806d-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="9806d-138">使用上述数据创建逗号分隔值 (.csv) 数据文件。</span><span class="sxs-lookup"><span data-stu-id="9806d-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="9806d-139">保存文件，以供在后续步骤中浏览。</span><span class="sxs-lookup"><span data-stu-id="9806d-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="9806d-140">在**仪表板**菜单中，选择**客户**，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="9806d-140">From the **Dashboard** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="9806d-141">选择**上传用户**。</span><span class="sxs-lookup"><span data-stu-id="9806d-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="9806d-142">在**上传用户信息**下，选择**浏览**。</span><span class="sxs-lookup"><span data-stu-id="9806d-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="9806d-143">在文件选择器中，选择数据文件，然后选择**打开**。</span><span class="sxs-lookup"><span data-stu-id="9806d-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="9806d-144">选择**验证**。</span><span class="sxs-lookup"><span data-stu-id="9806d-144">Select **Validate**.</span></span>

    <span data-ttu-id="9806d-145">**注意** 大多数帐户创建错误均由数据文件问题导致，包括缺少信息、电子邮件地址格式错误或重复，或者文件中有太多记录。</span><span class="sxs-lookup"><span data-stu-id="9806d-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="9806d-146">在合作伙伴仪表板验证文件后，选择新用户的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="9806d-146">After the Partner Dashboard validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="9806d-147">选择**保存**。</span><span class="sxs-lookup"><span data-stu-id="9806d-147">Select **Save**.</span></span>
9.  <span data-ttu-id="9806d-148">下载用户的临时密码信息。</span><span class="sxs-lookup"><span data-stu-id="9806d-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="9806d-149">**重要提示：** 确保现在就下载具有临时密码的文件，在后续步骤中将无法下载。</span><span class="sxs-lookup"><span data-stu-id="9806d-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="9806d-150">新用户必须使用新帐户的临时密码登录新帐户。</span><span class="sxs-lookup"><span data-stu-id="9806d-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="9806d-151">新用户自动分配的**可使用许可证和服务**的权限。</span><span class="sxs-lookup"><span data-stu-id="9806d-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



