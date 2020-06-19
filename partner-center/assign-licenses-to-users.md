---
title: 管理客户帐户中的用户
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何为客户创建用户帐户、添加或删除用户许可证、重置用户密码、删除用户帐户或还原用户帐户。
author: LauraBrenner
ms.author: labrenne
Keywords: 客户管理，帐户，创建帐户，许可证，分配许可证，用户管理，密码，重置密码，更改密码
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3fb55e341692e38250c4e751cf73f3120604c15a
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991035"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="71fc8-104">合作伙伴中心的客户帐户的用户管理任务</span><span class="sxs-lookup"><span data-stu-id="71fc8-104">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="71fc8-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="71fc8-105">**Applies to**</span></span>

- <span data-ttu-id="71fc8-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="71fc8-106">Partner Center</span></span>

<span data-ttu-id="71fc8-107">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="71fc8-107">**Appropriate roles**</span></span>

- <span data-ttu-id="71fc8-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="71fc8-108">Global admin</span></span>
- <span data-ttu-id="71fc8-109">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="71fc8-109">User management admin</span></span>
- <span data-ttu-id="71fc8-110">管理员代理</span><span class="sxs-lookup"><span data-stu-id="71fc8-110">Admin agent</span></span>
- <span data-ttu-id="71fc8-111">销售代理</span><span class="sxs-lookup"><span data-stu-id="71fc8-111">Sales agent</span></span>
- <span data-ttu-id="71fc8-112">支持人员代理</span><span class="sxs-lookup"><span data-stu-id="71fc8-112">Helpdesk agent</span></span>

<span data-ttu-id="71fc8-113">你可以在客户的帐户中创建和删除新用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-113">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="71fc8-114">你还可以还原以前在删除30天内删除的一个或多个用户帐户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-114">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="71fc8-115">用户之前分配的订阅也将还原（假设之前的分配可用）。</span><span class="sxs-lookup"><span data-stu-id="71fc8-115">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="71fc8-116">为客户购买新的订阅时，客户应为你提供一个列表，其中列出了需要帐户的所有用户、用户权限以及每个用户需要的服务。</span><span class="sxs-lookup"><span data-stu-id="71fc8-116">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="71fc8-117">可以一次[将订阅分配给多个用户](bulk-license-provisioning-for-multiple-users.md)，方法是使用 [Excel 兼容的 .csv 电子表格文件](adding-multiple-users-to-a-customer-account.md)导入这些名称。</span><span class="sxs-lookup"><span data-stu-id="71fc8-117">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="71fc8-118">为客户创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="71fc8-118">Create user accounts for a customer</span></span>

1. <span data-ttu-id="71fc8-119">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="71fc8-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="71fc8-120">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。 </span><span class="sxs-lookup"><span data-stu-id="71fc8-120">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="71fc8-121">在客户菜单中，选择“用户和许可证”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="71fc8-121">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="71fc8-122">对于每个用户，请选择**添加订阅**，然后填写信息，包括权限和许可证。</span><span class="sxs-lookup"><span data-stu-id="71fc8-122">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="71fc8-123">单击“保存”以保存更改。</span><span class="sxs-lookup"><span data-stu-id="71fc8-123">**Save** your changes.</span></span>

