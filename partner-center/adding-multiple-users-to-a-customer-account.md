---
title: 为客户帐户添加多个用户
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要将多个用户添加到客户帐户，请使用逗号分隔值 ( .csv) 文件格式将数据文件上传到合作伙伴中心。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474183"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="3ea9b-103">将用户的 .csv 文件上传到客户的帐户</span><span class="sxs-lookup"><span data-stu-id="3ea9b-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="3ea9b-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="3ea9b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3ea9b-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3ea9b-105">Global admin</span></span>

<span data-ttu-id="3ea9b-106">通过以逗号分隔的值文件)  ( 格式将数据文件上传到合作伙伴中心，将多个用户一次性添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="3ea9b-107">创建客户用户的文件并上传到客户帐户</span><span class="sxs-lookup"><span data-stu-id="3ea9b-107">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="3ea9b-108">使用上述数据创建逗号分隔值 (.csv) 数据文件。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-108">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="3ea9b-109">保存文件，以供在后续步骤中浏览。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-109">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="3ea9b-110">请参阅用于 [.csv 文件的字段以导入客户帐户的多个用户](file-customer-users.md)。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-110">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="3ea9b-111">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="3ea9b-112">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-112">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="3ea9b-113">选择客户的 " **用户和许可证** " 选项卡，然后选择 " **上载用户**"。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-113">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="3ea9b-114">在 " **上载用户信息**" 下，选择 " **浏览**"。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-114">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="3ea9b-115">在文件选择器中，选择数据文件，然后选择 " **打开**"。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-115">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="3ea9b-116">选择“验证”。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-116">Select **Validate**.</span></span>

    <span data-ttu-id="3ea9b-117">**注意** 大多数帐户创建错误均由数据文件问题导致，包括缺少信息、电子邮件地址格式错误或重复，或者文件中有太多记录。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-117">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="3ea9b-118">合作伙伴中心验证该文件后，选择新用户的地理 **位置** 。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-118">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="3ea9b-119">选择“保存”。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-119">Select **Save**.</span></span>
10. <span data-ttu-id="3ea9b-120">下载用户的临时密码信息。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-120">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="3ea9b-121">现在，请确保下载带有临时密码的文件，因为以后无法执行此操作。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-121">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="3ea9b-122">新用户必须使用新帐户的临时密码登录新帐户。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-122">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="3ea9b-123">系统会将 **可使用许可证和服务** 的权限自动分配给新用户。</span><span class="sxs-lookup"><span data-stu-id="3ea9b-123">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="3ea9b-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3ea9b-124">Next steps</span></span>

- [<span data-ttu-id="3ea9b-125">向客户授予合作伙伴中心的权限，以购买自己的产品或服务</span><span class="sxs-lookup"><span data-stu-id="3ea9b-125">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