5. <span data-ttu-id="71fc8-124">请确保记录用户名和临时密码以发送给用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-124">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="71fc8-125">如果要一次一个地添加多个用户，则使用**再次添加一个用户**。</span><span class="sxs-lookup"><span data-stu-id="71fc8-125">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="71fc8-126">你还可以通过[导入 Excel 兼容的 .csv 电子表格文件](adding-multiple-users-to-a-customer-account.md)一次添加多个用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-126">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="71fc8-127">等到添加完所有用户后，可从确认屏幕通过电子邮件发送或打印这些名称和密码。</span><span class="sxs-lookup"><span data-stu-id="71fc8-127">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="71fc8-128">为客户添加或删除用户许可证</span><span class="sxs-lookup"><span data-stu-id="71fc8-128">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="71fc8-129">以下步骤适用于在 Microsoft 产品中添加或删除用户许可证。</span><span class="sxs-lookup"><span data-stu-id="71fc8-129">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="71fc8-130">若要在商业应用商店中添加或删除基于许可证的 SaaS 订阅的用户许可证，请参阅[添加或删除 SaaS 订阅的许可证](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)。</span><span class="sxs-lookup"><span data-stu-id="71fc8-130">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="71fc8-131">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="71fc8-131">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="71fc8-132">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。 </span><span class="sxs-lookup"><span data-stu-id="71fc8-132">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="71fc8-133">在客户菜单中，选择“用户和许可证”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="71fc8-133">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="71fc8-134">从列表中选择一个或多个用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-134">Choose one or more users from the list.</span></span> <span data-ttu-id="71fc8-135">例如，如果客户刚刚购买了新的许可证，并且你想要将其分配给尚不具备这些许可证的用户，则可以使用**筛选用户依据 ...** 选项来查找适当的组。</span><span class="sxs-lookup"><span data-stu-id="71fc8-135">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="71fc8-136">选择 "**管理许可证**"。</span><span class="sxs-lookup"><span data-stu-id="71fc8-136">Select **Manage licenses**.</span></span> <span data-ttu-id="71fc8-137">进行更改，并**保存**。</span><span class="sxs-lookup"><span data-stu-id="71fc8-137">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="71fc8-138">对于[Azure Marketplace 产品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)，许可证分配和激活是通过发布产品的独立软件供应商（ISV）来管理的。</span><span class="sxs-lookup"><span data-stu-id="71fc8-138">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="71fc8-139">为客户重置用户密码</span><span class="sxs-lookup"><span data-stu-id="71fc8-139">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="71fc8-140">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="71fc8-140">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="71fc8-141">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。 </span><span class="sxs-lookup"><span data-stu-id="71fc8-141">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="71fc8-142">在客户菜单中，选择“用户和许可证”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="71fc8-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="71fc8-143">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-143">Choose the user from the list.</span></span>

4.  <span data-ttu-id="71fc8-144">在屏幕底部，选择 "**重置密码**"。</span><span class="sxs-lookup"><span data-stu-id="71fc8-144">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="71fc8-145">将新的临时密码发送给用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-145">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="71fc8-146">为客户删除用户帐户</span><span class="sxs-lookup"><span data-stu-id="71fc8-146">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="71fc8-147">从 "**合作伙伴中心**" 菜单中，选择 "**客户**"。</span><span class="sxs-lookup"><span data-stu-id="71fc8-147">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="71fc8-148">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-148">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="71fc8-149">在客户菜单中，选择“用户和许可证”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="71fc8-149">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="71fc8-150">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-150">Choose the user from the list.</span></span>

3.  <span data-ttu-id="71fc8-151">在屏幕底部选择“删除用户帐户”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="71fc8-151">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="71fc8-152">如果需要还原此帐户，可在客户的**用户和许可证**列表的**已删除用户**选项卡中找到它。</span><span class="sxs-lookup"><span data-stu-id="71fc8-152">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="71fc8-153">你有 30 天的时间还原已删除的用户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-153">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="71fc8-154">还原删除的用户帐户</span><span class="sxs-lookup"><span data-stu-id="71fc8-154">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="71fc8-155">从 "**合作伙伴中心**" 菜单中，选择 "**客户**"，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="71fc8-155">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="71fc8-156">选择 "**用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="71fc8-156">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="71fc8-157">选择**已删除的用户 ( )**，当存在可以还原的已删除用户时，应读取 **(1)** 或更大。</span><span class="sxs-lookup"><span data-stu-id="71fc8-157">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="71fc8-158">选择一个或多个已删除用户的复选框，然后选择 "**还原**"。</span><span class="sxs-lookup"><span data-stu-id="71fc8-158">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="71fc8-159">所有选定的用户帐户将重新出现在 "**用户和许可证**" 页中。</span><span class="sxs-lookup"><span data-stu-id="71fc8-159">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="71fc8-160">相关主题</span><span class="sxs-lookup"><span data-stu-id="71fc8-160">Related topics</span></span>


[<span data-ttu-id="71fc8-161">向多个用户分配或撤消许可证</span><span class="sxs-lookup"><span data-stu-id="71fc8-161">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="71fc8-162">为客户帐户创建多个用户</span><span class="sxs-lookup"><span data-stu-id="71fc8-162">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)